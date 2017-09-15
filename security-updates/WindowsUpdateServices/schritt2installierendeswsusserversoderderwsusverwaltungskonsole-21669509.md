---
TOCTitle: 'Schritt 2: Installieren des WSUS-Servers oder der WSUS-Verwaltungskonsole'
Title: 'Schritt 2: Installieren des WSUS-Servers oder der WSUS-Verwaltungskonsole'
ms:assetid: '6db6fcb0-c55d-43b9-9b07-4040c6267759'
ms:contentKeyID: 21669509
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939859(v=WS.10)'
---

Schritt 2: Installieren des WSUS-Servers oder der WSUS-Verwaltungskonsole
=========================================================================

Wenn der Server die Mindestsystemanforderungen erfüllt und die erforderlichen Kontoberechtigungen erteilt sind, können Sie Windows Server Upgrade Services 3.0 Service Pack 2 (WSUS 3.0 SP2) installieren. Starten Sie die Installation von WSUS 3.0 SP2 mithilfe des entsprechenden Verfahrens für Ihr Betriebssystem und die Installationsart (mit dem Server-Manager oder der Datei WSUSSetup.exe).

Bei Verwendung des Server-Managers
----------------------------------

**So starten Sie die Installation des WSUS 3.0 SP2-Servers mit dem Server-Manager**
1.  Melden Sie sich auf dem für die Installation von WSUS 3.0 SP2 vorgesehenen Server mit einem Konto an, das Mitglied der lokalen Administratorgruppe ist.

2.  Klicken Sie auf **Start**, zeigen Sie auf **Verwaltung**, und klicken Sie dann auf **Server-Manager**.

3.  Klicken Sie im Bereich "Rollenübersicht" auf der rechten Seite des Fensters "Server-Manager" auf **Rollen hinzufügen**.

4.  Wenn die Seite "Vorbemerkung" angezeigt wird, klicken Sie auf **Weiter**.

5.  Wählen Sie auf der Seite "Serverrollen auswählen" **Windows Server Update Services** aus.

6.  Klicken Sie auf der Seite "Windows Server Update Services" auf **Weiter**.

7.  Klicken Sie auf der Seite "Installationsauswahl bestätigen" auf **Installieren**.

8.  Wenn der Installationsassistent für WSUS 3.0 SP2 gestartet wurde, überspringen Sie den nächsten Abschnitt und gehen Sie zum Verfahren "So setzen Sie die Installation von WSUS 3.0 SP2 fort".

Bei Verwendung der Datei WSUSSetup.exe
--------------------------------------

**So starten Sie die Installation des WSUS 3.0 SP2-Servers oder der WSUS 3.0 SP2-Verwaltungskonsole mit der Datei WSUSSetup.exe**
1.  Melden Sie sich auf dem für die Installation von WSUS 3.0 SP2 vorgesehenen Server mit einem Konto an, das Mitglied der lokalen Administratorgruppe ist.

2.  Doppelklicken Sie auf die Installationsdatei **WSUSSetup.exe**.

3.  Wenn der Installationsassistent für Windows Server Update Services 3.0 SP2 gestartet wurde, gehen Sie zum Verfahren "So setzen Sie die Installation von WSUS 3.0 SP2 fort".

Verwenden des Installationsassistenten für WSUS 3.0 SP2
-------------------------------------------------------

Der WSUS-Installationsassistent wird vom Server-Manager oder von der Datei WSUSSetup.exe gestartet.

**So setzen Sie die Installation von WSUS 3.0 SP2 fort**
1.  Klicken Sie auf der Willkommensseite des Installationsassistenten für Windows Server Update Services 3.0 auf **Weiter**.

2.  Wählen Sie auf der Seite "Auswahl des Installationsmodus" **Vollständige Serverinstallation einschließlich Verwaltungskonsole**, wenn Sie den WSUS-Server auf diesem Computer installieren möchten, oder wählen Sie **Nur Verwaltungskonsole**, wenn nur die Verwaltungskonsole installiert werden soll.

3.  Lesen Sie auf der Seite "Lizenzvertrag" die Bestimmungen des Lizenzvertrags sorgfältig, klicken Sie auf **Ich stimme den Bedingungen des Lizenzvertrags zu** und anschließend auf **Weiter**.

4.  Auf der Seite "Updatequelle auswählen" des Installationsassistenten können Sie festlegen, wo Clients die Updates abrufen sollen. In den Standardeinstellungen ist das Kontrollkästchen **Updates lokal speichern** ausgewählt, und die Updates werden auf dem WSUS-Server am von Ihnen festgelegten Speicherort gespeichert. Wenn Sie das Kontrollkästchen **Updates lokal speichern** deaktivieren, erhalten Clientcomputer durch eine Verbindung zu Microsoft Update genehmigte Updates. Treffen Sie eine Auswahl, und klicken Sie auf **Weiter**.

5.  Wählen Sie auf der Seite "Datenbankoptionen" die Software aus, die zum Verwalten der WSUS 3.0-Datenbank verwendet werden soll. In den Standardeinstellungen schlägt der Installationsassistent die Installation der Windows Internal Database vor.

    Wenn Sie die Windows Internal Database nicht verwenden möchten, müssen Sie eine SQL Server-Instanz für WSUS bereitstellen. Wählen Sie hierfür **Einen vorhandenen Datenbankserver auf diesem Computer verwenden** oder **Einen vorhandenen Datenbankserver auf einem Remotecomputer verwenden**. Geben Sie den Namen der Instanz in das entsprechende Feld ein. Der Instanzname sollte als &lt;*serverName*&gt;\\&lt;*instanceName*&gt; angezeigt werden, wobei *serverName* der Name des Servers und *instanceName* der Name der SQL-Instanz ist. Treffen Sie eine Auswahl, und klicken Sie auf **Weiter**.

6.  Wenn Sie sich auf der Seite **Verbindungsherstellung mit der SQL Server-Instanz** für die Verbindung zu einem SQL-Server entschieden haben, versucht WSUS eine Verbindung zur angegebenen SQL Server-Instanz herzustellen. Klicken Sie auf **Weiter**, wenn die Verbindung erfolgreich hergestellt wurde.

7.  Geben Sie auf der Seite "Websiteauswahl" die Website an, die WSUS verwenden soll. Wenn die Standardwebsite über Port 80 verwendet werden soll, wählen Sie **Die vorhandene IIS-Standardwebsite verwenden**. Wenn Port 80 bereits eine andere Website zugewiesen ist, können Sie eine Alternativseite an Port 8530 erstellen, indem Sie **Neue Windows Server Update Services 3.0 SP2-Website erstellen** auswählen. Klicken Sie auf **Weiter**.

8.  Überprüfen Sie auf der Seite **Microsoft Windows Server Update Services kann jetzt installiert werden** die gewählten Einstellungen, und klicken Sie anschließend auf **Weiter**.

9.  Auf der letzten Seite des Installationsassistenten erfahren Sie, ob die WSUS-Installation erfolgreich abgeschlossen wurde. Wenn Sie auf **Fertig stellen** klicken, wird der Konfigurations-Assistent gestartet.

Nächster Schritt
----------------

[Schritt 3: Konfigurieren der Netzwerkverbindungen](https://technet.microsoft.com/42a144c5-f08e-4a6e-b360-47ddea77bd24)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
