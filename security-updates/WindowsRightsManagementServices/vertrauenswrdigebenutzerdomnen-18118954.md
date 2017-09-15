---
TOCTitle: Vertrauenswürdige Benutzerdomänen
Title: Vertrauenswürdige Benutzerdomänen
ms:assetid: 'a09b883f-f455-4c46-a4fd-d37b689e1d24'
ms:contentKeyID: 18118954
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747618(v=WS.10)'
---

Vertrauenswürdige Benutzerdomänen
=================================

Standardmäßig erteilt RMS (Rights Management Services oder Dienste für die Rechteverwaltung) keine Nutzungslizenzen an Benutzer, deren Rechtekontozertifikate von einer anderen Benutzerdomäne ausgestellt wurden. Eine Benutzerdomäne ist eine RMS-Installation, die aus einem Stammzertifizierungscluster, optionalen Lizenzierungsservern oder -clustern und zugeordneten Datenbanken besteht.

Sie können RMS für die Verarbeitung dieser Art von Anforderungen konfigurieren, indem Sie das Server-Lizenzgeberzertifikat einer anderen Benutzerdomäne importieren und der Liste der vertrauenswürdigen Benutzerdomänen hinzufügen. Bei dieser Konfiguration können Benutzer, deren Kontozertifikate von der vertrauenswürdigen Benutzerdomäne ausgestellt wurden, Anforderungen für Nutzungslizenzen an Ihre Installation senden. Diese Nutzungslizenzen werden genauso verarbeitet, als ob sie Anforderungen interner Benutzer wären.

| ![](images/Cc747618.note(WS.10).gif)Hinweis                                                                                                          |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Der Stammzertifizierungscluster wird automatisch in der Liste der vertrauenswürdigen Benutzerdomänen für alle RMS-Server aufgeführt, die sich in derselben Installation befinden. |

Sie können Benutzern aus verschiedenen Benutzerdomänen die gemeinsame Verwendung von geschützten Inhalten ermöglichen. Dies wird in den folgenden Beispielen beschrieben:

-   Ihre Organisation arbeitet mit einer anderen Organisation an vertraulichen Dokumenten eng zusammen, die Sie freigeben und schützen möchten. Die andere Organisation führt ebenfalls ein RMS-System aus. Die beiden Organisationen können die RMS-Installation der jeweils anderen Organisation ihrer Liste der vertrauenswürdigen Benutzerdomänen hinzufügen, so dass Benutzer aus beiden Organisationen gemeinsam an geschütztem Inhalt arbeiten und ihn über das Internet oder ein Extranet austauschen können.
-   Sie können immer nur jeweils eine RMS-Installation in einer Active Directory-Gesamtstruktur haben. In Ihrer Organisation sind mehrere Active Directory-Gesamtstrukturen implementiert und in jeder wird RMS ausgeführt. Benutzer möchten geschützte Inhalte mit anderen Benutzern gemeinsam verwenden – unabhängig davon, in welcher Gesamtstruktur sich diese befinden. Um dies zu ermöglichen, können Sie die RMS-Installationen der anderen Gesamtstrukturen der Liste der vertrauenswürdigen Benutzerdomänen hinzufügen, die in den jeweiligen Gesamtstrukturen vorhanden sind.
-   Benutzer in Ihrer Organisation arbeiten mit Benutzern in einer anderen Organisation an vertraulichen und zu schützenden Dokumenten zusammen. Die andere Organisation führt kein RMS-System aus. Benutzer in der anderen Organisation können .NET Passport-Konten einrichten, und Sie können .NET Passport zur Liste der vertrauenswürdigen Benutzerdomänen für Ihre RMS-Installation hinzufügen. Nun können die Benutzer in beiden Organisationen an geschützten Inhalten arbeiten und diese über das Internet austauschen.

Weitere Informationen zu vertrauenswürdigen Benutzerdomänen sowie schrittweise Anleitungen finden Sie unter „Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen“ und „Einrichten von Vertrauensrichtlinien“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.
