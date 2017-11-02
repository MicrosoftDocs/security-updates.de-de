---
TOCTitle: 'Schritt 6: Erstellen einer Computergruppe'
Title: 'Schritt 6: Erstellen einer Computergruppe'
ms:assetid: '6039e5dc-d2ce-4d4b-b737-17ebcadbd4a7'
ms:contentKeyID: 18127468
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720536(v=WS.10)'
---

Schritt 6: Erstellen einer Computergruppe
=========================================

Computergruppen sind ein wichtiger Teil bzw. eine Grundlage der WSUS-Bereitstellungen. Computergruppen ermöglichen Ihnen das gezielte Bereitstellen von Updates für bestimmte Computer. Es gibt zwei Standardcomputergruppen: **Alle Computer** und **Nicht zugeordnete Computer**. Standardmäßig fügt der WSUS-Server jeden Clientcomputer zu diesen beiden Gruppen hinzu, wenn ein Clientcomputer erstmals den WSUS-Server kontaktiert.

Sie können benutzerdefinierte Computergruppen erstellen. Das Erstellen von Computergruppen bietet den Vorteil, dass Sie Updates vor der umfassenden Bereitstellung testen können. Wenn das Testen erfolgreich verläuft, können Sie die Updates für die Gruppe **Alle Computer** bereitstellen. Sie können benutzerdefinierte Gruppen in unbegrenztem Umfang erstellen.

Das Einrichten von Computergruppen wird in drei Schritten durchgeführt. Im ersten Schritt geben Sie an, wie Sie Computer zu den Computergruppen zuweisen möchten. Zwei Optionen stehen zur Verfügung: *Serverseitige Ziele* und *clientseitige Ziele*. Bei serverseitigen Zielen wird jeder Computer mithilfe von WSUS manuell zur entsprechenden Gruppe hinzugefügt. Bei clientseitigen Zielen werden die Clients automatisch mithilfe von Gruppenrichtlinien oder Registrierungsschlüsseln hinzugefügt. Im zweiten Schritt erstellen Sie die Computergruppe in WSUS. Im dritten Schritt verschieben Sie die Computer mithilfe der im ersten Schritt ausgewählten Methode in Gruppen.

In diesem Dokument ist erläutert, wie Sie serverseitige Ziele verwenden und Computer manuell mithilfe der WSUS-Konsole in die Gruppen verschieben. Wenn Sie sehr viele Clientcomputer zu Computergruppen zuweisen müssten, könnten Sie clientseitige Ziele verwenden. Dadurch werden Computer automatisch in Computergruppen verschoben.

Sie können Schritt 6 verwenden, um eine Testgruppe mit mindestens einem Testcomputer einzurichten.

Dieser Schritt umfasst die folgenden Verfahren:

-   Angeben der serverseitigen Ziele.
-   Erstellen einer Gruppe.
-   Verschieben von Computern in die Gruppe.

**So geben Sie die Methode zum Zuweisen von Computern zu Gruppen an**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Optionen** und dann auf **Computeroptionen**.

2.  Klicken Sie im Feld **Computeroptionen** auf **Die Aufgabe "Computer verschieben" in Windows Server Update Services verwenden**.

3.  Klicken Sie unter **Aufgaben** auf **Einstellungen speichern**, und klicken Sie anschließend auf **OK**, wenn das Bestätigungsdialogfeld geöffnet wird.

**So erstellen Sie eine Gruppe**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Computer**.

2.  Klicken Sie unter **Aufgaben** auf **Computergruppe erstellen**.

3.  Geben Sie in das Feld **Gruppenname** den Namen **Test** ein, und klicken Sie auf **OK**.

Verwenden Sie das nachfolgende Verfahren, um einen für das Testen geeigneten Clientcomputer zur Testgruppe zuzuweisen. Für das Testen eignet sich jeder Clientcomputer, dessen Software und Hardware repräsentativ für die Mehrzahl der Computer im Netzwerk sind. Nicht geeignet ist jedoch ein Computer, dem eine wichtige Rolle zugewiesen ist. Sie können so feststellen, ob der Betrieb der mit dem Testcomputer vergleichbaren Computer mit den von Ihnen genehmigten Updates reibungslos verläuft.

**So fügen Sie einen Computer manuell zur Gruppe "Test" hinzu**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Computer**.

2.  Klicken Sie im Feld **Gruppen** auf die Gruppe mit dem Computer, den Sie verschieben möchten.

3.  Klicken Sie in der Liste der Computer auf den Computer, den Sie verschieben möchten.

4.  Klicken Sie unter **Aufgaben** auf **Ausgewählten Computer verschieben**.

5.  Wählen Sie in der Liste **Computergruppe** die Gruppe aus, in die Sie den Computer verschieben möchten, und klicken Sie auf **OK**.
