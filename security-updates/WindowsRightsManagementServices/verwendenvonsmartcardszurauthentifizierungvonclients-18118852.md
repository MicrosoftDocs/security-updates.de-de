---
TOCTitle: Verwenden von Smartcards zur Authentifizierung von Clients
Title: Verwenden von Smartcards zur Authentifizierung von Clients
ms:assetid: '5caacd67-fb16-46f1-b1ad-4aef0a632bf0'
ms:contentKeyID: 18118852
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747579(v=WS.10)'
---

Verwenden von Smartcards zur Authentifizierung von Clients
==========================================================

Wenn Sie in Ihrer Organisation bereits Smartcards verwenden, um mehr Sicherheit und bessere Steuermöglichkeiten für Benutzeranmeldeinformationen zu erreichen, können Sie diese jetzt auch beim Erwerb von Rechtekontozertifikaten und Nutzungslizenzen von Servern mit RMS einsetzen. Sie können den Server mit RMS so konfigurieren, dass er eine Clientauthentifizierung verlangt. Dazu muss SSL (Secure Sockets Layer) für die Website, auf der Sie RMS bereitgestellt haben, aktiviert und die Authentifizierungsmethode in den Internetinformationsdiensten (Internet Information Services oder IIS) konfiguriert werden. Führen Sie folgende Schritte aus, um diese Aufgabe auszuführen:

1.  Öffnen Sie den **Internetinformationsdienste-Manager**.
2.  Erweitern Sie den Servereintrag, rechtsklicken Sie auf den Websiteordner und klicken Sie dann auf **Eigenschaften**.
3.  Klicken Sie auf die Registerkarte **Verzeichnissicherheit** und markieren Sie im Bereich **Sichere Kommunikation** das Kontrollkästchen **Windows-Verzeichnisdienstzuordnung aktivieren**.
4.  Erweitern Sie den Websiteordner, öffnen Sie das virtuelle Verzeichnis **\_wmcs** und erweitern Sie dann das virtuelle Verzeichnis (entweder **Lizenzierung** oder **Zertifizierung**), für das die Authentifizierung konfiguriert werden soll.
    -   Zur Konfiguration der Authentifizierung beim Anfordern einer Nutzungslizenz durch einen Benutzer rechtsklicken Sie auf die Datei license.asmx, und klicken Sie danach auf **Eigenschaften**.
    -   Zur Konfiguration der Authentifizierung beim Anfordern eines Benutzerzertifikats durch einen Benutzer rechtsklicken Sie auf die Datei certification.asmx, und klicken Sie danach auf **Eigenschaften**.
5.  Klicken Sie auf die Registerkarte **Dateisicherheit**, und klicken Sie dann im Bereich **Sichere Kommunikation** auf **Bearbeiten**, um das Dialogfeld **Sichere Kommunikation** zu öffnen.
6.  Wählen Sie **Sicheren Kanal voraussetzen (SSL)** aus, und klicken Sie anschließend auf eine der folgenden Optionen:
    -   **Clientzertifikate voraussetzen**, wenn Sie möchten, dass nur Clients mit clientseitigen Zertifikaten, wie etwa Smartcards, eine Verbindung zum Dienst herstellen können.
    -   **Clientzertifikate akzeptieren**, wenn Sie möchten, dass Clients die Möglichkeit haben, als Benutzeranmeldeinformationen zur Authentifizierung entweder ein Smartcard-Zertifikat oder ihren Benutzernamen und ein Kennwort zu verwenden.
7.  Wählen Sie **Zuordnung von Clientzertifikaten aktivieren** aus, und klicken Sie dann auf **OK**.
8.  Wenn Sie die Clientauthentifizierung sowohl für die Zertifizierung als auch die Lizenzierung verwenden möchten, wiederholen Sie den Vorgang, wählen dabei aber den jeweils anderen virtuellen Ordner aus.

Nachdem Sie diese Einstellungen konfiguriert haben, werden Benutzer beim nächsten Zugriff auf RMS-geschützte Inhalte, die von diesem Server veröffentlicht werden, dazu aufgefordert, ihre Anmeldeinformationen zur Authentifizierung anzugeben. Erst danach stellt der Server den Benutzern ein Rechtekontozertifikat oder eine Nutzungslizenz aus.
