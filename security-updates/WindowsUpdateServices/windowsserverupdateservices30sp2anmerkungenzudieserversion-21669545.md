---
TOCTitle: 'Windows Server Update Services 3.0 SP2 – Anmerkungen zu dieser Version'
Title: 'Windows Server Update Services 3.0 SP2 – Anmerkungen zu dieser Version'
ms:assetid: 'b3723422-489d-47b7-abfa-663353647da0'
ms:contentKeyID: 21669545
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd939886(v=WS.10)'
---

Windows Server Update Services 3.0 SP2 – Anmerkungen zu dieser Version
======================================================================

In diesen Anmerkungen wird die Version Windows Server Update Services 3.0 Service Pack 2 (WSUS 3.0 SP2) beschrieben. Dieses Dokument enthält folgende Abschnitte:

1.  Neuigkeiten in dieser Version
2.  Systemanforderungen für die WSUS 3.0 SP2-Serverinstallation
3.  Konfigurationsvoraussetzungen und Best Practice-Empfehlungen für den WSUS-Server
4.  Voraussetzungen für Windows Small Business Server
5.  Systemanforderungen für die Installation der WSUS 3.0 SP2-Remotekonsole
6.  Systemanforderungen für die Clientinstallation
7.  Upgradeanforderungen und -empfehlungen
8.  Installieren von WSUS 3.0 SP2
9.  Setup-Befehlszeilenparameter für die unbeaufsichtigte Installation von WSUS 3.0 SP2
10. Bekannte Probleme

Neuigkeiten in dieser Version
-----------------------------

-   Integration mit Windows Server 2008 R2
-   Unterstützung des BranchCache-Features unter Windows Server 2008 R2
-   Unterstützung von Windows 7-Clients
-   Client-Verbesserungen für Windows Update-Agent (WUA) Der neue WUA-Client bietet eine Reihe von Leistungsverbesserungen, Verbesserungen der Benutzerfreundlichkeit sowie ein Array von Programmfehlerbehebungen, das auf Kundenfeedback basiert.
    -   Die Client-Scanzeit ist schneller als in früheren Versionen.
    -   Von WSUS-Servern verwaltete Computer können nun „ausgewählte“ Scanvorgänge für diese WSUS-Server ausführen, anstatt einen vollständigen Scan vorzunehmen. Dies resultiert bei Verwendung von Microsoft Update APIs wie Windows Defender in deutlich schnelleren Scanvorgängen für Anwendungen.
    -   Durch die verbesserte WUA-Benutzerfreundlichkeit können die Benutzer ihre Updates besser organisieren, und der Wert und das Verhalten der Updates wird deutlich klarer.
    -   Computer mit erstelltem Abbild werden in der WSUS-Konsole deutlicher dargestellt. Weitere Informationen dazu finden Sie im Artikel [Ein auf Windows 2000, Windows Server 2003 oder Windows XP basierender Computer, der mit einem Abbild von Windows 2000, Windows Server 2003 oder Windows XP eingerichtet wurde, wird in der WSUS-Konsole nicht angezeigt](http://go.microsoft.com/fwlink/?linkid=159749).
-   Neue Features:
    -   Mit Regeln für die automatische Genehmigung können Sie nun den Stichtag und die Uhrzeit für die Genehmigung für alle Computer oder bestimmte Computergruppen festlegen.
    -   Das Auswählen von Sprachen auf Downstreamservern wurde verbessert, und es wird ein neues Warnungsdialogfeld angezeigt, wenn Sie Updates nur für bestimmte Sprachen herunterladen möchten.
    -   Neue Update- und Computerstatusberichte ermöglichen die Filterung von Updates, die für die Installation genehmigt wurden. Sie können diese Berichte über die WSUS-Konsole ausführen oder diese Funktion mithilfe der API (Application Programming Interface) in Ihre eigenen Berichte integrieren.
-   Die Benutzeroberfläche ist zwischen Service Pack 1 und Service Pack 2 für WSUS 3.0 sowohl auf dem Client als auch auf dem Server kompatibel.
-   Softwareupdates
-   Bekannte Probleme mit dem Windows Update-Agent, die in dieser Version behoben wurden:
    1.  WSUS 3.0 SP2 und Windows 7 beinhalten eine neue Version des Windows Update-Agents (für Windows XP, Windows Vista, Windows Server 2000, Windows Server 2003 und Windows Server 2008). Mit dieser Version wird das folgende Problem behoben: APIs, die von nicht lokalen Systemaufrufern in einer nicht interaktiven Sitzung aufgerufen werden, schlagen fehl.
    2.  Problem, das mit Version 7.2.6001.788 des Windows Update-Agents behoben wird. Mit diesem Update wird das folgende Problem behoben: Wenn versucht wird, 80 oder mehr Updates über die Windows Update-Website oder über die Microsoft Update-Website gleichzeitig zu installieren, wird möglicherweise der Fehlercode „0x80070057“ angezeigt.
    3.  Verbesserungen und Probleme, die mit Version 7.2.6001.784 des Windows Update-Agents behoben werden. Dieses Update beinhaltet Folgendes: Verbesserte Überprüfungszeiten für Windows Update, schnellere Bereitstellung von Signaturupdates, Unterstützung der Neuinstallationsfunktion von Windows Installer und verbesserte Fehlermeldung

<span id="BKMK_SysReqWSUS30SP2"></span>
Systemanforderungen für die WSUS 3.0 SP2-Serverinstallation
-----------------------------------------------------------

In diesem Abschnitt werden die Anforderungen an die benötigte Software und Hardware für die Installation von WSUS 3.0 SP2 beschrieben.

### Softwarevoraussetzungen für den WSUS-Server

-   Eines der folgenden unterstützten Betriebssysteme muss installiert sein:
    -   Windows Server 2008 R2
    -   Windows Server 2008 SP1 oder neuere Versionen
<p> </p>
        <table style="border:1px solid black;">
        <colgroup>
        <col width="100%" />
        </colgroup>
        <thead>
        <tr class="header">
        <th><img src="images/Dd939886.Warning(WS.10).gif" />Warnung</th>
        </tr>
        </thead>
        <tbody>
        <tr class="odd">
        <td style="border:1px solid black;">Wenn WSUS 3.0 SP2 unter Windows Server 2008 installiert wird, bevor Sie ein Upgrade auf Windows Server 2008 R2 ausführen, schlägt das Upgrade auf Windows Server 2008 R2 fehl. Weitere Informationen dazu finden Sie im Abschnitt <a href="#bkmk_knownissues">Bekannte Probleme</a>.
        <p></p></td>
        </tr>
        </tbody>
        </table>
<p> </p>

    -   Windows Server 2003 SP1 oder neuere Versionen
    -   Windows Small Business Server 2008
    -   Windows Small Business Server 2003

    Beachten Sie, dass für Windows Small Business Server zusätzliche Voraussetzungen gelten. Weitere Informationen finden Sie im Abschnitt „Voraussetzungen für Windows Small Business Server“.
-   Internetinformationsdienste (IIS) 6.0 oder neuere Versionen
-   Microsoft .NET Framework 2.0 oder neuere Versionen
-   Eine der folgenden unterstützten Datenbanken muss installiert sein:
    -   Microsoft SQL Server 2008 Standard oder Enterprise Edition
    -   Microsoft SQL Server 2005 SP3 oder neuere Versionen
    -   Windows Internal Database

    Wenn keine der unterstützten Versionen von SQL Server installiert ist, wird Windows Internal Database vom Setup-Assistenten für WSUS 3.0 SP2 installiert.
-   Microsoft Management Console 3.0
-   Microsoft Report Viewer Redistributable 2008

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Important(WS.10).gif" />Wichtig</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Für Windows Server 2008 R2 ist WSUS 3.0 SP2 erforderlich. Wenn Sie Windows Server 2008 R2 installieren, sollten Sie WSUS 3.0 SP2 installieren. Verwenden Sie nicht WSUS 3.0 SP1 für Windows Server 2008 R2.
<p></p>  
In einer Remote-SQL-Konfiguration wird WSUS 3.0 SP2 nicht für die Verwendung für die Terminaldienste auf dem Front-End-Server unterstützt.
<p></p></td>
</tr>
</tbody>
</table>
<p> </p>

### Softwarevoraussetzungen für die WSUS-Verwaltungskonsole

-   Eines der folgenden unterstützten Betriebssysteme: Windows Server 2008 R2, Windows Server 2008, Windows Server 2003 SP2 oder neuere Versionen, Windows Small Business Server 2008 oder Windows Small Business Server 2003, Windows Vista oder Windows XP SP2
-   Microsoft .NET Framework 2.0 oder neuere Versionen
-   Microsoft Management Console 3.0
-   Microsoft Report Viewer Redistributable 2008

### Hardwaremindestanforderungen für den WSUS-Server

Die folgende Liste enthält die Hardwaremindestanforderungen, die für eine grundlegende Serverinstallation erfüllt sein müssen. Eine umfassende Liste der unterstützten Hardwarekonfigurationen finden Sie im WSUS 3.0 SP2-Bereitstellungshandbuch unter [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832).

-   Die Systempartition und die Partition, auf der WSUS 3.0 SP2 installiert wird, müssen mit dem NTFS-Dateisystem formatiert sein.
-   Mindestens 1 GB freier Speicherplatz auf der Systempartition.
-   Mindestens 2 GB freier Speicherplatz auf dem Datenträger, auf dem die Datenbankdateien gespeichert werden.
-   Mindestens 20 GB freier Speicherplatz auf dem Datenträger, auf dem Inhalte gespeichert werden (empfohlen werden 30 GB).

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Important(WS.10).gif" />Wichtig</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">WSUS 3.0 SP2 kann nicht auf komprimierten Laufwerken installiert werden.
<p></p></td>
</tr>
</tbody>
</table>
<p> </p>

Konfigurationsvoraussetzungen und Best Practice-Empfehlungen für den WSUS-Server
--------------------------------------------------------------------------------

Stellen Sie sicher, dass Sie die erforderlichen Aufgaben in diesem Abschnitt ausgeführt haben, bevor Sie WSUS 3.0 SP2 installieren.

### IIS

-   Installieren Sie auf der Seite „Rollendienste für Webserver (IIS)“ von Server-Manager die erforderlichen Features, alle IIS-Standardrollendienste und die folgenden Rollendienste: **ASP.NET**, **Windows-Authentifizierung**, **Dynamische Inhaltskomprimierung** und **IIS 6-Verwaltungskompatibilität**.
-   Wenn IIS im IIS 5.0-Isolationsmodus ausgeführt wird, schlägt die Installation fehl. Deaktivieren Sie den IIS 5.0-Isolationsmodus, bevor Sie WSUS 3.0 SP2 installieren.
-   Wenn IIS-Komponenten im 32-Bit-Kompatibilitätsmodus auf einer 64-Bit-Plattform installiert sind, kann die Installation von WSUS 3.0 SP2 fehlschlagen. Alle IIS-Komponenten sollten auf 64-Bit-Plattformen im 64-Bit-Modus installiert werden.

### Proxyserver

Mit WSUS 3.0 SP2 kann ein Proxyserver nur HTTP unterstützen. Als Best Practice wird empfohlen, einen zweiten Proxyserver für HTTPS über die Befehlszeile zu konfigurieren (**wsusutil configuresslproxy**), bevor Sie den WSUS-Server mithilfe des Konfigurations-Assistenten oder der Verwaltungskonsole konfigurieren.

### Websites auf Port 80

Wenn zwei oder mehrere Websites auf Port 80 ausgeführt werden (zum Beispiel Windows SharePoint Services), löschen Sie vor der WSUS-Installation alle bis auf eine davon. Andernfalls kann es sein, dass die Clients des Servers kein Selbstupdate durchführen.

### Antivirenprogramme

Beim Installieren von WSUS 3.0 SP2 müssen Antivirenprogramme möglicherweise deaktiviert werden, damit die Installation erfolgreich ausgeführt werden kann. Starten Sie den Computer nach dem Deaktivieren der Antivirensoftware neu, bevor Sie mit der Installation von WSUS beginnen. Durch den Neustart wird verhindert, dass für den Installationsvorgang erforderliche Dateien gesperrt werden. Aktivieren Sie die Antivirensoftware wieder, nachdem die Installation abgeschlossen ist. Auf der Website des Herstellers Ihrer Antivirensoftware finden Sie genaue Anweisungen zum Deaktivieren und erneuten Aktivieren Ihrer Antivirensoftware und Version.

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th><img src="images/Dd939886.Caution(WS.10).gif" />Vorsicht</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Diese Problemumgehung kann die Sicherheit des Computers oder Netzwerks vor Angriffen böswilliger Benutzer oder schädlicher Software wie Viren beeinträchtigen. Dieses Verfahren wird nicht empfohlen. Die Informationen werden jedoch zur Verfügung gestellt, damit Sie die Problemumgehung nach eigenem Ermessen verwenden können. Verwenden Sie diese Problemumgehung auf eigene Gefahr.
<p></p>  
Antivirensoftware soll Ihren Computer vor Viren schützen. Laden Sie keine Dateien von nicht vertrauenswürdigen Quellen herunter, bzw. öffnen Sie diese Dateien nicht, rufen Sie keine nicht vertrauenswürdigen Websites auf, und öffnen Sie keine E-Mail-Anlagen, während das Antivirenprogramm deaktiviert ist.
<p></p></td>
</tr>
</tbody>
</table>
<p> </p>

### Option für geschachtelte Trigger in SQL Server

Wenn Sie eine SQL Server-Datenbank als Datenspeicher für Windows Server Update Services verwenden möchten, sollte der SQL Server-Administrator überprüfen, ob die Option für geschachtelte Trigger auf dem Server aktiviert ist, bevor der WSUS-Administrator WSUS 3.0 SP2 installiert. Die Option für geschachtelte Trigger ist standardmäßig aktiviert. Sie kann jedoch vom SQL Server-Administrator deaktiviert werden. Die datenbankspezifische Funktion RECURSIVE\_TRIGGERS wird vom WSUS 3.0 SP2-Setup aktiviert. Die globale Serveroption für geschachtelte Trigger wird vom WSUS 3.0 SP2-Setup jedoch nicht aktiviert.

### Einschränkungen und Anforderungen für Remote-SQL

WSUS 3.0 SP2 unterstützt die Ausführung einer kompatiblen Version von SQL Server-Software auf einem anderen Computer als dem, auf dem die WSUS 3.0 SP2-Anwendung ausgeführt wird. Für eine Remote-SQL-Installation gelten folgende Anforderungen.

-   Als Back-End des Remote-SQL-Paars kann kein als Domänencontroller konfigurierter Server verwendet werden.
-   Auf dem Computer, der als Front-End-Server einer Remote-SQL-Installation eingerichtet wird, können die Terminaldienste nicht ausgeführt werden.
-   Der Front-End- und der Back-End-Computer müssen Mitglied derselben Active Directory-Domäne sein. Wenn sich der Front-End- und der Back-End-Computer in unterschiedlichen Domänen befinden, stellen Sie eine domänenübergreifende Vertrauensstellung zwischen den Domänen her, bevor Sie das WSUS-Setup ausführen.
-   Wenn Sie WSUS 2.0 bereits in einer Remote-SQL-Konfiguration installiert haben und auf WSUS 3.0 SP2 aktualisieren möchten, führen Sie folgende Schritte aus, bevor Sie WSUS installieren:
    1.  Deinstallieren Sie WSUS 2.0 (mithilfe von **Software** in der Systemsteuerung), aber stellen Sie dabei sicher, dass die vorhandene Datenbank intakt bleibt.
    2.  Installieren Sie SQL Server 2005 SP2 oder SQL Server 2008, und aktualisieren Sie die vorhandene Datenbank.

### IIS wird während des WSUS 3.0 SP2-Setups neu gestartet

IIS wird vom WSUS 3.0 SP2-Setup ohne Benachrichtigung neu gestartet. Dies hat möglicherweise Auswirkungen auf vorhandene Websites in Ihrer Organisation. Als Best Practice wird empfohlen, alle Betroffenen vor der Installation zu informieren. Beachten Sie, dass IIS vom WSUS 3.0 SP2-Setup gestartet wird, falls IIS nicht bereits ausgeführt wird.

Voraussetzungen für Windows Small Business Server
-------------------------------------------------

Wenn Sie WSUS 3.0 SP2 unter Windows Small Business Server installieren, gelten folgende Voraussetzungen.

### Wenn der virtuelle IIS-Stamm auf bestimmte IP-Adressen oder Domänennamen eingeschränkt ist

Bei einigen Installationen von Windows Small Business Server ist die IIS-Standardwebsite in den **Einschränkungen für IP-Adressen und Domänennamen** enthalten. In diesem Fall kann sich der Windows Update-Client auf dem Server möglicherweise nicht selbst aktualisieren. Entfernen Sie die Einschränkung, bevor Sie WSUS 3.0 SP2 installieren.

### Wenn Sie einen ISA-Proxyserver verwenden

-   Wenn in Windows Small Business Server ein ISA-Proxyserver für den Zugriff auf das Internet verwendet wird, geben Sie auf der Benutzeroberfläche unter **Einstellungen** folgende Informationen ein: **Proxyservereinstellungen, Proxyservername, Port**.
-   Wenn ISA die Windows-Authentifizierung verwendet, geben Sie die Anmeldeinformationen für den Proxyserver im Format *DOMÄNE*\\*Benutzer* ein. Der Benutzer muss Mitglied der Gruppe „Internetbenutzer“ sein.

### Wenn Sie Ihrem Netzwerk ohne die Windows Small Business Server-Assistenten ein Subnetz hinzugefügt haben

Während des Setupvorgangs des WSUS-Servers werden zwei virtuelle IIS-Stämme auf dem Server installiert: SelfUpdate und ClientWebService. Zudem werden beim Setup einige Dateien im Stammverzeichnis der Standardwebsite (auf Port 80) erstellt, mit denen Clientcomputer über die Standardwebsite ein Selbstupdate durchführen können. Normalerweise ist die Standardwebsite so konfiguriert, dass der Zugriff für alle IP-Adressen bis auf den lokalen Host bzw. für bestimmte mit dem Server verbundene Subnetze verweigert wird. Clientcomputer, die sich nicht auf dem lokalen Host oder in diesen bestimmten Subnetzen befinden, können daher kein Selbstupdate durchführen. Wenn Sie dem Netzwerk ein Subnetz hinzugefügt haben, ohne die Microsoft Windows Small Business Server-Assistenten zu verwenden, führen Sie folgende Schritte aus:

1.  Erweitern Sie in der Serververwaltung die Optionen **Erweiterte Verwaltung**, **Internetinformationsdienste**, **Websites** sowie **Standardwebsite**. Klicken Sie mit der rechten Maustaste auf das virtuelle Verzeichnis **Selbstaktualisierung**, und klicken Sie dann auf **Eigenschaften**.
2.  Klicken Sie auf **Verzeichnissicherheit**.
3.  Klicken Sie unter **Einschränkungen für IP-Adressen und Domänennamen** auf **Bearbeiten** und dann auf **Zugriff gewährt**.
4.  Klicken Sie auf **OK**. Klicken Sie mit der rechten Maustaste auf das virtuelle Verzeichnis **ClientWebService**, und klicken Sie dann auf **Eigenschaften**.
5.  Klicken Sie auf **Verzeichnissicherheit**.
6.  Klicken Sie unter **Einschränkungen für IP-Adressen und Domänennamen** auf **Bearbeiten** und dann auf **Zugriff gewährt**.

Systemanforderungen für die Installation der WSUS 3.0 SP2-Remotekonsole
-----------------------------------------------------------------------

Die WSUS 3.0 SP2-Remotekonsole kann unter folgenden Betriebssystemen installiert werden:

-   Windows Server 2008 R2, Windows Server 2008 SP1 oder neuere Versionen, Windows Server 2003 SP2 oder neuere Versionen, Windows Small Business Server 2003, Windows Small Business Server 2005 oder Windows Small Business Server 2008, Windows Vista, Windows XP Professional SP3 oder neuere Versionen

Systemanforderungen für die WSUS-Clientinstallation
---------------------------------------------------

Automatische Updates bzw. die WSUS-Clientsoftware können unter folgenden Betriebssystemen installiert werden:

-   Windows Server 2008 R2, Windows Server 2008 SP1 oder neuere Versionen, Windows Server 2003 SP2 oder neuere Versionen, Windows Small Business Server 2003, Windows Small Business Server 2005 oder Windows Small Business Server 2008, Windows Vista, Windows XP Professional RTM, Windows XP Professional SP1, Windows XP Professional SP2, Windows XP Professional SP3 oder neuere Versionen, Windows 2000 SP4 oder Windows 7.

Upgradeanforderungen und -empfehlungen
--------------------------------------

Die folgenden Versionen von WSUS können auf WSUS 3.0 SP2 aktualisiert werden, ohne dass die ältere Version deinstalliert werden muss:

-   WSUS 2.0, 2.0 SP1, 3.0 und 3.0 SP1

Upgrades von WSUS 1.0 auf WSUS 3.0 SP2 werden nicht unterstützt. Deinstallieren Sie SUS 1.0 (Software Update Services), bevor Sie WSUS 3.0 SP2 installieren.

Für Windows Server 2008 R2 ist WSUS 3.0 SP2 erforderlich. Wenn Sie Windows Server 2008 R2 installieren, sollten Sie WSUS 3.0 SP2 installieren. Verwenden Sie nicht WSUS 3.0 SP1 für Windows Server 2008 R2.

#### Vor dem Upgrade auf WSUS 3.0 SP2

1.  Überprüfen Sie, ob in den Ereignisprotokollen der letzten Zeit Fehler erfasst wurden und ob Probleme bei der Synchronisierung zwischen Downstream- und Upstreamservern oder bei der Clientberichterstellung aufgetreten sind. Beheben Sie diese Probleme vor dem Upgrade.

2.  Führen Sie optional DBCC CHECKDB aus, um sicherzustellen, dass die WSUS-Datenbank korrekt indiziert ist. Weitere Informationen zu DBCC CHECKDB finden Sie unter [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948).

3.  Sichern Sie die WSUS-Datenbank. Beachten Sie, dass die neue Datenbank während des WSUS 3.0 SP2-Setups dem Standardverzeichnis *Laufwerk*\\WSUS hinzugefügt wird (*Laufwerk* steht für das lokale NTFS-Laufwerk, das über den größten freien Speicherplatz verfügt). Wenn sich in diesem Verzeichnis bereits eine Datenbanksicherung befindet, wird diese möglicherweise überschrieben. Als Best Practice wird empfohlen, eine Datenbanksicherung der aktuellen Version von WSUS in einem anderen Verzeichnis zu speichern, bevor das Upgrade auf WSUS 3.0 SP2 durchgeführt wird.

4.  Wenn Sie den von WSUS verwendeten Port manuell geändert haben (also nicht das Hilfsprogramm „Wsusutil“ verwendet haben) und derzeit SUS 1.0 oder WSUS 2.0 verwenden, starten Sie die Standardwebsite, bevor Sie SUS 1.0 oder WSUS 2.0 64-Bit deinstallieren.

5.  Wenn Verbindungen zu einer vorhandenen WSUS-Datenbank hergestellt sind (z. B. wenn SQL Server Management Studio geöffnet ist), kann die Installation fehlschlagen. Trennen Sie alle Verbindungen, bevor Sie WSUS 3.0 SP2 installieren.

### Wiederherstellung nach einem fehlgeschlagenen Upgrade

Wenn Sie eine ältere Version von WSUS auf WSUS 3.0 SP2 aktualisieren und das Upgrade fehlschlägt, führen Sie die folgenden Schritte aus (es sei denn, Sie haben ein nicht unterstütztes Upgrade von SUS 1.0 versucht).

1.  Installieren Sie die ältere Version von WSUS erneut.
2.  Stellen Sie mithilfe der Sicherung, die Sie vor dem Upgradeversuch erstellt haben, die Datenbank wieder her. Ein erfolgreiches Upgrade ist nicht möglich, wenn eine WSUS 3.0 SP2-Datenbank aus einer vorherigen Installation vorhanden ist. In den meisten Fällen wird von WSUS automatisch eine Sicherung erstellt. Das Verzeichnis finden Sie in der Datei „WSUSSetup.log“.
3.  Bestimmen Sie mithilfe der Protokolle die Fehlerursache, und beheben Sie das Problem.
4.  Installieren Sie WSUS 3.0 SP2.

### Durch eine Änderung des Computernamens vor dem Upgrade auf WSUS 3.0 SP2 kann das Upgrade fehlschlagen

Wenn der Computername nach der Installation von WSUS 2.0 und vor dem Upgrade auf WSUS 3.0 SP2 geändert wird, kann das Upgrade fehlschlagen.

Mithilfe des folgenden Skripts können Sie die Administratorgruppen ASPNET und WSUS entfernen und erneut hinzufügen. Führen Sie das Upgrade anschließend erneut durch.

        ```

### Wenn Sie eine Migration von MSDE zu SQL Server 2008 oder SQL Server 2005 unter WSUS 2.0 durchgeführt haben, müssen Sie einen Registrierungswert ändern

Wenn Sie WSUS 2.0 installiert und eine Migration zu SQL Server 2008 oder SQL Server 2005 durchgeführt haben, müssen Sie den Wert **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** von 1 auf 0 ändern. Dies muss vor dem Upgrade auf WSUS 3.0 SP2 erfolgen, da dieses ansonsten fehlschlägt.

### Wenn WSUS 3.0 SP2 deinstalliert wird und die Protokolldateien beibehalten werden, ändern sich möglicherweise die zugehörigen Berechtigungen nach einer Neuinstallation

Bei der Deinstallation von WSUS 3.0 SP2 haben Sie die Option, die Protokolldateien der Installation beizubehalten. Wenn Sie WSUS 3.0 SP2 erneut installieren, verlieren die alten Protokolldateien möglicherweise ihre Berechtigungen (normalerweise nur für WSUS-Administratoren). Als Best Practice wird empfohlen, die Berechtigungen für diese Protokolldateien nach der Installation zu bestätigen.

### Wenn WSUS 2.0-Clients Updates mit dem Status „Nicht zutreffend“ aufweisen, werden die Updates eine kurze Zeit lang nach dem Upgrade auf WSUS 3.0 SP2 als „Unbekannt“ angezeigt.

Wenn Clients eines vorhandenen WSUS 2.0-Servers Updates mit dem Status **Nicht zutreffend** aufweisen, werden diese Updates nach dem Upgrade auf WSUS 3.0 SP2 möglicherweise eine kurze Zeit lang als **Unbekannt** aufgelistet. Nach der nächsten Prüfung auf dem Client wird wieder der Updatestatus **Nicht zutreffend** angezeigt.

Installieren von WSUS 3.0 SP2
-----------------------------

In der schrittweisen Installationsanleitung für WSUS unter [http://go.microsoft.com/fwlink/?LinkId=139836](http://go.microsoft.com/fwlink/?linkid=139836) finden Sie Anweisungen für die Installation von WSUS 3.0 SP2 mit dem Windows Server-Manager oder der Datei „WSUSSetup.exe“.

Vollständige Informationen zur Installation und Verwendung von WSUS finden Sie hier:

WSUS-Bereitstellungshandbuch unter [http://go.microsoft.com/fwlink/?LinkId=139832](http://go.microsoft.com/fwlink/?linkid=139832) (in englischer Sprache).

WSUS-Handbuch unter [http://go.microsoft.com/fwlink/?LinkId=139838](http://go.microsoft.com/fwlink/?linkid=139838) (in englischer Sprache).

Setup-Befehlszeilenparameter für die unbeaufsichtigte Installation von WSUS 3.0 SP2
-----------------------------------------------------------------------------------

Mithilfe des WSUS-Setupprogramms für die Befehlszeile können Sie unbeaufsichtigte Installationen von WSUS 3.0 SP2 durchführen. In dieser Tabelle werden die Befehlszeilenparameter für das Setup von WSUS 3.0 SP2 aufgeführt.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Option</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/q</strong></p></td>
<td style="border:1px solid black;"><p>Automatische Installation durchführen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p><strong>/u</strong></p></td>
<td style="border:1px solid black;"><p>Deinstallieren:</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/p</strong></p></td>
<td style="border:1px solid black;"><p>Voraussetzungsprüfung: Das System wird überprüft, und nicht erfüllte Voraussetzungen werden gemeldet.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p><strong>/?, /h</strong></p></td>
<td style="border:1px solid black;"><p>Befehlszeilenparameter und deren Beschreibungen anzeigen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p><strong>/g</strong></p></td>
<td style="border:1px solid black;"><p>Upgrade von der vorherigen Version auf WSUS durchführen (Upgrades von SUS 1.0 werden nicht unterstützt). Der einzige Parameter, der mit dieser Option verwendet werden kann, ist „/q“ (automatische Installation). Die einzige Eigenschaft, die mit dieser Option verwendet werden kann, ist DEFAULT_WEBSITE.</p></td>
</tr>  
</tbody>  
</table>
  
In dieser Tabelle werden die Befehlszeileneigenschaften für WSUS 3.0 SP2 aufgeführt.
  
###  

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Eigenschaft</th>  
<th>Beschreibung</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>CONTENT_LOCAL</p></td>
<td style="border:1px solid black;"><p>0=Inhalte lokal gehostet, 1=Auf Microsoft Update gehostet</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CONTENT_DIR</p></td>
<td style="border:1px solid black;"><p>Pfad zu Verzeichnis mit Inhalten Der Standardpfad ist <em>WSUS-Installationsverzeichnis\WSUS\WSUSContent</em>, wobei <em>WSUS-Installationsverzeichnis</em> für das lokale Laufwerk mit dem größten freien Speicherplatz steht.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>WYUKON_DATA_DIR</p></td>
<td style="border:1px solid black;"><p>Pfad zum Datenverzeichnis der Windows Internal Database.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>SQLINSTANCE_NAME</p></td>
<td style="border:1px solid black;"><p>Der Name sollte im Format <em>Servername</em>\<em>SQL-Instanzname</em> angezeigt werden. Wenn sich die Datenbankinstanz auf dem lokalen Computer befindet, verwenden Sie die Umgebungsvariable „%COMPUTERNAME%“. Wenn keine Instanz vorhanden ist, wird als Standard „%COMPUTERNAME%\WSUS“ festgelegt.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DEFAULT_WEBSITE</p></td>
<td style="border:1px solid black;"><p>0=Port 8530, 1=Port 80</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PREREQ_CHECK_LOG</p></td>
<td style="border:1px solid black;"><p>Pfad und Dateiname für Protokolldatei</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>CONSOLE_INSTALL</p></td>
<td style="border:1px solid black;"><p>0=WSUS-Server installieren, 1=Nur Konsole installieren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ENABLE_INVENTORY</p></td>
<td style="border:1px solid black;"><p>0=Inventurfeatures nicht installieren, 1=Inventurfeatures installieren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DELETE_DATABASE</p></td>
<td style="border:1px solid black;"><p>0=Datenbank beibehalten, 1=Datenbank entfernen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>DELETE_CONTENT</p></td>
<td style="border:1px solid black;"><p>0=Inhaltsdateien beibehalten, 1=Inhaltsdateien entfernen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DELETE_LOGS</p></td>
<td style="border:1px solid black;"><p>0=Protokolldateien beibehalten, 1=Protokolldateien entfernen (Verwendung mit dem Installationsparameter &quot;/u&quot;)</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>CREATE_DATABASE</p></td>
<td style="border:1px solid black;"><p>0=Aktuelle Datenbank verwenden, 1=Datenbank erstellen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>PROGRESS_WINDOW_HANDLE</p></td>
<td style="border:1px solid black;"><p>Fensterhandle zur Rückgabe von Windows Installer-Statusmeldungen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MU_ROLLUP</p></td>
<td style="border:1px solid black;"><p>1=Am Programm zur Verbesserung von Microsoft Update teilnehmen, 0=Nicht am Programm zur Verbesserung von Microsoft Update teilnehmen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>FRONTEND_SETUP</p></td>
<td style="border:1px solid black;"><p>1=Inhaltsordner nicht in die Datenbank schreiben, 0=Inhaltsordner in die Datenbank schreiben (für NLB)</p></td>
</tr>  
</tbody>  
</table>
  
### Beispiel:
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (Installation im stillen Modus über Port 8530) WSUSSetup.exe /q /u (Deinstallation von WSUS)  
```
<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="100%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><img src="images/Dd939886.Important(WS.10).gif" />Wichtig</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;">Wenn Sie WSUS 3.0 SP2 im stillen Modus (/q) installieren, und auf dem Computer nicht alle vorausgesetzten Komponenten installiert sind, wird während der Installation eine Datei mit der Bezeichnung „WSUSPreReqCheck.xml“ erstellt und im Verzeichnis „%TEMP%“ gespeichert.
<p></p></td>
</tr>
</tbody>
</table>
<p> </p>

<span id="BKMK_KnownIssues"></span>
Bekannte Probleme
-----------------

-   Nach dem erfolgreichen Abschluss des WSUS-Installations-Assistenten wird der Benutzer zum Klicken auf **Fertig stellen** aufgefordert. In seltenen Fällen wird ein Fehlerdialogfeld angezeigt, das folgende Meldung enthält: „**Bei der Kommunikation mit dem Server ist ein Fehler aufgetreten. Daher muss dieser Assistent geschlossen werden. Sie können den Assistenten für die WSUS-Serverkonfiguration auf der Seite „Optionen“ in der WSUS-Konsole neu starten.**“ Um sicherzustellen, dass Ihre Installationsauswahl gespeichert wurde, öffnen Sie in der WSUS-Verwaltungskonsole die Seite **Optionen**, und bestätigen Sie die Einstellungen in den einzelnen Abschnitten.
-   **Lokalisierte Versionen von WUA (Windows Update-Agent) werden nach WSUS 3.0 SP2 veröffentlicht**. Die Ursache dafür ist eine Abhängigkeit vom Lokalisierungszeitplan für Windows 7. Zwischen den Veröffentlichungen von WSUS 3.0 SP2  und der lokalisierten Version des WUA-Clients unterstützt der WUA-Client nur fünf Sprachen (Englisch, Deutsch, Französisch, Spanisch und Japanisch).
-   **Die in dieser SP2-Version eingeführten, neuen Update- und Computerstatusberichte können nicht in Umgebungen verwendet werden, in denen Downstreamserver mit WSUS 3.0 SP1 von einem WSUS 3.0 SP2-Server verwaltet werden**. Wenn die neuen Berichte für einen SP1-Server ausgeführt werden, wird die folgende Fehlermeldung angezeigt: „Beim Generieren des Berichts ist ein Fehler aufgetreten. Führen Sie den Bericht erneut aus, oder wenden Sie sich an den Netzwerkadministrator, wenn das Problem weiterhin besteht.“ Durch die erneute Ausführung des Berichts wird das Problem nicht gelöst. Das Problem bezieht sich auch nicht auf das Netzwerk. Die neuen Berichte sind von der API-Funktionalität abhängig, die in SP1 nicht vorhanden ist. Beim Verwalten eines SP1-Servers werden die neuen Berichte jedoch nicht von der SP2-Verwaltungskonsole blockiert.
-   **Das Upgrade auf WSUS 3.0 SP2 schlägt fehl, wenn SSL ohne Zertifikatnamen konfiguriert wurde**. Wenn Sie SSL konfigurieren, ist ein Zertifikatname erforderlich.
-   **Durch WSUS 3.0 SP2 mit Windows Internal Database, das unter Windows Server 2008 installiert ist, werden Upgrades auf Windows Server 2008 R2** verhindert. Vor dem Fortsetzen des Upgrades auf Windows Server 2008 R2 wird eine Fehlermeldung eines Kompatibilitätsberichts angezeigt, in der Sie zum Deaktivieren von Windows Internal Database angewiesen werden. Bevor Sie das Upgrade auf Windows Server 2008 R2 fortsetzen können, müssen Sie ein Upgrade für Windows Internal Database durchführen. Anweisungen und weitere Informationen zu Upgrades finden Sie unter [Abrufen des neuesten Service Packs für die Windows Internal Database](http://go.microsoft.com/fwlink/?linkid=162104) (http://go.microsoft.com/fwlink/?LinkId=162104)Windows Internal Database.

Urheberrechtshinweis
--------------------

Die Informationen in diesem Dokument, einschließlich URLs und anderer Verweise auf Internetwebsites, können ohne vorherige Ankündigung geändert werden. Die in den Beispielen verwendeten Firmen, Organisationen, Produkte, Domänenamen, E-Mail-Adressen, Logos, Personen, Orte und Ereignisse sind frei erfunden, soweit nicht anders angegeben. Jede Ähnlichkeit mit bestehenden Firmen, Organisationen, Produkten, Domänennamen, E-Mail-Adressen, Logos, Personen, Orten oder Ereignissen ist rein zufällig. Die Benutzer sind verpflichtet, sich an alle geltenden Urheberrechtsgesetze zu halten. Unabhängig von der Anwendbarkeit der entsprechenden Urheberrechtsgesetze darf ohne ausdrückliche schriftliche Erlaubnis der Microsoft Corporation kein Teil dieses Dokuments für irgendwelche Zwecke vervielfältigt, in einem Datenempfangssystem gespeichert oder darin eingelesen oder übertragen werden, unabhängig davon, auf welche Art und Weise oder mit welchen Mitteln (elektronisch, mechanisch, durch Fotokopieren, Aufzeichnen usw.) dies geschieht.

Möglicherweise besitzt Microsoft Rechte an Patenten bzw. angemeldeten Patenten, an Marken, Urheberrechten oder sonstigem geistigen Eigentum, die sich auf den fachlichen Inhalt dieses Dokuments beziehen. Das Bereitstellen dieses Dokuments gibt Ihnen jedoch keinen Anspruch auf diese Patente, Marken, Urheberrechte oder auf sonstiges geistiges Eigentum, es sei denn, dieser wird ausdrücklich in den schriftlichen Lizenzverträgen von Microsoft eingeräumt.

© 2009 Microsoft Corporation. Alle Rechte vorbehalten.

Microsoft, Active Directory, ActiveX, Authenticode, Excel, InfoPath, Internet Explorer, MSDN, Outlook, Visual Studio, Win32, Windows, Windows Server und Windows Vista sind Marken der Microsoft Corporation.

Alle weiteren Marken sind Eigentum der jeweiligen Inhaber.
