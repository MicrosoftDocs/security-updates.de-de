---
TOCTitle: 'Verwenden der Seite „Globale Verwaltung“'
Title: 'Verwenden der Seite „Globale Verwaltung“'
ms:assetid: '57bbf402-2351-4dee-823c-27f4dd32447c'
ms:contentKeyID: 18118842
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747575(v=WS.10)'
---

Verwenden der Seite „Globale Verwaltung“
========================================

Auf der Seite **Globale Verwaltung** der Verwaltungswebsite können Sie einen Server mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) bereitstellen und seine Bereitstellung beenden sowie das RMS-Dienstkonto ändern.

Führen Sie die folgenden Schritte aus, um von dem zu verwaltenden Server Zugriff auf diese Website zu erhalten:

1.  Melden Sie sich als lokaler Administrator an.
2.  Klicken Sie auf **Start,** zeigen Sie auf **Alle Programme**, zeigen Sie auf **Windows RMS**, und klicken Sie dann auf **Windows RMS-Verwaltung**.

Der Zugriff von einem Browser auf einem Remotecomputer auf die Seite **Globale Verwaltung** ist nicht möglich.

Wenn der Server, von dem Sie auf die Seite **Globale Verwaltung** zugreifen, noch nicht bereitgestellt wurde, werden für jede auf dem Server ausgeführte Website die folgenden Optionen angezeigt:

-   **RMS auf dieser Website bereitstellen**. Klicken Sie auf diese Verknüpfung, wenn es sich um den ersten Server handelt, den Sie in diesem Cluster bereitstellen möchten. Damit wird der Bereitstellungsprozess gestartet. Während dieses Prozesses werden RMS-Ressourcen installiert, wie z. B. virtuelle Verzeichnisse. Darüber hinaus werden die Datenbanken auf dem Datenbankserver installiert. Weitere Informationen hierzu finden Sie nachstehend unter „[So stellen Sie den ersten Stammzertifizierungsserver bereit](https://technet.microsoft.com/debc42f3-74ff-4c99-b7a4-4921fccdabc2)“.
-   **Diesen Server zu einem Cluster hinzufügen**. Klicken Sie auf diese Verknüpfung, wenn Sie den Server bereitstellen und zu einem vorhandenen Cluster hinzufügen möchten. Sie können einen Server entweder zum Stammzertifizierungsserver oder zu einem Lizenzierungsserver hinzufügen. RMS-Ressourcen werden installiert, wie z. B. virtuelle Verzeichnisse. Allerdings werden die Datenbanken nicht erstellt, weil dieser Server die Clusterdatenbanken verwendet. Weitere Informationen hierzu finden Sie nachstehend unter „[So fügen Sie einen Server zu einem Cluster hinzu](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733)“.

Wenn Sie von einem bereits bereitgestellten Server auf die Seite **Globale Verwaltung** zugreifen, werden die folgenden Optionen angezeigt:

-   **RMS auf dieser Website verwalten.** Klicken Sie auf diese Verknüpfung, um die Seite „Clusterverwaltung“ anzuzeigen. Weitere Informationen finden Sie nachstehend unter „[Verwenden der Verwaltungsstartseite](https://technet.microsoft.com/6c155977-bd0e-47d6-ac65-1746cddb505e)“.
-   **RMS-Dienstkonto ändern.** Klicken Sie auf diese Verknüpfung, um ein anderes RMS-Dienstkonto anzugeben, unter dem RMS ausgeführt werden soll. Weitere Informationen finden Sie nachstehend unter „[Ändern des RMS-Dienstkontos](https://technet.microsoft.com/f257d66d-b823-41e4-bcb7-7c90eb295238)“.
-   **RMS von dieser Website entfernen.** Klicken Sie auf diese Verknüpfung, um die Bereitstellung von RMS zu beenden. Beim Beenden der Bereitstellung von RMS werden die virtuellen Verzeichnisse und Anwendungen von RMS von diesem Server entfernt. RMS wird jedoch nicht deinstalliert. Weitere Informationen finden Sie nachstehend unter „[So deinstallieren Sie RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)“.

> [!NOTE]
> Einige Funktionen können auf der RMS-Verwaltungswebsite in Popup-Fenstern konfiguriert werden. Wenn Sie in Ihrem Webbrowser Popup-Blocker verwenden, sollten Sie Ihre Browsereinstellungen dahingehend ändern, dass Popup-Fenster der RMS-Verwaltungswebsite zugelassen werden. 
