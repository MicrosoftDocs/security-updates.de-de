---
TOCTitle: Infodatei für Windows Server Update Services
Title: Infodatei für Windows Server Update Services
ms:assetid: '4244109a-395a-4ff8-9989-ea55ab0964a3'
ms:contentKeyID: 18127435
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720505(v=WS.10)'
---

Infodatei für Windows Server Update Services
============================================

In diesem Dokument werden bekannte Probleme im Zusammenhang mit den Windows Server Update Services (WSUS) beschrieben. Sie finden hier Empfehlungen sowie die Systemanforderungen für die Installation von WSUS.

| ![](images/Cc720505.note(WS.10).gif)Hinweis                                                                                                        |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Dieses Dokument steht im Microsoft Download Center unter [http://go.microsoft.com/fwlink/?LinkId=48126](http://go.microsoft.com/fwlink/?linkid=48126) zum Herunterladen bereit. |

Vor Beginn
----------

#### Problem 1: IIS muss installiert sein

Damit Microsoft® Windows Server™ Update Services (WSUS) ordnungsgemäß funktioniert, müssen die Internetinformationsdienste (Internet Information Services, IIS) installiert sein. Bei Microsoft Windows Server 2003 und Microsoft Windows® 2000 Server wird IIS jedoch nicht standardmäßig installiert, sodass es vorkommen kann, dass das Setupprogramm für Windows Server Update Services anhält und meldet, dass IIS nicht installiert ist.

So installieren Sie IIS:

1.  Öffnen Sie die Systemsteuerung.
2.  Klicken Sie auf **Software**.
3.  Klicken Sie auf **Windows-Komponenten hinzufügen/entfernen**.
4.  Klicken Sie in der Liste **Komponenten** auf **Anwendungsserver**.
5.  Klicken Sie auf **Details**.
6.  Aktivieren Sie das Kontrollkästchen **ASP.NET**. Aktivieren Sie die Option **COM+-Netzwerkzugriff aktivieren**. Die Internetinformationsdienste (IIS) werden automatisch ausgewählt.
7.  Wählen Sie **Internet Information Services (IIS)** aus, und klicken Sie auf **Details**. Die Liste der optionalen IIS-Komponenten wird angezeigt.
8.  Wählen Sie alle optionalen Komponenten aus, die installiert werden sollen. Die optionale Komponente „WWW-Dienste“ enthält wichtige Unterkomponenten, beispielsweise Active Server Pages oder die Remoteverwaltung (HTML). Um diese Unterkomponenten abzurufen und auszuwählen, klicken Sie auf „WWW-Dienste“ und dann auf „Details“. Klicken Sie wiederholt auf „OK“, bis Sie wieder zum Assistenten für Windows-Komponenten gelangen.
9.  Klicken Sie auf **Weiter**, und führen Sie die weiteren Schritte im Rahmen des Assistenten für Windows-Komponenten durch.
10. Führen Sie nach der Installation von IIS das Installationsprogramm von Windows Server Update Services aus.

#### Problem 2: Bei Servern mit Windows 2000 Server muss mindestens eine Website in IIS vorhanden sein, bevor WSUS installiert werden kann

Das Setupprogramm für Windows Server Update Services kann unter Umständen keine Websites erstellen, wenn beim Ausführen des Setupprogramms in IIS keine Websites vorhanden waren. Dies kann beispielsweise der Fall sein, wenn in IIS nur eine SUS 1.0-Website (Software Update Services) vorhanden war und diese gelöscht wurde, bevor Sie mit der Installation von WSUS begonnen haben.

Erstellen Sie in diesem Fall mit dem IIS-Manager-Snap-In eine neue Website. Anschließend können Sie diese Website auswählen oder während der WSUS-Installation eine neue Website angeben.

Falls Sie bereits versucht haben, WSUS zu installieren, und die Installation fehlgeschlagen ist, weil keine Websites vorhanden waren, öffnen Sie das IIS-Manager-Snap-In, und löschen Sie die Website „Website Nr. 1“. Führen Sie anschließend die oben genannten Schritte aus, und starten Sie Setup erneut.

#### Problem 3: Installieren erforderlicher Komponenten

#### Softwareanforderungen

In der nachstehenden Tabelle wird die erforderliche Software für die verschiedenen unterstützten Betriebssysteme aufgeführt. Überprüfen Sie, ob der WSUS-Server diese Anforderungen erfüllt, bevor Sie das WSUS-Setupprogramm starten. Falls der Computer nach der Installation eines der Updates neu gestartet werden muss, führen Sie diesen Neustart durch, bevor Sie WSUS installieren.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Betriebssystem</th>
<th style="border:1px solid black;" >Anforderungen</th>
<th style="border:1px solid black;" >Downloads</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alle Betriebssysteme</td>
<td style="border:1px solid black;">Microsoft IIS 5.0 (Internet Information Services, Internetinformationsdienste)</td>
<td style="border:1px solid black;">Installation vom Betriebssystem.
Siehe Problem 1: IIS muss installiert sein.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alle Betriebssysteme</td>
<td style="border:1px solid black;">BITS 2.0 (Background Intelligent Transfer Service, Intelligenter Hintergrundübertragungsdienst)</td>
<td style="border:1px solid black;">Informationen zu Windows Server 2003-Betriebssystemen finden Sie unter <a href="http://go.microsoft.com/fwlink/?linkid=47251">Update für den Intelligenten Hintergrundübertragungsdienst (BITS) 2.0 und WinHTTP 5.1 unter Windows Server 2003</a> (KB842773) im Download Center (http://go.microsoft.com/fwlink/?LinkId=47251).
Informationen zu Windows Server 2000-Betriebssystemen finden Sie unter <a href="http://go.microsoft.com/fwlink/?linkid=46794">Update für den Intelligenten Hintergrundübertragungsdienst (BITS) 2.0 und WinHTTP 5.1 unter Windows 2000</a> (KB842773) im Download Center (http://go.microsoft.com/fwlink/?LinkId=46794).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003</a>
Stattdessen können Sie auch zur <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update-Website</a> gehen und nach wichtigen Updates und Service Packs suchen. Installieren Sie Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003</td>
<td style="border:1px solid black;">Datenbanksoftware, die vollständig mit Microsoft SQL kompatibel ist</td>
<td style="border:1px solid black;">Nicht zutreffend</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Datenbanksoftware, die vollständig mit Microsoft SQL kompatibel ist</td>
<td style="border:1px solid black;">Falls Sie nicht Microsoft SQL Server 2000 verwenden, können Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) installieren. Hierzu sind mehrere Schritte notwendig. Weitere Informationen finden Sie weiter unten unter „Installieren von MSDE unter Windows 2000“.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft Internet Explorer 6.0 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Redistributable Package</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework 1.1 Redistributable Package</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows 2000 Server</td>
<td style="border:1px solid black;">Microsoft .NET Framework 1.1 Service Pack 1</td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a>
Stattdessen können Sie auch zur <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update-Website</a> gehen und nach wichtigen Updates und Service Packs suchen. Installieren Sie Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2000.</td>
</tr>
</tbody>
</table>
 

Zusätzlich zu diesen Anforderungen installiert oder konfiguriert WSUS möglicherweise auch ASP.NET 1.1 auf dem Server. (Das WSUS-Installationsprogramm konfiguriert ASP.NET.)

#### Installieren von MSDE 2000 unter Windows 2000

Wenn Sie Windows 2000 für WSUS verwenden und keinen Zugriff auf Microsoft SQL Server 2000 haben, installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE), bevor Sie das WSUS-Setupprogramm starten. Ist MSDE bereits auf dem WSUS-Server installiert, muss keine eigene MSDE-Instanz für WSUS eingerichtet werden. In diesem Fall geben Sie während der WSUS-Installation einfach den Namen der vorhandenen Instanz an.

Die Installation von MSDE unter Windows 2000 Server umfasst vier Hauptschritte: Als Erstes müssen Sie das MSDE-Archiv in einen Ordner auf dem WSUS-Server herunterladen und es in einen Ordner auf Ihrem WSUS-Server entpacken. Starten Sie dann das MSDE-Setupprogramm über eine Eingabeaufforderung und mit den entsprechenden Befehlszeilenoptionen, legen Sie das Systemadministratorkennwort fest, und legen Sie als Instanzname „WSUS“ fest. Überprüfen Sie nach Abschluss der MSDE-Installation, ob die Instanz „WSUS“ als NT-Dienst ausgeführt wird. Zum Schluss müssen Sie zum Schutz des WSUS-Servers ein Sicherheitsupdate für MSDE hinzufügen.

#### Schritt 1: Herunterladen und Entpacken des MSDE-Archivs

Laden Sie das MSDE-Archiv in einen Ordner auf dem WSUS-Server herunter, und entpacken Sie das Archiv. Siehe [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Version A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Schritt 2: Installieren von MSDE

Starten Sie das MSDE-Setupprogramm über eine Eingabeaufforderung und mit den entsprechenden Befehlszeilenoptionen, legen Sie das Systemadministratorkennwort fest, und legen Sie als Instanzname „WSUS“ fest. Überprüfen Sie nach Abschluss der MSDE-Installation, ob die Instanz „WSUS“ als NT-Dienst ausgeführt wird.

So können Sie MSDE installieren, das Systemadministratorkennwort festlegen und einen Instanznamen zuweisen:

1.  Wechseln Sie an der Eingabeaufforderung zu dem MSDE-Installationsordner, den Sie in Schritt 1, „Herunterladen und Entpacken des MSDE-Archivs“, angegeben haben.
2.  Geben Sie Folgendes ein: **setup sapwd="***Kennwort***" instancename=WSUS**
    *Kennwort* bezeichnet hierbei ein sicheres Kennwort für das Systemadministratorkonto dieser MSDE-Instanz, **instancename** ist der Name der Datenbankinstanz. Stattdessen können Sie auch den Standardinstanznamen (anstelle von „WSUS“) für Ihre WSUS-Datenbank verwenden. In diesem Fall kann die Angabe **instancename=WSUS** im Befehlszeilenparameter entfallen. Mit diesem Befehl wird das MSDE-Setupprogramm gestartet, das Systemadministratorkennwort festgelegt und dieser MSDE-Instanz der angegebene Name zugewiesen.

#### Schritt 3: Überprüfen, dass die MSDE-Instanz „WSUS“ installiert ist

Vergewissern Sie sich, dass Sie die MSDE-Instanz „WSUS“ sehen können.

1.  Klicken Sie auf **Start** und dann auf **Ausführen**.
2.  Geben Sie im Feld **Öffnenservices.msc** ein, und klicken Sie auf **OK**.

Blättern Sie durch die Liste der Dienste, und überprüfen Sie, ob der Dienst mit der Bezeichnung „MSSQL$WSUS“ (bei Verwendung von „WSUS“ als Instanzname) bzw. „MSSQLSERVER“ (bei Verwendung des Standardinstanznamens) aufgeführt wird.

#### Schritt 4: Starten der MSDE-Instanz

Zum Abschluss der MSDE-Installation muss die Instanz gestartet werden. Falls Sie die Instanz „WSUS“ benannt haben, starten Sie entsprechend „MSSQL$WSUS“. Bei Verwendung des Standardinstanznamens muss „MSSQLSERVER“ gestartet werden. Wird dieser Dienst nicht gestartet, ist WSUS nicht in der Lage, auf die Datenbankinstanz zuzugreifen.

#### Schritt 5: Aktualisieren von MSDE

Downloaden Sie das Sicherheitsupdate, das im Bulletin [MS03-031: Kumulativer Sicherheitspatch für SQL Server](http://go.microsoft.com/fwlink/?linkid=47364) beschrieben ist, und installieren Sie den Patch.

Informationen zum Herunterladen des Sicherheitsupdates finden Sie unter [SQL Server 2000 (32-Bit) - Sicherheitspatch MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Problem 4: Mindestanforderungen an den Speicherplatz

Für die Installation der Windows Server Update Services gelten die folgenden Mindestanforderungen an den Speicherplatz:

-   1 Gigabyte (GB) auf der Systempartition
-   2 GB im Volume, in dem die Datenbankdateien gespeichert werden
-   6 GB, je nach prognostiziertem Umfang der Inhalte

#### Problem 5: Frühere Versionen von WSUS müssen über die Option „Software“ in der Systemsteuerung deinstalliert werden, bevor die neueste Version installiert werden kann

Falls die Windows Server Update Services auf einem Server installiert werden sollen, auf dem bereits Windows Update Services Beta 1 oder Beta 2 installiert ist, muss diese frühere Version zunächst über die Option „Software“ in der Systemsteuerung deinstalliert werden.

#### Problem 6: Für WSUS muss die Option für geschachtelte Trigger in SQL Server aktiviert sein

Diese Option ist standardmäßig aktiviert, kann jedoch durch einen SQL Server-Administrator deaktiviert werden.

Wenn als Windows Server Update Services-Datenspeicher eine SQL Server-Datenbank verwendet werden soll, sollte der SQL Server-Administrator überprüfen, ob die Option für geschachtelte Trigger auf dem Server aktiviert ist, bevor der WSUS-Administrator WSUS installiert und beim Einrichten von WSUS die Datenbank angibt.

Das WSUS-Setupprogramm aktiviert die datenbankspezifische Option „RECURSIVE\_TRIGGERS“, die (serverweite) Option für geschachtelte Trigger wird jedoch nicht aktiviert.

Mit dem folgenden Befehl überprüfen Sie, ob geschachtelte Trigger aktiviert sind:

**sp\_configure 'nested triggers'**

Um die Option für geschachtelte Trigger in SQL Server zu aktivieren, führen Sie den folgenden Code in einer Batchdatei auf dem Computer aus, auf dem SQL Server ausgeführt wird:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Problem 7: Befehlszeilenparameter für das WSUS-Setupprogramm

WSUS kann auch unbeaufsichtigt installiert werden. Weitere Informationen sowie Angaben zu den verfügbaren Befehlszeilenparametern finden Sie in Anhang A des Artikels zur [Bereitstellung von Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (möglicherweise in englischer Sprache), der sich mit der unbeaufsichtigten Installation beschäftigt.

Bekannte Probleme
-----------------

#### Problem 1: IIS-Lockdown-Assistent

Wenn Sie IIS auf einem Computer mit Windows 2000 Server ausführen, installieren Sie die neueste Version des IIS-Lockdown-Assistenten (mit URLScan) von der IIS-Lockdown-Tool-Webseite in Microsoft TechNet. Die Installation dieses Tools wird dringend empfohlen, damit die Sicherheit der IIS-Server gewährleistet ist. Der IIS-Lockdown-Assistent deaktiviert nicht benötigte Features von IIS und senkt damit das Sicherheitsrisiko.

| ![](images/Cc720505.note(WS.10).gif)Hinweis                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diese Komponenten werden nicht über das WSUS-Setupprogramm installiert, sondern müssen manuell installiert werden. Bei Computern mit Windows Server 2003 ist die IIS-Lockdown-Funktion bereits integriert und muss daher nicht gesondert installiert werden. |

#### Problem 2: Direkte Änderungen der WSUS-Konfiguration in der Datenbank werden nicht unterstützt

Windows Server Update Services speichert die Konfigurationsdaten in einer Datenbank (MSDE oder SQL Server). Eine Änderung dieser Konfigurationsdaten per direkten Zugriff auf die Datenbank wird nicht unterstützt. Die Administratoren sollten nicht versuchen, die WSUS-Konfiguration auf diese Weise zu ändern. Die WSUS-Konfiguration kann über die WSUS-Konsole oder durch Aufrufen der entsprechenden WSUS-APIs geändert werden.

#### Problem 3: Für den Zugriff auf die WSUS-Verwaltungswebsite muss Active Scripting aktiviert sein

Auf der Arbeitsstation des Administrators muss Internet Explorer so konfiguriert werden, dass Active Scripting zugelassen wird, damit Sie über Internet Explorer auf die Website zur WSUS-Verwaltung zugreifen können.

#### Problem 4: IIS wird während der Installation von WSUS neu gestartet

Das Setupprogramm von Windows Server Update Services startet IIS ohne weitere Benachrichtigung neu. Dies kann sich auf vorhandene Websites im Unternehmen auswirken.

#### Problem 5: Ändern des Zugriffs auf virtuelle Verzeichnisse der WSUS- oder SMS-Verwaltungspunkte (MPs)

Standardmäßig ist das virtuelle Verzeichnis der Inhalte für Windows Server Update Services für den anonymen Zugriff eingerichtet. Wenn Sie diese Einstellung so ändern, dass eine Authentifizierung erforderlich ist, erhalten die Clients Authentifizierungsfehler, und der Zugriff wird verweigert, sodass die Clients keine Updates herunterladen können. Dies ist ein bekanntes Problem. „Winhttp.dll“ greift bei der implizierten Authentifizierung auf den falschen Authentifizierungskontext zurück, wodurch die Authentifizierung fehlschlägt. Um dieses Problem zu vermeiden, richten Sie den WSUS-Server und die SMS-MPs so ein, dass sie anonym auf virtuelle IIS-Verzeichnisse zugreifen.

#### Problem 6: Bei der Installation von WSUS unter Windows Small Business Server 2003 müssen die Einstellungen für den Zugriff auf das virtuelle WSUS-Stammverzeichnis der Standardwebsite so geändert werden, dass die WSUS-Clients selbst die notwendigen Aktualisierungen über den Server ausführen können

Der WSUS-Server installiert zwei virtuelle Stammverzeichnisse („SelfUpdate“ und „ClientWebService“) sowie einige Dateien im Stammverzeichnis der Standardwebsite (an Port 80). Auf diese Weise sind die Clients in der Lage, selbst die notwendigen Aktualisierungen über die Standardwebsite vorzunehmen. Bei Windows Small Business Server 2003 ist die Standardwebsite standardmäßig so konfiguriert, dass der Zugriff für alle IP-Adressen und alle lokalen Hosts (localhost) verweigert wird, mit Ausnahme der IP-Adressen und der lokalen Hosts (localhost) des Servers. Damit wird der Zugriff auf die virtuellen Stammverzeichnisse „SelfUpdate“ und „ClientWebService“ verweigert, sodass die Clients die Aktualisierungen nicht selbst starten können. Um den Clients den Zugriff zu gewähren und ihnen damit die Möglichkeit zu geben, die Aktualisierungen selbst zu starten, führen Sie die nachstehenden Schritte für die virtuellen Stammverzeichnisse „SelfUpdate“ und „ClientWebService“ der Standardwebsite aus.

1.  Klicken Sie im virtuellen Stammverzeichnis auf **Eigenschaften**, klicken Sie auf **Verzeichnissicherheit**, dann auf **Beschränkungen für IP-Adressen und Domänennamen** und schließlich auf **Bearbeiten**.
2.  Aktivieren Sie die Option **Zugriff gewährt**, und klicken Sie auf **OK**. Schließen Sie alle Eigenschaftsseiten.

#### Problem 7: Installation von WSUS unter Small Business Server: Probleme mit der Integration

-   Wenn Windows Small Business Server 2003 über einen ISA-Proxyserver auf das Internet zugreift, müssen die folgenden Angaben manuell in die Benutzeroberfläche **Einstellungen** eingetragen werden: Proxyservereinstellungen, Proxyservername, Port.
-   Greift ISA auf die Windows-Authentifizierung zurück, sind die Anmeldeinformationen für den Proxyserver im Format „DOMÄNE\\Benutzer“ anzugeben. (Der Benutzer muss dabei zur Gruppe der Internetbenutzer gehören.)

#### Problem 8: Bei der Verlagerung eines Computers in eine andere Computergruppe kann es passieren, dass dieser Computer erst nach einer Stunde auf der Verwaltungskonsole angezeigt wird

Wenn Sie einen Computer erstmalig einer Zielgruppe zuweisen, werden die Daten auf dem Computer gemäß den Gruppeninformationen angepasst. Die Daten werden in regelmäßigen Abständen (oder stündlich) aktualisiert. Wird ein Computer in eine andere Computergruppe verlagert, kann es daher bis zu einer Stunde dauern, bis diese Daten auf dem Client aktualisiert und mit den entsprechenden Änderungen auf der WSUS-Verwaltungskonsole angezeigt werden.

#### Problem 9: Wird WSUS auf einem Mitgliedsserver installiert und dieser danach zum Domänencontroller hochgestuft, muss WSUS erst deinstalliert werden

Wenn Sie WSUS auf einem Mitgliedsserver installieren und dann den Mitgliedsserver zum Domänencontroller hochstufen möchten, ist wie folgt vorzugehen:

1.  Deinstallieren Sie WSUS.
2.  Stufen Sie den Server zum Domänencontroller hoch.
3.  Installieren Sie WSUS neu.

#### Problem 10: Soll ein WSUS-Server von einem Domänencontroller zu einem Mitgliedsserver herabgestuft werden, muss WSUS erst deinstalliert werden

Wenn Sie WSUS-Server auf einem Domänencontroller ausführen und dann den Domänencontroller zu einem Mitgliedsserver herabstufen möchten, fallen die folgenden Schritte an:

1.  Deinstallieren Sie WSUS unter Beibehaltung der Datenbank.
2.  Erstellen Sie ein neues Benutzerkonto mit dem Namen „ASPNET“.
3.  Geben Sie an der Eingabeaufforderung Folgendes ein: **aspnet\_regiis -i**.
4.  Deinstallieren Sie WSUS, und verwenden Sie die beibehaltene Datenbank.

#### Problem 11: Wenn .NET Framework 1.0 oder 2.0 nach WSUS installiert wird, wird die WSUS-Verwaltungskonsole nicht angezeigt

Der Grund hierfür liegt darin, dass sich .NET Framework 1.0 bei IIS registriert, der WSUS-Server aber .NET Framework 1.1 voraussetzt. Öffnen Sie zur Behebung dieses Problems „aspnet\_regiis.exe“, und führen Sie die nachstehenden Befehle aus. *Website-ID* bezeichnet dabei den Wert im folgenden Registrierungsschlüssel:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website-ID*&gt;\\ROOT\\Content

#### Problem 12: Einschränkungen bei Remote-SQL

WSUS bietet nur eingeschränkte Unterstützung für die Ausführung von Datenbanksoftware auf einem anderen Computer als dem, auf dem der Rest der WSUS-Anwendung installiert ist.

-   Windows 2000 Server kann nicht als Front-End-Computer in einem SQL-Remotepaar eingesetzt werden.
-   Es ist nicht möglich, einen als Domänencontroller konfigurierten Server als Front-End oder Back-End des SQL-Remotepaars zu verwenden.
-   Auf dem Back-End-Computer können Sie nicht WMSDE oder MSDE als Datenbanksoftware nutzen.
-   Die Einrichtung von SQL Server (zur Verwendung als WSUS-Datenbank) auf einem Remoteserver schlägt fehl, wenn auf dem Remoteserver Terminaldienste installiert ist und im Anwendungsmodus ausgeführt wird. Beim Installieren von SQL Server auf einem Terminaldienste-Server müssen Sie Folgendes tun:
    1.  Bevor Sie das Setupprogramm starten, öffnen Sie eine Eingabeaufforderung, und geben Sie Folgendes ein: **change user /install**
    2.  Führen Sie das SQL Server-Setupprogramm aus.
    3.  Geben Sie im Anschluss an die SQL Server-Installation an der Eingabeaufforderung Folgendes ein: **change user /execute**
-   Um die WSUS-Datenbank auf dem SQL Server-Remoteserver einrichten zu können, müssen Sie sowohl auf dem Front-End-Computer als auch auf dem Back-End-Computer zur lokalen Sicherheitsgruppe der Administratoren gehören.
-   Weitere Informationen zu Problemen mit SQL Server auf Remoteservern finden Sie im Anhang C des Artikels zur [Bereitstellung von Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (möglicherweise in englischer Sprache), der sich mit Remote-SQL beschäftigt.

#### Problem 13: Ein Downstream-Replikatserver besitzt weniger Genehmigungen als der übergeordnete Upstreamserver

Ein Downstream-Replikatserver besitzt unter Umständen weniger Genehmigungen als der übergeordnete Upstreamserver. Der Grund hierfür liegt darin, dass Installationsgenehmigungen erst dann an einen Downstreamserver weitergegeben werden, wenn der Download des Inhalts auf dem Upstreamserver beendet ist.

#### Problem 14: Wenn die Synchronisierung fehlschlägt, führen Sie erneut eine Synchronisierung aus

Wenn die Synchronisierung fehlschlägt, wird u. U. eine Fehlermeldung angezeigt. Versuchen Sie in diesem Fall zunächst erneut, eine Synchronisierung vorzunehmen.

#### Problem 15: Beim Zugriff auf die WSUS-Verwaltungskonsole wird eine Fehlermeldung vom Typ „System.IO.FileNotFoundException“ angezeigt

Wenn Sie die folgende Fehlermeldung erhalten, müssen ggf. die Berechtigungen für das Netzwerkdienst- oder ASP.NET-Konto angepasst werden:

System.IO.FileNotFoundException: Datei- oder Assemblyname '*xxxxxx*.dll' oder eine Abhängigkeit davon wurde nicht gefunden

*xxxx* bezeichnet hierbei einen beliebigen Dateinamen.

Um dieses Problem in Betriebssystemen der Windows Server 2003-Produktfamilie zu beheben, gewähren Sie dem Netzwerkdienstkonto Schreib-/Lesezugriff auf „%systemroot%\\Temp“. Bei Windows 2000 Server gewähren Sie entsprechend dem ASP.NET-Konto Schreib-/Lesezugriff auf „%systemroot%\\Temp“.

#### Problem 16: SQL-Sicherheitsupdate MS03-031 (KB815495)

Unter Umständen wird dieses Update beim WSUS-Server auch dann als installiert angezeigt, wenn die Installation auf dem Client fehlgeschlagen ist. Das Paket wird dem Client daher ggf. erneut angeboten. Um dieses Problem zu umgehen, können Sie die Genehmigung für das Update auf dem Server wieder aufheben.

#### Problem 17: IIS-Einstellungen gehen beim RTM-Upgrade verloren

Wenn Sie WSUS RTM auf einem Server ausführen, auf dem sich eine frühere Version von WSUS befindet (beispielsweise RC), wird diese frühere Version durch WSUS RTM deinstalliert. Anschließend wird die neue Version installiert. Dies bedeutet, dass alle virtuellen Stammverzeichnisse und alle Dateien gelöscht werden, die mit WSUS in IIS verknüpft sind.

Wurde WSUS auf der Standard-Website installiert, gehen alle WSUS-spezifischen Einstellungen verloren, die Sie an den virtuellen WSUS-Stammverzeichnissen vorgenommen haben. Wenn Sie beispielsweise die virtuellen WSUS-Stammverzeichnisse für SSL so konfiguriert haben, dass WSUS abgesichert wird, müssen diese Stammverzeichnisse nach der Installation der RTM-Version von WSUS neu konfiguriert werden. Hinweis: Auf der WSUS-Konsole wird eine Benachrichtigung angezeigt, dass SSL nicht aktiviert ist.

Wenn Sie WSUS auf einer anderen Website installiert haben (also nicht auf der Standardwebsite), gehen alle zusätzlichen Einstellungen auf der Ebene der WSUS-Website verloren.

#### Problem 18: Verwenden von Hostheadern

Wenn der Standardwebsite (WSUS-Website) in IIS bestimmte Hostheaderwerte zugewiesen werden sollen, nehmen Sie in die Liste der IP-Adressen ohne Hostheaderwert für die Standardwebsite den Eintrag „Keine zugewiesen“ bzw. eine zugewiesene IP-Adresse auf. Dieser Eintrag sollte auch auf der anderen Website ergänzt werden.

**Warnung**: Dies kann die Funktionsfähigkeit von Windows® SharePoint® Services und Exchange beeinträchtigen.

#### Problem 19: Die URL der WSUS-Konsole muss auf Computern, auf denen eine stärkere Absicherung von Internet Explorer aktiviert ist, in die Webinhaltszonen „Vertrauenswürdige Sites“ und „Lokales Intranet“ aufgenommen werden

Wenn die stärkere Absicherung von Internet Explorer (die Komponente „Verstärkte Sicherheitskonfiguration für Internet Explorer“ in Microsoft Windows Server 2003) auf einem Computer aktiviert ist und Sie die WSUS-Konsole nicht in die Webinhaltszonen „Vertrauenswürdige Sites“ und „Lokales Intranet“ eintragen, werden Sie bei jedem Öffnen einer Seite in der WSUS-Konsole aufgefordert, Ihre Anmeldeinformationen einzugeben.

So nehmen Sie die WSUS-Konsole in die Webinhaltszonen **Lokales Intranet** und **Vertrauenswürdige Sites** auf:

1.  Öffnen Sie **Internetoptionen**. (Klicken Sie hierzu beispielsweise auf **Start**, zeigen Sie auf **Systemsteuerung**, und klicken Sie dort auf **Internetoptionen**).
2.  Klicken Sie auf der Registerkarte **Sicherheit** auf **Lokales Intranet**, dann auf **Sites** und auf **Erweitert**. Geben Sie die URL ein (http://*WSUSServername*/WSUSAdmin), und klicken Sie auf **OK**.
3.  Klicken Sie auf **Vertrauenswürdige Sites** und dann auf **Sites**. Geben Sie die URL der WSUS-Konsole ein. Klicken Sie auf **OK** und dann zum Schließen von **Internetoptionen** erneut auf **OK**.

#### Problem 20: Upgrade des WSUS Release Candidate schlägt fehl

Ein Upgrade vom WSUS Release Candidate kann fehlschlagen, weil beim Selbstaktualisieren des Verzeichnisses ein Problem auftritt. Zu diesem Problem kann es kommen, wenn mehrere Clients zu dem Zeitpunkt eine eigene Aktualisierung vornehmen, zu dem Sie versuchen, das Upgrade durchzuführen.

So lösen Sie dieses Problem:

1.  Trennen Sie den WSUS-Server vom Netzwerk, d. h., sorgen Sie dafür, dass die Clients keine Verbindung zum WSUS-Server herstellen können.
2.  Geben Sie an einer Eingabeaufforderung Folgendes ein: **iisrestart /reset**. Drücken Sie dann die EINGABETASTE.
3.  Führen Sie das Upgrade aus.

#### Problem 21: Bei einigen Genehmigungen von SUS 1.0 schlägt die Migration auf WSUS fehl.

Beim Migrieren von SUS 1.0 auf WSUS werden einige Genehmigungen auf dem SUS 1.0-Server nicht auf den WSUS-Server migriert. Dies liegt daran, dass eine Reihe von Updates, die für SUS 1.0 verfügbar waren, für WSUS nicht mehr zur Verfügung stehen. Da WSUS auch mehr Updates unterstützt als SUS, können nach Abschluss des Migrationsprozesses auf Ihrem WSUS-Server wichtige Updates vorhanden sein, die nicht genehmigt sind.

Microsoft empfiehlt daher dringend, nach der Migration von SUS 1.0 die auf dem WSUS-Server vorhandenen nicht genehmigten Updates zu prüfen.

Weitere Informationen zum Migrieren von SUS 1.0 auf WSUS finden Sie in den [Schrittanweisungen zum Migrieren von Software Update Services auf Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=48042) unter http://go.microsoft.com/fwlink/?LinkId=48042 (möglicherweise in englischer Sprache).

#### Problem 22: Korrigieren Sie diesen Registrierungsschlüssel vor dem Upgrade auf WSUS 2.0 Service Pack 1, sofern Sie eine Migration von WMSDE auf SQL Server durchgeführt haben

Wenn Sie WSUS 2.0 auf Service Pack 1 aktualisieren möchten und Sie Ihre WMSDE-Installation auf SQL Server migriert haben (gleich, ob remote oder lokal), müssen Sie den folgenden Registrierungseintrag ändern:

HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled

Der Wert muss von 1 in 0 geändert werden.

#### Problem 23: Migrieren einer Remote-SQL-Installation auf WSUS 2.0 Service Pack 1

Führen Sie zum Migrieren einer Remote-SQL-Installation auf WSUS 2.0 Service Pack 1 die folgenden Schritte aus:

1) Führen Sie das Setup-Paket auf dem Front-End-Computer aus, ohne zusätzliche Optionsschalter zu verwenden, und wählen Sie die Option zum Upgraden.

2) Führen Sie das Setup-Paket auf dem Back-End-Computer aus, ohne zusätzliche Optionsschalter zu verwenden, und wählen Sie die Option zum Upgraden.

#### Copyright

Die in diesem Dokument enthaltenen Angaben entsprechen dem Wissensstand der Microsoft Corporation zu den beschriebenen Problemen zum Zeitpunkt der Veröffentlichung. Microsoft muss auf veränderte Marktbedingungen reagieren und ist daher weder in der Lage noch dazu verpflichtet, die Richtigkeit der dargelegten Informationen über das Datum der Veröffentlichung hinaus zu garantieren.

Dieses Dokument dient lediglich zu Informationszwecken. MICROSOFT ÜBERNIMMT KEINE AUSDRÜCKLICHE, KONKLUDENTE ODER GESETZLICHE GEWÄHRLEISTUNG FÜR DIE INFORMATIONEN IN DIESEM DOKUMENT.

Die Benutzer sind verpflichtet, sich an alle geltenden Urheberrechtsgesetze zu halten. Unabhängig von der Anwendbarkeit der geltenden Urheberrechtsgesetze darf ohne ausdrückliche schriftliche Genehmigung der Microsoft Corporation kein Teil dieses Dokuments für beliebige Zwecke vervielfältigt, in einem Datenempfangssystem gespeichert oder darin eingelesen werden oder übertragen werden, unabhängig davon, auf welche Art und Weise oder mit welchen Mitteln (elektronisch, mechanisch, durch Fotokopieren, Aufzeichnen usw.) dies geschieht.

Es ist möglich, dass Microsoft Patente bzw. angemeldete Patente, Marken, Urheberrechte oder sonstige geistige Eigentumsrechte besitzt, die sich auf den fachlichen Inhalt dieses Dokuments beziehen. Das Bereitstellen dieses Dokuments gibt Ihnen jedoch keinen Anspruch auf diese Patente, Marken, Urheberrechte oder auf sonstiges geistiges Eigentum, es sei denn, dies wird ausdrücklich in schriftlichen Lizenzverträgen von Microsoft eingeräumt.

Die in den Beispielen verwendeten Firmen, Organisationen, Produkte, Domänennamen, E-Mail-Adressen, Logos, Personen, Orte und Ereignisse sind frei erfunden, soweit nichts anderes angegeben ist. Jede Ähnlichkeit mit bestehenden Firmen, Organisationen, Produkten, Domänennamen, E-Mail-Adressen, Logos, Personen, Orten oder Ereignissen ist rein zufällig.

© 2005 Microsoft Corporation. Alle Rechte vorbehalten.

Microsoft, SQL Server, Windows und Windows Server sind Marken oder eingetragene Marken der Microsoft Corporation in den USA und/oder in anderen Ländern.

Andere in diesem Dokument aufgeführte Produkt- und Firmennamen sind möglicherweise Marken der jeweiligen Eigentümer.
