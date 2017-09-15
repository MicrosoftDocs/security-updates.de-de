---
TOCTitle: 'Schritt 7: Genehmigen und Bereitstellen von Updates'
Title: 'Schritt 7: Genehmigen und Bereitstellen von Updates'
ms:assetid: '38db25a9-6702-4e43-b536-764e8814afc6'
ms:contentKeyID: 18127416
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720504(v=WS.10)'
---

Schritt 7: Genehmigen und Bereitstellen von Updates
===================================================

In diesem Schritt genehmigen Sie ein Update für alle Testclientcomputer in der Gruppe **Test**. Computer in der Gruppe melden sich innerhalb der nächsten 24 Stunden am WSUS-Server an. Danach können Sie die WSUS-Berichterstattungsfunktion verwenden, um festzustellen, ob diese Updates auf den Computern bereitgestellt wurden. Wenn das Testen erfolgreich verläuft, können Sie dasselbe Update dann für die restlichen Computer in Ihrer Organisation genehmigen.

Schritt 7 umfasst die folgenden Verfahren:

-   Genehmigen und Bereitstellen eines Updates.
-   Überprüfen des Updatestatus-Berichts.

**So genehmigen Sie ein Update und stellen es bereit**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Updates**. Standardmäßig wird die Liste der Updates gefiltert, damit nur wichtige Updates und Sicherheitsupdates angezeigt werden, die für die Ermittlung auf Clientcomputern genehmigt sind. Verwenden Sie für dieses Verfahren den Standardfilter.

2.  Markieren Sie in der Liste der Updates die Updates, die Sie zum Installieren genehmigen möchten. Informationen zu einem markierten Update sind auf der Registerkarte **Details** verfügbar. Um mehrere zusammenhängende Updates zu markieren, halten Sie beim Markieren die Umschalttaste gedrückt. Um mehrere nicht zusammenhängende Updates zu markieren, halten Sie beim Markieren die STRG-Taste gedrückt.

3.  Klicken Sie unter **Updateaufgaben** auf **Genehmigung ändern**. Das Dialogfeld **Updates genehmigen** wird geöffnet.

4.  Klicken Sie in der Liste **Gruppengenehmigungseinstellungen für die ausgewählten Updates** in der Liste der Spalte **Genehmigung** für die Gruppe **Test** auf **Installieren**, und klicken Sie dann auf **OK**.

| ![](images/Cc720504.note(WS.10).gif)Hinweis                                                                                                                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Dem Genehmigen von Updates sind zahlreiche Optionen zugewiesen, z. B. das Festlegen von Stichtagen und das Deinstallieren von Updates. Diese werden im Whitepaper "Microsoft Windows Server Update Services-Betriebshandbuch" (möglicherweise in englischer Sprache) behandelt. |

Nach 24 Stunden können Sie die WSUS-Berichterstattungsfunktion verwenden, um festzustellen, ob diese Updates auf den Computern bereitgestellt wurden.

**So überprüfen Sie den Updatestatus-Bericht**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Berichte**.

2.  Klicken Sie auf der Seite **Berichte** auf **Updatestatus**.

3.  Wenn Sie die Liste der Updates filtern möchten, wählen Sie unter **Ansicht** die gewünschten Kriterien aus, und klicken Sie dann auf **Übernehmen**.

4.  Wenn Sie den Status eines Updates nach Computergruppen und dann nach Computern anzeigen möchten, erweitern Sie die Updateansicht nach Bedarf.

5.  Wenn Sie den Updatestatus-Bericht drucken möchten, klicken Sie unter **Aufgaben** auf **Bericht drucken**.

Wenn die Updates erfolgreich für die Gruppe **Test** bereitgestellt wurden, können Sie dieselben Updates für die restlichen Computer in Ihrer Organisation genehmigen.
