---
TOCTitle: 'Schritt 7: Genehmigen und Bereitstellen von Updates in WSUS 3.0'
Title: 'Schritt 7: Genehmigen und Bereitstellen von Updates in WSUS 3.0'
ms:assetid: '88fac442-a9d3-4e74-92f6-3822b7237af1'
ms:contentKeyID: 18127511
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708475(v=WS.10)'
---

Schritt 7: Genehmigen und Bereitstellen von Updates in WSUS 3.0
===============================================================

In diesem Schritt wird ein Update für alle Testclientcomputer in der Testgruppe genehmigt. Die Computer in dieser Gruppe stellen innerhalb der nächsten 24 Stunden eine Verbindung zum WSUS-Server her. Danach können Sie die WSUS-Berichterstattungsfeature verwenden, um festzustellen, ob diese Updates auf den Computern bereitgestellt wurden. Wenn der Test erfolgreich verläuft, können Sie die gleichen Updates dann für die restlichen Computer in Ihrer Organisation genehmigen.

**Schritt 7 umfasst die folgenden Verfahren**:

-   Genehmigen und Bereitstellen eines Updates
-   Überprüfen des Updatestatus

**So genehmigen Sie ein Update und stellen es bereit**
1.  Klicken Sie auf der WSUS-Verwaltungskonsole auf **Updates**. Dadurch wird eine Zusammenfassung der Updates in den Standardansichten angezeigt (**Alle Updates**, **Updates mit hoher Priorität**, **Sicherheitsupdates** und **WSUS-Updates**). Verwenden Sie für dieses Verfahren die Ansicht **Alle Updates**.

2.  Wählen Sie in der Liste die Updates aus, die Sie zum Installieren genehmigen möchten. Informationen zu einem gewählten Update finden Sie im untersten Fenster des Bereichs "Updates". Um mehrere zusammenhängende Updates auszuwählen, halten Sie beim Auswählen der Updates die UMSCHALTTASTE gedrückt. Zur Auswahl mehrerer nicht zusammenhängender Updates halten Sie beim Auswählen STRG gedrückt.

3.  Klicken Sie mit der rechten Maustaste auf die Auswahl, und wählen Sie die Option **Genehmigen** aus. Das Dialogfeld **Updates genehmigen** wird angezeigt.

4.  Wählen Sie eine der Gruppen aus (beispielsweise die Testgruppe), und klicken Sie auf den Pfeil links neben der Gruppe. Ein Kontextmenü mit folgenden Optionen wird angezeigt: **Für die Installation genehmigt**, **Zur Entfernung genehmigt**, **Nicht genehmigt**, **Stichtag**, **Identisch mit übergeordnetem Objekt** und **Für untergeordnete Elemente übernehmen**. Klicken Sie auf die Option **Für die Installation genehmigt**, und klicken Sie anschließend auf **OK**.

5.  Das Fenster **Status der Genehmigung** wird angezeigt. Hier wird der Status der verschiedenen Aufgaben angezeigt, die sich auf die Genehmigung der Updates auswirken. Klicken Sie nach Abschluss der Genehmigung auf **Schließen**, um das Fenster zu schließen.

| ![](images/Cc708475.note(WS.10).gif)Hinweis                                                                      |
|-----------------------------------------------------------------------------------------------------------------------------------------------|
| Zahlreiche Optionen stehen in Verbindung mit dem Genehmigen von Updates, z. B. das Festlegen von Terminen und das Deinstallieren von Updates. |

Nach 24 Stunden können Sie das WSUS-Berichterstattungsfeature verwenden, um festzustellen, ob die Updates auf den Computern bereitgestellt wurden.

**So überprüfen Sie den Status eines Updates**
1.  Klicken Sie in der WSUS-Verwaltungskonsole im linken Fenster auf **Berichte**.

2.  Auf der Seite **Berichte** werden einige Standardberichte angezeigt. Klicken Sie auf die Option **Updatestatus-Zusammenfassung**. Das Fenster **Updatebericht** wird angezeigt.

3.  Wenn Sie die Liste mit Updates filtern möchten, wählen Sie die entsprechenden Kriterien aus (beispielsweise **Updates in folgenden Klassifizierungen einbeziehen**). Klicken Sie anschließend auf der Symbolleiste des Fensters auf **Bericht erstellen**.

4.  Das Fenster **Updatebericht** wird angezeigt. Sie können den Status einzelner Updates überprüfen, indem Sie das Update im linken Bereich des Fensters auswählen. Im letzten Abschnitt des Berichtsfensters wird die Zusammenfassung des Updatestatus angezeigt.

5.  Sie können den Bericht speichern oder drucken. Klicken Sie hierfür in der Symbolleiste auf das entsprechende Symbol.

Wenn die Updates erfolgreich für die Testgruppe bereitgestellt wurden, können Sie die gleichen Updates für die restlichen Computer in Ihrer Organisation bereitstellen.
