---
TOCTitle: 'Schritt 2: Installieren von WSUS auf dem Server'
Title: 'Schritt 2: Installieren von WSUS auf dem Server'
ms:assetid: 'f593532c-e92e-47f3-914a-38a6c2519e94'
ms:contentKeyID: 18127669
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708622(v=WS.10)'
---

Schritt 2: Installieren von WSUS auf dem Server
===============================================

Nach dem Überprüfen der Installationsanforderungen können Sie WSUS installieren. Sie müssen sich mit einem Konto, das Mitglied der lokalen Gruppe **Administratoren** ist, auf dem Server anmelden, auf dem Sie WSUS installieren möchten. Nur Mitglieder der lokalen Gruppe **Administratoren** können WSUS installieren.

Beim folgenden Verfahren werden die standardmäßigen Installationsoptionen von WSUS für Windows Server 2003 verwendet. Dazu gehören das Installieren von Windows SQL Server 2000 Desktop Engine (WMSDE) für die WSUS-Datenbanksoftware, das lokale Speichern von Updates und das Verwenden der IIS-Standardwebsite auf Port 80. Verfahren für benutzerdefinierte Installationsoptionen, wie z. B. das Verwenden eines anderen Betriebssystems, anderer Datenbanksoftware oder einer Website mit einer benutzerdefinierten Portnummer, finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache).

**So installieren Sie WSUS unter Windows Server 2003**
1.  Doppelklicken Sie auf die Installerdatei **WSUSSetup.exe**.

    | ![](images/Cc708622.note(WS.10).gif)Hinweis                                                                                                                                                                                                 |
    |--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Die neueste Version von **WSUSSetup.exe** steht auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=47374) zu Windows Server Update Services unter **http://go.microsoft.com/fwlink/?LinkId=24384** (möglicherweise in englischer Sprache) zur Verfügung. |

2.  Klicken Sie auf der Seite **Willkommen** des Assistenten auf **Weiter**.

3.  Lesen Sie sich die Bestimmungen des Lizenzvertrags sorgfältig durch, klicken Sie auf **Ich stimme den Bedingungen des Lizenzvertrags zu**, und klicken Sie dann auf **Weiter**.

4.  Auf der Seite **Updatequelle auswählen** können Sie angeben, wo Clients Updates erhalten. Wenn Sie das Kontrollkästchen **Updates lokal speichern** aktivieren, werden Updates auf dem WSUS-Server gespeichert, und Sie wählen zum Speichern der Updates einen Speicherort im Dateisystem aus. Wenn Sie Updates nicht lokal speichern, stellen Clientcomputer eine Verbindung zu Microsoft Update her, um genehmigte Updates zu erhalten.

    Behalten Sie die Standardoptionen bei, und klicken Sie auf **Weiter**.

    ![](images/Cc708622.fa6ac6a6-6814-4b7e-96e8-e08af5e534b8(WS.10).gif)

5.  Auf der Seite **Datenbankoptionen** wählen Sie die Software aus, die zum Verwalten der WSUS-Datenbank verwendet wird. Standardmäßig bietet WSUS Setup an, WMSDE zu installieren, wenn auf dem Computer für die Installation Windows Server 2003 ausgeführt wird.

    Wenn Sie WMSDE nicht verwenden können, müssen Sie eine SQL Server-Instanz bereitstellen, die WSUS verwenden kann. Klicken Sie dazu auf **Einen vorhandenen Datenbankserver auf diesem Computer verwenden**, und geben Sie den Namen der Instanz in das Feld **SQL-Instanzname** ein. Weitere Informationen zu anderen Datenbanksoftwareoptionen als WMSDE finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache).

    Behalten Sie die Standardoptionen bei, und klicken Sie auf **Weiter**.

    ![](images/Cc708622.bc0b73ad-b338-437c-a3c7-0299e819840d(WS.10).gif)

6.  Auf der Seite **Websiteauswahl** geben Sie die Website an, die WSUS verwendet. Auf dieser Seite sind auch zwei wichtige URLs aufgeführt, die auf dieser Auswahl basieren: der URL, auf den Sie WSUS-Clients verweisen, um Updates zu erhalten, und der URL für die WSUS-Konsole, in der Sie WSUS konfigurieren.

    Wenn bereits eine Website an Port 80 angegeben ist, müssen Sie die WSUS-Website möglicherweise an einem benutzerdefinierten Port erstellen. Weitere Informationen zum Ausführen von WSUS an einem benutzerdefinierten Port finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache).

    Behalten Sie die Standardoption bei, und klicken Sie auf **Weiter**.

    ![](images/Cc708622.64ed7643-a050-4f54-bf9f-04cf7931adc0(WS.10).gif)

7.  Auf der Seite **Updateeinstellungen spiegeln** können Sie die Verwaltungsrolle für den WSUS-Server angeben. Überspringen Sie diesen Bildschirm, wenn es sich um den ersten WSUS-Server im Netzwerk handelt oder Sie eine verteilte Verwaltungstopologie möchten.

    Wenn Sie eine zentrale Verwaltungstopologie möchten und es sich nicht um den ersten WSUS-Server im Netzwerk handelt, aktivieren Sie das Kontrollkästchen, und geben Sie den Namen eines zusätzlichen WSUS-Servers im Feld **Servername** ein. Weitere Informationen zu Verwaltungsrollen finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache).

    Behalten Sie die Standardoption bei, und klicken Sie auf **Weiter**.

    ![](images/Cc708622.f26e09d5-983c-418d-8511-8960850403ef(WS.10).gif)

8.  Überprüfen Sie auf der Seite **Microsoft Windows Server Update Services kann jetzt installiert werden** die Auswahl, und klicken Sie auf **Weiter**.

    ![](images/Cc708622.20de7d09-3d30-4867-9253-6f353dd1923d(WS.10).gif)

9.  Wenn auf der letzten Seite des Assistenten bestätigt wird, dass die WSUS-Installation erfolgreich abgeschlossen wurde, klicken Sie auf **Fertig stellen**.
