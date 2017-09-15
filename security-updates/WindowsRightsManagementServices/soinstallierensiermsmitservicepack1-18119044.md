---
TOCTitle: So installieren Sie RMS mit Service Pack 1
Title: So installieren Sie RMS mit Service Pack 1
ms:assetid: 'dab20175-a690-43f8-b943-768d289daa0d'
ms:contentKeyID: 18119044
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747689(v=WS.10)'
---

So installieren Sie RMS mit Service Pack 1
==========================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Der Computer, auf dem Sie RMS installieren, muss Mitglied in einer Domäne oder ein Domänencontroller sein. Sie können RMS nicht auf einem eigenständigen Server in einer Arbeitsgruppe bereitstellen.

| ![](images/Cc747689.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Stellen Sie RMS nicht auf anderen Servern bereit, bevor Sie die Installation und die Bereitstellung des ersten Stammzertifizierungsservers abgeschlossen haben. Informationen hierzu finden Sie nachstehend unter [So stellen Sie den ersten Stammzertifizierungsserver bereit](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2), [So stellen Sie einen Lizenzierungsserver bereit](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e) oder unter [So fügen Sie einen Server zu einem Cluster hinzu](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733). |

| ![](images/Cc747689.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                 |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| RMS SP1 kann auf einem Server installiert werden, auf dem aktuell die vorherige Version von RMS ausgeführt wird. Wenn Sie RMS jedoch außer Betrieb gesetzt haben, muss RMS in der Systemsteuerung im Menüpunkt „Software“ vollständig entfernt werden, bevor Sie RMS SP1 installieren können. |

Installieren von RMS mit Service Pack 1
---------------------------------------

#### So installieren Sie RMS mit Service Pack 1

1.  Melden Sie sich bei dem Server, auf dem Sie RMS SP1 installieren möchten, mit einem Domänenkennwort an, das Mitglied in der lokalen Administratorengruppe ist.

2.  Wenn das Dialogfeld **Willkommen** angezeigt wird, überprüfen Sie die Liste der zu installierenden Software, und klicken Sie dann auf **Weiter**.

3.  Lesen Sie im Dialogfeld **Lizenzvertrag** den Vertrag, und wählen Sie **Ich stimme zu** aus. Klicken Sie dann auf **Weiter**.

4.  Akzeptieren Sie unter **Ordner** den Standardordner, oder geben Sie einen neuen Ordner an. Klicken Sie dann auf **Weiter**.

5.  Klicken Sie im Dialogfeld **Installation bestätigen** auf **Installieren**, um die Installation zu starten.

6.  Wenn das Dialogfeld **Installation beendet** angezeigt wird, klicken Sie auf **Schließen**.

    | ![](images/Cc747689.note(WS.10).gif)Hinweis                                                                                       |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Bei einer Fehlermeldung, die besagt, dass die Anwendung neu gestartet wird, aktualisieren Sie in Microsoft Internet Explorer die Seite **Globale Verwaltung**. |

Sie können RMS außerdem über eine Eingabeaufforderung installieren. Weitere Informationen hierzu finden Sie nachstehend unter „[RMS-Serverinstallation mithilfe einer Eingabeaufforderung](https://technet.microsoft.com/b55b1e2a-dd14-4168-a37f-9cdedbec660b)“.
