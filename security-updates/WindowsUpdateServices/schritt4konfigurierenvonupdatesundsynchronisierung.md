---
TOCTitle: 'Schritt 4: Konfigurieren von Updates und Synchronisierung'
Title: 'Schritt 4: Konfigurieren von Updates und Synchronisierung'
ms:assetid: 'deeaa7e1-9b50-45cb-9537-d75f70de3405'
ms:contentKeyID: 21669590
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939924(v=WS.10)'
---

Schritt 4: Konfigurieren von Updates und Synchronisierung
=========================================================

In diesem Abschnitt wird beschrieben, wie Sie die mit dem Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) herunterzuladende Updategruppe konfigurieren.

Verfahren in Schritt 4
----------------------

Diese Verfahren können Sie mit dem WSUS-Konfigurations-Assistenten oder der WSUS-Verwaltungskonsole durchführen.

1.  Speichern und Herunterladen von Upstream- und Proxyserverinformationen
2.  Auswählen der Sprache für die Updates
3.  Auswählen der Produkte, für die Updates abgerufen werden sollen
4.  Auswählen der Updateklassifizierungen
5.  Festlegen des Synchronisierungszeitplans für diesen Server

Nach dem Konfigurieren der Netzwerkverbindung können Sie Updates herunterladen, indem Sie den WSUS-Server synchronisieren. Die Synchronisierung beginnt, wenn der WSUS-Server eine Verbindung zu Microsoft Update herstellt. Wenn die Verbindung hergestellt ist, stellt WSUS fest, ob seit der letzten Synchronisierung neue Updates zur Verfügung gestellt wurden. Wenn Sie den WSUS-Server zum ersten Mal synchronisieren, sind alle Updates verfügbar und können für die Installation genehmigt werden. Die erste Synchronisierung nimmt möglicherweise einige Zeit in Anspruch.

Die Verfahren in diesem Abschnitt beschreiben die Synchronisierung mit den Standardeinstellungen. WSUS 3.0 SP2 bietet auch Optionen zur Minimierung der Bandbreitenauslastung während der Synchronisierung.

Bei Verwendung des Konfigurationsassistenten für Windows Server Update Services
-------------------------------------------------------------------------------

In Schritt 3 haben Sie die Konfiguration des Upstream- und des Proxyservers abgeschlossen. Die nächsten Verfahren beginnen auf der Seite **Mit Upstreamserver verbinden** dieses Konfigurations-Assistenten.

**Speichern und Herunterladen von Upstream- und Proxyserverinformationen**
1.  Klicken Sie auf der Seite "Mit Upstreamserver verbinden" des Konfigurations-Assistenten auf die Schaltfläche **Verbindung starten**. Dadurch werden Ihre Einstellungen gespeichert und hochgeladen sowie Informationen zu verfügbaren Updates gesammelt.

2.  Während der Verbindungsherstellung kann der Vorgang über die Schaltfläche **Verbinden beenden** abgebrochen werden. Bei Verbindungsfehlern klicken Sie auf **Verbinden beenden**, beheben Sie die Probleme, und starten Sie die Verbindung erneut.

3.  Nach erfolgreichem Abschluss des Downloads klicken Sie auf **Weiter**.

**So wählen Sie Updatesprachen aus**
1.  Auf der Seite "Sprachen auswählen" können Sie den Erhalt von Updates aus allen Sprachen oder aus einer festgelegten Sprachauswahl festlegen. Wenn nur eine Teilmenge von Sprachen ausgewählt wird, ist nicht so viel Festplattenspeicherplatz erforderlich. Sie sollten jedoch alle Sprachen auswählen, die von den Clients dieses WSUS-Servers benötigt werden.

    Wählen Sie **Updates nur in folgenden Sprachen herunterladen**, wenn Sie nur Updates für bestimmte Sprachen erhalten möchten, und wählen Sie anschließend die gewünschten Sprachen.

2.  Klicken Sie auf **Weiter**.

**So wählen Sie Updateprodukte aus**
1.  Auf der Seite "Produkte auswählen" können Sie die Produkte festlegen, für die Sie Updates erhalten möchten. Wählen Sie Produktkategorien, beispielsweise Windows, oder bestimmte Produkte, beispielsweise Windows Server 2008. Wenn Sie eine Produktkategorie wählen, werden alle Produkte der Kategorie einbezogen.

2.  Klicken Sie auf **Weiter**.

**So wählen Sie Updateklassifizierungen aus**
1.  Auf der Seite "Klassifizierungen auswählen" können Sie die abzurufenden Updateklassifizierungen festlegen. Wählen Sie alle Klassifizierungen oder nur bestimmte Teile.

2.  Klicken Sie auf **Weiter**.

**So konfigurieren Sie den Synchronisierungszeitplan**
1.  Auf der Seite "Synchronisierungszeitplan festlegen" können Sie auswählen, ob die Synchronisierung manuell oder automatisch ausgeführt werden soll.

    Wenn Sie **Manuell synchronisieren** auswählen, müssen Sie den Synchronisierungsvorgang von der WSUS-Verwaltungskonsole aus starten.

    Wenn Sie **Automatisch synchronisieren** auswählen, wird die Synchronisierung vom WSUS-Server in den angegebenen Intervallen ausgeführt. Legen Sie den Zeitpunkt für die **Erste Synchronisierung** fest, und geben Sie an, wie viele **Synchronisierungen pro Tag** auf diesem Server ausgeführt werden sollen. Wenn Sie z. B. vier Synchronisierungen pro Tag angeben, beginnend um 3:00 Uhr morgens, werden Synchronisierungen um 3:00 Uhr und 9:00 Uhr morgens sowie um 15:00 Uhr und 21:00 Uhr ausgeführt.

2.  Klicken Sie auf **Weiter**.

3.  Auf der Seite "Fertig stellen" können Sie die WSUS-Verwaltungskonsole starten, indem Sie das Kontrollkästchen **Snap-In "Windows Server Update Services-Verwaltung" starten** aktiviert lassen, und die erste Synchronisierung wird gestartet, wenn das Kontrollkästchen **Erstsynchronisierung starten** aktiviert ist.

4.  Klicken Sie auf **Fertig stellen**.

 
    <table style="border:1px solid black;">
    <colgroup>
    <col width="100%" />
    </colgroup>
    <thead>
    <tr class="header">
    <th style="border:1px solid black;" ><img src="images/Dd939924.Important(WS.10).gif" />Wichtig</th>
    </tr>
    </thead>
    <tbody>
    <tr class="odd">
    <td style="border:1px solid black;">Konfigurationsänderungen, die während der Synchronisierung des Servers vorgenommen werden, können nicht gespeichert werden. Nehmen Sie daher erst Änderungen vor, wenn die Synchronisierung abgeschlossen ist.
    </td>
    </tr>
    </tbody>
    </table>
 

Bei Verwendung der WSUS-Verwaltungskonsole
------------------------------------------

Mit den folgenden Verfahren können Sie die Konfigurationsschritte mit der WSUS-Verwaltungskonsole ausführen.

**So wählen Sie Produkte und Updateklassifizierungen aus**
1.  Klicken Sie im Bereich **Optionen** auf **Produkte und Klassifizierungen**. Es wird ein Dialogfeld mit den Registerkarten **Produkte** und **Klassifizierungen** angezeigt.

2.  Wählen Sie auf der Registerkarte **Produkte** die Produktkategorie oder bestimmte Produkte, für die dieser Server Updates abrufen soll, oder wählen Sie **Alle Produkte**.

3.  Wählen Sie auf der Registerkarte **Klassifizierungen** die gewünschten Updateklassifizierungen oder **Alle Klassifizierungen**.

4.  Klicken Sie auf **OK**, um Ihre Einstellungen zu speichern.

**So wählen Sie Updatedateien und -sprachen aus**
1.  Klicken Sie im Bereich **Optionen** auf **Dateien und Sprachen aktualisieren**. Es wird ein Dialogfeld mit den Registerkarten **Updatedateien** und **Updatesprachen** angezeigt.

2.  Auf der Registerkarte **Updatedateien** können Sie die Option **Updatedateien lokal auf diesem Server speichern** auswählen oder Installationen von Microsoft Update für alle Clientcomputer ausführen lassen. Wenn Sie sich dafür entscheiden, die Updatedateien auf diesem Server zu speichern, können Sie festlegen, ob nur genehmigte Updates heruntergeladen werden oder ob Schnellinstallationsdateien heruntergeladen werden sollen.

3.  Wenn Sie Updatedateien lokal speichern, wählen Sie in der Registerkarte **Updatesprachen** entweder die Option **Updates für alle Sprachen herunterladen** (Standard) oder **Updates nur in den angegebenen Sprachen herunterladen**. Wenn diesem WSUS-Server Downstreamserver zugeordnet sind, erhalten diese nur Updates in den vom Upstreamserver festgelegten Sprachen.

4.  Klicken Sie auf **OK**, um diese Einstellungen zu speichern.

**So synchronisieren Sie den WSUS-Server**
1.  Klicken Sie im Abschnitt **Optionen** auf **Synchronisierungszeitplan**.

2.  In der Registerkarte **Synchronisierungszeitplan** können Sie auswählen, ob die Synchronisierung manuell oder automatisch ausgeführt werden soll.

    Wenn Sie **Manuell synchronisieren** auswählen, müssen Sie den Synchronisierungsvorgang von der WSUS-Verwaltungskonsole aus starten.

    Wenn Sie **Automatisch synchronisieren** auswählen, wird die Synchronisierung vom WSUS-Server in den angegebenen Intervallen ausgeführt. Legen Sie den Zeitpunkt für die **Erste Synchronisierung** fest, und geben Sie an, wie viele **Synchronisierungen pro Tag** auf diesem Server ausgeführt werden sollen. Wenn Sie z. B. vier Synchronisierungen pro Tag angeben, beginnend um 3:00 Uhr morgens, werden Synchronisierungen um 3:00 Uhr und 9:00 Uhr morgens sowie um 15:00 Uhr und 21:00 Uhr ausgeführt.

3.  Klicken Sie auf **OK**, um Ihre Einstellungen zu speichern.

4.  Wählen Sie im Navigationsbereich der WSUS-Verwaltungskonsole **Synchronisierungen**.

5.  Klicken Sie mit der rechten Maustaste, oder klicken Sie rechts im Fenster **Aktionen** auf **Jetzt synchronisieren**.

    Wenn das Fenster **Aktionen** nicht auf der rechten Seite der Konsole angezeigt wird, klicken Sie auf der Symbolleiste der Konsole auf **Ansicht** und dann auf **Anpassen**. Stellen Sie sicher, dass das Kontrollkästchen **Aktionsbereich** aktiviert ist.

6.  Klicken Sie nach Abschluss der Synchronisierung im linken Bildschirmbereich auf **Updates**, um eine Liste der Updates anzuzeigen.

Nächster Schritt
----------------

[Schritt 5: Konfigurieren von Client-Updates](https://technet.microsoft.com/5ae60ead-3e94-456c-a692-c0f193ea5d5a)

Weitere Ressourcen
------------------

[Schrittweise Anleitung für Windows Server Update Services 3.0 SP2](https://technet.microsoft.com/4b504edc-93b3-45b0-a7e8-d0107f1a4442)
