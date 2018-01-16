---
TOCTitle: 'Planen der Datenbankserver-Infrastruktur'
Title: 'Planen der Datenbankserver-Infrastruktur'
ms:assetid: 'b12354bd-3143-4d1f-b5aa-450c4550653c'
ms:contentKeyID: 18118990
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747731(v=WS.10)'
---

Planen der Datenbankserver-Infrastruktur
========================================

Zum Ausführen von Operationen greift RMS auf Datenbanken und gespeicherte Verfahren zurück. Aus diesem Grund ist eine Datenbankinfrastruktur notwendig, damit Sie RMS in Ihrem Unternehmen nutzen können. Der Datenbankserver kann sich dabei wahlweise auf demselben Server wie RMS befinden oder auch auf einem anderen Server. Falls Ihre Infrastruktur keinen Datenbankserver für die Unterstützung von RMS umfasst, können Sie zum Testen von RMS die Microsoft SQL Server 2000 Desktop Engine (MSDE 2000), Release A, heranziehen.

Sie sollten Microsoft SQL Server Desktop Engine (MSDE) nur in Testumgebungen zur Unterstützung von RMS-Datenbanken verwenden, da Microsoft SQL Server Desktop Engine nicht die notwendigen Tools für die uneingeschränkte Ausführung und Unterstützung einer unternehmensweiten Datenbank enthält. MSDE unterstützt außerdem nicht den Remote-Netzwerkbetrieb und muss daher auf demselben Server wie RMS installiert werden. Zudem können Sie keine weiteren RMS-Server in den RMS-Cluster aufnehmen. In den Nutzungsbedingungen für Microsoft SQL Server Desktop Engine wird angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer Microsoft SQL Server Desktop Engine-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder die RMS-Konfigurationsdatenbank sichern und wiederherstellen noch Protokollierungsinformationen anzeigen oder in der Konfigurationsdatenbank gespeicherte Daten direkt bearbeiten.

Wenn Sie planen, die Datenbanken auf einem anderen Server als die RMS-Installation auszuführen, benötigen Sie ein komplettes Datenbankserverprodukt (z. B. SQL Server), das die notwendige Datenbankunterstützung bietet. Erteilen Sie dem RMS-Dienstkonto die entsprechenden Berechtigungen zum Lesen, Schreiben und Erstellen von Datenbanken, die sich auf dem Datenbankserver für RMS befinden.

Obwohl RMS speziell für Datenbankserver, auf denen SQL Server 2000 und MSDE ausgeführt wird, ausgelegt und getestet wurde und Microsoft die Verwendung von RMS mit anderen Datenbankanbietern als SQL Server 2000 oder MSDE nicht unterstützt, kann RMS auch auf anderen Datenbankservern mit ADO.NET-Schnittstellen ausgeführt werden, die von Microsoft .NET Framework bereitgestellt werden. Deshalb ist es möglich, dass andere Datenbankhersteller kompatible Datenbankanbieter für RMS entwickelt haben. Sie können einen beliebigen Datenbankanbieter mit RMS verwenden, sofern der entsprechende Datenbankserver folgende Kriterien erfüllt:

-   Der Datenbankserver muss Transact-SQL-kompatibel sein, da Transact-SQL von den RMS-Initialisierungsskripts und den gespeicherten RMS-Verfahren verwendet wird.
-   Der Datenbankserver muss alle für Microsoft SQL Server spezifischen Erweiterungen unterstützen.

Der Datenbankanbieter muss folgende Funktionen ausführen können:

-   Auf Methodenaufrufe des Namespace System.Data.SqlClient von .NET Framework reagieren
-   Die entsprechende Funktionalität des Namespace System.Data.SqlClient bereitstellen
-   Integrierte Windows-Authentifizierung anstelle der SQL-Authentifizierung verwenden

Wenn Sie RMS in einer anderen Konfiguration als dieser verwenden, wenden Sie sich an den Datenbankhersteller oder Lösungsanbieter, dessen Datenbankanbieter Sie in Ihrer angepassten Bereitstellung einsetzen.

| ![](images/Cc747731.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Die RMS-Datenbanken werden standardmäßig mit aktivierter vollständiger Wiederherstellung erstellt; Transaktionsprotokoll-Sicherungsjobs werden jedoch nicht angelegt. Dies kann dazu führen, dass der gesamte Speicherplatz auf der Festplatte des Servers belegt wird, und schließlich in einem Ausfall des Datenbankservers resultieren. Für die DRMS-Konfigurationsdatenbank wird die vollständige Wiederherstellung empfohlen. Die anderen DRMS-Datenbanken können für ein anderes Wiederherstellungsverfahren gemäß den Anforderungen Ihres Unternehmens konfiguriert werden. |

Dieser Abschnitt behandelt die folgenden Themen:

-   [Schätzen des Wachstums der Datenbank](https://technet.microsoft.com/87652cc2-b886-4797-8d40-356669768089)
-   [Pflegen der Verzeichnisdienste-Datenbank](https://technet.microsoft.com/911a62f2-c1d6-4091-99b0-b53211be27a7)
-   [Pflegen der Protokollierungsdatenbank](https://technet.microsoft.com/de55058b-0d1a-4997-8a45-e14678ddd13f)