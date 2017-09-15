---
TOCTitle: Systemsicherungen für RMS
Title: Systemsicherungen für RMS
ms:assetid: 'c29894da-ee00-428c-8d48-80d8e5a83678'
ms:contentKeyID: 18118998
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747746(v=WS.10)'
---

Systemsicherungen für RMS
=========================

Bevor Sie die Infrastruktur einrichten und RMS installieren, sichern Sie – je nach Bedarf – die folgenden Komponenten:

-   Wenn Sie eine bereits vorhandene SQL Server-Datenbank verwenden, um die Konfigurations- und Protokollierungsdatenbanken bereitzustellen, sichern Sie zuvor alle Datenbanken und Servereinstellungen. Wenn Sie eine frühere Version von RMS aktualisieren oder RMS neu installieren, stellen Sie sicher, dass alle früheren Konfigurations- und Protokollierungsdatenbanken gesichert wurden.
-   Sichern Sie auch den Systemstatus des Servers, auf dem RMS installiert werden soll. Durch diese Sicherung werden Registrierungsschlüssel und Werte gespeichert, die für eine möglicherweise erforderliche Serverwiederherstellung benötigte Daten enthalten.
-   Mithilfe des Snap-Ins für Zertifikate können Sie Zertifikate in eine Datei exportieren. Das Snap-In für Zertifikate dient auch zur Sicherung der Daten des privaten Schlüssels für RMS in einer PKCS12-Datei, die mit einem Kennwort verschlüsselt wird. Wenn Sie RMS aktualisieren oder neu installieren und die Standardsoftwareverschlüsselung zum Schutz des privaten Schlüssels für RMS verwendet haben, wurde dieser im Rahmen der Sicherung der Konfigurationsdatenbank verschlüsselt und gespeichert.
-   Wenn Sie ein Hardwaresicherheitsmodul verwenden, um den privaten Schlüssel zu sichern, sollten Sie dessen Konfiguration nach den Anleitungen des Herstellers sichern.

Die Sicherungsdateien sollten an einem sicheren Speicherort zusammen mit dem Kennwort gespeichert werden, das zum Verschlüsseln der privaten Schlüssel verwendet wurde.
