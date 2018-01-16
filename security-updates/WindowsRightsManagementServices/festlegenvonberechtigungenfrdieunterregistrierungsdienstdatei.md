---
TOCTitle: Festlegen von Berechtigungen für die Unterregistrierungsdienstdatei
Title: Festlegen von Berechtigungen für die Unterregistrierungsdienstdatei
ms:assetid: '737bb69b-fe26-4057-9569-e632f7bbf295'
ms:contentKeyID: 18118889
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747627(v=WS.10)'
---

Festlegen von Berechtigungen für die Unterregistrierungsdienstdatei
===================================================================

Der Unterregistrierungsdienst wird auf dem Stammzertifizierungsserver ausgeführt und registriert einen Lizenzierungsserver während der Bereitstellung. Standardmäßig ermöglicht der Unterregistrierungsdienst nur den Zugriff auf das Konto des lokalen Systems, das sich auf dem Stammzertifizierungsserver befindet. Um einen Lizenzierungsserver bereitzustellen, müssen Sie sich mit einem solchen Konto am Lizenzierungsserver anmelden. Als Alternative hierzu kann ein lokaler Administrator auf dem Stammzertifizierungsserver die DACL (Discretionary Access Control List oder Zugriffssteuerungsliste) in der Unterregistrierungsdienstdatei SubEnrollService.asmx ändern. Auf diese Weise wird dem Benutzerkonto Zugriff gewährt, das die Bereitstellung auf dem Lizenzierungsserver durchführt. SubEnrollService.asmx ist im virtuellen Verzeichnis für die Zertifizierung auf dem Stammzertifizierungsserver gespeichert.