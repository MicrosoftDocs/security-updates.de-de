---
TOCTitle: 'Schritt 6: Konfigurieren von Computergruppen'
Title: 'Schritt 6: Konfigurieren von Computergruppen'
ms:assetid: '70518732-2179-4e41-9609-7f9999867f41'
ms:contentKeyID: 21669510
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939860(v=WS.10)'
---

Schritt 6: Konfigurieren von Computergruppen
============================================

Computergruppen sind ein wichtiger Punkt bei der Bereitstellung von Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2). Computergruppen ermöglichen das Testen und gezielte Bereitstellen von Updates für bestimmte Computer. Es gibt zwei Standardcomputergruppen: "Alle Computer" und "Nicht zugewiesene Computer". In der Standardeinstellung wird jeder Clientcomputer vom Server beiden Gruppen zugeordnet, sobald der Clientcomputer zum ersten Mal eine Verbindung mit dem WSUS-Server herstellt.

Sie können so viele benutzerdefinierte Computergruppen erstellen, wie es für das Verwalten von Updates in Ihrer Organisation erforderlich ist. Am besten erstellen Sie mindestens eine Computergruppe für das Testen von Updates, bevor diese für andere Computer in der Organisation bereitgestellt werden.

Verfahren in Schritt 6
----------------------

1.  Erstellen einer Testcomputergruppe
2.  Verschieben von mindestens einem Computer in die Testgruppe

**So erstellen Sie eine Testgruppe**
1.  Erweitern Sie **Computer** in der WSUS-Verwaltungskonsole, und wählen Sie **Alle Computer**.

2.  Klicken Sie mit der rechten Maustaste auf **Alle Computer**, und klicken Sie auf **Computergruppe hinzufügen**.

3.  Geben Sie im Dialogfeld **Computergruppe hinzufügen** den **Namen** der neuen Testgruppe an, und klicken Sie auf **Hinzufügen**.

Mithilfe des folgenden Verfahrens weisen Sie der Testgruppe einen Clientcomputer zu. Ein Testcomputer ist jeder Computer, dessen Soft- und Hardware mit der Mehrheit der Clientcomputer im Netzwerk übereinstimmt, dem allerdings keine kritische Rolle zugewiesen wurde. Nach erfolgreichem Abschluss der Tests können Sie die Updates für Computer einer beliebigen Gruppe genehmigen.

**So weisen Sie der Testgruppe einen Computer zu**
1.  Klicken Sie in der WSUS-Verwaltungskonsole auf **Computer**.

2.  Klicken Sie auf die Gruppe des Computers, welcher der Testgruppe zugewiesen werden soll.

3.  Wählen Sie in der Liste den oder die Computer aus, die der Testgruppe zugewiesen werden sollen.

4.  Klicken Sie mit der rechten Maustaste auf **Mitgliedschaft ändern**.

5.  Wählen Sie im Dialogfeld **Gruppenmitgliedschaft für Computer festlegen** die zuvor erstellte Testgruppe aus, und klicken Sie anschließend auf **OK**.

Wiederholen Sie diese beiden Verfahren, d. h. erstellen Sie eine Gruppe und weisen Sie ihr einen oder mehrere Computer zu, um so viele Computergruppen zu erstellen, wie für das Verwalten der Updates erforderlich sind.

Nächster Schritt
----------------

[Schritt 7: Genehmigen und Bereitstellen von WSUS-Updates](https://technet.microsoft.com/c4e58e17-d5e3-4194-8f26-b459e0c03b86)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
