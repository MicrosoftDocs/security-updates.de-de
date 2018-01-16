---
TOCTitle: Nutzungslizenzen und externe Benutzer
Title: Nutzungslizenzen und externe Benutzer
ms:assetid: '02db9bda-180e-438f-863d-26252083a471'
ms:contentKeyID: 18118748
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720176(v=WS.10)'
---

Nutzungslizenzen und externe Benutzer
=====================================

RMS ermöglicht Verfassern geschützter Inhalte, diese Inhalte autorisierten externen Benutzern über das Internet zugänglich zu machen. RMS bietet den gleichen Schutz für das Bereitstellen von Inhalten für interne und externe Benutzer, da die mit dem Inhalt assoziierten Rechte über den RMS-Server lizenziert werden müssen. Damit wird Organisationen die gemeinsamen Verwendung von und Zusammenarbeit an vertraulichen Dokumenten, z. B. Verträgen, über das Internet ermöglicht.

Ein externer Benutzer greift normalerweise über das Internet auf RMS zu. (Wenn ein externer Benutzer direkt auf das interne Netzwerk zugreifen kann, beispielsweise über eine VPN-Verbindung, entspricht er in funktioneller Hinsicht einem internen Benutzer). Es ist unerheblich, ob der Benutzer der veröffentlichenden Organisation angehört oder extern ist; das Erwerben einer Lizenz verläuft grundsätzlich nach dem gleichen Muster wie oben unter [Erwerb von Nutzungslizenzen](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac) beschrieben. Zum Anfordern einer Nutzungslizenz muss sich der Benutzer nicht innerhalb des Netzwerks des Autors befinden oder über ein Benutzerkonto dafür verfügen.

Die einzigen Anforderungen lauten:

-   Der Benutzer verfügt über ein gültiges Rechtekontozertifikat.
-   Der Benutzer hat Zugriff auf den RMS-Lizenzierungsserver, der die Veröffentlichungslizenz ausstellte. Dieser Server kann sich sowohl im Intranet als auch im Extranet befinden.
-   Die RMS-Installation, von der das Kontozertifikat des Benutzers ausgestellt wurde, befindet sich auf der Liste der vertrauenswürdigen Benutzerdomänen der RMS-Installation, die die Nutzungslizenz ausstellt.

Folgende Typen externer Benutzer können Nutzungslizenzen erhalten:

-   Benutzer, deren Konto Teil einer anderen Active Directory-Struktur ist, in der sich auch eine RMS-Installation befindet. Die RMS-Installation in der zweiten Struktur muss als vertrauenswürdige Benutzerdomäne für die erste Installation definiert sein.
-   Benutzer einer anderen Organisation, die ebenfalls eine RMS-Installation verwendet, die für die betreffende Installation zur Liste der vertrauenswürdigen Benutzerdomänen hinzugefügt wurde
-   Benutzer, die über Rechtekontozertifikate auf Basis von .NET Passport verfügen, vorausgesetzt, der Microsoft RMS-Zertifizierungsdienst wurde für die betreffende Installation in die Liste vertrauenswürdiger Benutzerdomänen aufgenommen

Eine separate Organisation oder eine andere RMS-Installation von innerhalb der Organisation kann zur Liste der vertrauenswürdigen Benutzerdomänen hinzugefügt werden. Nachdem Sie eine Domäne hinzugefügt haben, können Sie die vertrauenswürdigen E-Mail-Domänen in dieser Domäne definieren und die vertrauenswürdigen Sicherheits-IDs (Security Identifiers oder SIDs) in der Domäne auswählen.

Eine andere Organisation oder eine andere RMS-Installation in Ihrer Organisation kann Ihre RMS-Installation in die Liste der vertrauenswürdigen Benutzerdomänen aufnehmen, so dass die RMS-Server dieser Organisation bzw. Installation Nutzungslizenzanfragen von Ihren Benutzern verarbeiten können.

Weitere Informationen zur Erstellung vertrauenswürdiger Benutzerdomänen zwischen RMS und anderen Organisationen finden Sie nachstehend unter [Vertrauenswürdige Benutzerdomänen](https://technet.microsoft.com/a09b883f-f455-4c46-a4fd-d37b689e1d24) und „Hinzufügen und Entfernen von vertrauenswürdigen Veröffentlichungsdomänen“ in „Betreiben eines RMS-Servers“ in dieser Dokumentensammlung.