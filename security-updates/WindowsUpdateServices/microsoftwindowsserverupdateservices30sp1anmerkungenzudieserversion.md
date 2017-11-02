---
TOCTitle: 'Microsoft Windows Server Update Services 3.0 SP1 – Anmerkungen zu dieser Version'
Title: 'Microsoft Windows Server Update Services 3.0 SP1 – Anmerkungen zu dieser Version'
ms:assetid: 'a5aa93bf-842b-4ad4-ab0f-fe867843cb02'
ms:contentKeyID: 18127564
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708525(v=WS.10)'
---

Microsoft Windows Server Update Services 3.0 SP1 – Anmerkungen zu dieser Version
================================================================================

In den Anmerkungen zu dieser Version werden bekannte Probleme im Zusammenhang mit Microsoft® Windows® Server Update Services (WSUS) 3.0 Service Pack 1 beschrieben. Darüber hinaus erhalten Sie Empfehlungen und Informationen zu Voraussetzungen für die Installation der Anwendung. Folgende Abschnitte sind enthalten:

-   Systemanforderungen für die Installation des WSUS 3.0 SP1-Servers
-   Konfigurationsanforderungen für die Installation des WSUS 3.0 SP1-Servers
-   Systemanforderungen für die Installation der Remotekonsole von WSUS 3.0 SP1
-   Systemanforderungen für die Clientinstallation
-   Softwareanforderungen für die Installation des WSUS SP1-Servers
-   Mindestanforderungen an den Datenträgerspeicherplatz für die Installation des WSUS 3.0 SP1-Servers
-   Anforderungen für WSUS 3.0 SP1-Updates
-   Befehlszeilenparameter von Setup
-   Installationsprobleme
-   Updateprobleme
-   Bekannte Probleme
-   WSUS 3.0 SP1 unter Windows Server® 2008
-   WSUS 3.0 SP1 unter Windows Small Business Server 2003

Systemanforderungen für die Installation des WSUS 3.0 SP1-Servers
-----------------------------------------------------------------

#### Unterstützung von WSUS 3.0 SP1-Server unter Windows Server 2008 und Windows Server 2003 Service Pack 1

Der WSUS 3.0 SP1-Server wird unter Windows Server 2008 und Windows Server 2003 Service Pack 1 unterstützt.

#### Keine Unterstützung von Windows 2000 Server für WSUS 3.0 SP1-Server

Microsoft Windows® 2000 Server ist kein unterstütztes Betriebssystem für WSUS 3.0 SP1-Server.

#### Keine Unterstützung für WSUS 3.0 SP1 auf Servern, die Terminaldienste ausführen

Zwar kann WSUS 3.0 SP1 möglicherweise auf Servern, die Terminaldienste ausführen, ausgeführt werden, doch diese Konstellation wird weder unterstützt noch empfohlen. WSUS 3.0 SP1 kann auf einem Server, der Terminaldienste ausführt, in Konfigurationen, die Remote-SQL Server-Implementierungen verwenden, nicht ausgeführt werden. Da alle benutzerdefinierten Remoteaktionen (einschließlich der Installation) auf einem Terminaldienste-Lizenzserver unter dem Systemkonto ausgeführt werden, schlägt die Installation fehl, wenn das Systemkonto des Servers über keine Berechtigungen auf dem Remotecomputer mit SQL Server verfügt.

Konfigurationsanforderungen für die Installation des WSUS 3.0 SP1-Servers
-------------------------------------------------------------------------

#### Installation von IIS erforderlich

Für WSUS 3.0 SP1 sind die Internetinformationsdienste (IIS) erforderlich, die standardmäßig unter Windows Server 2008 oder Microsoft Windows Server 2003 nicht installiert werden. Bei dem Versuch, WSUS 3.0 SP1 ohne IIS zu installieren, zeigt das Installationsprogramm von Windows Server Update Services eine Fehlermeldung an, die besagt, dass IIS nicht installiert ist.

#### Fehler der Installation bei Ausführung von IIS im IIS 5.0-Isolationsmodus

Wenn der Server von Windows 2000 Server auf Windows Server 2003 aktualisiert wurde, wird IIS möglicherweise im IIS 5.0-Kompatibilitätsmodus ausgeführt. Es ist auch möglich, den IIS 5.0-Isolationsmodus im IIS-Manager zu aktivieren. Hierdurch schlägt die Installation fehl. Sie müssen den IIS 5.0-Isolationsmodus vor der Installation von WSUS 3.0 SP1 deaktivieren.

#### Fehler bei der Installation von WSUS 3.0 SP1, wenn eine IIS-Komponente auf einer 64-Bit-Plattform im 32-Bit-Kompatibilitätsmodus installiert ist

Alle IIS-Komponenten müssen auf 64-Bit-Plattformen im einheitlichen Modus installiert sein. Die Installation schlägt fehl, wenn sich auch nur eine IIS-Komponente im 32-Bit-Kompatibilitätsmodus befindet.

#### Unterstützung von ausschließlich HTTP oder HTTP und HTTPS durch Proxyserver

In WSUS 3.0 SP1 ist es möglich, dass ein Proxyserver nur HTTP unterstützt. Sie müssen vor der Konfiguration des WSUS-Servers im Konfigurations-Assistenten oder der Verwaltungskonsole mithilfe der Befehlszeile (**wsusutil configuresslproxy**) einen zweiten Proxyserver konfigurieren, auf dem HTTPS ausgeführt wird.

#### Bei Ausführung von mindestens zwei Websites an Port 80 müssen alle bis auf eine vor der Installation von WSUS gelöscht werden

Wenn Sie mindestens zwei Websites an Port 80 ausführen (z. B. Windows® SharePoint® Services), müssen Sie alle bis auf eine vor der Installation von WSUS löschen. Wird dies nicht ausgeführt, kommt es zu Selbstupdatefehlern bei den Clients des Servers.

#### Deaktivieren von Antivirenprogrammen bei der Installation von WSUS 3.0 SP1 erforderlich

Bei der Installation von WSUS 3.0 SP1 müssen Sie möglicherweise Antivirenprogramme deaktivieren, damit die Installation erfolgreich ausgeführt werden kann. Starten Sie den Computer im Anschluss an die Deaktivierung der Antivirenprogramme neu, bevor Sie WSUS installieren. Durch den Neustart des Computers wird verhindert, dass Dateien gesperrt sind, wenn der Installationsprozess darauf Zugriff benötigt. Stellen Sie im Anschluss an die Installation sicher, dass die Antivirenprogramme wieder aktiviert werden. Die genaue Vorgehensweise zum Deaktivieren und erneuten Aktivieren Ihrer Antivirenprogramme und der speziellen Versionen finden Sie auf der Website des Lieferanten des Antivirenprogramms.

| ![](images/Cc708525.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                     |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diese Problemumgehung erhöht möglicherweise die Verletzbarkeit Ihres Computers oder Netzwerks gegenüber Angriffen von bösartigen Benutzern oder bösartiger Software wie Viren. Zwar wird diese Problemumgehung nicht empfohlen, doch werden die Informationen bereitgestellt, damit Sie die Implementierung der Problemumgehung nach eigenem Ermessen vornehmen können. Diese Problemumgehung wird auf eigenes Risiko verwendet. |

> [!NOTE]
> Ein Antivirenprogramm ist darauf ausgelegt, Ihren Computer vor Viren zu schützen. Wenn das Antivirenprogramm deaktiviert ist, dürfen Sie keine Dateien herunterladen oder öffnen, die aus nicht vertrauenswürdigen Quellen stammen, keine Websites besichtigen, die nicht vertrauenswürdig sind, und keine E-Mail-Anlagen öffnen. 

#### Aktivierung der Option für geschachtelte Auslöser in SQL Server ist für WSUS 3.0 SP1 erforderlich

Die Option für geschachtelte Auslöser ist standardmäßig aktiviert. Sie kann aber von einem SQL Server-Administrator deaktiviert werden.

Wenn Sie beabsichtigen, eine SQL Server-Datenbank als Windows Server Update Services-Datenspeicher zu verwenden, muss der SQL Server-Administrator sicherstellen, dass die Option für geschachtelte Auslöser auf dem Server aktiviert ist, bevor der WSUS 3.0 SP1-Administrator WSUS 3.0 SP1 installiert und im Verlauf der Installation die Datenbank angibt.

Die Option RECURSIVE\_TRIGGERS, bei der es sich um eine datenbankspezifische Option handelt, wird von WSUS 3.0 SP1-Setup aktiviert. Die Option für geschachtelte Auslöser, bei der es sich um eine globale Serveroption handelt, wird jedoch nicht aktiviert.

Verwenden Sie folgende Zeile, um anzuzeigen, ob die Option für geschachtelte Auslöser aktiviert ist:

**sp\_configure 'nested triggers'**

Führen Sie die folgenden Zeilen in einer Batchdatei auf dem Computer mit SQL Server aus, um die Option für geschachtelte Auslöser in SQL Server zu aktivieren:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

Wenn auf Ihrem Server SQL Server Management Studio nicht installiert ist, müssen Sie SQL-Skripts über die Befehlszeile ausführen. Sie können das Befehlszeilenabfrage-Dienstprogramm von Microsoft SQL Server 2005 im [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=70728) (http://go.microsoft.com/fwlink/?LinkId=70728) herunterladen. Führen Sie **sqlcmd** aus, um zu beginnen.

Wenn Sie SQL-Skripts in der Windows Internal Database ausführen möchten, müssen Sie auf derselben Downloadseite den SQL Server Native Client herunterladen.

#### Einschränkungen und Anforderungen für Remote-SQL

WSUS 3.0 SP1 unterstützt das Ausführen von Datenbanksoftware auf einem Computer, der von dem Computer mit der restlichen WSUS 3.0 SP1-Anwendung getrennt ist. Für das Konfigurieren einer Remote-SQL-Installation bestehen einige Anforderungen:

-   Sie können keinen Server als Back-End-Computer des Remote-SQL-Paars verwenden, der als Domänencontroller konfiguriert ist.
-   Auf dem Computer, der als Front-End-Server einer Remote-SQL-Installation fungieren soll, darf kein Terminalserver ausgeführt werden.
-   Auf dem Back-End-Computer muss mindestens Microsoft SQL Server 2005 Service Pack 1 (verfügbar im [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=66143) (http://go.microsoft.com/fwlink/?LinkId=66143) als Datenbanksoftware verwendet werden, wenn dieser Windows Server 2003 ausführt, bzw. SQL Server 2005 Service Pack 2, wenn der Back-End-Computer Windows Server® 2008 ausführt.
-   Sowohl der Front-End- als auch der Back-End-Computer muss einer Active Directory-Domäne beigetreten sein. Befinden sich beide Computer in unterschiedlichen Domänen, müssen Sie sonst domänenübergreifende Vertrauenswürdigkeit zwischen den Domänen einrichten, bevor WSUS-Setup ausgeführt wird.
-   Wenn WSUS 2.0 bereits in einer Remote-SQL-Konfiguration installiert ist und Sie auf WSUS 3.0 SP1 aktualisieren möchten, müssen Sie auf dem Back-End-Computer WSUS 2.0 (in der Systemsteuerung mithilfe von **Software**) deinstallieren und gleichzeitig sicherstellen, dass die vorhandene Datenbank intakt bleibt. Danach müssen Sie SQL Server 2005 SP1 oder SP2 installieren und die vorhandene Datenbank aktualisieren. Abschließend müssen Sie auf dem Front-End-Computer WSUS 3.0 SP1 installieren.

Systemanforderungen für die Installation der Remotekonsole von WSUS 3.0 SP1
---------------------------------------------------------------------------

Die WSUS 3.0 SP1-Remotekonsole kann auf folgenden Plattformen installiert werden:

-   Windows Server 2008
-   Windows Vista® oder höher
-   Windows Server 2003 SP1 oder höher
-   Windows XP SP2 oder höher

Systemanforderungen für die Clientinstallation
----------------------------------------------

Die Clientsoftware von WSUS ist „Automatische Updates“. Sie kann mit WSUS auf jedem der folgenden Betriebssysteme verwendet werden:

-   Windows Vista oder höher
-   Windows Server 2008 oder höher
-   Microsoft Windows Server 2003, alle Editionen
-   Microsoft Windows XP Professional SP2 oder höher
-   Microsoft Windows 2000 Professional SP4, Windows 2000 Server SP4 oder Windows 2000 Advanced Server mit SP4

Softwareanforderungen für die Installation des WSUS 3.0 SP1-Servers
-------------------------------------------------------------------

In der folgenden Tabelle wird die für Windows Server 2003 SP1-Plattformen erforderliche Software aufgeführt. Die für Windows Server 2008 erforderliche Software wird in dem Abschnitt behandelt, der sich mit WSUS 3.0 SP1 unter Windows Server 2008 beschäftigt.

Stellen Sie sicher, dass der WSUS 3.0 SP1-Server diese Liste mit Anforderungen erfüllt, bevor Sie WSUS 3.0 SP1-Setup ausführen. Wenn eins dieser Updates einen Neustart des Computers nach Abschluss der Installation erforderlich macht, muss dieser Neustart vor der Installation von WSUS 3.0 SP1 ausgeführt werden.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Anforderung</th>
<th style="border:1px solid black;" >Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internetinformationsdienste (IIS)</td>
<td style="border:1px solid black;">Aus dem Betriebssystem installieren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework, Version 2.0, Redistributable Package</td>
<td style="border:1px solid black;">Siehe Microsoft .NET Framework, Version 2.0, Redistributable Package (x86) im <a href="http://go.microsoft.com/fwlink/?linkid=68935">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=68935). Für 64-Bit-Plattformen siehe Microsoft .NET Framework, Version 2.0, Redistributable Package (x64) im <a href="http://go.microsoft.com/fwlink/?linkid=70637">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=70637).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0 für Windows Server 2003</td>
<td style="border:1px solid black;">Dies ist eine Voraussetzung für die Verwendung der Benutzeroberfläche von WSUS 3.0 SP1. Siehe Microsoft Management Console 3.0 für Windows Server 2003 (KB907265) im <a href="http://go.microsoft.com/fwlink/?linkid=70412">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=70412). Für 64-Bit-Plattformen siehe Microsoft Management Console 3.0 für Windows Server 2003 x64 Edition (KB907265) im <a href="http://go.microsoft.com/fwlink/?linkid=70638">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=70638).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dies ist eine Voraussetzung für die Verwendung der Benutzeroberfläche von WSUS 3.0 SP1. Siehe Microsoft Report Viewer Redistributable 2005 im <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SQL Server 2005 (optional)</td>
<td style="border:1px solid black;">WSUS 3.0 SP1 installiert Windows Internal Database, wenn nicht bereits eine kompatible Version von SQL Server installiert ist. Wenn Sie beabsichtigen, eine vollständige SQL Server-Datenbank zu verwenden, müssen Sie (mindestens) SQL Server 2005 SP1 verwenden (verfügbar im <a href="http://go.microsoft.com/fwlink/?linkid=66143">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=66143)) unter Windows Server 2003, oder SQL Server 2005 SP2 (verfügbar im <a href="http://go.microsoft.com/fwlink/?linkid=84823">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=84823)) unter Windows Server 2008 verwenden.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc708525.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                 |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Wenn bereits WSUS 2.0 installiert ist und SQL Server 2000, SQL Server Desktop Engine 2000 oder eine andere SQL Server-Datenbankversion verwendet wird, die niedriger als SQL Server 2005 SP1 (oder SQL Server 2005 SP2 unter Windows Server 2008) ist, installiert das WSUS 3.0 SP1-Installationsprogramm Windows® Internal Database und migriert die Datenbank dorthin. |
  
Mindestanforderungen an den Datenträgerspeicherplatz für die Installation des WSUS 3.0 SP1-Servers  
--------------------------------------------------------------------------------------------------
  
Im Folgenden finden Sie die Mindestanforderungen an den Datenträgerspeicherplatz für die Installation von Windows Server Update Services:
  
-   1 GB auf der Systempartition  
-   2 GB für das Volume, auf dem Datenbankdateien gespeichert werden sollen  
-   20 GB für das Volume, auf dem Inhalte gespeichert werden sollen
  
| ![](images/Cc708525.Important(WS.10).gif)Wichtig                                                                  |  
|------------------------------------------------------------------------------------------------------------------------------------------------|  
| WSUS 3.0 SP1 kann nicht auf komprimierten Laufwerken installiert werden. Stellen Sie sicher, dass das gewählte Laufwerk nicht komprimiert ist. |
  
Anforderungen für WSUS 3.0 SP1-Updates  
--------------------------------------
  
#### Sicherstellung der ordnungsgemäßen Ausführung der WSUS-Installation und Sichern der WSUS-Datenbank vor der Aktualisierung
  
Wenn Sie von einer früheren Version auf WSUS 3.0 SP1 aktualisieren, müssen Sie sicherstellen, dass die aktuelle Installation ordnungsgemäß ausgeführt wird, und die WSUS-Datenbank vor der Aktualisierung sichern.
  
1.  Überprüfen Sie die Ereignisprotokolle auf aktuelle Fehler, prüfen Sie auf Probleme bei der Synchronisierung zwischen Downstream- und Upstreamservern sowie auf Probleme mit Clients, die keine Meldungen liefern. Stellen Sie sicher, dass diese Probleme behoben wurden, bevor Sie den Vorgang fortsetzen.  
2.  Führen Sie DBCC CHECKDB aus, um sicherzustellen, dass die WSUS-Datenbank ordnungsgemäß indiziert ist. Weitere Informationen zu DBCC CHECKDB finden Sie unter [DBCC CHECKDB](http://go.microsoft.com/fwlink/?linkid=86948) (http://go.microsoft.com/fwlink/?LinkId=86948).  
3.  Sichern Sie die WSUS-Datenbank.
  
#### Deinstallation von WSUS vor der Aktualisierung, wenn der von WSUS verwendete Port manuell geändert wurde
  
Verwenden Sie zum Ändern des Ports für WSUS immer das Dienstprogramm **wsusutil**, statt den Port manuell zu ändern. Wenn der Port manuell geändert wurde und zuvor von Software Update Services 1.0 auf WSUS 2.0 aktualisiert wurde:
  
1.  Wenn WSUS 3.0 noch nicht installiert ist, deinstallieren Sie WSUS 2.0 unter Erhaltung der Datenbank mit ihren Inhalten. (Wenn WSUS 3.0 bereits installiert ist, deinstallieren Sie es unter Erhaltung der Datenbank mit ihren Inhalten.)  
2.  Starten Sie die Standardwebsite, aktivieren Sie vorübergehend wieder SUS 1.0, wodurch das Deinstallationsprogramm Zugriff darauf erhält.  
3.  Deinstallieren Sie SUS 1.0.  
4.  Installieren Sie WSUS 3.0.
  
#### Deinstallation von Software Update Services 1.0 erforderlich
  
Die Installation von WSUS 3.0 SP1 schlägt fehl, wenn Software Update Services 1.0 auf demselben Computer installiert ist. Sie müssen Software Update Services 1.0 vor der Installation von WSUS 3.0 SP1 deinstallieren.
  
#### Aktualisierung von WSUS 2.0 auf WSUS 3.0 SP1 auf einem 64-Bit-Betriebssystem nicht möglich
  
WSUS 2.0 wird auf 64-Bit-Betriebssystemen nicht unterstützt. Es ist nicht möglich, auf einem 64-Bit-Betriebssystem von WSUS 2.0 auf WSUS 3.0 SP1 zu aktualisieren.
  
Befehlszeilenparameter von Setup  
--------------------------------
  
Sie können unbeaufsichtigte Installationen von WSUS 3.0 SP1 mithilfe des Befehlszeilen-Installationsprogramms von WSUS ausführen. Diese Tabelle führt die Befehlszeilenparameter für WSUS 3.0 SP1-Setup auf.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parameter</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>/q</strong></td>
<td style="border:1px solid black;">Eine stille Installation ausführen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/u</strong></td>
<td style="border:1px solid black;">Das Produkt deinstallieren. Wenn eine Windows Internal Database-Instanz installiert ist, wird diese ebenfalls deinstalliert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/p</strong></td>
<td style="border:1px solid black;">Nur Voraussetzungen überprüfen. Das Produkt wird nicht installiert, aber das System wird untersucht, und alle nicht erfüllten Voraussetzungen werden gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>/?, /h</strong></td>
<td style="border:1px solid black;">Befehlszeilenparameter mit Beschreibung anzeigen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>/g</strong></td>
<td style="border:1px solid black;">Von der vorherigen Version von WSUS aktualisieren. (Versuchen Sie nicht, von SUS 1.0 zu aktualisieren.) Der einzige gültige Parameter für diese Option ist <strong>/q</strong> (stille Installation). Die einzige gültige Eigenschaft für diese Option ist DEFAULT_WEBSITE.</td>
</tr>
</tbody>
</table>
  
Diese Tabelle führt die Befehlszeileneigenschaften für WSUS 3.0 SP1 auf.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Eigenschaft</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CONTENT_LOCAL</td>
<td style="border:1px solid black;">0 = Inhalte lokal gehostet, 1 = Auf Microsoft Update gehostet</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CONTENT_DIR</td>
<td style="border:1px solid black;">Pfad zu Verzeichnis mit Inhalten. Standard ist <em>WSUSInstallationsLaufwerk</em><strong>\WSUS\WSUSContent</strong>, wobei <em>WSUSInstallationsLaufwerk</em> das lokale Laufwerk mit dem meisten freien Speicherplatz ist.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WYUKON_DATA_DIR</td>
<td style="border:1px solid black;">Pfad zum Datenverzeichnis der Windows Internal Database.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SQLINSTANCE_NAME</td>
<td style="border:1px solid black;">Der Name muss im Format <em>ServerName</em>\<em>SQLInstanzName</em> sein. Wenn sich die Datenbankinstanz auf dem lokalen Computer befindet, verwenden Sie die Umgebungsvariable <strong>%COMPUTERNAME%</strong>. Fehlt eine vorhandene Instanz, ist der Standardname <strong>%COMPUTERNAME%\WSUS</strong>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DEFAULT_WEBSITE</td>
<td style="border:1px solid black;">0 = Port 8530, 1 = Port 80</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PREREQ_CHECK_LOG</td>
<td style="border:1px solid black;">Pfad und Dateiname für die Protokolldatei</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CONSOLE_INSTALL</td>
<td style="border:1px solid black;">0 = WSUS-Server installieren, 1 = Nur Konsole installieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ENABLE_INVENTORY</td>
<td style="border:1px solid black;">0 = Inventurfeatures nicht installieren, 1 = Inventurfeatures installieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_DATABASE</td>
<td style="border:1px solid black;">0 = Datenbank erhalten, 1 = Datenbank entfernen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DELETE_CONTENT</td>
<td style="border:1px solid black;">0 = Inhaltsdateien erhalten, 1 = Inhaltsdateien entfernen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DELETE_LOGS</td>
<td style="border:1px solid black;">0 = Protokolldateien erhalten, 1 = Protokolldateien entfernen (Verwendung zusammen mit dem Installationsparameter /u).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CREATE_DATABASE</td>
<td style="border:1px solid black;">0 = Aktuelle Datenbank verwenden, 1 = Datenbank erstellen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PROGRESS_WINDOW_HANDLE</td>
<td style="border:1px solid black;">Fensterhandle zur Rückgabe von MSI-Statusmeldungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MU_ROLLUP</td>
<td style="border:1px solid black;">1 = Am Programm zur Verbesserung von Microsoft Update teilnehmen, 0 = Am Programm zur Verbesserung von Microsoft Update nicht teilnehmen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">FRONTEND_SETUP</td>
<td style="border:1px solid black;">1 = Den Inhaltsspeicherort nicht in die Datenbank schreiben, 0 = Den Inhaltsspeicherort in die Datenbank schreiben (für NLB)</td>
</tr>
</tbody>
</table>
  
#### Beispielsyntax
  
```  
WSUSSetup.exe /q DEFAULT\_WEBSITE=0 (install in quiet mode using port 8530) WSUSSetup.exe /q /u (uninstall WSUS)  
```  
| ![](images/Cc708525.Important(WS.10).gif)Wichtig                                                                                                                                                                                    |  
|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Wenn Sie WSUS 3.0 SP1 im stillen Modus (**/q**) installieren und auf dem Computer nicht alle vorausgesetzten Komponenten installiert sind, generiert die Installation eine Datei namens **WSUSPreReqCheck.xml**, die im Verzeichnis **%TEMP%** gespeichert wird. |
  
Installationsprobleme  
---------------------
  
#### Neustart von IIS während der Installation von WSUS 3.0 SP1
  
IIS wird von WSUS 3.0 SP1-Setup ohne Benachrichtigung neu gestartet. Dies kann Websites innerhalb Ihrer Organisation beeinträchtigen. Wenn IIS nicht ausgeführt wird, wird es von WSUS 3.0 SP1-Setup gestartet.
  
#### Fehler bei der Installation bei bestehenden Verbindungen mit einer vorhandenen WSUS-Datenbank
  
Wenn Sie bei bestehenden Verbindungen mit einer vorhandenen WSUS-Datenbank (z. B. bei geöffnetem SQL Server Management Studio) von einer bestehenden Installation auf WSUS 3.0 SP1 aktualisieren, schlägt die Installation möglicherweise fehl. Schließen Sie alle Verbindungen und installieren Sie WSUS 3.0 SP1 erneut.
  
#### Anzeige des falschen Verzeichnisses für Datenbankdateien durch WSUS-Setup
  
In WSUS-Setup wird im Bildschirm **Windows Server Update Services 3.0 SP1 kann jetzt installiert werden** fälschlicherweise das übergeordnete Verzeichnis des Datenbankspeicherorts als Datenbankspeicherort angegeben. Wenn der Standardspeicherort beispielsweise **%systemdrive%\\WSUS\\UpdateServicesDbFiles** ist, wird dieser Speicherort stattdessen fehlerhaft als **%systemdrive%\\WSUS** angezeigt.
  
#### Wenn WSUS auf einem Computer installiert ist, der über Sprachpakete für mehrsprachige Benutzeroberflächen verfügt und eine andere Standardsprache als Englisch hat, wird die Hilfe in der Standardsprache statt in Englisch angezeigt.
  
Auch wenn ein Computer vorhanden ist, der über Sprachpakete für mehrsprachige Benutzeroberflächen verfügt und eine andere Standardsprache als Englisch hat, können Sie weiterhin WSUS installieren, wenn das Gebietsschema des aktuellen Benutzers „Englisch“ ist. Die Benutzeroberfläche wird in Englisch angezeigt, doch um die Hilfe in Englisch anzuzeigen, müssen Sie eine Problemumgehung anwenden. Kopieren Sie die englischsprachigen CHM-Datei der Hilfe (*WSUSInstallVerz***\\documentation\\mui\\0409\\WSUS30Help.chm**) in das Hauptdokumentationsverzeichnis (*WSUSInstallVerz***\\documentation\\WSUS30Help.chm**). Jetzt sollte die Hilfe ordnungsgemäß in allen Sprachen angezeigt werden.
  
Updateprobleme  
--------------
  
#### Wiederherstellung von einer fehlerhaften Aktualisierung
  
Gehen Sie wie folgt vor, wenn es beim Aktualisieren von einer vorherigen Version von WSUS (WSUS 3.0, WSUS 2.0 SP1 oder WSUS 2.0) auf WSUS 3.0 SP1 zu Fehlern kommt:
  
1.  Installieren Sie die vorherige Version von WSUS erneut.  
2.  Stellen Sie die Datenbank aus der Sicherungskopie wieder her, die vor der Aktualisierung angefertigt wurde. (In den meisten Fällen erstellt WSUS ebenfalls automatisch eine Sicherungskopie. Deren Speicherort finden Sie in der Datei **WSUSSetup.log**.)  
3.  Überprüfen Sie die Protokolle auf die Ursache des Fehlers, und beheben Sie das Problem.  
4.  Versuchen Sie erneut, WSUS zu aktualisieren.
  
#### Aktualisierung von WSUS 2.0 auf WSUS 3.0 SP1 bei Vorhandensein einer WSUS 3.0 SP1-Datenbank aus einer vorherigen Installation nicht möglich
  
Wenn WSUS 3.0 SP1 bereits zuvor installiert war und WSUS 2.0 erneut installiert wird, muss die WSUS 3.0 SP1-Datenbank auf dem Computer gelöscht werden, bevor die erneute Installation von WSUS 3.0 SP1 ausgeführt wird.
  
#### Fehler der Aktualisierung auf WSUS 3.0 SP1 durch Änderung des Computernamens vor dem Aktualisierungsvorgang
  
Wenn im Anschluss an die Installation von WSUS 2.0 der Name des Computers geändert wird, bevor auf WSUS 3.0 SP1 aktualisiert wird, schlägt die Aktualisierung fehl.
  
Verwenden Sie folgendes Skript, um die Administratorengruppen ASPNET und WSUS zu entfernen und erneut hinzuzufügen. Führen Sie anschließen die Aktualisierung erneut aus.
  
*&lt;DBLocation&gt;* muss dabei durch den Ordner ersetzt werden, in dem die Datenbank installiert ist, und *&lt;ContentDirectory&gt;* durch den lokalen Speicherordner.
  
```  
sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=name from sysusers WHERE name like '%ASPNET' EXEC sp\_revokedbaccess @asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=name from sysusers WHERE name like '%WSUS Administrators' EXEC sp\_revokedbaccess @wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @asplogin varchar(200) SELECT @asplogin=HOST\_NAME()+'\\ASPNET' EXEC sp\_grantlogin @asplogin EXEC sp\_grantdbaccess @asplogin EXEC sp\_addrolemember webService,@asplogin" sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "USE SUSDB DECLARE @wsusadminslogin varchar(200) SELECT @wsusadminslogin=HOST\_NAME()+'\\WSUS Administrators' EXEC sp\_grantlogin @wsusadminslogin EXEC sp\_grantdbaccess @wsusadminslogin EXEC sp\_addrolemember webService,@wsusadminslogin"   sqlcmd.exe -S *&lt;DBLocation&gt;* -E -Q "backup database SUSDB to disk=N'*&lt;ContentDirectory&gt;*\\SUSDB.Dat' with init"  
```
  
#### Überschreiben einer vorherigen Datenbanksicherungskopie durch Setup
  
WSUS 3.0 SP1-Setup fügt die Datenbank dem Standardverzeichnis hinzu, bei dem es sich um *Laufwerk***\\WSUS** handelt (wobei *Laufwerk* das lokale NTFS-Laufwerk ist, auf dem die größte Menge freier Speicherplatz vorhanden ist). Wenn sich in diesem Verzeichnis eine Sicherungskopie der Datenbank befindet, wird diese möglicherweise überschrieben. Administratoren müssen eine Sicherungskopie der Datenbank in der aktuellen Version an einem anderen Speicherort speichern, bevor auf WSUS 3.0 SP1 aktualisiert wird.
  
#### Änderung eines Registrierungswerts erforderlich nach Migration von MSDE nach SQL Server 2000 oder SQL Server 2005 auf WSUS 2.0
  
Wenn Sie bei vorhandener Installation von WSUS 2.0 eine Migration nach SQL Server 2000 oder SQL Server 2005 ausgeführt haben, müssen Sie den Wert des Schlüssels **HKLM\\SOFTWARE\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled** von **1** in **0** ändern. Wird dies vor der Aktualisierung auf WSUS 3.0 SP1 versäumt, schlägt die Aktualisierung fehl.
  
#### Bei Starten und Abbrechen von WSUS 2.0-Setup wird der WSUS-Registrierungsschlüssel gelöscht
  
Wenn WSUS 2.0-Setup zuerst gestartet und dann abgebrochen wird, wird der WSUS-Registrierungsschlüssel gelöscht. Hierdurch kann es zu Problemen kommen, wenn WSUS 3.0 SP1 bereits installiert ist. Dasselbe Problem tritt auf, wenn Sie zuerst die Deinstallation von WSUS 2.0 starten, den Vorgang dann abbrechen und schließlich versuchen, von WSUS 2.0 auf WSUS 3.0 SP1 zu aktualisieren.
  
#### Protokolldateien verfügen nicht über die richtigen Berechtigungen nach erneuter Installation, wenn WSUS 3.0 SP1 installiert und die Protokolldateien erhalten wurden
  
Wenn WSUS 3.0 SP1 deinstalliert wird, haben Sie die Möglichkeit, die Protokolldateien der Installation zu behalten. Bei der erneuten Installation von WSUS 3.0 SP1 verlieren die alten Protokolldateien ihre Berechtigungen (üblicherweise nur für WSUS-Administratoren). Die Berechtigungen dieser Protokolldateien müssen wiederhergestellt werden.
  
#### Bei WSUS 2.0-Clients mit Updates mit dem Status "Nicht zutreffend" werden die Updates im Anschluss an die Aktualisierung auf WSUS 3.0 SP1 für kurze Zeit mit "Kein Status" angezeigt
  
Wenn ein WSUS 2.0-Server über Clients mit Updates mit dem Status **Nicht zutreffend** verfügt, werden diese Updates im Anschluss an die Aktualisierung des Servers auf WSUS 3.0 SP1 für kurze Zeit mit dem Status **Kein Status** angezeigt Der Updatestatus wechselt zurück zu **Nicht zutreffend**, sobald der Client die nächste Überprüfung begonnen hat.
  
Bekannte Probleme  
-----------------
  
#### Problembehandlung von Downloadfehlern oder wiederholten Clientsynchronisierungsfehlern
  
Wenn WSUS 3.0 SP1-Clients mehrfache Downloadfehler melden bzw. wenn bei Clients über einen längeren Zeitraum Fehler bei der Synchronisierung mit dem WSUS 3.0 SP1-Server auftreten, liegt möglicherweise ein fehlerhafter Downloadcache vor. Um diesen Zustand zu beheben, können Sie versuchen, den Clientdownloadcache im Dateisystem zu löschen.
  
So löschen Sie den Clientdownloadcache
  
1.  Löschen Sie alle Dateien und Unterverzeichnisse an folgendem Speicherort auf dem Clientcomputer: **%windir%\\SoftwareDistribution\\Download**  
2.  Versuchen Sie erneut, das Update zu installieren, indem Sie den Clientcomputer erneut mit WSUS 3.0 SP1 synchronisieren. Dieser Installationsversuch sollte folgenden Fehler zurückgeben: **WU\_E\_DM\_NOTDOWNLOADED, "The update has not been downloaded."** (Das Update wurde nicht heruntergeladen.)  
3.  Im Anschluss an diesen Fehler startet der Clientcomputer den Download automatisch erneut und die Installation kann fortgesetzt werden.
  
#### Bei einem Fehler der Synchronisierung diese erneut versuchen
  
Bei einem Synchronisierungsfehler müssen Sie als erste Problembehandlungsmaßnahme versuchen, den Server erneut zu synchronisieren. Kommt es bei folgenden Synchronisierungen ebenfalls zu Fehlern, wenden Sie die im [Windows Server Update Services 3.0 Operations Guide](http://go.microsoft.com/fwlink/?linkid=81072) (http://go.microsoft.com/fwlink/?LinkId=81072) aufgeführten Problembehandlungsinformationen an.
  
#### Die Änderung der WSUS 3.0 SP1-Konfiguration direkt in der Datenbank wird nicht unterstützt
  
Windows Server Update Services speichert seine Konfigurationsdaten in einer SQL Server-Datenbank. Das Ändern der Konfigurationsdaten durch direkten Zugriff auf die Datenbank wird aber nicht unterstützt. Versuchen Sie nicht, die WSUS 3.0 SP1-Konfiguration zu ändern, indem Sie direkt auf die Datenbank zugreifen. Ändern Sie die WSUS 3.0 SP1-Konfiguration unter Verwendung der WSUS 3.0 SP1-Konsole oder durch Aufrufen von WSUS 3.0 SP1-APIs.
  
#### Downloadfehler werden bei aktivierten Datenträgerkontingenten nicht schnell gemeldet
  
Wenn Datenträgerkontingente aktiviert sind und erreicht werden, werden Fehler bei Updatedownloads auf dem WSUS-Server möglicherweise nicht rechtzeitig gemeldet. Zur Vermeidung dieses Problems deaktivieren Sie die Datenträgerkontingente oder erhöhen deren Werte.
  
#### Bei Bereitstellung von WSUS 3.0 SP1 mithilfe von SSL kommt es bei Clientcomputern zu einem Fehler mit dem Fehlercode "0x8024400a"
  
Manchmal kommt es bei Clientcomputern während der Kommunikation mit dem WSUS 3.0 SP1-Server über SSL zu einem Fehler mit dem Fehlercode "0x8024400a". Ein Update, das dieses Problem behandelt, finden Sie im Artikel [KB 905422](http://go.microsoft.com/fwlink/?linkid=70593) (http://go.microsoft.com/fwlink/?LinkId=70593).
  
#### Bei Deinstallation von WSUS wird das Domänenkonto "WSUS-Administratoren" nicht gelöscht
  
Die Gruppe **WSUS-Administratoren** wird auf Domänencontrollern als Domänenkonto (nicht als lokales Konto) erstellt, sodass alle Installationen, die dieses Domänenkonto verwenden, deaktiviert werden, wenn das Konto im Rahmen der Deinstallation von WSUS gelöscht wird. Aus diesem Grund wird das Domänenkonto **WSUS-Administratoren** bei einer Deinstallation von WSUS nicht gelöscht.
  
#### Bei Konvertierung eines Downstreamservers in einen Upstreamserver müssen Katalogsiteupdates erneut importiert werden
  
Wenn ein Downstreamserver zu einem Upstreamserver heraufgestuft wird, müssen Sie ebenfalls alle Katalogsiteupdates neu importieren. Andernfalls schlägt die Synchronisierung neuer Katalogsiteupdate-Versionen mit diesem Server über die Site fehl.
  
#### Bei Verwendung von IIS mit SSL ist immer noch unverschlüsselter Zugriff möglich, es sei denn "Sicherer Kanal (SSL) erforderlich" ist aktiviert
  
Wenn Sie IIS für die Verwendung von SSL durch Installation eines Zertifikats einrichten, kann immer noch so lange über unverschlüsseltes HTTP auf die Site zugegriffen werden, bis die Option **Sicherer Kanal (SSL) erforderlich** aktiviert wird. Weitere Informationen finden Sie in der Dokumentation für [IIS](http://go.microsoft.com/fwlink/?linkid=98084) (http://go.microsoft.com/fwlink/?LinkId=98084).
  
#### Katalogsiteimport-Fehler ohne Lese-/Schreibberechtigungen für den Ordner "%windir%\\TEMP folder"
  
Wenn das Konto **Netzwerkdienst** beim Import einer Katalogsite nicht über Lese-/Schreibberechtigungen für den Ordner **%windir%\\TEMP** verfügt, kommt es beim Import zu einem Fehler mit einer der folgenden Meldung ähnlichen Fehlermeldung: Server was unable to process request. ---&gt; Could not find file "C:\\WINDOWS\\TEMP\\*tempDateiName*.dll".
  
#### Verringerte Leistung beim Synchronisieren zwischen WSUS 3.0 SP1 und einem Downstream-Replikatserver, der WSUS 2.0 ausführt
  
Wenn WSUS 3.0 SP1 auf einem Upstreamserver installiert wird und Sie versuchen, eine Synchronisierung mit einem Downstream-Replikatserver auszuführen, der WSUS 2.0 ausführt, kann es zu Leistungsproblemen kommen. Informationen zur Behandlung dieses Problems finden Sie im Artikel [KB 910847](http://go.microsoft.com/fwlink/?linkid=70669) (http://go.microsoft.com/fwlink/?LinkId=70669).
  
#### Fehler der E-Mail-Benachrichtigung ohne Meldung bei heruntergefahrenem oder nicht verfügbarem E-Mail-Server
  
Wenn der E-Mail-Server des Netzwerks offline ist, kommt es zu einem nicht gemeldeten Fehler von WSUS 3.0 SP1 beim Senden von E-Mail-Benachrichtigungen. In das Ereignisprotokoll wird aber das Ereignis 10052 (**HealthCoreEmailNotificationRed**) geschrieben.
  
#### Geänderte Einstellungen auf einem Upstreamserver werden nicht sofort an den Downstreamserver weitergegeben
  
Wenn die Upstreamserver-Konfiguration geändert wird, kann es einige Zeit dauern, bis diese Konfigurationsänderungen tatsächlich übernommen werden. Wird beispielsweise eine Einstellung auf dem Upstreamserver geändert, z. B. Auswahl einer neuen Sprache, und sofort eine Synchronisierung auf dem Downstreamserver ausgelöst, wird die Änderung nicht angezeigt. Stattdessen wird sie bei der nächsten geplanten Synchronisierung an den Downstreamserver weitergeleitet. Die Wartezeit erhöht sich in Abhängigkeit von der Anzahl der auf dem Upstreamserver vorhandenen Updates.
  
#### Bei Deinstallation von WSUS 3.0 SP1 wird die Datenbankinstanz nicht deinstalliert
  
Wenn WSUS 3.0 SP1 deinstalliert wird, wird die Datenbankinstanz nicht deinstalliert. Da die Instanz möglicherweise von mehr als einer Anwendung verwendet wird, würde deren Entfernung zu Fehlern bei anderen Anwendungen führen.
  
Wenn es erforderlich ist, Windows Internal Database zu deinstallieren, ist dies mit folgenden Befehlen möglich:
  
(auf 32-Bit-Plattformen)
  
```  
msiexec /x {CEB5780F-1A70-44A9-850F-DE6C4F6AA8FB} callerid=ocsetup.exe  
```  
(auf 64-Bit-Plattformen)
  
```  
msiexec /x {BDD79957-5801-4A2D-B09E-852E7FA64D01} callerid=ocsetup.exe  
```  
Wenn Windows Internal Database Service Pack 2 unter Windows Server 2008 deinstalliert werden soll, können Sie dies mithilfe des Server-Managers ausführen.
  
Durch das Entfernen der Anwendung werden aber nicht notwendigerweise die MDF- und LDF-Standarddateien entfernt, wodurch es zu einem Fehler einer darauf folgenden WSUS 3.0 SP1-Installation kommt. Diese Dateien können im Verzeichnis **%windir%\\SYSMSI\\SSEE** gelöscht werden.
  
#### Bei Änderung des Upstreamservers durch seinen Downstreamserver werden Updates mit dem Status "Kein Status" als "Nicht zutreffend" gemeldet
  
Wenn ein Downstreamserver eine Synchronisierung von einem anderen Upstreamserver beginnt, werden Updates mit einem Status von **Kein Status** auf dem neuen Upstreamserver als **Nicht zutreffend** gemeldet. Dieser Zustand ist vorübergehend und wird bei der nächsten Statusmeldung durch den Downstreamserver berichtigt, nachdem dessen Clients sich mit ihm synchronisiert haben.
  
#### Unterbrechung der Verbindung mit allen Servern bei einem Timeout des Assistenten für die Serverbereinigung auf einem Server, wenn dieser von einer Remotekonsole aus auf mehreren Servern ausgeführt wird
  
Der Assistent für die Serverbereinigung kann über eine einzelne Remotekonsole auf mehreren Servern ausgeführt werden. Kommt es aber bei dem Bereinigungsprozess zu einem Timeout auf einem der Server, wird die Verbindung zwischen der Konsole und allen Servern unterbrochen. Zwar gehen keine Daten verloren, aber der Administrator muss die Remoteverbindung auf jedem der Server zurücksetzen.
  
#### Fehlermeldung "Kein Synchronisierungsfehler" im Assistenten für die WSUS-Serverkonfiguration durch Starten und Beenden der Verbindung in schneller Abfolge
  
Bei der Konfiguration von WSUS muss eine Verbindung mit dem Upstreamserver (entweder Microsoft Update oder der Intranet-Upstreamserver) hergestellt werden, um grundlegende Serverinformationen zu übertragen. Wenn Sie auf **Verbindung starten** klicken und dann sofort auf **Verbinden beenden**, wird die fehlerhafte Fehlermeldung **Kein Synchronisierungsfehler** angezeigt.
  
WSUS 3.0 SP1 unter Windows Server 2008  
--------------------------------------
  
#### Unterstützte Versionen
  
WSUS 3.0 SP1 unterstützt die 32-Bit- und 64-Bit-Versionen von Windows Server 2008.
  
#### Voraussetzungen
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Anforderung</th>
<th style="border:1px solid black;" >Details</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Internetinformationsdienste (IIS)</td>
<td style="border:1px solid black;">Aus dem Betriebssystem installieren. Stellen Sie sicher, dass folgende Komponenten aktiviert sind:
<ul>
<li>Windows-Authentifizierung<br />
<br />
</li>
<li>Statischer Inhalt<br />
<br />
</li>
<li>ASP.NET<br />
<br />
</li>
<li>6.0-Verwaltungskompatibilität<br />
<br />
</li>
<li>6.0 IIS Metabase-Kompatibilität<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft .NET Framework, Version 2.0, Redistributable Package (x86)</td>
<td style="border:1px solid black;">Nicht erforderlich unter Windows Server 2008, da bereits als Bestandteil des Betriebssystems installiert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Management Console 3.0</td>
<td style="border:1px solid black;">Nicht erforderlich unter Windows Server 2008, da bereits als Bestandteil des Betriebssystems installiert.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Report Viewer</td>
<td style="border:1px solid black;">Dies ist eine Voraussetzung für die Verwendung der Benutzeroberfläche von WSUS. Siehe Microsoft Report Viewer Redistributable 2005 im <a href="http://go.microsoft.com/fwlink/?linkid=70410">Microsoft Download Center</a> (http://go.microsoft.com/fwlink/?LinkId=70410).</td>
</tr>
</tbody>
</table>
  
#### Verwenden des Sicherheitskonfigurations-Assistenten
  
Bei Ausführung des Sicherheitskonfigurations-Assistenten (Security Configuration Wizard, SCW) in Windows Server 2008 können Sie die Rolle **WSUS** auswählen und deren Abhängigkeiten aktivieren. Zeigen Sie zum Ausführen des SCW im Menü **Start** auf **Verwaltung**, und klicken Sie dann auf **Sicherheitskonfigurations-Assistent**.
  
Folgende bekannte Probleme bestehen bei der Verwendung des SCW in Verbindung mit der Rolle **WSUS**:
  
-   **Der Windows Internal Database-Dienst ist aktiviert, obwohl er nicht von WSUS verwendet wird.** Konfigurieren Sie WSUS für die Verwendung einer Datenbank, entweder Windows Internal Database oder eine SQL Server-Datenbank. Wenn WSUS mit SQL Server installiert ist und Sie im SCW die Rolle **WSUS** wählen, wird der Windows Internal Database-Dienst aktiviert, wenn er auf dem Computer installiert ist, aber von WSUS nicht verwendet. Deaktivieren Sie den Windows Internal Database-Dienst, wenn Sie anstelle von Windows Internal Database eine SQL Server-Datenbank verwenden.  
-   **Firewallregeln für WSUS auf einer benutzerdefinierten Website werden nicht standardmäßig ausgewählt.** Wenn Sie WSUS auf einer benutzerdefinierten Website (Port 8530 oder 8531) installieren, werden die erforderlichen Firewallregeln auch dann nicht automatisch ausgewählt, wenn im SCW die Rolle **WSUS** gewählt wurde. Aktivieren Sie die geeigneten Firewallregeln für WSUS in Abhängigkeit davon, ob SSL (Secure Sockets Layer) für den WSUS-Server konfiguriert ist.
  
WSUS 3.0 SP1 unter Windows Small Business Server 2003  
-----------------------------------------------------
  
#### Bei Einschränkung des virtuellen IIS-Stamms auf bestimmte IP-Adressen oder Domänennamen kann sich der WSUS 3.0 SP1-Server nicht selbst aktualisieren
  
Bei einigen Installationen von Windows Small Business Server ist die IIS-Standardwebsite eventuell für **Einschränkungen für IP-Adressen und Domänennamen** konfiguriert. Sollte dies der Fall sein, ist der Windows Update-Client auf dem Server möglicherweise nicht in der Lage, sich selbst zu aktualisieren.
  
#### Integrationsprobleme beim Installieren von WSUS 3.0 SP1 unter Small Business Server
  
-   Wenn Windows Small Business Server 2003 einen ISA-Proxyserver für den Zugriff auf das Internet verwendet, muss Folgendes in der Benutzeroberfläche für **Einstellungen** eingegeben werden: **Proxyservereinstellungen, Proxyservername, Port**.  
-   Wenn ISA Windows-Authentifizierung verwendet, müssen Proxyserver-Anmeldeinformationen im Format *DOMÄNE*\\*Benutzer* eingegeben werden, und der Benutzer muss Mitglied der Gruppe **Internetbenutzer** sein.
  
#### Folgendes Verfahren muss ausgeführt werden, wenn dem Netzwerk ohne Verwendung des Windows SBS-Assistenten ein Subnetz hinzugefügt wurde
  
Der Installationsprozess des WSUS-Servers installiert zwei virtuelle IIS-Stämme auf dem Server: **SelfUpdate** und **ClientWebService**. Dabei werden außerdem einige Dateien unterhalb des Basisverzeichnisses der Standardwebsite (an Port 80) abgelegt, wodurch Clientcomputer sich über die Standardwebsite selbst aktualisieren können. Standardmäßig ist die Standardwebsite so konfiguriert, dass sie allen IP-Adressen mit Ausnahme des Localhost den Zugriff auf bestimmte, dem Server zugeordnete Subnetze verweigert. Demzufolge können sich Clientcomputer, die sich nicht auf dem Localhost oder in einem dieser spezifischen Subnetze befinden, nicht selbst aktualisieren. Wenn Sie Ihrem Netzwerk ein Subnetz ohne Verwendung des Microsoft Windows Small Business Server 2003-Assistenten (Windows SBS) hinzugefügt haben, müssen Sie folgendes Verfahren ausführen:
  
1.  Erweitern Sie in der **Serververwaltung** die Einträge **Erweiterte Verwaltung**, **Internetinformationsdienste**, **Websites** und **Standardwebsite**, klicken Sie mit der rechten Maustaste auf das virtuelle Verzeichnis **Selfupdate**, und klicken Sie dann auf **Eigenschaften**.  
2.  Klicken Sie auf **Verzeichnissicherheit**.  
3.  Klicken Sie unter **Einschränkungen für IP-Adressen und Domänennamen** auf **Bearbeiten** und dann auf **Zugriff gewährt**.  
4.  Klicken Sie auf **OK**, klicken Sie mit der rechten Maustaste auf das virtuelle Verzeichnis **ClientWebService**, und klicken Sie anschließend auf **Eigenschaften**.  
5.  Klicken Sie auf **Verzeichnissicherheit**.  
6.  Klicken Sie unter **Einschränkungen für IP-Adressen und Domänennamen** auf **Bearbeiten** und dann auf **Zugriff gewährt**.
  
Copyright  
---------
  
Die in diesem Dokument enthaltenen Informationen, einschließlich URL- und anderen Internetwebsite-Verweisen, können ohne vorherige Ankündigung geändert werden. Die in den Beispielen verwendeten Firmen, Organisationen, Produkte, Domänennamen, E-Mail-Adressen, Logos, Personen, Orte und Ereignisse sind frei erfunden, soweit nichts anderes angegeben ist. Jede Ähnlichkeit mit tatsächlichen Firmen, Organisationen, Produkten, Domänennamen, E-Mail-Adressen, Logos, Personen, Orten und Ereignissen ist rein zufällig. Die Benutzer sind verantwortlich für das Einhalten aller anwendbaren Urheberrechtsgesetze. Unabhängig von der Anwendbarkeit der entsprechenden Urheberrechtsgesetze darf ohne ausdrückliche schriftliche Erlaubnis der Microsoft Corporation kein Teil dieses Dokuments für irgendwelche Zwecke vervielfältigt oder in einem Datenempfangssystem gespeichert oder darin eingelesen werden, unabhängig davon, auf welche Art und Weise oder mit welchen Mitteln (elektronisch, mechanisch, durch Fotokopieren, Aufzeichnen usw.) dies geschieht.
  
Microsoft kann Inhaber von Patenten, Patentanträgen, Marken, Urheberrechten oder anderem geistigen Eigentum sein, die den Inhalt dieses Dokuments betreffen. Die Bereitstellung dieses Dokuments gewährt keinerlei Lizenzrechte an diesen Patenten, Marken, Urheberrechten oder anderem geistigen Eigentum, es sei denn, dies wurde ausdrücklich durch einen schriftlichen Lizenzvertrag mit Microsoft vereinbart.
  
© 2007 Microsoft Corporation. Alle Rechte vorbehalten.
  
Microsoft, SQL Server, Windows und Windows Server sind entweder eingetragene Marken oder Marken der Microsoft Corporation in den USA und/oder anderen Ländern.
  
Alle anderen Marken sind Marken der jeweiligen Eigentümer.
