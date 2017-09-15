---
TOCTitle: So deinstallieren Sie RMS
Title: So deinstallieren Sie RMS
ms:assetid: '885e3b4f-ea32-466f-9f7f-d8440b0f7c28'
ms:contentKeyID: 18118933
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747587(v=WS.10)'
---

So deinstallieren Sie RMS
=========================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**, um die Seite **Globale Verwaltung** zu öffnen.

Deinstallieren von RMS
----------------------

#### So deinstallieren Sie RMS

1.  Melden Sie sich an dem Server an, auf dem Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) deinstallieren möchten.

    | ![](images/Cc747587.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                                                                                             |
    |-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Wenn Sie RMS von einem Server im Stammzertifizierungscluster entfernen, müssen Sie die Bereitstellung dieses Servers zunächst beenden. Öffnen Sie hierzu die Seite **Globale Verwaltung**, und klicken Sie dann auf **RMS von dieser Website entfernen**. Die Bereitstellung eines Lizenzierungsservers muss nicht beendet werden, bevor RMS auf diesem Server deinstalliert werden kann. |

2.  Klicken Sie in der **Systemsteuerung** auf **Software**.

3.  Klicken Sie im Dialogfeld **Software** auf **Dienste für die Windows-Rechteverwaltung**, und klicken Sie dann auf **Entfernen**, um RMS SP1 zu entfernen.
