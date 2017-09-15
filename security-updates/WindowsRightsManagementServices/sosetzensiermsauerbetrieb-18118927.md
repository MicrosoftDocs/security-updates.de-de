---
TOCTitle: So setzen Sie RMS außer Betrieb
Title: So setzen Sie RMS außer Betrieb
ms:assetid: '8b563c25-17cd-4b9b-ae42-695497ab6439'
ms:contentKeyID: 18118927
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747665(v=WS.10)'
---

So setzen Sie RMS außer Betrieb
===============================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

| ![](images/Cc747665.Warning(WS.10).gif)Warnung                                                                                                          |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie einen Server außer Betrieb setzen, kann dieser nicht mehr in einer RMS-Standardkonfiguration wiederhergestellt werden. Dieser Vorgang kann nicht rückgängig gemacht werden. |

| ![](images/Cc747665.Warning(WS.10).gif)Warnung                                                                                                                   |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nachdem RMS außer Betrieb gesetzt wurde, muss RMS in der Systemsteuerung über die Funktion „Software“ vollständig entfernt werden, bevor Sie eine andere Instanz von RMS installieren können. |

Außerbetriebsetzung von RMS
---------------------------

#### So setzen Sie RMS außer Betrieb

1.  Melden Sie sich an dem Server an, auf dem Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) außer Betrieb setzen möchten.

2.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann auf die Verknüpfung **RMS auf dieser Website verwalten**.

3.  Klicken Sie auf der **Verwaltungsstartseite** auf die Verknüpfung **Sicherheitseinstellungen**.

4.  Aktivieren Sie im Bereich **RMS außer Betrieb setzen** das Kontrollkästchen **Außerbetriebsetzung der RMS-Installation aktivieren**, und klicken Sie dann auf **Außerbetriebsetzen**.

5.  Wenn Sie dazu aufgefordert werden, klicken Sie auf **OK**, um zu bestätigen, dass die RMS-Installation dauerhaft außer Betrieb gesetzt werden soll.
