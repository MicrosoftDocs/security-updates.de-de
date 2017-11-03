---
TOCTitle: 'Überprüfen des RMS-Designs'
Title: 'Überprüfen des RMS-Designs'
ms:assetid: '0ed1dd67-8e07-47c9-9e2e-0104438bd19f'
ms:contentKeyID: 18118759
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720185(v=WS.10)'
---

Überprüfen des RMS-Designs
==========================

Stellen Sie vor Beginn der Bereitstellung sicher, dass die folgenden Punkte in Ihrem RMS-Plan berücksichtigt sind:

-   Eine RMS-fähige Clientanwendung wurde ausgewählt, und die entsprechenden Einführungspläne wurden aufgestellt.
-   Es wurde eine Methode für die Verteilung des RMS-Clients bestimmt.
-   Ein Datenbankserver ist installiert und verfügbar.
-   Es wurde eine RMS-Topologie (einfache oder verteilte Topologie) ausgewählt.
-   Active Directory ist auf den Domänencontrollern installiert, auf denen Windows 2000 mit Service Pack 3 (SP3) oder höher installiert ist, und alle Benutzer verfügen über ein Kontaktobjekt mit konfiguriertem E-Mail-Attribut. Windows Server 2003 ist mit den neuesten Aktualisierungen installiert. Message Queuing, Internet Information Services und ASP.NET Version 1.1 sind aktiviert.

> [!NOTE]
> Soll RMS auf einem 64-Bit-Computer installiert werden, beachten Sie die besonderen Konfigurationsanweisungen im Abschnitt „Softwareanforderungen für RMS“ unter „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung. 

-   Die Methoden für den Lastenausgleich und das Server-Failover sind definiert.
-   Die DNS-Registrierung ist für die RMS-Server konfiguriert.
-   Pläne für die Sicherung und Wiederherstellung sind aufgestellt.
-   Die geeigneten Sicherheitsmaßnahmen für Ihr Unternehmen sind vollständig aufgestellt.