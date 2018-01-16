---
TOCTitle: Einrichten der Berechtigungen für das virtuelle Verzeichnis
Title: Einrichten der Berechtigungen für das virtuelle Verzeichnis
ms:assetid: '45112111-9608-45b1-9a86-7b313d0a1579'
ms:contentKeyID: 18118820
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747549(v=WS.10)'
---

Einrichten der Berechtigungen für das virtuelle Verzeichnis
===========================================================

Sobald Sie die Außerbetriebsetzung aktiviert haben, steht diese als Dienst zur Verfügung. Der Außerbetriebsetzungsdienst besteht allerdings aus einem virtuellen IIS-Verzeichnis mit den entsprechenden Zugriffsberechtigungen. Damit die Benutzer diesen Dienst verwenden können, müssen Berechtigungen für das virtuelle Verzeichnis sowie für die eigentliche Datei („decommission.asmx“) festgelegt werden.

Standardmäßig ist Integrierte Windows-Authentifizierung für das virtuelle Verzeichnis aktiviert; der Zugriff auf die eigentliche Datei ist jedoch nur System- und Administratorkonten vorbehalten. Beim Festlegen der Berechtigungen für die DACL der Datei „decommission.asmx“ können Sie einer bestimmten Gruppe von Benutzern den Zugriff gewähren, die hinsichtlich des Entfernens des eigentlichen RMS-Schutzes als vertrauenswürdig gelten, oder auch den Zugriff auf den Dienst für alle Benutzer zulassen.

Bevor die Benutzer den Außerbetriebsetzungsdienst verwenden können, muss die Anwendung der Benutzer so geändert werden, dass Anforderungen nach einer Nutzungslizenz an diese neue Außerbetriebssetzungs-Pipeline gesendet werden können. Bei Microsoft Office System 2003 wird hierzu ein Registrierungseintrag auf dem Computer des Benutzers angelegt. Wenn Sie Office 2003 benutzen, können Sie diesen Schritt gemäß dem folgenden Verfahren durchführen:

1.  Öffnen Sie den Registrierungs-Editor.
2.  Navigieren Sie zu `HKEY_CURRENT_USER\Software\Microsoft\Office\11.0\Common\DRM`, und fügen Sie einen neuen Schlüssel mit der Bezeichnung `Außerbetriebsetzung` hinzu.
3.  Fügen Sie unter dem Schlüssel „Außerbetriebsetzung“ den folgenden neuen Eintrag mit einer **Zeichenfolge** hinzu (ersetzen Sie hierbei den Platzhalter *Ihr-Lizenzserver* mit der Bezeichnung Ihres RMS-Servers):

    `http://`*Ihr-Lizenzserver*`/_wmcs/licensing`
4.  Klicken Sie anschließend mit der rechten Maustaste auf den Eintrag, und wählen Sie **Ändern** aus. Geben Sie dann den Datenwert ein, der auf den Außerbetriebsetzungsdienst verweist:

    `http://`*Ihr-Lizenzserver*`/_wmcs/decommission`

> [!NOTE]
> Wenn sich mehrere RMS-Server im Unternehmen im Außerbetriebsetzungsmodus befinden, können mehrere Einträge für diesen Schlüssel vorliegen. 