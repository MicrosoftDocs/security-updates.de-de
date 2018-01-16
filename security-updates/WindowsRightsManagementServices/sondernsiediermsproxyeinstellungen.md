---
TOCTitle: 'So ändern Sie die RMS-Proxyeinstellungen'
Title: 'So ändern Sie die RMS-Proxyeinstellungen'
ms:assetid: '8f50bd4d-26b1-4996-b361-722ee21607f3'
ms:contentKeyID: 18118946
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747594(v=WS.10)'
---

So ändern Sie die RMS-Proxyeinstellungen
========================================

Zum Ausführen dieses Verfahrens müssen Sie lokal bei der Verwaltungswebsite mit einem Domänenbenutzerkonto angemeldet sein, das ein Mitglied der Gruppe Administratoren auf dem Computer ist, auf den Sie zugreifen. Außerdem kann dieses Verfahren von Mitgliedern der Gruppe Domänen-Admins ausgeführt werden. Als bewährte Sicherheitsmethode sollten Sie für dieses Verfahren **Ausführen als** verwenden.

Weitere Informationen zu Authentifizierungsmethoden für Proxyserver und deren Funktionsweise in Windows Server 2003 finden Sie in der Hilfe zu „Internetinformationsdienste“ (Internet Information Services oder IIS).

Ändern der RMS-Proxyeinstellungen
---------------------------------

#### So ändern Sie die RMS-Proxyeinstellungen

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie unter **Clusterverwaltung** auf **Sicherheitseinstellungen**.

3.  Wenn Sie erstmals einen Proxyserver mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwenden, aktivieren Sie das Kontrollkästchen **Dieser Computer verwendet für Verbindungen mit dem Internet einen Proxyserver**. Auf der Seite werden zusätzliche Einstellungen angezeigt, die vervollständigt werden müssen.

4.  Geben Sie in das Feld **Adresse:** die IP-Adresse oder den DNS-Namen ein, den Sie verwenden möchten.

5.  Geben Sie im Feld **Port:** die Portnummer ein, die der Proxyserver für die Verbindung zum Internet verwendet.

6.  Wird kein Proxyserver für die Verbindung mit lokalen Ressourcen verwendet, aktivieren Sie das Kontrollkästchen **Proxyserver für lokale Adressen umgehen**.

7.  Aktivieren Sie gegebenenfalls das Kontrollkästchen **Dieser Proxyserver erfordert keine Authentifizierung**.

    -   Wählen Sie den Authentifizierungstyp aus der Liste aus, entweder **Standardauthentifizierung**, **Digestauthentifizierung** oder **Integrierte Windows-Authentifizierung**
    -   Geben Sie in das Feld **Benutzername:** den Benutzernamen ein, der als Antwort bei Anforderungen vom Proxyserver angegeben werden soll.
    -   Geben Sie in das Feld **Kennwort:** das Kennwort ein, das als Antwort bei Anforderungen vom Proxyserver angegeben werden soll.
    -   Geben Sie in das Feld **Kennwort bestätigen:** das zuvor angegebene Kennwort erneut ein, um sicherzustellen, dass Sie es korrekt eingeben haben.
    -   Wenn der Proxyserver „Integrierte Windows-Authentifizierung“ verwendet, geben Sie in das Feld **Domäne** den für den Benutzer zugehörigen Domänentyp ein.

8.  Klicken Sie auf **Absenden**.