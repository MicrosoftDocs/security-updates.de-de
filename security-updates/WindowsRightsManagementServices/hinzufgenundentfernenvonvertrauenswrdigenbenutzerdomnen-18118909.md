---
TOCTitle: Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen
Title: Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen
ms:assetid: '7c440b15-01c4-49f1-b43c-00f67f3388c1'
ms:contentKeyID: 18118909
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747571(v=WS.10)'
---

Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen
===============================================================

RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verarbeitet standardmäßig keine Anforderungen von Benutzern, deren Rechtekontozertifikate von einer anderen RMS-Installation ausgestellt wurden. Sie können aber Benutzerdomänen zur Liste der vertrauenswürdigen Benutzerdomänen hinzufügen, damit RMS solche Anforderungen verarbeitet.

Für jede vertrauenswürdige Domäne können Sie bestimmte Benutzer oder Benutzergruppen hinzufügen oder entfernen. Darüber hinaus können Sie eine vertrauenswürdige Benutzerdomäne entfernen. Das Entfernen des Stammzertifizierungsclusters für diese Active Directory-Gesamtstruktur aus den vertrauenswürdigen Benutzerdomänen ist jedoch nicht möglich. Für jeden Server mit RMS in einer Bereitstellung, einschließlich des Stammzertifizierungsservers, ist der Stammzertifizierungscluster in der eigenen Gesamtstruktur automatisch vertrauenswürdig.

Sie können vertrauenswürdige Benutzerdomänen folgendermaßen verwalten:

-   Zur Unterstützung externer Benutzer im Allgemeinen können Sie den Microsoft® .NET Passport-Dienst zur Liste der vertrauenswürdigen Domänen hinzufügen. Damit kann ein Server mit RMS in einem Unternehmen Lizenzierungsanforderungen verarbeiten, die ein vom Microsoft .NET Passport-Dienst ausgestelltes Rechtekontozertifikat einschließen.
-   Soll externen Benutzern aus der RMS-Installation einer anderen Organisation vertraut werden, können Sie diese Organisation zur Liste der vertrauenswürdigen Benutzerdomänen hinzufügen. Damit kann ein Server mit RMS eine Lizenzierungsanforderung verarbeiten, die ein von einem RMS-Server in der anderen Organisation ausgestelltes Rechtekontozertifikat einschließt.
-   Ebenso können Sie die RMS-Installation in einer anderen Active Directory-Gesamtstruktur zur Liste der vertrauenswürdigen Benutzerdomänen hinzufügen. Damit verarbeiten Sie Lizenzierungsanforderungen von Benutzern in der eigenen Organisation, die sich in der anderen Gesamtstruktur befinden. Dadurch kann ein in der aktuellen Gesamtstruktur befindlicher Server mit RMS eine Lizenzierungsanforderung verarbeiten, die ein Rechtekontozertifikat einschließt, das von einem RMS-Server in der anderen Gesamtstruktur ausgestellt wurde.
-   Sie können für jede vertrauenswürdige Benutzerdomäne festlegen, welche E-Mail-Domänen vertrauenswürdig sind. Für vertrauenswürdige Passport-Domänen können Sie festlegen, welche E-Mail-Benutzer oder -Domänen nicht vertrauenswürdig sind.

Wenn Sie eine RMS-Installation zur Liste der vertrauenswürdigen Benutzerdomänen hinzufügen möchten, müssen Sie das Server-Lizenzgeberzertifikat der hinzuzufügenden RMS-Installation importieren. Der Administrator muss dazu zunächst das Server-Lizenzgeberzertifikat des vertrauenswürdigen Servers oder Clusters exportieren und an Sie senden. Dann können Sie die Datei unter Angabe des Speicherortes importieren. Ein Benutzer kann die Datei speichern, sofern er über Berechtigungen für den freigegebenen Ordner verfügt. Die Informationen zum privaten Schlüssel werden beim Einrichten einer vertrauenswürdigen Benutzerdomäne nicht übertragen.

Schritt-für-Schritt-Anleitungen zum Einrichten von vertrauenswürdigen Benutzerdomänen finden Sie nachstehend unter [So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu](https://technet.microsoft.com/ed672e58-6272-4ac0-a434-d1d938037e93).
