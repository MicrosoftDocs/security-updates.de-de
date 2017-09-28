---
TOCTitle: Infodatei für WSUS mit Servixe Pack 1
Title: Infodatei für WSUS mit Servixe Pack 1
ms:assetid: '937ecfe9-e8e0-41ac-85f7-4b65956f3d1e'
ms:contentKeyID: 18127532
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc708486(v=WS.10)'
---

Infodatei für WSUS mit Servixe Pack 1
=====================================

In diesem Dokument werden bekannte Probleme im Zusammenhang mit den Windows Server Update Services (WSUS) mit Service Pack 1 (SP1) beschrieben. Direkt im Anschluss an die Informationen zu WSUS mit SP1 sind alle Angaben aus der ursprünglichen WSUS-Infodatei aufgeführt. Hier finden Sie weitere Empfehlungen sowie die Systemvoraussetzungen für die Installation von WSUS. Weitere Informationen zum Herunterladen von WSUS mit SP1 finden Sie im [Microsoft Download Center](http://go.microsoft.com/fwlink/?linkid=67516).

Neuigkeiten in WSUS mit SP1
---------------------------

WSUS mit SP1 ist eine Service Pack-Version, mit der die Sicherheit, Zuverlässigkeit, Skalierbarkeit, Kompatibilität und Leistung von WSUS optimiert werden. Neue Features und Verbesserungen:

-   Unterstützung für Windows Vista-Clients: Computer mit Windows Vista können über den WSUS SP1-Server aktualisiert werden.
-   Unterstützung für mehr Clientsprachen: Es werden alle Sprachen aus Office und Windows Vista unterstützt.
-   Neue WMSDE-Version: Bei der WMSDE-Version bewirkt WSUS mit SP1 ein Upgrade auf WMSDE SP4 (WSUS RTM nutzt WMSDE SP3).
-   Leistungsverbesserungen: WSUS mit SP1 umfasst verschiedene Leistungsverbesserungen, mit denen die Reaktionszeit der Benutzeroberfläche verkürzt wird.
-   Alle Hotfixes: WSUS mit SP1 enthält alle Änderungen und Hotfixes, die seit der Einführung von WSUS RTM veröffentlicht wurden.
-   Unterstützung für SQL Server 2005.

Vor Beginn des Upgrades auf WSUS mit SP1
----------------------------------------

Beim Upgrade auf WSUS mit SP1 sind die nachstehenden Probleme zu beachten. Die Probleme und Anforderungen im Abschnitt „Vor Beginn“ in der Originalversion dieses Themas werden im vorliegenden Abschnitt nicht mehr genannt und sind weiterhin gültig. Die Voraussetzungen für die Einrichtung, die im ursprünglichen Abschnitt „Vor Beginn“ aufgeführt sind, gelten beispielsweise nach wie vor.

**Hinweis**   Nach der Installation von SP1 für WSUS 2.0 ist es nicht möglich, das Service Pack wieder zu deinstallieren. Bei der Deinstallation von SP1 wird das gesamte Produkt deinstalliert.

**Wichtig**   Dieses Dokument enthält Angaben zur Bearbeitung der Registrierung. Fertigen Sie zunächst eine Sicherungskopie der Registrierung an, bevor Sie Änderungen daran vornehmen. Informieren Sie sich, wie Sie die Registrierung wiederherstellen, falls ein Problem auftritt. Weitere Informationen zum Sichern, Wiederherstellen und Bearbeiten der Registrierung finden Sie im folgenden Artikel in der Microsoft Knowledge Base:

[Beschreibung der Microsoft Windows Registrierung](http://support.microsoft.com/kb/256986) (http://support.microsoft.com/kb/256986/)

#### Problem 1: Freier Speicherplatz für die Sicherung der Datenbank

Beim Upgrade von WSUS RTM legt das Setupprogramm für WSUS mit SP1 automatisch eine Sicherung der WSUS-Datenbank an. Der Speicherplatz im Dateisystem des WSUS-Servers muss die Sicherungskopie der WSUS-Datenbank aufnehmen können; ansonsten schlägt das Setup für WSUS mit SP1 fehl.

**So ermitteln Sie, ob ausreichend Speicherplatz zur Verfügung steht:**
1.  Öffnen Sie den Windows Explorer, und wechseln Sie zum Ordner, in dem die WSUS-Datenbank gespeichert ist. Standardmäßig wird die WSUS-Datenbank im folgenden Ordner gespeichert:

    
        ```
2.  Halten Sie **STRG** gedrückt, markieren Sie die Dateien **SUSDB.MDF** und **SUSDB\_log.LDF**, klicken Sie mit der rechten Maustaste auf eine der Dateien, und klicken Sie dann auf **Eigenschaften**.

3.  Beachten Sie im Dialogfeld **Dateien** den Wert im Feld **Größe auf Datenträger**. Der Datenträger muss mindestens diese Menge an freiem Speicherplatz aufweisen, damit WSUS mit SP1 installiert werden kann.

4.  Klicken Sie im Menü **Start** auf **Arbeitsplatz**. Überprüfen Sie, ob der erforderliche Speicherplatz auf dem Datenträger, auf dem WSUS installiert ist, tatsächlich zur Verfügung steht.

Falls das Setup für WSUS mit SP1 fehlschlägt, stellen Sie die gesicherte Datenbank manuell wieder her. Weitere Informationen zum Wiederherstellen der WSUS-Datenbank finden Sie im [WSUS Operations Guide](http://technet2.microsoft.com/windowsserver/en/library/05f2e884-ae62-4c90-9681-6c9f2f3c9fd91033.mspx).

#### Problem 2: WSUS mit SP1 gilt nur als Upgrade für WSUS RTM

Mit WSUS mit SP1 können Sie lediglich das Upgrade für WSUS RTM durchführen. Derzeit besteht keine Unterstützung für ein Upgrade des WSUS Release Candidate. Falls der WSUS Release Candidate oder eine frühere Version von WSUS installiert ist, müssen Sie diese Builds deinstallieren und dann WSUS mit SP1 ausführen.

#### Problem 3: Der IIS-Dienst auf dem Server wird beim Upgrade auf WSUS mit SP1 angehalten

Das Installationsprogramm für das Upgrade auf WSUS mit SP1 hält den IIS-Dienst (Internetinformationsdienste) auf dem Server an, während das Upgrade durchgeführt wird. Dies bedeutet, dass alle Websites, die von der IIS-Installation auf dem Server gehostet werden, über den Zeitraum des Upgrades nicht zur Verfügung stehen. Nach Beendigung des Upgrades wird IIS automatisch gestartet.

#### Problem 4: Beim Upgrade dürfen keine Anwendungen ausgeführt werden, mit denen WSUS-APIs aufgerufen werden

Aufrufe von WSUS-APIs (Anwendungsprogrammierschnittstelle) führen zu Konflikten mit dem Installationsprogramm für WSUS mit SP1, wodurch das Upgrade mit einem Fehler abgebrochen wird. (Sie erhalten eine Meldung, dass Sie den Server neu starten sollen, um das Upgrade abzuschließen.)

#### Problem 5: Beim Upgrade auf WSUS mit SP1 müssen ggf. Antivirenprogramme deaktiviert werden

Bei einem Upgrade von WSUS auf WSUS mit SP1 müssen unter Umständen die Antivirenprogramme deaktiviert werden, bevor Sie das Upgrade durchführen oder das Service Pack installieren können. Sobald Sie die Antivirenprogramme deaktiviert haben, starten Sie den Windows Server-Computer neu, und installieren Sie dann erst das Upgrade oder das Service Pack. Auf diese Weise ist dafür gesorgt, dass keine Dateien gesperrt sind, auf die der Upgradevorgang zugreift. Nach Abschluss der Installation aktivieren Sie das Antivirenprogramm wieder. Weitere Anweisungen zum Deaktivieren und erneuten Aktivieren Ihres Antivirenprogramms in der vorliegenden Version finden Sie auf der Website des Programmherstellers.

| ![](images/Cc708486.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                   |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Durch diese Behelfslösung ist Ihr Computer oder Ihr Netzwerk anfälliger für Angriffe von böswilligen Benutzern oder durch schädliche Software (z. B. Viren). Die Behelfslösung wird nicht empfohlen, sondern soll hier nur der Vollständigkeit halber angegeben werden, so dass Sie selbst entscheiden können, ob Sie sie einsetzen oder nicht. Die Verwendung dieser Behelfslösung erfolgt auf eigene Gefahr. |

| ![](images/Cc708486.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                           |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Antivirenprogramme schützen Ihren Computer vor Viren. Wenn das Antivirenprogramm deaktiviert ist, dürfen Sie keine Dateien herunterladen oder öffnen, die aus Quellen stammen, denen Sie nicht vertrauen. Außerdem dürfen Sie keine Websites besuchen, denen Sie nicht vertrauen, und keine E-Mail-Anhänge öffnen. |

#### Problem 6: Bei Verwendung eines Proxyservers werden der Benutzername und das Kennwort für die Proxykonfiguration beim Upgrade auf SP1 ggf. gelöscht

Wenn Sie einen Proxyserver verwenden, werden der Benutzername und das Kennwort für die Proxykonfiguration beim Upgrade auf SP1 ggf. gelöscht. Bei der Synchronisierung der Microsoft-Server kann dies zu einem Fehler wegen eines ungültigen Parameters führen. Zur Behebung dieses Problems setzen Sie den Benutzernamen und das Kennwort zurück, und synchronisieren Sie den Server neu.

#### Problem 7: Wiederherstellung des WSUS-Servers nach einem fehlgeschlagenen Upgrade in einen konsistenten Zustand; anschließend Neustart des Upgrades

Wenn beim Upgrade auf WSUS mit SP1 ein Fehler auftritt, ist die WSUS-Installation unter Umständen inkonsistent oder nicht verwendbar. Um das Upgrade auf WSUS mit SP1 erneut durchführen zu können, muss die WSUS-Installation wieder in einen konsistenten Zustand gebracht werden. Setzen Sie hierzu den WSUS-Server mithilfe der Sicherungsdatenbank, die zu Beginn des Upgradevorgangs angelegt wurde, auf den Stand vor Beginn des Upgrades zurück.

Für den Fall, dass ein Fehler beim Upgrade auftritt, starten Sie das Upgrade auf WSUS mit SP1 wie folgt neu:

**So starten Sie das Upgrade auf WSUS mit SP1 neu:**
1.  Ermitteln Sie den Pfad der Sicherungsdatenbank anhand der Angaben in der Protokolldatei „WSUSSetup\_%timestamp%.log“. Diese Datei befindet sich im folgenden Ordner:

    -   %programfiles%\\Update Services\\LogFiles

2.  Stellen Sie die Sicherungsdatenbank mit dem folgenden Befehl auf dem WSUS-Computer wieder her:

    -   osql.exe -S &lt;Datenbankinstanz&gt; -E -Q "USE master ALTER DATABASE SUSDB SET SINGLE\_USER WITH ROLLBACK IMMEDIATE RESTORE DATABASE SUSDB FROM DISK=N'&lt;Datenbanksicherungspfad&gt;' WITH REPLACE ALTER DATABASE SUSDB SET MULTI\_USER"
    -   Ersetzen Sie die Platzhalter &lt;Datenbankinstanz&gt; und &lt;Datenbanksicherungspfad&gt; mit den entsprechenden Werten für Ihre Installation.
    -   Geben Sie unter &lt;Datenbankinstanz&gt; den Wert aus dem folgenden Registrierungsschlüssel ein:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\SqlServerName
    -   Geben Sie unter &lt;Datenbanksicherungspfad&gt; den Wert aus Schritt 1 ein.

3.  Deinstallieren Sie WSUS, ohne jedoch die WSUS-Datenbank, die Protokolldateien und die Updatedateien zu löschen, selbst wenn Sie dazu aufgefordert werden. (Stellen Sie sicher, dass alle Optionen unter **Microsoft Windows Server Update Services entfernen** deaktiviert sind.)

4.  Installieren Sie WSUS RTM neu (die ursprüngliche Version, nicht WSUS mit SP1). Geben Sie die vorhandene Datenbank an, wenn Sie dazu aufgefordert werden. Damit wird das WSUS-System wieder in einen konsistenten Status zurückgeführt.

5.  Installieren Sie WSUS mit SP1.

**Hinweis**    Bei einer Neuinstallation von WSUS mit SP1 können Sie nicht die gesicherte Datenbank aus Schritt 1 verwenden. Das Datenbankschema wurde geändert; ohne Upgrade auf WSUS mit SP1 ist diese Datenbank also nicht kompatibel.

#### Problem 8: Möglicher Fehler beim Upgrade auf WSUS mit SP1 nach einer Migration der WMSDE-Datenbank

Die Lösung ist davon abhängig, ob Sie auf einen lokalen SQL-Server oder auf einen SQL-Remoteserver migriert haben.

#### Migration der WMSDE-Datenbank auf einen lokalen SQL 2000-Server

Damit das Setuppaket für WSUS mit SP1 erkennt, dass keine WMSDE-Datenbank vorhanden ist, muss der Wert eines Registrierungsschlüssels geändert werden.

Wenn Sie WMSDE auf einen lokalen SQL 2000-Server migriert haben, nehmen Sie die folgende Änderung an der Registrierung vor, bevor Sie das Upgrade auf WSUS mit SP1 durchführen:

-   Ändern Sie den Wert des folgenden Registrierungsschlüssels von „1“ in „0“:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled  

#### Migration der WMSDE-Datenbank auf einen SQL 2000-Remoteserver

Damit das Setuppaket für WSUS mit SP1 erkennt, dass keine WMSDE-Datenbank vorhanden ist, muss der Wert zweier Registrierungsschlüssel geändert werden. Das Update muss erst auf dem Back-End-Server durchgeführt werden und dann auf dem Front-End-Server.  

Wenn Sie WMSDE auf einen SQL 2000-Remoteserver migriert haben, nehmen Sie die folgenden Änderungen an der Registrierung vor, bevor Sie das Upgrade auf WSUS mit SP1 durchführen:

1.  Ändern Sie den Wert des folgenden Registrierungsschlüssels von „1“ in „0“:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\WmsdeInstalled 
2.  Ändern Sie den Wert des folgenden Registrierungsschlüssels von „0x80“ in „0x20“:
    -   HKLM\\Software\\Microsoft\\Update Services\\Server\\Setup\\InstallType 

Sobald Sie diese Registrierungsschlüsselwerte aktualisiert haben, starten Sie das Upgrade auf den Back-End-Servern und danach auf den Front-End-Servern.

#### Problem 9: WSUS mit SP1 gilt nicht als Upgrade für WSUS-Server, die mit SQL-Remotebereitstellungen eingerichtet wurden

Das Setuppaket für WSUS mit SP1 muss sowohl auf dem Front-End-Server als auch auf dem Back-End-Server ausgeführt werden.

**So aktualisieren Sie auf WSUS mit SP1 bei Verwendung von Remote-SQL:**
1.  Führen Sie das Setuppaket auf dem Front-End-Server aus (ohne Befehlszeilenschalter), und starten Sie das Upgrade.

2.  Führen Sie das Setuppaket auf dem Back-End-Server aus (ohne Befehlszeilenschalter), und starten Sie das Upgrade.

#### Problem 10: Änderungen des Computernamens vor dem Upgrade auf WSUS mit SP1 kann zu einem Fehler beim Upgrade führen

Wenn Sie den Computernamen ändern, nachdem Sie WSUS RTM installiert haben und bevor Sie das Upgrade auf WSUS mit SP1 durchführen, schlägt das Upgrade auf WSUS mit SP1 unter Umständen fehl.

Entfernen Sie die Gruppen der ASPNET- und WSUS-Administratoren mit dem nachstehenden Skript, und fügen Sie die Gruppen wieder hinzu. Starten Sie anschließend das Upgrade erneut.

        ```
| ![](images/Cc708486.note(WS.10).gif)Hinweis                          |
|---------------------------------------------------------------------------------------------------|
| Ersetzen Sie &lt;Inhalt\_Verzeichnis&gt; in der letzten Zeile durch den Pfad zum Inhaltsspeicher. |

Inhalt der ursprünglichen WSUS-Infodatei
----------------------------------------

Im Folgenden wird der Inhalt der ursprünglichen WSUS-Infodatei aufgeführt. WSUS mit SP1 bietet *keine* Lösungen für die nachstehenden Probleme. Der Inhalt dieser Datei wird hier nur der Vollständigkeit halber wiedergegeben.

Vor Beginn
----------

#### Problem 1: IIS muss installiert sein

Für Microsoft® Windows Server™ Update Services (WSUS) müssen die Internetinformationsdienste (IIS) installiert sein. Bei Microsoft Windows Server 2003 und Microsoft Windows® 2000 Server wird IIS jedoch nicht standardmäßig installiert, so dass das Setupprogramm für Windows Server Update Services ggf. anhält und stattdessen eine Fehlermeldung angezeigt wird, dass IIS nicht installiert ist.

So installieren Sie IIS:

1.  Öffnen Sie die Systemsteuerung.
2.  Klicken Sie auf **Software**.
3.  Klicken Sie auf **Windows-Komponenten hinzufügen/entfernen**.
4.  Klicken Sie in der Liste **Komponenten** auf **Anwendungsserver**.
5.  Klicken Sie auf **Details**.
6.  Aktivieren Sie das Kontrollkästchen **ASP.NET**. Aktivieren Sie die Option **COM+-Netzwerkzugriff aktivieren**. Die Internetinformationsdienste (IIS) werden automatisch aktiviert.
7.  Wählen Sie **Internet Information Services (IIS)**, und klicken Sie auf **Details**. Die Liste der optionalen IIS-Komponenten wird angezeigt.
8.  Markieren Sie alle optionalen Komponenten, die installiert werden sollen. Die optionale Komponente „WWW-Dienste“ enthält wichtige Unterkomponenten, beispielsweise Active Server Pages oder die Remoteverwaltung (HTML). Um diese Unterkomponenten abzurufen und auszuwählen, klicken Sie auf „WWW-Dienste“ und dann auf „Details“. Klicken Sie wiederholt auf „OK“, bis Sie wieder zum Assistenten für Windows-Komponenten gelangen.
9.  Klicken Sie auf **Weiter**, und arbeiten Sie den Assistenten für Windows-Komponenten weiter durch.
10. Führen Sie im Anschluss an die IIS-Installation das Setup für die Windows Server Update Services durch.

#### Problem 2: Bei Servern mit Windows 2000 Server muss mindestens eine Website in IIS vorliegen, bevor WSUS installiert werden kann

Das Setupprogramm für Windows Server Update Services kann unter Umständen keine Websites erstellen, wenn beim Ausführen des Setupprogramms keine Websites in IIS vorhanden waren. Dieses Problem kann beispielsweise eintreten, wenn Sie eine Website mit SUS 1.0 (Software Update Services) als einzige Website in IIS geführt hatten und diese Website vor Beginn der Installation von WSUS gelöscht wurde.

In diesem Fall erstellen Sie eine neue Website mit dem IIS-Manager-Snap-In (Internetinformationsdienste). Anschließend können Sie diese Website auswählen oder eine neue Website mit dem WSUS-Setupprogramm angeben.

Falls Sie bereits die Installation von WSUS gestartet haben und ein Fehler beim Setupprogramm aufgetreten ist, weil keine Websites vorhanden waren, starten Sie das IIS-Manager-Snap-In, und löschen Sie die Website „Website \#1“. Führen Sie anschließend die oben genannten Schritte aus, und starten Sie das Setupprogramm erneut.

#### Problem 3: Installieren erforderlicher Komponenten

#### Softwareanforderungen

In der nachstehenden Tabelle wird die erforderliche Software für die verschiedenen unterstützten Betriebssysteme aufgeführt. Überprüfen Sie, ob der WSUS-Server diese Anforderungen erfüllt, bevor Sie das WSUS-Setupprogramm starten. Falls der Computer bei einem Update neu gestartet werden muss, sobald die Installation abgeschlossen ist, führen Sie diesen Neustart durch, bevor Sie WSUS installieren.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Betriebssystem</th>
<th>Anforderungen</th>
<th>Downloads</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Alle Betriebssysteme</p></td>
<td style="border:1px solid black;"><p>Microsoft Internet Information Services (IIS) 5.0</p></td>
<td style="border:1px solid black;"><p>Führen Sie die Installation über das Betriebssystem durch.</p>
<p>Siehe Problem 1: IIS muss installiert sein.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Alle Betriebssysteme</p></td>
<td style="border:1px solid black;"><p>Intelligenter Hintergrundübertragungsdienst (BITS) 2.0</p></td>
<td style="border:1px solid black;"><p>Bei Betriebssystemen der Windows Server 2003-Produktfamilie beachten Sie den Artikel zum Update für den Intelligenten Hintergrundübertragungsdienst (BITS) 2.0 und WinHTTP 5.1 unter Windows Server 2003 (KB842773) im Download Center (<a href="http://go.microsoft.com/fwlink/?linkid=47251">http://go.microsoft.com/fwlink/?LinkId=47251</a>).</p>
<p>Bei Betriebssystemen der Windows Server 2000-Produktfamilie beachten Sie den Artikel zum Update für den Intelligenten Hintergrundübertragungsdienst (BITS) 2.0 und WinHTTP 5.1 unter Windows 2000 (KB842773) im Download Center (<a href="http://go.microsoft.com/fwlink/?linkid=46794">http://go.microsoft.com/fwlink/?LinkId=46794</a>).</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows Server 2003</p></td>
<td style="border:1px solid black;"><p>Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47358">Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003</a></p>
<p>Alternativ besuchen Sie die <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update-Website</a>, und suchen Sie nach wichtigen Updates und Service Packs. Installieren Sie dann Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows Server 2003</p></td>
<td style="border:1px solid black;"><p>Datenbanksoftware, die vollständig mit Microsoft SQL kompatibel ist</p></td>
<td style="border:1px solid black;"><p>Nicht zutreffend</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Datenbanksoftware, die vollständig mit Microsoft SQL kompatibel ist</p></td>
<td style="border:1px solid black;"><p>Falls Sie nicht Microsoft SQL Server 2000 verwenden, können Sie Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) installieren. Hierzu sind mehrere Schritte notwendig. Weitere Informationen finden Sie weiter unten unter „Installieren von MSDE unter Windows 2000“.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Microsoft Internet Explorer 6.0 Service Pack 1</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47359">Internet Explorer 6 Service Pack 1</a></p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Microsoft .NET Framework 1.1 Redistributable Package</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47369">Microsoft .NET Framework 1.1 Redistributable Package</a></p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows 2000 Server</p></td>
<td style="border:1px solid black;"><p>Microsoft .NET Framework 1.1 Service Pack 1</p></td>
<td style="border:1px solid black;"><p><a href="http://go.microsoft.com/fwlink/?linkid=47368">Microsoft .NET Framework 1.1 Service Pack 1</a></p>
<p>Alternativ besuchen Sie die <a href="http://go.microsoft.com/fwlink/?linkid=47370">Windows Update-Website</a>, und suchen Sie nach wichtigen Updates und Service Packs. Installieren Sie dann Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2000.</p></td>
</tr>
</tbody>
</table>
<p> </p>

Neben diesen Anforderungen wird ggf. ASP.NET 1.1 durch WSUS auf dem Server installiert oder konfiguriert. (Mit dem WSUS-Setupprogramm wird ASP.NET konfiguriert.)

#### Installieren von MSDE 2000 unter Windows 2000

Wenn Sie Windows 2000 für WSUS verwenden und keinen Zugriff auf Microsoft SQL Server 2000 besitzen, installieren Sie Microsoft SQL Server 2000 Desktop Engine (MSDE), bevor Sie das WSUS-Setupprogramm starten. Ist MSDE bereits auf dem WSUS-Server installiert, muss keine eigene MSDE-Instanz für WSUS eingerichtet werden. In diesem Fall geben Sie einfach den Namen der vorhandenen Instanz während der WSUS-Installation an.

Bei der Installation von MSDE unter Windows 2000 Server fallen vier Schritte an. Als Erstes laden Sie das MSDE-Archiv in einen Ordner auf dem WSUS-Server herunter, und entpacken Sie das Archiv. Starten Sie dann das MSDE-Setupprogramm über eine Eingabeaufforderung und mit den entsprechenden Befehlszeilenoptionen, legen Sie das Systemadministratorkennwort fest, und weisen Sie WSUS als Instanzname zu. Sobald die MSDE-Installation abgeschlossen ist, überprüfen Sie, ob die WSUS-Instanz als NT-Dienst ausgeführt wird. Abschließend installieren Sie einen Sicherheitspatch für MSDE, mit dem der WSUS-Server geschützt wird.

#### Schritt 1: Herunterladen und Entpacken des MSDE-Archivs

Laden Sie das MSDE-Archiv in einen Ordner auf dem WSUS-Server herunter, und entpacken Sie das Archiv. Siehe [Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Release A](http://go.microsoft.com/fwlink/?linkid=47366).

#### Schritt 2: Installieren von MSDE

Starten Sie das MSDE-Setupprogramm über eine Eingabeaufforderung und mit den entsprechenden Befehlszeilenoptionen, legen Sie das Systemadministratorkennwort fest, und weisen Sie WSUS als Instanzname zu. Sobald die MSDE-Installation abgeschlossen ist, überprüfen Sie, ob die WSUS-Instanz als NT-Dienst ausgeführt wird.

So können Sie MSDE installieren, das Systemadministratorkennwort festlegen und einen Instanznamen zuweisen:

1.  Wechseln Sie an der Eingabeaufforderung zum MSDE-Installationsordner aus „Schritt 1: Herunterladen und Entpacken des MSDE-Archivs“.
2.  Geben Sie Folgendes ein: **setup sapwd="***Kennwort***" instancename=WSUS**
    *Kennwort* bezeichnet hierbei ein sicheres Kennwort für das Systemadministratorkonto dieser MSDE-Instanz, **instancename** ist der Name der Datenbankinstanz. Alternativ können Sie den Standard-Instanznamen (anstelle von „WSUS“) für die WSUS-Datenbank verwenden. In diesem Fall kann die Angabe **instancename=WSUS** im Befehlszeilenparameter entfallen. Mit diesem Befehl wird das MSDE-Setupprogramm gestartet, das Systemadministratorkennwort festgelegt und dieser MSDE-Instanz der angegebene Wert als Name zugewiesen.

#### Schritt 3: Überprüfen der Installation der WSUS-Instanz von MSDE

1.  Klicken Sie auf **Start** und dann auf **Ausführen**.
2.  Geben Sie in das Feld **Öffnen** den Dateinamen **services.msc** ein, und klicken Sie auf **OK**.

Blättern Sie durch die Liste der Dienste, und überprüfen Sie, ob der Dienst mit der Bezeichnung „MSSQL$WSUS“ („WSUS“ als Instanzname) bzw. „MSSQLSERVER“ (Standard-Instanzname) vorhanden ist.

#### Schritt 4: Starten der MSDE-Instanz

Zum Abschluss der MSDE-Installation muss die Instanz gestartet werden. Falls Sie den Instanznamen „WSUS“ verwendet haben, starten Sie entsprechend „MSSQL$WSUS“. Beim Standard-Instanznamen starten Sie „MSSQLSERVER“. Wird dieser Dienst nicht gestartet, ist WSUS nicht in der Lage, auf die Datenbankinstanz zuzugreifen.

#### Schritt 5: Aktualisieren von MSDE

Laden Sie den Sicherheitspatch herunter, der im Bulletin [MS03-031: Kumulativer Sicherheitspatch für SQL Server](http://go.microsoft.com/fwlink/?linkid=47364) beschrieben ist, und installieren Sie den Patch.

Weitere Informationen zum Herunterladen des Sicherheitspatches finden Sie unter [SQL Server 2000 (32-Bit) – Sicherheitspatch MS03-031](http://go.microsoft.com/fwlink/?linkid=47363).

#### Problem 4: Mindestanforderungen an den Speicherplatz

Für die Installation der Windows Server Update Services gelten die folgenden Mindestanforderungen an den Speicherplatz:

-   1 Gigabyte (GB) auf der Systempartition
-   2 GB im Volume, in dem die Datenbankdateien gespeichert werden
-   6 GB, je nach prognostiziertem Umfang der Inhalte

#### Problem 5: Frühere Versionen von WSUS müssen über „Software“ deinstalliert werden, bevor die neueste Version installiert werden kann

Falls die Windows Server Update Services auf einem Server installiert werden sollen, auf dem bereits Windows Update Services Beta 1 oder Beta 2 installiert ist, muss diese frühere Version zunächst über das Dienstprogramm „Software“ in der Systemsteuerung deinstalliert werden.

#### Problem 6: Für WSUS muss die Option für geschachtelte Trigger in SQL Server aktiviert sein

Diese Option ist standardmäßig aktiviert, kann jedoch durch einen SQL Server-Administrator deaktiviert werden.

Wenn Sie eine SQL Server-Datenbank als Datenspeicher für Windows Server Update Services einplanen, sollte der SQL Server-Administrator sicherstellen, dass die Option für geschachtelte Trigger auf dem Server aktiviert ist, bevor der WSUS-Administrator die WSUS-Installation startet und die Datenbank im Setupprogramm angibt.

Das WSUS-Setupprogramm aktiviert die datenbankspezifische Option RECURSIVE\_TRIGGERS; die (serverweite) Option für geschachtelte Trigger wird jedoch nicht aktiviert.

Mit diesem Befehl überprüfen Sie, ob geschachtelte Trigger aktiviert sind:

**sp\_configure 'nested triggers'**

Um die Option für geschachtelte Trigger in SQL Server zu aktivieren, führen Sie den folgenden Code in einer Batchdatei auf dem Computer aus, auf dem SQL Server vorliegt:

**sp\_configure 'nested triggers', 1**

**GO**

**RECONFIGURE**

**GO**

#### Problem 7: Befehlszeilenparameter für das WSUS-Setupprogramm

Es ist möglich, unbeaufsichtigte Installationen von WSUS durchzuführen. Weitere Informationen sowie Angaben zu den verfügbaren Befehlszeilenparametern finden Sie in Anhang A über die unbeaufsichtigte Installation im Artikel zur [Bereitstellung von Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (möglicherweise in englischer Sprache).

Bekannte Probleme
-----------------

#### Problem 1: IIS-Lockdown-Assistent

Wenn Sie die Internetinformationsdienste (IIS) auf einem Computer mit Windows 2000 Server ausführen, installieren Sie die neueste Version des IIS-Lockdown-Assistenten (mit URLScan) von der Webseite über IIS-Lockdowntools in Microsoft TechNet. Die Installation dieses Tools wird dringend empfohlen, damit die Sicherheit der IIS-Server gewährleistet ist. Der IIS-Lockdown-Assistent deaktiviert die nicht benötigten IIS-Features und vermindert so das Sicherheitsrisiko.

| ![](images/Cc708486.note(WS.10).gif)Hinweis                                                                                                                                                                                     |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Diese Komponenten werden nicht über das WSUS-Setupprogramm installiert, sondern müssen manuell installiert werden. Bei Computern mit Windows Server 2003 ist die IIS-Lockdown-Funktion bereits integriert und muss daher nicht gesondert installiert werden. |

#### Problem 2: Direkte Änderungen der WSUS-Konfiguration in der Datenbank werden nicht unterstützt

Windows Server Update Services speichert die Konfigurationsdaten in einer Datenbank (MSDE oder SQL Server). Eine Änderung dieser Konfigurationsdaten per direktem Zugriff auf die Datenbank wird nicht unterstützt. Die Administratoren sollten die WSUS-Konfiguration nicht auf diese Weise ändern. Die WSUS-Konfiguration kann über die WSUS-Konsole oder durch Aufrufen der entsprechenden WSUS-APIs geändert werden.

#### Problem 3: Für den Zugriff auf die WSUS-Verwaltungswebsite muss Active Scripting aktiviert sein

Auf der Arbeitsstation des Administrators muss Internet Explorer so konfiguriert werden, dass Active Scripting zugelassen wird, damit Sie über Internet Explorer auf die WSUS-Verwaltungswebsite zugreifen können.

#### Problem 4: IIS wird beim WSUS-Setupprogramm neu gestartet

Das Setupprogramm von Windows Server Update Services startet IIS ohne weitere Benachrichtigung neu. Dies kann sich auf vorhandene Websites im Unternehmen auswirken.

#### Problem 5: Ändern des Zugriffs auf virtuelle Verzeichnisse der WSUS- oder SMS-Verwaltungspunkte (MP)

Standardmäßig ist das virtuelle Verzeichnis der Inhalte für Windows Server Update Services für den anonymen Zugriff eingerichtet. Wenn Sie diese Einstellung so ändern, dass eine Authentifizierung erforderlich ist, erhalten die Clients nur Authentifizierungsfehler, und der Zugriff wird verweigert, so dass die Clients keine Updates herunterladen können. Dies ist ein bekanntes Problem. „Winhttp.dll“ greift bei der implizierten Authentifizierung auf den falschen Authentifizierungskontext zurück, wodurch die Authentifizierung fehlschlägt. Um dieses Problem zu vermeiden, richten Sie den WSUS-Server und die SMS-MPs für den anonymen Zugriff auf virtuelle IIS-Verzeichnisse ein.

#### Problem 6: Bei der Installation von WSUS unter Windows Small Business Server 2003 müssen die Einstellungen für den Zugriff auf das virtuelle WSUS-Stammverzeichnis der Standard-Website so geändert werden, dass die WSUS-Clients selbst die notwendigen Aktualisierungen über den Server ausführen können

Der WSUS-Server installiert zwei virtuelle Stammverzeichnisse („SelfUpdate“ und „ClientWebService“) sowie einige Dateien im Stammverzeichnis der Standard-Website (an Port 80). Auf diese Weise sind die Clients in der Lage, selbst die notwendigen Aktualisierungen über die Standard-Website vorzunehmen. Bei Windows Small Business Server 2003 ist die Standard-Website standardmäßig so konfiguriert, dass der Zugriff für alle IP-Adressen und alle lokalen Hosts (localhost) verweigert wird, mit Ausnahme der IP-Adressen und der lokalen Hosts (localhost) des Servers. Damit wird der Zugriff auf die virtuellen Stammverzeichnisse „SelfUpdate“ und „ClientWebService“ verweigert, so dass die Clients die Aktualisierungen nicht selbst starten können. Um den Clients den Zugriff zu gewähren und ihnen damit die Möglichkeit zu geben, die Aktualisierungen selbst zu starten, führen Sie die nachstehenden Schritte für die virtuellen Stammverzeichnisse „SelfUpdate“ und „ClientWebService“ der Standard-Website durch.

1.  Klicken Sie im virtuellen Stammverzeichnis auf **Eigenschaften**, klicken Sie auf **Verzeichnissicherheit**, dann auf **Beschränkungen für IP-Adressen und Domänennamen** und schließlich auf **Bearbeiten**.
2.  Aktivieren Sie die Option **Zugriff gewährt**, und klicken Sie auf **OK**. Schließen Sie alle Eigenschaftsseiten.

#### Problem 7: Installation von WSUS unter Small Business Server: Probleme mit der Integration

-   Wenn Windows Small Business Server 2003 über einen ISA-Proxyserver auf das Internet zugreift, müssen die folgenden Angaben manuell in die Benutzeroberfläche **Einstellungen** eingetragen werden: Proxyservereinstellungen, Proxyservername, Port.
-   Greift ISA auf die Windows-Authentifizierung zurück, sind die Anmeldeinformationen für den Proxyserver im Format „DOMAIN\\user“ anzugeben. (Der Benutzer muss dabei zur Gruppe der Internetbenutzer gehören.)

#### Problem 8: Bei der Verlagerung eines Computers in eine andere Computergruppe wird dieser Computer an der Verwaltungskonsole ggf. bis zu eine Stunde später in der neuen Gruppe aufgeführt

Wenn Sie einen Computer erstmalig einer Zielgruppe zuweisen, werden die Daten auf dem Computer gemäß den Gruppeninformationen angepasst. Die Daten werden in regelmäßigen Abständen (stündlich) aktualisiert. Wird ein Computer in eine andere Computergruppe verlagert, kann es daher bis zu einer Stunde dauern, bis diese Daten auf dem Client aktualisiert und mit den entsprechenden Änderungen auf der WSUS-Verwaltungskonsole angezeigt werden.

#### Problem 9: Ist WSUS auf einem Mitgliedsserver installiert, der zum Domänencontroller hochgestuft werden soll, muss WSUS erst deinstalliert werden

Wenn Sie WSUS auf einem Mitgliedsserver installieren und dann den Mitgliedsserver zum Domänencontroller hochstufen möchten, fallen die folgenden Schritte an:

1.  Deinstallieren Sie WSUS.
2.  Stufen Sie den Server zum Domänencontroller hoch.
3.  Installieren Sie WSUS neu.

#### Problem 10: Soll ein WSUS-Server von einem Domänencontroller zu einem Mitgliedsserver herabgestuft werden, muss WSUS erst deinstalliert werden

Wenn Sie WSUS-Server auf einem Domänencontroller ausführen und dann den Domänencontrolle zu einem Mitgliedsserver herabstufen möchten, fallen die folgenden Schritte an:

1.  Deinstallieren Sie WSUS, und behalten Sie die Datenbank bei.
2.  Legen Sie das Benutzerkonto ASPNET an.
3.  Geben Sie an der Eingabeaufforderung Folgendes ein: **aspnet\_regiis -i**.
4.  Deinstallieren Sie WSUS, und verwenden Sie die beibehaltene Datenbank.

#### Problem 11: Bei der Installation von .NET Framework 1.0 oder 2.0 nach WSUS wird die WSUS-Verwaltungskonsole nicht angezeigt

Der Grund hierfür liegt darin, dass .NET Framework 1.0 in IIS registriert wird, wobei .NET Framework 1.1 für den WSUS-Server erforderlich ist. Zur Behebung dieses Problems öffnen Sie „aspnet\_regiis.exe“, und führen Sie die nachstehenden Befehle aus. *Website\_ID* bezeichnet dabei den Wert in den folgenden Registrierungsschlüsseln:

HKLM\\Software\\Microsoft\\WindowsUpdateServices\\Server\\Setup\\IISTargetWebsiteIndex

-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\ReportingWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\ClientWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\SimpleAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\WSUSAdmin
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\AdministrationWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\ServrSyncWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\DssAuthWebService
-   %windir%\\Microsoft.NET\\Framework\\v1.1.4322\\\\aspnet\_regiis.exe -s W3SVC\\&lt;*Website\_ID*&gt;\\ROOT\\Content

#### Problem 12: Einschränkungen bei Remote-SQL

WSUS bietet eine eingeschränkte Unterstützung für die separate Ausführung von Datenbanksoftware auf einem anderen Computer (also nicht auf dem Computer, auf dem sich die restlichen Bestandteile der WSUS-Anwendung befinden).

-   Windows 2000 Server kann nicht als Front-End-Computer in einem SQL-Remotepaar eingesetzt werden.
-   Es ist nicht möglich, einen als Domänencontroller konfigurierten Server als Front-End oder Back-End des SQL-Remotepaars zu verwenden.
-   Auf dem Back-End-Computer können Sie nicht WMSDE oder MSDE als Datenbanksoftware nutzen.
-   Die Einrichtung eines SQL-Remoteservers (der als WSUS-Datenbank verwendet werden soll) schlägt fehl, wenn die Terminaldienste auf dem Remoteserver installiert sind und im Anwendungsmodus ausgeführt werden. Bei der Installation von SQL Server auf einem Server mit Terminaldiensten gehen Sie wie folgt vor:
    1.  Bevor Sie das Setupprogramm starten, öffnen Sie eine Eingabeaufforderung, und geben Sie Folgendes ein: „change user /install“
    2.  Führen Sie das SQL Server-Setupprogramm aus.
    3.  Geben Sie im Anschluss an die Einrichtung Folgendes an der Eingabeaufforderung ein: „change user /execute“
-   Um die WSUS-Datenbank auf dem SQL-Remoteserver einrichten zu können, müssen Sie sowohl auf dem Front-End-Computer als auch auf dem Back-End-Computer zur lokalen Sicherheitsgruppe der Administratoren gehören.
-   Weitere Informationen zu Problemen mit Remote-SQL finden Sie in Anhang C über Remote SQL im Artikel zur [Bereitstellung von Microsoft Windows Server Update Services](http://go.microsoft.com/fwlink/?linkid=41777) (möglicherweise in englischer Sprache).

#### Problem 13: Ein Downstream-Replikatserver besitzt weniger Genehmigungen als der übergeordnete Upstreamserver

Ein Downstream-Replikatserver besitzt unter Umständen weniger Genehmigungen als der übergeordnete Upstreamserver. Der Grund hierfür liegt darin, dass Installationsgenehmigungen erst dann an einen Downstreamserver weitergegeben werden, wenn der Download des Inhalts auf dem Upstreamserver beendet ist.

#### Problem 14: Wiederholung der Synchronisierung nach einem Fehler bei der ersten Synchronisierung

Wenn ein Fehler bei der Synchronisierung auftritt, sollten Sie als Erstes versuchen, den Server erneut zu synchronisieren. Falls auch nachfolgende Synchronisierungsvorgänge fehlschlagen, beachten Sie die Informationen zur Problembehandlung im WSUS Operations Guide.

#### Problem 15: Beim Zugriff auf die WSUS-Verwaltungskonsole wird eine Fehlermeldung vom Typ „System.IO.FileNotFoundException“ angezeigt

Wenn Sie die folgende Fehlermeldung erhalten, müssen ggf. die Berechtigungen für das Netzwerkdienst- oder ASP.NET-Konto angepasst werden:

System.IO.FileNotFoundException: Datei- oder Assemblyname *xxxxxx*.dll oder eine Abhängigkeit davon wurde nicht gefunden

*xxxx* bezeichnet hierbei einen beliebigen Dateinamen.

Um dieses Problem in Betriebssystemen der Windows Server 2003-Produktfamilie zu beheben, gewähren Sie dem Netzwerkdienstkonto den Schreib-/Lesezugriff auf „%systemroot%\\Temp“. Bei Windows 2000 Server gewähren Sie entsprechend dem ASP.NET-Konto den Schreib-/Lesezugriff auf „%systemroot%\\Temp“.

#### Problem 16: SQL-Sicherheitsupdate MS03-031 (KB815495)

Unter Umständen wird dieses Update beim WSUS-Server auch dann als installiert angezeigt, wenn die Installation auf dem Client fehlgeschlagen ist. Das Paket wird dem Client daher ggf. erneut angeboten. Um dieses Problem zu umgehen, können Sie die Genehmigung für das Update auf dem Server wieder aufheben.

#### Problem 17: IIS-Einstellungen gehen beim RTM-Upgrade verloren

Wenn Sie WSUS RTM auf einem Server ausführen, auf dem sich eine frühere Version von WSUS befindet (beispielsweise RC), wird diese frühere Version durch WSUS RTM deinstalliert, wobei anschließend die neue Version installiert wird. Dies bedeutet, dass alle virtuellen Stammverzeichnisse und alle Dateien gelöscht werden, die mit WSUS in IIS verknüpft sind.

Wurde WSUS auf der Standard-Website installiert, gehen alle WSUS-spezifischen Einstellungen verloren, die Sie an den virtuellen WSUS-Stammverzeichnissen vorgenommen haben. Wenn Sie beispielsweise die virtuellen WSUS-Stammverzeichnisse für SSL so konfiguriert haben, dass WSUS abgesichert wird, müssen diese Stammverzeichnisse nach der Installation der RTM-Version von WSUS neu konfiguriert werden. Hinweis: An der WSUS-Konsole wird eine Benachrichtigung angezeigt, dass SSL nicht aktiviert ist.

Wenn Sie WSUS auf einer anderen Website installiert haben (also nicht auf der Standard-Website), gehen alle zusätzlichen Einstellungen auf der WSUS-Website verloren.

#### Problem 18: Verwenden von Hostheadern

Wenn der Standard-Website (WSUS-Website) in IIS bestimmte Hostheaderwerte zugewiesen werden sollen, nehmen Sie den Eintrag „Keine zugewiesen“ bzw. eine zugewiesene IP-Adresse in die Liste der IP-Adressen ohne Hostheaderwert auf der Standard-Website auf. Dieser Eintrag sollte auch auf der anderen Website ergänzt werden.

**Warnung**: Dieser Vorgang führt unter Umständen dazu, dass Microsoft SharePoint und Exchange nicht mehr funktionsfähig sind.

#### Problem 19: Die URL der WSUS-Konsole muss auf Computern, auf denen eine stärkere Absicherung von Internet Explorer aktiviert ist, in die Webinhaltszonen „Vertrauenswürdige Sites“ und „Lokales Intranet“ aufgenommen werden

Wenn die stärkere Absicherung von Internet Explorer (die Komponente „Verstärkte Sicherheitskonfiguration für Internet Explorer“ in Microsoft Windows Server 2003) auf einem Computer aktiviert ist und Sie die WSUS-Konsole nicht in Webinhaltszonen „Vertrauenswürdige Sites“ und „Lokales Intranet“ eintragen, werden Sie bei jedem Öffnen einer Seite in der WSUS-Konsole aufgefordert, Ihre Anmeldeinformationen einzugeben.

So nehmen Sie die WSUS-Konsole in die Webinhaltszonen **Lokales Intranet** und **Vertrauenswürdige Sites** auf:

1.  Öffnen Sie **Internetoptionen**. (Klicken Sie hierzu beispielsweise auf **Start**, zeigen Sie auf **Systemsteuerung**, und klicken Sie dort auf **Internetoptionen**).
2.  Klicken Sie auf der Registerkarte **Sicherheit** auf **Lokales Intranet**, dann auf **Sites** und auf **Erweitert**. Geben Sie die URL ein (http://*WSUSServername*/WSUSAdmin), und klicken Sie auf **OK**.
3.  Klicken Sie auf **Vertrauenswürdige Sites** und dann auf **Sites**. Geben Sie die URL der WSUS-Konsole ein. Klicken Sie auf **OK** und dann zum Schließen von **Internetoptionen** erneut auf **OK**.

#### Copyright

Die in diesem Dokument enthaltenen Angaben entsprechen dem Wissensstand der Microsoft Corporation zu den beschriebenen Problemen zum Zeitpunkt der Veröffentlichung. Microsoft muss auf veränderte Marktbedingungen reagieren und ist daher weder in der Lage noch dazu verpflichtet, die Richtigkeit der dargelegten Informationen über das Datum der Veröffentlichung hinaus zu garantieren.

Dieses Dokument dient lediglich zu Informationszwecken. MICROSOFT ÜBERNIMMT KEINE AUSDRÜCKLICHE, KONKLUDENTE ODER GESETZLICHE GEWÄHRLEISTUNG FÜR DIE INFORMATIONEN IN DIESEM DOKUMENT.

Die Benutzer sind verpflichtet, sich an alle geltenden Urheberrechtsgesetze zu halten. Unabhängig von der Anwendbarkeit der geltenden Urheberrechtsgesetze darf ohne ausdrückliche schriftliche Genehmigung der Microsoft Corporation kein Teil dieses Dokuments für beliebige Zwecke vervielfältigt, in einem Datenempfangssystem gespeichert oder darin eingelesen werden oder übertragen werden, unabhängig davon, auf welche Art und Weise oder mit welchen Mitteln (elektronisch, mechanisch, durch Fotokopieren, Aufzeichnen usw.) dies geschieht.

Es ist möglich, dass Microsoft Patente bzw. angemeldete Patenten, Marken, Urheberrechte oder sonstige geistige Eigentumsrechte besitzt, die sich auf den fachlichen Inhalt dieses Dokuments beziehen. Das Bereitstellen dieses Dokuments gibt Ihnen jedoch keinen Anspruch auf diese Patente, Marken, Urheberrechte oder auf sonstiges geistiges Eigentum, es sei denn, dies wird ausdrücklich in schriftlichen Lizenzverträgen von Microsoft eingeräumt.

Die in den Beispielen verwendeten Firmen, Organisationen, Produkte, Domänennamen, E-Mail-Adressen, Logos, Personen, Orte und Ereignisse sind frei erfunden, soweit nichts anderes angegeben ist. Jede Ähnlichkeit mit bestehenden Firmen, Organisationen, Produkten, Domänennamen, E-Mail-Adressen, Logos, Personen, Orten oder Ereignissen ist rein zufällig.

© 2006 Microsoft Corporation. Alle Rechte vorbehalten.

Microsoft, SQL Server, Windows und Windows Server sind Marken oder eingetragene Marken der Microsoft Corporation in den USA und/oder in anderen Ländern.

Andere in diesem Dokument aufgeführte Produkt- und Firmennamen sind möglicherweise Marken der jeweiligen Eigentümer.
