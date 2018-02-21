---
TOCTitle: 'Schritt 6: Erstellen einer Computergruppe für Updates'
Title: 'Schritt 6: Erstellen einer Computergruppe für Updates'
ms:assetid: 'fe219654-eae8-45ca-a44b-c1e05c3c3e93'
ms:contentKeyID: 18127660
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708629(v=WS.10)'
---

Schritt 6: Erstellen einer Computergruppe für Updates
=====================================================

Computergruppen sind ein wichtiger Teil bzw. eine Grundlage der WSUS-Bereitstellungen. Computergruppen ermöglichen Ihnen das gezielte Bereitstellen von Updates für bestimmte Computer. Es gibt zwei Standardcomputergruppen: "Alle Computer" und "Nicht zugeordnete Computer". In der Standardeinstellung wird jeder Clientcomputer vom Server beiden Gruppen zugeordnet, sobald der Clientcomputer zum ersten Mal eine Verbindung mit dem WSUS-Server herstellt.

Sie können benutzerdefinierte Computergruppen erstellen. Das Erstellen von Computergruppen bietet den Vorteil, dass Sie Updates vor der umfassenden Bereitstellung testen können. Wenn der Test erfolgreich verläuft, können Sie die Updates für die Gruppe "Alle Computer" bereitstellen. Sie können benutzerdefinierte Gruppen in unbegrenztem Umfang erstellen.

**So richten Sie Computergruppen ein**
1.  Legen Sie fest, wie Sie die Computer den Computergruppen zuweisen möchten. Zwei Optionen stehen zur Verfügung: serverseitige Zielzuordnung und clientseitige Zielzuordnung. Bei serverseitiger Zielzuordnung wird jeder Computer mithilfe von WSUS manuell zur entsprechenden Gruppe hinzugefügt. Bei clientseitiger Zielzuordnung werden die Clients automatisch mithilfe von "Gruppenrichtlinien" oder Registrierungsschlüsseln hinzugefügt.

2.  Erstellen Sie die Computergruppe unter WSUS.

3.  Verschieben Sie die Computer mithilfe der im ersten Schritt ausgewählten Methode in Gruppen.

In diesem Abschnitt wird erläutert, wie Sie die serverseitige Zielzuordnung verwenden und Computer manuell mithilfe der WSUS-Verwaltungskonsole in die Gruppen verschieben. Wenn Sie den Computergruppen mehrere Clientcomputer zuweisen möchten, können Sie die clientseitige Zielzuordnung verwenden. Dadurch werden Computer automatisch in Computergruppen verschoben.

Sie können Schritt 6 verwenden, um eine Testgruppe mit mindestens einem Testcomputer einzurichten.

**Schritt 6 umfasst die folgenden Verfahren:**

-   Erstellen einer Gruppe
-   Hinzufügen eines Computers zu der Gruppe

**So erstellen Sie eine Gruppe**
1.  Erweitern Sie **Computer** in der WSUS-Verwaltungskonsole, und wählen Sie **Alle Computer** aus.

2.  Klicken Sie mit der rechten Maustaste auf **Alle Computer**, oder klicken Sie im Fenster **Aktionen** auf **Computergruppe hinzufügen**.

3.  Das Dialogfeld **Computergruppe hinzufügen** wird angezeigt. Geben Sie den Namen der neuen Gruppe an.

Mithilfe des folgenden Verfahrens weisen Sie einen Clientcomputer der Testgruppe zu. Für das Testen eignet sich jeder Clientcomputer, dessen Software und Hardware repräsentativ für die Mehrzahl der Computer im Netzwerk sind. Nicht geeignet ist jedoch ein Computer, dem eine wichtige Rolle zugewiesen ist. Auf diese Weise können Sie feststellen, ob der Betrieb der mit dem Testcomputer vergleichbaren Computer mit den von Ihnen genehmigten Updates reibungslos verläuft.

**So fügen Sie einen Computer zu der Gruppe hinzu**
1.  Klicken Sie in der WSUS-Verwaltungskonsole auf **Computer**.

2.  Klicken Sie auf die Gruppe mit dem Computer, den Sie verschieben möchten.

3.  Wählen Sie den Computer, den Sie verschieben möchten, aus der Liste der Computer aus.

4.  Klicken Sie mit der rechten Maustaste auf **Mitgliedschaft ändern**.

5.  Im angezeigten Dialogfeld **Gruppenmitgliedschaft für Computer festlegen** finden Sie eine Liste von Gruppen.

6.  Markieren Sie die Gruppe, in die Sie den Computer verschieben möchten, und klicken Sie anschließend auf **OK**.
