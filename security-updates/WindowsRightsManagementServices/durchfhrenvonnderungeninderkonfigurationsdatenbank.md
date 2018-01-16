---
TOCTitle: Durchführen von Änderungen in der Konfigurationsdatenbank
Title: Durchführen von Änderungen in der Konfigurationsdatenbank
ms:assetid: '6a7bec73-09e4-4060-b551-5990836df4bc'
ms:contentKeyID: 18118864
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747606(v=WS.10)'
---

Durchführen von Änderungen in der Konfigurationsdatenbank
=========================================================

Mithilfe der Verwaltungswebsite durchgeführte Konfigurationsänderungen werden in der Konfigurationsdatenbank des Servers oder Clusters widergespiegelt. Konfigurationseinstellungen sollten unbedingt auf der Verwaltungswebsite und nicht manuell in der Konfigurationsdatenbank geändert werden. Es können jedoch zwei Situationen eintreten, in denen Sie die Datenbank manuell ändern müssen:

-   **Verschieben der Protokollierungsdatenbank auf einen anderen Server.** Die Protokollierungsdatenbank wird standardmäßig auf dem gleichen Server wie die Konfigurationsdatenbank installiert. Wenn Sie sie aber auf einen anderen Server verschieben möchten, müssen Sie die Konfigurationsdatenbank so ändern, dass sie auf den neuen Speicherort verweist. Weitere Informationen zum Verschieben einer Protokollierungsdatenbank, einschließlich Informationen zum Aktualisieren des Speicherortes in der Konfigurationsdatenbank, finden Sie oben unter „[Verschieben der Protokollierungsdatenbank](https://technet.microsoft.com/34ea8045-dc94-422e-9601-29927cfc1534)“.
-   **Entfernen von Benutzerschlüsseln, die Rechtekontozertifikaten zugeordnet sind** Wenn Sie ein Benutzerkonto über die Verwaltungswebsite aus Active Directory entfernen oder ein Rechtekontozertifikat ausschließen oder sperren möchten, werden die dem Rechtekontozertifikat zugeordneten Benutzerschlüssel aus der Konfigurationsdatenbank nicht entfernt. Sie müssen inaktive Benutzerschlüssel sowohl aus Sicherheitsgründen als auch zum Nachverfolgen der Anzahl von Clientzugriffslizenzen (Client Access Licenses oder CAL) manuell aus der Konfigurationsdatenbank entfernen. Weitere Informationen zum Entfernen von Benutzerschlüsseln aus der Konfigurationsdatenbank finden Sie unter „[Löschen von Benutzerkonten](https://technet.microsoft.com/bf73b141-d4d1-4807-a773-3aaff58b0db6)“ weiter oben in diesem Thema. Weitere Informationen zum Nachverfolgen von CALs finden Sie unter „[Nachverfolgen von Rechtekontozertifikaten](https://technet.microsoft.com/5bb0f3cf-fc44-4e60-a93f-c789d6f8a902)“ weiter oben in diesem Thema.

Wenn Sie Änderungen direkt an einer Konfigurationsdatenbank vornehmen möchten, wenden Sie sich an den Datenbankserver-Administrator.