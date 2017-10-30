---
TOCTitle: Verschieben der Protokollierungsdatenbank
Title: Verschieben der Protokollierungsdatenbank
ms:assetid: '34ea8045-dc94-422e-9601-29927cfc1534'
ms:contentKeyID: 18118794
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720238(v=WS.10)'
---

Verschieben der Protokollierungsdatenbank
=========================================

Bei der RMS-Standardkonfiguration werden die Konfigurationsdatenbank und die Protokollierungsdatenbank auf dem gleichen Server abgelegt. Sie sollten regelmäßig überprüfen, ob SQL Server über ausreichend Speicherplatz für beide Datenbanken verfügt.

Wenn die Protokollierungsdatenbank zu groß wird, können Sie sie jederzeit auf einen anderen Server verschieben. Das Verschieben der Protokollierungsdatenbank mithilfe der Verwaltungswebsite ist nicht möglich. Sie müssen sie vielmehr mit den folgenden Schritten manuell verschieben:

1.  Deaktivieren Sie die Protokollierung, wie nachstehend unter „[So aktivieren oder deaktivieren Sie die Protokollierung](https://technet.microsoft.com/8e672f95-566f-4070-9a2a-2f70f087148f)“ beschrieben.
2.  Kopieren Sie die Protokollierungsdatenbank mithilfe von SQL Server Enterprise Manager vom Quellserver auf den Zielserver. Stellen Sie sicher, dass die Tabellen und gespeicherten Verfahren in der neuen Datenbank erstellt werden. Zum Kopieren der Datenbank können Sie den Assistenten zum Kopieren von Datenbanken von SQL Server Enterprise Manager verwenden.
3.  Ändern Sie die Konfigurationsdatenbank so, dass die Namen des neuen Servers und der Datenbank widergespiegelt werden. Führen Sie in der Tabelle DRMS\_ClusterPolicies der Konfigurationsdatenbank des Clusters, dessen Datenbank Sie verschieben, die folgenden Aktionen aus:
    -   Ändern Sie den Wert der LoggingDatabaseServer-Richtlinie so, dass der Name des neuen Datenbankservers widergespiegelt wird.
    -   Ändern Sie den Wert der LoggingDatabaseName-Richtlinie so, dass der neue Datenbankname widergespiegelt wird.

    | ![](images/Cc720238.note(WS.10).gif)Hinweis                                                                                                                                                                                                                             |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | SQL Server Enterprise Manager unterstützt Felder vom Typ „db\_variant“ nicht. Sie können diese also nicht für diese Aufgabe verwenden. Stattdessen können Sie aber das im Lieferumfang von SQL Server enthaltene Tool Query Analyzer oder ein anderes Tool zum Bearbeiten von Datenbanken verwenden. |

4.  Starten Sie IIS auf allen im Cluster enthaltenen Servern neu.
5.  Aktivieren Sie die Protokollierung erneut.