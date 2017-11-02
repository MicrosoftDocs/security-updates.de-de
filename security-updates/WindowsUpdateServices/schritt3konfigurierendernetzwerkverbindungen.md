---
TOCTitle: 'Schritt 3: Konfigurieren der Netzwerkverbindungen'
Title: 'Schritt 3: Konfigurieren der Netzwerkverbindungen'
ms:assetid: '42a144c5-f08e-4a6e-b360-47ddea77bd24'
ms:contentKeyID: 21669453
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939815(v=WS.10)'
---

Schritt 3: Konfigurieren der Netzwerkverbindungen
=================================================

Nach der Installation von Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) wird der Konfigurationsassistent automatisch gestartet. Sie können den Assistenten auch später über die Seite **Optionen** der WSUS-Verwaltungskonsole ausführen.

Bevor Sie mit dem Konfigurationsvorgang beginnen, sollten folgende Fragen geklärt sein:

1. Ist die Firewall des Servers so konfiguriert, dass Clients auf den Server zugreifen können?

2. Kann dieser Computer eine Verbindung zum Upstreamserver herstellen (beispielsweise Microsoft Update)?

3. Verfügen Sie über den Namen des Proxyservers und die Anmeldeinformationen für den Proxyserver, sofern diese benötigt werden?

In der Standardeinstellung ist WSUS 3.0 SP2 so konfiguriert, dass Microsoft Update als Speicherort verwendet wird, von dem Updates abgerufen werden. Wenn Sie in Ihrem Netzwerk über einen Proxyserver verfügen, können Sie WSUS 3.0 SP2 so konfigurieren, dass dieser Proxyserver verwendet wird. Wenn sich zwischen WSUS und dem Internet eine Unternehmensfirewall befindet, müssen Sie die Firewall unter Umständen neu konfigurieren, um sicherzustellen, dass WSUS Updates erhalten kann.

 
> [!NOTE]
> Zum Herunterladen von Updates von Microsoft Update benötigen Sie eine Internetverbindung. WSUS bietet Ihnen jedoch auch die Möglichkeit, Updates in Netzwerke ohne Internetverbindung zu importieren.
 

Schritt 3 umfasst die folgenden Verfahren:

-   Konfigurieren der Firewall
-   Angeben, wie dieser Server Updates abrufen soll (entweder von Microsoft Update oder von einem anderen WSUS-Server)
-   Konfigurieren der Proxyservereinstellungen, damit WSUS Updates abrufen kann

**So konfigurieren Sie die Firewall**
-   Wenn sich zwischen WSUS und dem Internet eine Unternehmensfirewall befindet, müssen Sie diese möglicherweise konfigurieren, damit WSUS Updates abrufen kann. Der WSUS-Server verwendet Port 80 für das Protokoll HTTP und Port 443 für HTTPS, um Updates von Microsoft Update zu erhalten. Diese Einstellung ist nicht konfigurierbar.

-   Wenn Ihre Organisation nicht zulässt, dass Port 80 und Port 443 für alle Adressen geöffnet sind, können Sie den Zugriff auf die folgenden Domänen beschränken, damit WSUS und die Funktion für automatische Updates mit Microsoft Update kommunizieren können:

    -   http://windowsupdate.microsoft.com
    -   http://\*.windowsupdate.microsoft.com
    -   https://\*.windowsupdate.microsoft.com
    -   http://\*.update.microsoft.com
    -   https://\*.update.microsoft.com
    -   http://\*.windowsupdate.com
    -   http://download.windowsupdate.com
    -   http://download.microsoft.com
    -   http://\*.download.windowsupdate.com
    -   http://wustat.windows.com
    -   http://ntservicepack.microsoft.com

 
> [!NOTE]
> Diese Anweisungen zum Konfigurieren der Firewall beziehen sich auf eine Unternehmensfirewall zwischen WSUS und dem Internet. Da WSUS seinen gesamten Netzwerkverkehr selbst initiiert, muss die Windows-Firewall auf dem WSUS-Server nicht konfiguriert werden.
 

Für die Verbindung zwischen Microsoft Update und WSUS müssen die Ports 80 und 443 offen sein. Sie können jedoch auch mehrere WSUS-Server so konfigurieren, dass sie mit einem benutzerdefinierten Port synchronisiert werden.

Bei den nächsten beiden Verfahren wird vorausgesetzt, dass Sie den Konfigurations-Assistenten verwenden. In einem späteren Abschnitt in diesem Schritt lernen Sie, wie das WSUS-Verwaltungs-Snap-In gestartet und der Server über die Seite "Optionen" konfiguriert wird.

**So legen Sie fest, wie dieser Server Updates abruft**
1.  Nachdem Sie dem Programm zur Verbesserung von Microsoft Update beigetreten sind, klicken Sie im Konfigurations-Assistenten auf **Weiter**, um den Upstreamserver auszuwählen.

2.  Wenn Sie sich für die Synchronisierung mit Microsoft Update entscheiden, haben Sie den Vorgang mit der Seite "Optionen" abgeschlossen. Klicken Sie auf **Weiter**, oder wählen Sie im Navigationsbereich die Option **Proxyserver angeben** aus.

3.  Wenn Sie die Synchronisation von einem anderen WSUS-Server aus durchführen möchten, geben Sie den Servernamen und den Port an, auf dem dieser Server mit dem Upstreamserver kommuniziert.

4.  Wenn SSL verwendet werden soll, aktivieren Sie das Kontrollkästchen **SSL beim Synchronisieren der Updateinformationen verwenden**. In diesem Fall verwenden die Server Port 443 für die Synchronisierung. (Sie sollten sicherstellen, dass sowohl dieser Server als auch der Upstreamserver SSL unterstützen.)

5.  Wenn es sich um einen Replikatserver handelt, aktivieren Sie das Kontrollkästchen **Dieser Server ist ein Replikat des Upstreamservers**.

6.  An diesem Punkt haben Sie die Konfiguration des Upstreamservers abgeschlossen. Klicken Sie auf **Weiter**, oder wählen Sie links im Navigationsbereich **Proxyserver angeben** aus.

**So konfigurieren Sie Proxyservereinstellungen**
1.  Aktivieren Sie im Konfigurations-Assistenten auf der Seite **Proxyserver angeben** das Kontrollkästchen **Proxyserver für die Synchronisierung verwenden**, und geben Sie den Proxyservernamen und die Portnummer (in der Standardeinstellung Port 80) in die entsprechenden Felder ein.

2.  Wenn Sie die Verbindung zum Proxyserver mithilfe bestimmter Benutzeranmeldeinformationen herstellen möchten, aktivieren Sie das Kontrollkästchen **Benutzeranmeldeinformationen für die Verbindungsherstellung mit dem Proxyserver verwenden**, und geben Sie dann den Benutzernamen, die Domäne und das Kennwort des Benutzers in die entsprechenden Felder ein. Wenn Sie die Standardauthentifizierung für Benutzer aktivieren möchten, die eine Verbindung zum Proxyserver herstellen, aktivieren Sie das Kontrollkästchen **Standardauthentifizierung zulassen (Kennwort wird in Klartext gesendet)**.

3.  An diesem Punkt haben Sie die Konfiguration des Proxyservers abgeschlossen. Klicken Sie auf **Weiter**, um zur nächsten Seite zu wechseln, auf der Sie mit dem Einrichten des Synchronisierungsprozesses beginnen können.

Bei den beiden folgenden Verfahren wird vorausgesetzt, dass Sie das WSUS-Verwaltungs-Snap-In für die Konfiguration verwenden. In diesen beiden Verfahren wird gezeigt, wie Sie das WSUS-Verwaltungs-Snap-In starten und den Server auf der Seite **Optionen** konfigurieren.

**So starten Sie die WSUS-Verwaltungskonsole**
-   Zum Starten der WSUS-Verwaltungskonsole klicken Sie auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Verwaltung**, und klicken Sie anschließend auf **Microsoft Windows Server Update Services 3.0**.

 
> [!NOTE]
> Damit Sie alle Features der Konsole verwenden können, müssen Sie sich als Mitglied der WSUS-Administratorengruppe oder der lokalen Administratorensicherheitsgruppe auf dem Server anmelden, auf dem WSUS installiert ist. Für Mitglieder der Sicherheitsgruppe &quot;WSUS-Berichterstatter&quot; ist die Konsole schreibgeschützt.
 

**So geben Sie eine Updatequelle und einen Proxyserver an**
1.  Klicken Sie links in der WSUS-Konsole unter dem Namen dieses Servers auf **Optionen**, und klicken Sie anschließend im mittleren Bereich auf **Updatequelle und Proxyserver**.

    Ein Dialogfeld mit den Registerkarten **Updatequelle** und **Proxyserver** wird angezeigt.

2.  Wählen Sie auf der Registerkarte **Updatequelle** den Speicherort aus, von dem dieser Server Updates abruft. Wenn Sie mit Microsoft Update synchronisieren (Standardeinstellung), haben Sie diese Seite des Assistenten abgeschlossen.

3.  Wenn Sie sich für die Synchronisierung mit einem anderen WSUS-Server entscheiden, müssen Sie den Port angeben, über den die Server kommunizieren sollen (in der Standardeinstellung ist dies Port 80). Wenn Sie einen anderen Port auswählen, sollten Sie sicherstellen, dass dieser Port von beiden Servern verwendet werden kann.

4.  Sie können auch angeben, ob zum Synchronisieren mit dem WSUS-Upstreamserver SSL verwendet werden soll. In diesem Fall verwenden die Server Port 443, um vom Upstreamserver zu synchronisieren.

5.  Wenn es sich bei diesem Server um ein Replikat des zweiten WSUS-Servers handelt, aktivieren Sie das Kontrollkästchen **Dies ist ein Replikat des Upstreamservers**. In diesem Fall müssen sämtliche Updates nur durch den WSUS-Upstreamserver genehmigt werden.

6.  Aktivieren Sie auf der Registerkarte **Proxyserver** das Kontrollkästchen **Proxyserver für die Synchronisierung verwenden**, und geben Sie dann den Namen des Proxyservers und die Portnummer (standardmäßig Port 80) in die entsprechenden Felder ein.

7.  Wenn Sie die Verbindung zum Proxyserver mithilfe bestimmter Benutzeranmeldeinformationen herstellen möchten, aktivieren Sie das Kontrollkästchen **Benutzeranmeldeinformationen für die Verbindungsherstellung mit dem Proxyserver verwenden**, und geben Sie dann den Benutzernamen, die Domäne und das Kennwort des Benutzers in die entsprechenden Felder ein. Wenn Sie für den Benutzer, der eine Verbindung zum Proxyserver herstellt, die Standardauthentifizierung aktivieren möchten, aktivieren Sie das Kontrollkästchen **Standardauthentifizierung zulassen (Kennwort wird in Klartext gesendet)**.

8.  Klicken Sie auf **OK**, um diese Einstellungen zu speichern.

Nächster Schritt
----------------

[Schritt 4: Konfigurieren von Updates und Synchronisierung](https://technet.microsoft.com/deeaa7e1-9b50-45cb-9537-d75f70de3405)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
