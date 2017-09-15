---
TOCTitle: 'Schritt 3: Konfigurieren der Netzwerkverbindung'
Title: 'Schritt 3: Konfigurieren der Netzwerkverbindung'
ms:assetid: 'cd77566d-7780-4ce4-aa56-41183c65c4a7'
ms:contentKeyID: 18127628
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708559(v=WS.10)'
---

Schritt 3: Konfigurieren der Netzwerkverbindung
===============================================

Nach dem Installieren von WSUS können Sie auf die WSUS-Konsole zugreifen, um WSUS zu konfigurieren und erste Schritte auszuführen. Standardmäßig verwendet WSUS den Microsoft Updates-Pfad, um Updates zu erhalten. Wenn im Netzwerk ein Proxyserver vorhanden ist, konfigurieren Sie WSUS mithilfe der WSUS-Konsole so, dass der Proxyserver verwendet wird. Wenn sich zwischen WSUS und dem Internet ein Unternehmensfirewall befindet, müssen Sie den Firewall möglicherweise neu konfigurieren, um sicherzustellen, dass WSUS Updates erhalten kann.

| ![](images/Cc708559.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                               |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Zum Downloaden von Updates von Microsoft Update benötigen Sie eine Internetverbindung. WSUS bietet Ihnen jedoch auch die Möglichkeit, Updates in Netzwerke ohne Internetverbindung zu importieren. Weitere Informationen finden Sie im Whitepaper "Bereitstellen von Microsoft Server Windows Update Services" (möglicherweise in englischer Sprache). |

Schritt 3 umfasst die folgenden Verfahren:

-   Konfigurieren des Firewalls, sodass WSUS Updates erhalten kann.
-   Öffnen der WSUS-Konsole.
-   Konfigurieren der Proxyservereinstellungen, sodass WSUS Updates erhalten kann.

**So konfigurieren Sie den Firewall**
-   Wenn sich zwischen WSUS und dem Internet ein Unternehmensfirewall befindet, müssen Sie den Firewall möglicherweise neu konfigurieren, um sicherzustellen, dass WSUS Updates erhalten kann. Der WSUS-Server verwendet Port 80 für das Protokoll HTTP und Port 443 für HTTPS, um Updates von Microsoft Update zu erhalten. Diese Einstellung ist nicht konfigurierbar.

-   Wenn Ihre Organisation diese Ports und Protokolle, die allen Adressen offenstehen, nicht zulässt, können Sie den Zugriff auf die folgenden Domänen beschränken, damit WSUS und die automatischen Updates mit Microsoft Update kommunizieren können:

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

| ![](images/Cc708559.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Die oben stehenden Schritte zum Konfigurieren des Firewalls beziehen sich auf einen Unternehmensfirewall, der sich zwischen WSUS und dem Internet befindet. Da WSUS den gesamten eigenen Netzwerkverkehr selbst initiiert, muss der Windows-Firewall auf dem WSUS-Server nicht konfiguriert werden. Für die Verbindung zwischen Microsoft Update und WSUS müssen die Ports 80 und 443 offen sein. Sie können jedoch auch mehrere WSUS-Server so konfigurieren, dass sie mit einem benutzerdefinierten Port synchronisiert werden. Weitere Informationen zum Synchronisieren von WSUS-Servern mit einem benutzerdefinierten Port finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache). |

**So öffnen Sie die WSUS-Konsole**
-   Klicken Sie auf dem WSUS-Server auf **Start**, zeigen Sie auf **Alle Programme**, zeigen Sie auf **Verwaltung**, und klicken Sie dann auf **Microsoft Windows Server Update Services**.

| ![](images/Cc708559.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Um die WSUS-Konsole zu verwenden, müssen Sie Mitglied der Sicherheitsgruppe **WSUS-Administratoren** oder der lokalen Sicherheitsgruppe **Administratoren** auf dem Server sein, auf dem WSUS installiert ist. Wenn Sie nicht **http://&lt;***Name der WSUS-Website***&gt;** zur Liste der Websites in der Zone **Lokales Intranet** in Internet Explorer unter Windows Server 2003 hinzufügen, werden Sie möglicherweise bei jedem Öffnen der WSUS-Konsole aufgefordert, Anmeldeinformationen einzugeben. Wenn Sie die Portzuweisung in Internetinformationsdienste (Internet Information Services, IIS) nach dem Installieren von WSUS ändern, müssen Sie die Verknüpfung im Startmenü manuell aktualisieren. Sie können die WSUS-Konsole auch auf einem beliebigen Server oder Computer im Netzwerk in Internet Explorer öffnen, indem Sie den folgenden URL eingeben: **http://***WSUS-Servername***/WSUSAdmin** |

**So geben Sie einen Proxyserver an**
1.  Klicken Sie auf der Symbolleiste der WSUS-Konsole auf **Optionen** und dann auf **Synchronisierungsoptionen**.

2.  Aktivieren Sie im Feld **Proxyserver** das Kontrollkästchen **Proxyserver für die Synchronisierung verwenden**, und geben Sie dann den Namen des Proxyservers und die Portnummer (standardmäßig Port 80) in die entsprechenden Felder ein.

3.  Wenn Sie die Verbindung zum Proxyserver mithilfe bestimmter Benutzeranmeldeinformationen herstellen möchten, aktivieren Sie das Kontrollkästchen **Benutzeranmeldeinformationen für die Verbindungsherstellung mit dem Proxyserver verwenden**, und geben Sie dann den Benutzernamen, die Domäne und das Kennwort des Benutzers in die entsprechenden Felder ein. Wenn Sie für den Benutzer, der eine Verbindung zum Proxyserver herstellt, Standardauthentifizierung aktivieren möchten, aktivieren Sie das Kontrollkästchen **Standardauthentifizierung (Kennwort wird in Klartext gesendet) zulassen**.

4.  Klicken Sie unter **Aufgaben** auf **Einstellungen speichern**, und klicken Sie anschließend im Bestätigungsdialogfeld auf **OK**.
