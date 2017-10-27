---
TOCTitle: 'So vertrauen Sie Passport-basierten Rechtekontozertifikaten'
Title: 'So vertrauen Sie Passport-basierten Rechtekontozertifikaten'
ms:assetid: 'c096fa36-c40d-4b28-843c-e9cbbe8eef70'
ms:contentKeyID: 18119070
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747655(v=WS.10)'
---

So vertrauen Sie Passport-basierten Rechtekontozertifikaten
===========================================================

Microsoft bietet einen Kontozertifizierungsservice an, der Microsoft .NET-Passportinformationen zum Einrichten eines Rechtekontozertifkats für den Benutzer verwendet. Wenn Sie möchten, dass Benutzer mit Rechtekontozertifikaten von diesem Dienst Lizenzen von Ihrem RMS-Cluster erhalten können, müssen Sie eine vertrauenswürdige Benutzerdomäne einrichten, die Benutzerinformationen vom Kontozertifizierungsdienst von Microsoft akzeptiert.

Um diese Funktion zu verwenden, müssen Sie Internetinformationsdienste (IIS) so konfigurieren, dass anonymer Zugriff auf den RMS-Lizenzierungsdienst möglich ist. Dieser Schritt ist für externe Benutzer besonders wichtig, da der Lizenzierungsdienst für die standardmäßige Verwendung der Windows-integrierten Authentifizierung konfiguriert ist. Wenn kein anonymer Zugriff eingerichtet wird, können externe Benutzer mit Passport-basierten Rechtekontozertifikaten (RACs) keine Lizenzen einholen.

Vertrauen auf Passport-basierte Rechtekontozertifikaten
-------------------------------------------------------

#### Für anonymen Zugriff auf den RMS-Lizenzierungsdienst

1.  Öffnen Sie das **Internetinformationsdienste-Manager**-Snap-in und erweitern Sie den Server mit RMS.

2.  In der Konsolenstruktur erweitern Sie **Websites** und dann die Website, auf der Sie RMS konfiguriert haben. Standardmäßig ist das die **Standardwebsite**.

3.  In der Konsolenstruktur erweitern Sie die Website **\_wmcs**, und wählen Sie dann das virtuelle Verzeichnis **Lizenzierung**.

4.  Klicken Sie mit der rechten Maustaste auf das virtuelle Verzeichnis **Lizenzierung**, und wählen Sie **Eigenschaften** aus.

5.  Klicken Sie im Dialogfeld **Lizenzierungseigenschaften** auf die Registerkarte **Verzeichnissicherheit**.

6.  Klicken Sie im Bereich **Authentifizierung und Zugriffssteuerung** auf **Bearbeiten**.

7.  Wählen Sie das Kontrollkästchen **Anonymen Zugriff aktivieren**.

#### So vertrauen Sie Passport-basierten Rechtekontozertifikaten

1.  Öffnen Sie die Seite **Globale Verwaltung**, und klicken Sie dann neben der Website, auf der Sie Passport-basierten Rechtekontozertifikaten vertrauen möchten, auf **RMS auf dieser Website verwalten**.

2.  Klicken Sie im Bereich **Verwaltungsverknüpfungen** auf **Vertrauensrichtlinien**.

3.  Klicken Sie im Bereich **Vertrauenswürdige Benutzerdomänen** auf **Passport-RACs vertrauen**. Der Microsoft RM-Zertifizierungsdienst wird in der Liste **Vertrauenswürdige Benutzerdomänen** angezeigt.

4.  Sie können Benutzer basierend auf deren E-Mail-Adresse ausschließen. Klicken Sie hierzu auf **Ausgeschlossene Identitäten**, und geben Sie dann die E-Mail-Adresse des nicht vertrauenswürdigen Benutzers ein.