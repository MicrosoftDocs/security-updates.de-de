---
TOCTitle: 'Schritt 4: Konfigurieren von Updates und Einrichten der Synchronisierung'
Title: 'Schritt 4: Konfigurieren von Updates und Einrichten der Synchronisierung'
ms:assetid: '734cc2ed-98be-4772-a42c-8fd38b39d864'
ms:contentKeyID: 18127490
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708447(v=WS.10)'
---

Schritt 4: Konfigurieren von Updates und Einrichten der Synchronisierung
========================================================================

Vor dem Herunterladen von Updates müssen Sie festlegen, welche Updates Sie herunterladen möchten. In diesem Abschnitt wird beschrieben, wie Sie die herunterzuladende Updategruppe konfigurieren.

In diesem Schritt werden folgende Verfahren beschrieben:

-   Speichern und Herunterladen von Upstream- und Proxyserverinformationen
-   Auswählen der Sprache für die Updates
-   Auswählen der Produkte, für die Updates abgerufen werden sollen
-   Auswählen der Updateklassifizierungen
-   Festlegen des Synchronisierungszeitplans für diesen Server

In den nächsten fünf Verfahren wird das Konfigurieren der Updates mithilfe des Konfigurations-Assistenten beschrieben. In den weiter unten beschriebenen Verfahren wird erläutert, wie diese Konfiguration über die Auswahl bestimmter Optionen in der WSUS-Verwaltungskonsole ausgeführt wird.

**Speichern und Herunterladen von Upstream- und Proxyserverinformationen**
1.  Die Konfiguration des Upstream- und Proxyservers sollte bereits im Konfigurations-Assistenten abgeschlossen sein, und die Seite **Mit Upstreamserver verbinden** sollte angezeigt werden.

2.  Klicken Sie auf die Schaltfläche **Verbindung starten**, um Ihre Einstellungen zu speichern und hochzuladen sowie Informationen über verfügbare Updates abzurufen.

3.  Während der Verbindungsherstellung kann der Vorgang über die Schaltfläche **Verbinden beenden** abgebrochen werden. Bei Verbindungsfehlern klicken Sie auf **Verbinden beenden**, beheben Sie die Probleme, und starten Sie die Verbindung erneut.

4.  Klicken Sie nach dem erfolgreichen Herunterladen auf **Weiter**, um zur Seite **Sprachen auswählen** zu wechseln, oder wählen Sie im linken Bildschirmbereich eine andere Seite aus.

**Auswählen der Updatesprachen**
1.  Über die Seite **Sprachen auswählen** können Sie Updates aus allen Sprachen oder aus einer festgelegten Sprachauswahl abrufen. Wenn nur eine Teilmenge von Sprachen ausgewählt wird, ist nicht so viel Festplattenspeicherplatz erforderlich. Sie sollten jedoch alle Sprachen auswählen, die von allen Clients dieses WSUS-Servers benötigt werden.

2.  Wählen Sie **Updates nur in folgenden Sprachen herunterladen**, wenn Sie nur Updates für bestimmte Sprachen erhalten möchten, und wählen Sie anschließend die gewünschten Sprachen aus. Klicken Sie auf **Weiter**, um zur Seite **Produkte auswählen** zu wechseln, oder wählen Sie im linken Bildschirmbereich eine andere Seite.

**Auswählen der Updateprodukte**
1.  Über die Seite **Produkte auswählen** können Sie die Produkte festlegen, für die Sie Updates erhalten möchten.

2.  Sie können Produktkategorien, wie z. B. Windows, oder bestimmte Produkte auswählen, wie z. B. Windows Server 2003. Wenn Sie eine Produktkategorie wählen, werden alle untergeordneten Produkte einbezogen. Klicken Sie auf **Weiter**, um zur Seite **Klassifizierungen auswählen** zu wechseln, oder wählen Sie im linken Bildschirmbereich eine andere Seite.

**Auswählen der Updateklassifizierungen**
1.  Auf der Seite **Klassifizierungen auswählen** können Sie die abzurufenden Updateklassifizierungen auswählen. Sie können alle Klassifizierungen oder nur bestimmte Teile auswählen.

2.  Klicken Sie auf **Weiter**, um zur Seite **Synchronisierungszeitplan konfigurieren** zu wechseln, oder wählen Sie im linken Bildschirmbereich eine andere Seite.

**Konfigurieren des Synchronisierungszeitplans**
1.  Die Seite **Synchronisierungszeitplan festlegen** wird angezeigt, auf der Sie auswählen können, ob die Synchronisierung manuell oder automatisch ausgeführt werden soll.

2.  Wenn Sie die Synchronisierung auf diesem Server manuell ausführen möchten, müssen Sie den Synchronisierungsvorgang von der WSUS-Verwaltungskonsole aus starten.

3.  Wenn Sie automatische Synchronisierung auswählen, wird die Synchronisierung vom WSUS-Server in den angegebenen Intervallen ausgeführt. Legen Sie den Zeitpunkt für die erste Synchronisierung fest, und geben Sie an, wie viele Synchronisierungen auf diesem Server täglich ausgeführt werden sollen. Wenn Sie z. B. vier Synchronisierungen pro Tag angeben, beginnend um 3:00 Uhr morgens, werden Synchronisierung um 3:00 Uhr und 9:00 Uhr morgens sowie um 15:00 Uhr und 21:00 Uhr ausgeführt.

Wählen Sie im Konfigurations-Assistenten die Seite **Fertig stellen** aus, wenn Sie alle oben beschriebenen Konfigurationsschritte abgeschlossen haben. Sie können die WSUS-Verwaltungskonsole starten, indem Sie das Kontrollkästchen **Snap-In "Windows Server Update Services-Verwaltung" starten** aktiviert lassen, und die erste Synchronisierung wird gestartet, wenn das Kontrollkästchen **Erstsynchronisierung starten** aktiviert ist.

> [!NOTE]
> Konfigurationsänderungen, die während der Synchronisierung des Servers vorgenommen werden, können nicht gespeichert werden. Nehmen Sie daher erst Änderungen vor, wenn die Synchronisierung abgeschlossen ist. 

![](images/Cc708447.3f774fd1-af87-47d8-8f50-a5d585687d70(WS.10).gif)

Mit den folgenden Verfahren können Sie die oben beschriebenen Konfigurationsschritte über die Seite **Optionen** der WSUS-Verwaltungskonsole ausführen:

-   Auswählen von Produkten und Klassifizierungen
-   Aktualisieren von Dateien und Sprachen

**Auswählen von Produkten und Klassifizierungen**
1.  Starten Sie die WSUS-Verwaltungskonsole: Klicken Sie dazu auf **Start**, **Alle Programme**, zeigen Sie auf **Verwaltung**, und klicken Sie dann auf **Microsoft Windows Server Update Services**.

2.  Wählen Sie im linken Bildschirmbereich für Ihren WSUS-Server **Optionen** aus.

3.  Wählen Sie im mittleren Bildschirmbereich **Produkte und Klassifizierungen** aus.

4.  Es wird ein Dialogfeld mit den folgenden beiden Registerkarten angezeigt: **Produkte** und **Klassifizierungen**.

5.  Wählen Sie auf der Registerkarte **Produkte** die Produktkategorie oder ein bestimmtes Produkt, für das dieser Server Updates abrufen soll, oder wählen Sie **Alle Produkte**.

6.  Wählen Sie auf der Registerkarte **Klassifizierungen** die gewünschten Updateklassifizierungen oder **Alle Klassifizierungen**.

7.  Klicken Sie auf **OK**, um Ihre Einstellungen zu speichern.

**Aktualisieren von Dateien und Sprachen**
1.  Wählen Sie auf der Seite **Optionen** die Option **Dateien und Sprachen aktualisieren** aus.

2.  Es wird ein Dialogfeld mit den folgenden beiden Registerkarten angezeigt: **Updatedateien** und **Updatesprachen**.

3.  Auf der Registerkarte **Updatedateien** können Sie auswählen, ob Updatedateien lokal gespeichert oder Installationen von Microsoft Update für alle Clientcomputer ausgeführt werden sollen. Wenn Sie sich dafür entscheiden, die Updatedateien auf diesem Server zu speichern, können Sie festlegen, ob die Updatedateien nur heruntergeladen werden, wenn die Updates genehmigt sind, oder ob Schnellinstallationsdateien heruntergeladen werden sollen.

4.  Auf der Registerkarte **Updatesprachen** können Sie auswählen, ob Sie Updates für alle Sprachen (Standardeinstellung) oder nur für bestimmte Sprachen abrufen möchten. Wenn diesem WSUS-Server Downstreamserver zugeordnet sind, erhalten diese nur Updates in den vom Upstreamserver festgelegten Sprachen.

5.  Klicken Sie auf **OK**, um diese Einstellungen zu speichern.

Nach dem Konfigurieren der Netzwerkverbindung können Sie Updates herunterladen, indem Sie den WSUS-Server synchronisieren.

Beim Synchronisieren stellt der WSUS-Server eine Verbindung zu Microsoft Update her. Wenn die Verbindung hergestellt ist, stellt WSUS fest, ob seit der letzten Synchronisierung neue Updates zur Verfügung gestellt wurden. Da es sich hier um die erste Synchronisierung des WSUS-Servers handelt, sind alle Updates verfügbar und können für die Installation genehmigt werden. Die erste Synchronisierung nimmt möglicherweise einige Zeit in Anspruch.

> [!NOTE]
> In diesem Dokument wird das Synchronisieren mit den Standardeinstellungen beschrieben, WSUS umfasst jedoch auch Optionen, durch die Sie die Bandbreitenauslastung während der Synchronisierung reduzieren können. 

**So synchronisieren Sie den WSUS-Server**
1.  Wählen Sie in der WSUS-Verwaltungskonsole **Synchronisierungen** aus.

2.  Klicken Sie mit der rechten Maustaste, oder klicken Sie rechts im Fenster **Aktionen** auf **Jetzt synchronisieren**.

> [!NOTE]
> Wenn das Fenster **Aktionen** nicht auf der rechten Seite der Konsole angezeigt wird, klicken Sie auf der Symbolleiste der Konsole auf **Ansicht** und dann auf **Anpassen**. Stellen Sie sicher, dass das Kontrollkästchen **Aktionsbereich** aktiviert ist. 

Klicken Sie nach Abschluss der Synchronisierung im linken Bildschirmbereich auf **Updates**, um eine Liste der Updates anzuzeigen.
