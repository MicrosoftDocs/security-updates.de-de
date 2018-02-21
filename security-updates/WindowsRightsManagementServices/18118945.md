---
TOCTitle: 'Active Directory-Unterstützung für RMS'
Title: 'Active Directory-Unterstützung für RMS'
ms:assetid: '9589127d-19b3-44f1-b7a1-01992e78218a'
ms:contentKeyID: 18118945
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747604(v=WS.10)'
---

Active Directory-Unterstützung für RMS
======================================

RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendet Active Directory für folgende Zwecke:

-   **Bereitstellen von Benutzerauthentifizierung.** Active Directory stellt die Verzeichnisdienste bereit, die zur Authentifizierung der RMS-Benutzer dienen. Weitere Informationen zur Authentifizierung und RMS finden Sie unter „[RMS-Sicherheitsmodell](https://technet.microsoft.com/665db831-366d-4dca-9bb3-cc2912481fe1)“ weiter unten in diesem Thema.
-   **Auflösen der Gruppenmitgliedschaft und einzelner Benutzerkonto-IDs.** Active Directory stellt die Informationen zur Gruppenmitgliedschaft bereit, die RMS beim Erteilen von Nutzungslizenzen für RMS-geschützten Inhalt verwendet, wenn sich die von der Veröffentlichungslizenz erteilten Rechte nicht auf einzelne Benutzerkonten, sondern auf Gruppen beziehen. Um die Anzahl der an Active Directory gestellten LDAP-Abfragen zu verringern, speichert RMS die ermittelten Informationen in einem lokalen Cache sowie in einer zentralen Datenbank der Verzeichnisdienste. Weitere Informationen hierzu finden Sie unter „[Active Directory-Cache für RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)“ und „[Datenbank der RMS-Verzeichnisdienste](https://technet.microsoft.com/6f6b8586-5d17-4a40-94a3-4dc738195301)“ weiter oben in diesem Thema.
-   **Speichern des Pfads für die Suche nach RMS-Diensten.** Dienstanforderungen (wie z. B. für eine Nutzungslizenz, eine Veröffentlichungslizenz oder die Unterregistrierung eines Lizenzierungsservers) müssen an den URL für das ausführbare Modul des Webdienstes gesendet werden, der die Anforderung verarbeitet. Alle Dienstanforderungen beginnen mit einer Active Directory-Abfrage zum URL des Serverwebdienstes (Server.asmx), wodurch der entsprechende URL für die Dienstanforderung bereitgestellt wird. Weitere Informationen hierzu finden Sie unter „[Veröffentlichung und Suche von RMS-Diensten](https://technet.microsoft.com/336c0d55-fd7f-4aa9-b3e6-bfd6565b1086)“ weiter unten in diesem Thema.