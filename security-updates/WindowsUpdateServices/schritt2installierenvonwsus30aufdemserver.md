---
TOCTitle: 'Schritt 2: Installieren von WSUS 3.0 auf dem Server'
Title: 'Schritt 2: Installieren von WSUS 3.0 auf dem Server'
ms:assetid: '191e62a0-7671-41eb-9841-17c64313fa68'
ms:contentKeyID: 18127389
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720469(v=WS.10)'
---

Schritt 2: Installieren von WSUS 3.0 auf dem Server
===================================================

Nachdem Sie sichergestellt haben, dass Ihre Server den Installationsanforderungen entsprechen, können Sie WSUS 3.0 installieren. Sie müssen sich auf dem für die Installation von WSUS 3.0 vorgesehenen Server mit einem Konto anmelden, das Mitglied der lokalen Administratorgruppe ist. WSUS 3.0 kann nur von Mitgliedern der lokalen Administratorgruppe installiert werden.

Für das folgende Verfahren werden die WSUS-Standardinstallationsoptionen verwendet. Dazu gehören die Installation von Windows Internal Database für die WSUS 3.0-Datenbanksoftware, das lokale Speichern von Updates und das Verwenden der IIS-Standardwebsite mit Port 80.

**So installieren Sie WSUS 3.0**
1.  Doppelklicken Sie auf die Installationsdatei **WSUSSetup.exe**.

2.  Klicken Sie auf der Seite **Willkommen** des Installations-Assistenten auf **Weiter**.

3.  Klicken Sie auf der Seite **Auswahl des Installationsmodus** auf **Vollständige Serverinstallation einschließlich Verwaltungskonsole**, wenn Sie den Server auf diesem Computer installieren möchten, oder klicken Sie auf **Nur Verwaltungskonsole**, wenn nur die Verwaltungskonsole installiert werden soll.

4.  Lesen Sie auf der Seite **Lizenzvertrag** die Bestimmungen des Lizenzvertrags sorgfältig, klicken Sie auf **Ich stimme den Bedingungen des Lizenzvertrags zu** und anschließend auf **Weiter**.

    ![](images/Cc720469.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Auf der Seite **Updatequelle auswählen** des Installations-Assistenten können Sie angeben, wo Clients die Updates abrufen. Wenn Sie das Kontrollkästchen **Updates lokal speichern** aktivieren, werden Updates auf dem WSUS 3.0-Server gespeichert. Wählen Sie anschließend einen Speicherort im Dateisystem zum Speichern der Updates aus. Wenn Sie Updates nicht lokal speichern, stellen Clientcomputer eine Verbindung zu Microsoft Update her, um genehmigte Updates abzurufen. Verwenden Sie die Standardeinstellungen, und klicken Sie auf **Weiter**.

    ![](images/Cc720469.c8bac396-ca39-4491-8b0c-742a0e470535(WS.10).gif)

6.  Wählen Sie auf der Seite **Datenbankoptionen** die Software aus, die zum Verwalten der WSUS 3.0-Datenbank verwendet werden soll. In der Standardeinstellung bietet WSUS-Setup an, Windows Internal Database zu installieren, wenn auf dem Installationscomputer Windows Server 2003 ausgeführt wird.

7.  Wenn Sie Windows Internal Database nicht verwenden möchten, müssen Sie eine SQL Server-Instanz bereitstellen, die von WSUS verwendet werden kann. Klicken Sie dazu auf **Einen vorhandenen Datenbankserver** **auf diesem Computer verwenden**, und geben Sie den Namen der Instanz in das Feld ein. Der Instanzname sollte als &lt;*serverName*&gt;\\&lt;*instanceName*&gt; angezeigt werden, wobei *serverName* der Name des Servers und *instanceName* der Name der SQL-Instanz ist. Treffen Sie eine Auswahl, und klicken Sie auf **Weiter**.

8.  Auf der Seite **Verbindungsherstellung mit der SQL Server-Instanz** versucht WSUS, eine Verbindung zur angegebenen SQL Server-Instanz herzustellen. Klicken Sie auf **Weiter**, wenn die Verbindung erfolgreich hergestellt wurde.

    ![](images/Cc720469.36c6af0c-a61e-4151-ae50-c754a106cb1b(WS.10).gif)

9.  Geben Sie auf der Seite **Websiteauswahl** die Website an, die für WSUS 3.0 verwendet werden soll. Wählen Sie die erste Option aus, wenn Sie die IIS-Standardwebsite mit Port 80 verwenden möchten. Wenn Port 80 bereits eine andere Website zugewiesen ist, können Sie die zweite Option auswählen und eine andere Site für Port 8530 erstellen. Verwenden Sie die Standardeinstellungen, und klicken Sie auf **Weiter**.

10. Überprüfen Sie auf der Seite **Microsoft Windows Server Update Services kann jetzt installiert werden** die gewählten Einstellungen, und klicken Sie anschließend auf **Weiter**.

11. Auf der letzten Seite des Installations-Assistenten wird angezeigt, ob die WSUS 3.0-Installation erfolgreich abgeschlossen wurde. Wenn Sie auf **Fertig stellen** geklickt haben, wird der Konfigurations-Assistent gestartet.
