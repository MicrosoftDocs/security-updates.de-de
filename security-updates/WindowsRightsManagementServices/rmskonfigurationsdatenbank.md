---
TOCTitle: 'RMS-Konfigurationsdatenbank'
Title: 'RMS-Konfigurationsdatenbank'
ms:assetid: '769adbdc-f32f-464b-85c4-e8b160036187'
ms:contentKeyID: 18118895
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747634(v=WS.10)'
---

RMS-Konfigurationsdatenbank
===========================

RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendet einen Datenbankserver, wie z. B. Microsoft® SQL Server oder Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A, um Konfigurations- und Richtlinieninformationen zu speichern. Für jeden RMS-Server oder -Cluster wird eine eigene Konfigurationsdatenbank angelegt, in der die Konfigurationsdaten und sonstige Daten gespeichert, freigegeben und abgerufen werden.

Die Konfigurationsdatenbank für den Stammzertifizierungsserver oder -cluster enthält eine Liste mit Windows-Benutzer-IDs und deren Rechtekontozertifikaten. Das Schlüsselpaar des Zertifikats wird mit dem öffentlichen RMS-Serverschlüssel verschlüsselt, bevor es in der Datenbank gespeichert wird. Die Konfigurationsdatenbanken für Lizenzierungsserver enthalten diese Informationen nicht.

Die RMS Service Group (RMS-Dienstgruppe) verfügt über die Berechtigungen Ausführen für die gespeicherten Prozeduren der Datenbank.

**Wichtig** MSDE 2000 sollte zur Unterstützung von RMS-Datenbanken nur in Testumgebungen eingesetzt werden, da MSDE 2000 keine Netzwerkschnittstellen unterstützt. Darüber hinaus wird in den Nutzungsbedingungen für MSDE 2000 angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer MSDE 2000-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder Protokollierungsinformationen anzeigen noch in der Konfigurationsdatenbank gespeicherte Daten ändern.