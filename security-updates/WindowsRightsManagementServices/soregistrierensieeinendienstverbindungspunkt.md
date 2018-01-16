---
TOCTitle: So registrieren Sie einen Dienstverbindungspunkt
Title: So registrieren Sie einen Dienstverbindungspunkt
ms:assetid: '630cc3c3-9ed9-4423-8874-cbaceb43b353'
ms:contentKeyID: 18118869
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720283(v=WS.10)'
---

So registrieren Sie einen Dienstverbindungspunkt
================================================

Registrieren eines Dienstverbindungspunktes
-------------------------------------------

Wenn Sie die Registrierung eines Dienstverbindungspunkts (Service Connection Point oder SCP) auf einem Server mit RMS ausführen, der sich in einer Unterdomäne befindet, wird möglicherweise eine Fehlermeldung angezeigt, die besagt, dass die Registrierung fehlgeschlagen ist. In vielen Fällen war die Registrierung dennoch erfolgreich. Die Registrierung wird jedoch zuerst in der Domäne der höchsten Ebene ausgeführt, so dass es einige Zeit dauern kann, bis die Replikation auf der Subdomäne, wo der Server mit RMS nach dem SCP-Objekt sucht, ausgeführt wurde. Sobald der Dienstverbindungspunkt auf allen globalen Katalogservern in der Gesamtstruktur repliziert wurde, wird diese Meldung nicht mehr angezeigt. Wenn Sie diese Meldung erhalten, sollten Sie einige Zeit mit der Fehlerbehebung warten. Möglicherweise besteht das Problem dann schon nicht mehr.

#### So registrieren Sie einen Dienstverbindungspunkt

1.  Melden Sie sich an dem Server, auf dem ein Dienstverbindungspunkt registriert werden soll, mithilfe eines Domänenkontos an. Dieses sollte über ausreichende Berechtigungen verfügen, um ein Containerobjekt unterhalb des Services-Containers im Konfigurationscontainer der Active Directory-Gesamtstruktur zu erstellen. Die vordefinierte Sicherheitsgruppe **Organisations-Admins** ist ein Beispiel für ein Konto mit den erforderlichen Berechtigungen.

2.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann auf die Verknüpfung **RMS auf dieser Website verwalten**.

3.  Klicken Sie auf der **Verwaltungsstartseite** auf die Verknüpfung **RMS-Dienstverbindungspunkt**.

4.  Klicken Sie auf der Seite **RMS-Dienstverbindungspunkt** auf die Schaltfläche **URL registrieren**.