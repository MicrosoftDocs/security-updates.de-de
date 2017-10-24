---
TOCTitle: So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu
Title: So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu
ms:assetid: 'ed672e58-6272-4ac0-a434-d1d938037e93'
ms:contentKeyID: 18119089
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747793(v=WS.10)'
---

So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu
========================================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Hinzufügen von vertrauenswürdigen Benutzerdomänen
-------------------------------------------------

#### So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie eine vertrauenswürdige Benutzerdomäne hinzufügen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vertrauensrichtlinien**.

3.  Klicken Sie im Bereich **Vertrauenswürdige Benutzerdomänen** auf **Durchsuchen**, suchen Sie das Server-Lizenzgeberzertifikat der Benutzerdomäne, das Sie zum Einrichten der Vertrauensstellung importieren möchten, und doppelklicken Sie darauf. Klicken Sie dann auf **Hinzufügen**.

    Der Name der Domäne wird in der Liste **Vertrauenswürdige Benutzerdomänen** angezeigt.

4.  Um anzugeben, welche E-Mail-Domänen innerhalb der vertrauenswürdigen Benutzerdomäne vertrauenswürdig sind, klicken Sie neben dem Zertifikatsnamen in der Liste auf **Vertrauenswürdige Domänen**, um das Fenster **Vertrauenswürdige E-Mail-Domänen** zu öffnen.

5.  Wählen Sie eine der folgenden Optionen für die Vertrauensstellungen aus:

    -   Wählen Sie die Option **Allen E-Mail-Domänen vertrauen** aus, um allen Benutzerkonten zu vertrauen, die Mitglied dieser Domäne sind.

        – oder –

    -   Wählen Sie die Option **Nur angegebenen E-Mail-Domänen vertrauen**, geben Sie dann den als vertrauenswürdig einzustufenden Domänennamen ein, z. B. Beispiel.com, und klicken Sie auf **Hinzufügen**. Dadurch wird die Domäne zur Liste Vertrauenswürdige E-Mail\_Domänen hinzugefügt. Zum Entfernen eines Namens aus der Liste wählen Sie den Namen aus, und klicken Sie dann auf **Entfernen**. Eine aufgelistete Domäne schließt alle zugehörigen Unterdomänen ein.

6.  Wenn Sie RMS in einer Umgebung verwenden, in der Sie die Gruppenmitgliedschaft gesamtstrukturübergreifend erweitern müssen, aktivieren Sie das Kontrollkästchen **RM-Lizenzierungen an Sicherheits-ID (SIDs) für diese Benutzerdomäne vertrauen**.

7.  Klicken Sie nach Abschluss des Verfahrens auf **Fenster schließen und zu Vertrauensrichtlinien zurückkehren**.

Weitere Informationen zum Ausführen dieses Verfahrens finden Sie oben unter [Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1).