---
TOCTitle: 'Anmerkungen zu dieser Version von Windows Rights Management Services (Dienste für die Windows-Rechteverwaltung oder RMS) Service Pack 2'
Title: 'Anmerkungen zu dieser Version von Windows Rights Management Services (Dienste für die Windows-Rechteverwaltung oder RMS) Service Pack 2'
ms:assetid: '78067886-681f-49a6-b43d-bfd08a369b69'
ms:contentKeyID: 18118901
ms:mtpsurl: 'https://msdn.microsoft.com/de-de/library/Cc747637(v=WS.10)'
---

Anmerkungen zu dieser Version von Windows Rights Management Services (Dienste für die Windows-Rechteverwaltung oder RMS) Service Pack 2
=======================================================================================================================================

*Release-Datum: Dezember 2006*

Vor Beginn
----------

Lesen Sie die folgenden Informationen, bevor Sie Microsoft® Windows®-Rechteverwaltungsdienst (Rights Management Services, RMS) Service Pack 2 (SP2) installieren. Die Informationen in diesen Anmerkungen gelten für die Serverkomponente von RMS mit SP2, nicht für den RMS-Client. Informationen zu RMS-Clients finden Sie im Thema zum Rechteverwaltungsdienst ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) (möglicherweise in englischer Sprache).

#### Systemanforderungen

Die Hardwareanforderungen für RMS SP2 werden in der folgenden Tabelle aufgeführt.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Anforderung</th>
<th style="border:1px solid black;" >Empfehlung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PC mit einem Pentium III-Prozessor (800 MHz oder höher)</td>
<td style="border:1px solid black;">PC mit zwei Pentium 4-Prozessoren (1500 MHz oder höher)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">256 MB Arbeitsspeicher</td>
<td style="border:1px solid black;">512 MB Arbeitsspeicher</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">20 GB freier Festplattenspeicher</td>
<td style="border:1px solid black;">40 GB freier Festplattenspeicher</td>
</tr>
</tbody>
</table>
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                   |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Die Serverkomponente von RMS mit SP2 wurde für 32-Bit-Computer entwickelt. Wenn sie auf einem 64-Bit-Computer installiert wird, wird sie im Emulationsmodus ausgeführt. |
  
Die Softwareanforderungen für die Serverkomponente von RMS SP2 werden in der folgenden Tabelle aufgeführt.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Komponente</th>
<th style="border:1px solid black;" >Anforderung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Betriebssystem</td>
<td style="border:1px solid black;">Microsoft Windows Server® 2003, mit Ausnahme der Web Edition, für RMS mit SP2</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS mit SP2</td>
<td style="border:1px solid black;">Vor dem Upgrade auf RMS mit SP2 muss RMS mit Service Pack 1 (SP1) installiert werden. Für den RMS mit SP2-Client gilt diese Voraussetzung nicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Dateisystem</td>
<td style="border:1px solid black;">Das NTFS-Dateisystem wird empfohlen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Vorausgesetzte Komponenten</td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (auch als MSMQ bezeichnet) mit aktivierter Active Directory®-Verzeichnisdienst-Integration<br />
<br />
</li>
<li>Internet Information Services (IIS) mit aktivierter Komponente ASP.NET<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
 

| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                                                             |
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie RMS mit SP2 so konfigurieren, dass eine Remoteverwaltung möglich ist, muss der Computer, der die Verbindung mit dem RMS mit SP2-Verwaltungsdienst herstellt, Internet Explorer 6.0 oder höher verwenden. |

Die Infrastrukturanforderungen für RMS mit SP2-Server werden in der folgenden Tabelle aufgeführt.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Komponente</th>
<th style="border:1px solid black;" >Anforderungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Verzeichnisdienste</td>
<td style="border:1px solid black;">Active Directory muss auf Domänencontrollern ausgeführt werden, auf denen Windows Server 2000 mit SP3 (oder höher) ausgeführt wird; diese Controller müssen sich in derselben Domäne befinden, in der RMS installiert ist. Alle Benutzer und Gruppen, die RMS zum Erwerben von Lizenzen und Veröffentlichen von Inhalt verwenden, müssen über eine in Active Directory konfigurierte E-Mail-Adresse verfügen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Datenbankserver</td>
<td style="border:1px solid black;">RMS mit SP2 erfordert eine Datenbank und gespeicherte Prozeduren zum Ausführen von Operationen. Sie können Microsoft SQL Server™ 2000 mit SP3a oder höher oder Microsoft SQL Server 2005 verwenden. Zum Testen oder für andere Bereitstellungen auf nur einem Computer können Sie Microsoft SQL Server Desktop Engine (MSDE 2000) Version A oder Microsoft SQL Server 2005 Express Edition verwenden.</td>
</tr>
</tbody>
</table>
  
RMS wurde für Datenbankserver unter Microsoft SQL Server 2000 und Microsoft SQL Server 2005 entwickelt und entsprechend getestet. RMS kann auf anderen Datenbankservern ausgeführt werden, wenn diese die folgenden Anforderungen erfüllen:
  
-   Sie unterstützen von Microsoft .NET Framework 1.1 bereitgestellte ADO.NET-Schnittstellen.  
-   Sie sind mit Transact SQL, der strukturierten Abfragesprache von Microsoft SQL Server, kompatibel, da RMS-Initialisierungsskripte und die gespeicherten RMS-Prozeduren Transact-SQL verwenden.  
-   Sie unterstützen alle Microsoft SQL Server-spezifischen Erweiterungen.  
-   Sie reagieren auf Methodenaufrufe des .NET Framework-Namespace „System.Data.SqlClient“.  
-   Sie stellen die entsprechende Funktionalität des Namespace „System.Data.SqlClient“ bereit.  
-   Sie verwenden den Windows-Authentifizierungsmodus.
  
Um herauszufinden, ob der Datenbankserver die oben aufgelisteten Kriterien erfüllt, wenden Sie sich an den entsprechenden Datenbankanbieter.
  
In der folgenden Tabelle werden die zum Ausführen verschiedener Aktivitäten mit RMS erforderlichen Benutzerrechte und Berechtigungen aufgelistet.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Aktivität</th>
<th style="border:1px solid black;" >Kontoanforderungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Installieren von RMS</td>
<td style="border:1px solid black;">Domänenbenutzer mit Anmeldeinformationen für den Administrator des lokalen Computers</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bereitstellen eines RMS-Stammclusters</td>
<td style="border:1px solid black;">Domänenbenutzer mit Anmeldeinformationen für den Administrator des lokalen Computers und Active Directory-Such- und -Schreibrechten</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bereitstellen eines reinen RMS-Lizenzierungsclusters</td>
<td style="border:1px solid black;">Domänenbenutzer mit Anmeldeinformationen für den Administrator des lokalen Computers und Active Directory-Suchrechten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bereitstellen unter Verwendung einer neuen Konfigurationsdatenbank</td>
<td style="border:1px solid black;">Domänenbenutzer mit Anmeldeinformationen für den Administrator des lokalen Computers und Lese-, Schreib- und Erstellungsrechten für einen Computer mit SQL Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bereitstellen unter Verwendung einer bestehenden Konfigurationsdatenbank</td>
<td style="border:1px solid black;">Domänenbenutzer mit Administratorrechten für den lokalen Computer und Lese- und Schreibrechten für einen Computer mit Datenbankserver</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verwalten von RMS</td>
<td style="border:1px solid black;">Domänenbenutzer mit Anmeldeinformationen für den Administrator des lokalen Computers</td>
</tr>
</tbody>
</table>
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                                                                                                                                               |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Weitere Informationen zur Windows-Serverkonfiguration, Active Directory, Message Queuing, IIS und Dateisystemen finden Sie im Windows Server 2003 TechCenter ([http://go.microsoft.com/fwlink/?LinkId=78135](http://go.microsoft.com/fwlink/?linkid=78135)) (möglicherweise in englischer Sprache). |
  
Wenn Sie RMS in einer Bereitstellung mit Clustern verwenden, beachten Sie die Punkte in der nachstehenden Tabelle.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Zustand</th>
<th style="border:1px solid black;" >Empfehlung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Große Zahl von Desktops, die RMS verwenden</td>
<td style="border:1px solid black;">Verwenden Sie zur Installation des RMS mit SP2-Clients Systems Management Server (SMS) oder Gruppenrichtlinien.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Große Zahl von Clientanforderungen</td>
<td style="border:1px solid black;">Verwenden Sie einen Lastenausgleichsserver, den Netzwerklastenausgleichdienst im Windows-Serverbetriebssystem oder Lastenausgleichhardware, um die Anforderungen gleichmäßig auf das Cluster zu verteilen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zwei Netzwerkadapter mit virtueller IP-Adressierung für Extranet- und Intranetanforderungen</td>
<td style="border:1px solid black;">Stellen Sie sicher, dass alle Registrierungen des Domain Name System (DNS), die die virtuelle IP-Adresse im Extranet anzeigen, die Adresse auch im Intranet bereitstellen.</td>
</tr>
</tbody>
</table>
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Wird die DNS-Registrierung im Intranet nicht durchgeführt, schlagen Lizenzanforderungen von internen Clients fehl. Falls Sie die DNS-Einstellungen nicht ändern können, bearbeiten Sie die Hosttabelle für die einzelnen Server im Cluster, und ordnen Sie dort die Cluster-URL der virtuellen IP-Adresse des Clusters zu. Die DNS-Registrierung muss vor der Bereitstellung von RMS vorgenommen werden. Wenn Sie den Dienst schon bereitgestellt haben, muss RMS vom Server entfernt werden. Führen Sie anschließend den Bereitstellungsvorgang erneut durch. |
  
#### Unterstützte Clients für diese Version
  
Der Client für RMS ohne Service Pack, RMS mit SP1 oder RMS mit SP2 kann auf jedem Computer installiert werden, auf dem Microsoft Windows 2000, Windows XP und Windows Server 2003 ausgeführt wird. Frühere Versionen der Windows-Betriebssysteme werden nicht unterstützt.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.Caution(WS.10).gif)Vorsicht                                                                                             |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Bei Verwendung des Clients für RMS ohne Service Pack ist der Client nicht in der Lage, Onlineveröffentlichungen auf einem RMS-Server mit SP1 oder später vorzunehmen. |
  
Änderungen an der Funktionalität  
--------------------------------
  
In RMS mit SP2 stehen zahlreiche neue Features zur Verfügung:
  
-   [Verbesserte gesamtstrukturübergreifende Gruppenerweiterung](#bkmk_cif1)  
-   [Änderungen bei der Datenbankprotokollierung](#bkmk_cif2)  
-   [Größere Serverbatches](#bkmk_cif3)  
-   [Kompatibilität mit Microsoft SQL Server 2005](#bkmk_cif4)
  
<span id="BKMK_CIF1"></span>
#### Verbesserte gesamtstrukturübergreifende Gruppenerweiterung
  
#### Was nützt mir dieses Feature?
  
In RMS bietet die gesamtstrukturübergreifende Gruppenerweiterung die Möglichkeit, die Mitgliedschaft in der Active Directory Universal-Gruppe auf eine andere Gesamtstruktur zu erweitern, wobei Gruppenmitgliedschaften nicht repliziert werden. Wenn ein Benutzer in einer Gesamtstruktur durch Rechte geschützten Inhalt an einen Benutzer in einer anderen Gesamtstruktur sendet, durchläuft RMS eine Ermittlungsphase, in der überprüft wird, ob der Benutzer Zugriff auf den Inhalt hat. Dieser Überprüfungsprozess geschieht mithilfe einer LDAP-Abfrage von einer Gesamtstruktur zur nächsten, um nach dem RMS-Dienstverbindungspunkt (Service Connection Point oder SCP) der Remotegesamtstruktur zu suchen. Wenn der SCP für die Remotegesamtstruktur ermittelt wurde, sendet das RMS-Dienstkonto eine Anfrage an die Gruppenerweiterungs-Pipeline. In der Anfrage wird die Remotegesamtstruktur gefragt, ob der Benutzer Mitglied einer Gruppe ist.
  
#### Für wen eignet sich dieses Feature?
  
Dieses neue Feature ist für RMS-Kunden in einer Active Directory-Umgebung mit mehreren Gesamtstrukturen interessant, deren Mitgliedschaft in der Universal-Gruppe nicht zwischen den Gesamtstrukturen repliziert wird.
  
#### Warum ist diese Änderung wichtig?
  
Das neue Vertrauenserweiterungsprotokoll für Gesamtstrukturen verbessert die Verlässlichkeit für Kunden, die eine Active Directory-Umgebung mit mehreren Gesamtstrukturen bereitstellen.
  
#### Was unterscheidet die neue Version von ihren Vorgängern?
  
Vor RMS mit SP2 wurde die Gruppenerweiterung zwischen Gesamtstrukturen über .NET-Remoteaufrufe erreicht. In dieser Version wurde das Protokoll für die gesamtstrukturübergreifende Gruppenerweiterung in einen ASP.NET-Webdienst geändert, der mit SOAP/HTTP-Anfragen für die Pipeline der Gruppenerweiterung für Gesamtstrukturvertrauensstellungen arbeitet.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                     |  
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Damit die Abwärtskompatibilität gewährleistet ist, werden .NET-Remoteaufrufe in RMS mit SP2 weiterhin unterstützt. Um von allen Vorteilen des neuen Protokolls für die Gruppenerweiterung zwischen Gesamtstrukturen zu profitieren, müssen alle RMS-Cluster mindestens mit RMS mit SP2 ausgeführt werden. |
  
#### Welche Einstellungen wurden in RMS mit SP2 hinzugefügt oder geändert?
  
Die neue RMS-Pipeline für die Gruppenerweiterung wird in RMS mit SP2 standardmäßig mit den sichersten Einstellungen konfiguriert, sodass nur die lokalen RMS-Dienst- und Administratorgruppen Zugriff haben. Um einem Konto den Zugriff zu gewähren, müssen Sie die Zugriffssteuerungsliste in der Gruppenerweiterungs-Pipeline unter „wwwroot\\\_wmcs\\GroupExpansion\\GroupExpansion.asmx“ ändern.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                                                                                                                                                                           |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Stellen Sie sicher, dass das RMS-Dienstkonto in jeder Active Directory-Gesamtstruktur Zugriff auf die Gruppenerweiterungs-Pipeline auf jedem RMS-Server im Cluster hat. Wenn die Konten keinen Zugriff haben, schlägt die Gruppenerweiterung fehl. Sie können auch dasselbe Konto in allen Gesamtstrukturen erstellen und allen diesen Konten dasselbe Kennwort zuordnen. In diesem Fall müssten Sie nur das eine Konto der Gruppenerweiterungs-Pipeline hinzufügen. |
  
RMS mit SP2 wurden neue Ereignisse hinzugefügt, um Sie über problematische Nachrichten zu informieren, die nicht in den Message Queuing-Dienst aufgenommen wurden. Diese neuen Ereignisprotokollierungen enthalten Ereignisse, die Sie darüber informieren, wenn eine Nachricht nicht digital signiert oder überprüft werden kann. Dazu gehören beispielsweise fehlerhafte Nachrichten, ein fehlender bzw. falscher Hashwert oder eine fehlende bzw. falsche Signatur.
  
<span id="BKMK_CIF2"></span>
#### Änderungen an Datenbankprotokollierungen
  
#### Was nützt mir dieses Feature?
  
RMS nutzt einen Protokollierungslistenerdienst, der alle RMS-Kommunikation über Message Queuing an die Protokollierungsdatenbank sendet. Der RMS-Cluster sendet Nachrichten an den Message Queuing-Dienst, und der Protokollierungslistenerdienst empfängt diese Nachrichten aus der Message Queuing-Warteschlange und schreibt sie in die Protokollierungsdatenbank.
  
#### Für wen eignet sich dieses Feature?
  
Dieses Feature eignet sich für derzeitige Benutzer von RMS, die den RMS-Protokollierungslistenerdienst verwenden, und neue Benutzer von RMS mit SP2, die darüber nachdenken, den RMS-Protokollierungslistenerdienst zu verwenden.
  
#### Warum ist diese Änderung wichtig?
  
In vorherigen Versionen von RMS wurde die RMS-Protokollierungswarteschlange durch die Verwendung von Zugriffssteuerungslisten geschützt, aber die Authentifizierung war nicht aktiviert. Ohne Authentifizierung konnte ein Angreifer falsche Nachrichten in die RMS-Protokollierungswarteschlange schreiben.
  
#### Was unterscheidet die neue Version von ihren Vorgängern?
  
In RMS SP2 erhalten die Nachrichten, die über das RMS-Cluster versendet werden, durch Message Queuing eine zusätzliche Authentifizierung. Zusätzlich zu den Zugriffssteuerungslisten, die den unautorisierten Zugriff auf die Nachrichtenwarteschlange verhindern, wird die Message Queuing-Warteschlange auch durch einen Mechanismus zur Prüfung der Echtheit von Nachrichten geschützt. Wenn eine Nachricht an den Message Queuing-Dienst gesendet wird, erstellen die RMS-Pipelines einen Hashwert der Nachricht und signieren sie mithilfe des privaten Schlüssels des RMS-Clusters digital. Der Protokollierungslistenerdienst berechnet zuerst seinen eigenen Hashwert der Nachricht und vergleicht ihn mit dem Hashwert, der der Nachricht beigefügt ist. Wenn die Hashwerte übereinstimmen, überprüft der Protokollierungslistenerdienst die Signatur mithilfe des öffentlichen Schlüssels des Clusters und des Hashwerts der Nachricht. Wenn die Hashwerte übereinstimmen und die Signatur überprüft wurde, wird die Nachricht an die Protokollierungsdatenbank gesendet. Wenn die Überprüfungsschritte nicht erfolgreich sind, wird die Nachricht dauerhaft aus der Message Queuing-Warteschlange gelöscht, und in das Anwendungsprotokoll der Ereignisanzeige wird eine Ereigniswarnung geschrieben.
  
#### Welche Einstellungen wurden in RMS mit SP2 hinzugefügt oder geändert?
  
RMS mit SP2 wurden neue Ereignisse hinzugefügt, um Sie über problematische Nachrichten zu informieren, die nicht in den Message Queuing-Dienst aufgenommen wurden. Diese neuen Ereignisse werden in das Anwendungsprotokoll geschrieben und enthalten Nachrichten, die nicht digital signiert werden können bzw. bei denen die digitale Signatur nicht überprüft werden kann. Dazu gehören beispielsweise fehlerhafte Nachrichten, ein fehlender bzw. falscher Hashwert oder eine fehlende bzw. falsche Signatur.
  
<span id="BKMK_CIF3"></span>
#### Größere Serverbatches
  
#### Was nützt mir dieses Feature?
  
Batching in RMS verbessert die Arbeitsgeschwindigkeit, da mehrere Lizenzierungsanfragen als eine einzige Anfrage an den RMS-Cluster gesendet werden können, anstatt für jede Lizenz eine eigene Anfrage zu senden.
  
#### Für wen eignet sich dieses Feature?
  
Die Unterstützung größerer Serverbatches ist für RMS-fähige Anwendungen geeignet, die mehrere Lizenzen für durch Rechte geschützten Inhalt benötigen.
  
#### Warum ist diese Änderung wichtig?
  
Durch RMS-Batching können mit einer einzigen Anfrage an die AcquireLicense-RMS-Pipeline Nutzungslizenzen für mehrere RACs (Rights Accounts Certificate) abgerufen werden, für die es eine oder mehrere Veröffentlichungslizenzen gibt. Ohne eine Batchgröße über 1 müsste die RMS-fähige Anwendung eine Nutzungslizenz für jeden Benutzer einzeln anfordern.
  
#### Was unterscheidet die neue Version von ihren Vorgängern?
  
In RMS-Versionen vor RMS mit SP2 unterstützte der RMS-Cluster eine maximale Batchgröße von 1. Wenn die maximale Größe auf eine Zahl größer als 1 gesetzt wurde, wurde sie vom Cluster ignoriert. Bei Verwendung von RMS mit SP2 kann diese maximale Batchgröße bis 100 betragen.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis |  
|-----------------------------------------------------------------------|  
| Nur die „AcquireLicense“-RMS-Pipeline unterstützt Batchanfragen.      |
  
In RMS mit SP2 wurde die Fehlerberichterstattung erweitert, sodass auch Batchanfragen berücksichtigt werden. Wenn Sie beispielsweise einen Batch mit zehn Anfragen senden und die zweite und dritte Anfrage fehlschlägt, wird für jedes Fehlschlagen ein Ereignis in das Ereignisprotokoll geschrieben.
  
<span id="BKMK_CIF4"></span>
#### Kompatibilität mit Microsoft SQL Server 2005
  
#### Was nützt mir dieses Feature?
  
In RMS mit SP2 kann Microsoft SQL Server 2005 als Datenbankserver verwendet werden, der die RMS-Konfiguration und die Protokollierungsdatenbank unterstützt, ohne dass zusätzliche Konfigurationsschritte erforderlich sind.
  
#### Für wen eignet sich dieses Feature?
  
Die Unterstützung von Microsoft SQL Server 2005 für RMS mit SP2 ist für RMS-Kunden interessant, die Microsoft SQL Server 2005 als RMS-Datenbank nutzen möchten.
  
#### Warum ist diese Änderung wichtig?
  
In älteren Versionen von RMS waren die Datentypen einiger der Parameter, die in der „sysmessages“-Tabelle genutzt werden, nicht mit der Formatspezifikation von Microsoft SQL Server 2005 kompatibel. Weitere Informationen erhalten Sie in Artikel 913372 in der Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)) (möglicherweise in englischer Sprache).
  
#### Was unterscheidet die neue Version von ihren Vorgängern?
  
In RMS-Versionen vor RMS mit SP2 wurden SQL-RAISERROR-Anweisungen verwendet, um den RMS-Benutzer darüber zu informieren, dass ein Fehler aufgetreten ist. Die RAISERROR-Anweisung fragt die „sysmessages“-Tabelle ab, um die dort gespeicherten RMS-Fehlermeldungen zu erhalten. RMS mit SP2 verwendet eine andere Technik, um SQL-Fehler zu übertragen. Es besteht daher keine Abhängigkeit von der „sysmessages“-Tabelle mehr.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                       |  
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Wenn Sie von RMS mit SP1 auf RMS mit SP2 aktualisieren, wird die „sysmessages“-Tabelle nicht mehr nach Fehlermeldungen abgefragt. Die Fehlermeldungen selbst bleiben jedoch in der „sysmessages“-Tabelle gespeichert. Durch eine saubere Installation von RMS SP2 werden der „sysmessages“-Tabelle keine zusätzlichen Einträge hinzugefügt. |
  
Bekannte Probleme  
-----------------
  
In den nachfolgenden Abschnitten werden bekannte Probleme mit dieser vorliegenden Version von RMS besprochen.
  
#### Die Hilfedatei verweist immer noch auf RMS mit Service Pack 1
  
Die Hilfedatei, die in der Installation von RMS mit SP2 enthalten ist, verweist immer noch auf RMS mit SP1. Informationen zu RMS mit SP2 finden Sie im Thema zum Rechteverwaltungsdienst ([http://go.microsoft.com/fwlink/?LinkId=68637](http://go.microsoft.com/fwlink/?linkid=68637)) (möglicherweise in englischer Sprache).
  
#### Windows Update kann den RMS mit SP2-Client nicht auf x64- oder Itanium-basierten Computern installieren
  
Wenn der RMS-Client oder der RMS mit SP1-Client auf einem x64-basierten Computer installiert ist und Sie versuchen, den Client über Windows Update auf RMS mit SP2 (x64) zu aktualisieren, schlägt die Installation fehl. Obwohl die älteren RMS-Clients, die für 32-Bit-Systeme konzipiert wurden, auf x64-basierten Computern funktionieren, können sie nicht auf RMS mit SP2 (x64) aktualisiert werden. Sie müssen den vorherigen RMS-Client zuerst deinstallieren und anschließend die Aktualisierung neu starten. Windows Update ermittelt die Version des Betriebssystems und stellt den entsprechenden RMS mit SP2-Client zur Verfügung. Dies gilt auch für Itanium-basierte Computer.
  
#### Die Neubereitstellung startet nie den Protokollierungslistenerdienst
  
Wenn der Cluster nicht bereitgestellt wird, kann der Protokollierungslistenerdienst den Dienst nicht in einem angehaltenen Status beenden. Um den Dienst vollständig anzuhalten, müssen Sie den Computer neu starten.
  
#### Nicht auf Software basierende vertrauenswürdige Veröffentlichungsdomäne kann nicht entfernt werden
  
Nachdem Sie eine vertrauenswürdige Veröffentlichungsdomäne mit einer nicht auf Software basierenden Implementierung des privaten Schlüssels importiert haben, können Sie sie nicht mehr löschen. Der Import eines nicht auf Software basierenden privaten Schlüssels sollte nicht über die RMS-Verwaltungskonsole geschehen. Wenden Sie sich an den entsprechenden Hardwareanbieter, um Anweisungen dazu zu erhalten, wie der private Schlüssel exportiert und importiert wird.
  
#### Microsoft .NET Framework 2.0 ändert die virtuellen IIS-Stammverzeichnisse, wenn es auf dem RMS-Server installiert wird
  
RMS mit SP2 verwendet die ASP.NET-Skriptzuordnung aus .NET Framework Version 1.1. Die Zuordnung in höheren Versionen ist nicht mit RMS mit SP2 kompatibel. Die beiden Versionen können jedoch parallel verwendet werden, ohne dass andere abhängige Anwendungen beeinträchtigt würden. Ist auf dem Server .NET Framework 1.1 und .NET Framework 2.0 (oder höher) installiert, arbeitet der RMS-Cluster unter Umständen auch dann nicht einwandfrei, wenn RMS mit SP2 scheinbar erfolgreich installiert und bereitgestellt wurde. Der Grund hierfür liegt darin, dass die virtuellen RMS-Stammverzeichnisse bei Version 1.1 der ASP.NET-Skriptzuordnung registriert werden müssen, nicht bei Version 2.0. Um die virtuellen RMS-Stammverzeichnisse mit Version 1.1 der ASP.NET-Skriptzuordnung zu registrieren, geben Sie in einer Eingabeaufforderung den folgenden Befehl ein:
  
**%windir%\\Microsoft.NET\\Framework\\v1.1.4322&gt;aspnet\_regiis.exe -s W3SVC/1/ROOT/\_wmcs**
  
Durch diesen Befehl werden die virtuellen RMS-Stammverzeichnisse ordnungsgemäß registriert, sodass RMS mit SP2 auf dem Server ausgeführt werden kann.
  
#### Bei der Verwendung der systemeigenen Funktionsebene von Active Directory Windows 2000 kann die Gruppenmitgliedschaft fehlen
  
Wenn Sie RMS in einer Umgebung bereitstellen, in der die Active Directory-Infrastrukturebenen auf die systemeigene Funktionsebene von Windows 2000 erhöht wurden, kann RMS möglicherweise nicht das „memberOf“-Attribut der Active Directory-Objekte lesen, wenn Sie versuchen, die Gruppenmitgliedschaft von ausgeblendeten Verteilerlisten zu erweitern. Das RMS-Dienstkonto muss ein Konto auf Domänenebene verwenden, das Mitglied der vordefinierten Gruppe „Prä-Windows 2000 kompatibler Zugriff“ ist, um RMS das Lesen des „memberOf“-Attributs zu ermöglichen. Weitere Informationen erhalten Sie im Artikel 812841 der Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=78152](http://go.microsoft.com/fwlink/?linkid=78152)) (möglicherweise in englischer Sprache).
  
#### Der Protokollierungslistenerdienst sendet Message Queuing-Nachrichten an die Warteschlange für unzustellbare Nachrichten, wenn ein Zugriff auf die Datenbank nicht möglich ist
  
Es kann passieren, dass der Protokollierungslistenerdienst die Datenbank nicht erreichen kann, z. B. wenn die Datenbank ausgefallen oder die Netzwerkverbindung unterbrochen ist. In diesem Fall werden die Nachrichten an eine Warteschlange für unzustellbare Nachrichten gesendet. Die einzige Möglichkeit, diese Nachrichten wiederherzustellen (d. h. sie an die Protokollierungsdatenbank zu senden), besteht darin, das RMS-Tool für die Warteschlangenwiederherstellung (Queue Recovery Tool) zu verwenden, das in den RMS-Verwaltungsprogrammen enthalten ist. Sie können die RMS-Verwaltungsprogramme unter [http://go.microsoft.com/fwlink/?LinkId=33841](http://go.microsoft.com/fwlink/?linkid=33841) (möglicherweise in englischer Sprache) herunterladen.
  
| ![](https://msdn.microsoft.com/de-de/Cc747637.note(WS.10).gif)Hinweis                                                                                                                                                                                                    |  
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| „Recover“ und „RecoverandPurge“ wurden aus „LogRecoveryCmd“ entfernt. Dadurch wird sichergestellt, dass alle Nachrichten durch den Message Queuing-Dienst zurückgeleitet und authentifiziert werden, bevor die Nachricht an die Protokollierungsdatenbank gesendet wird. |
  
#### Sie müssen RMS mit SP2 aktualisieren, bevor Sie auf Microsoft SQL Server  2005 aktualisieren
  
Wenn Sie auf RMS mit SP2 und von Microsoft SQL Server 2000 auf Microsoft SQL Server 2005 aktualisieren, müssen Sie zuerst RMS aktualisieren. Dadurch werden Kompatibilitätsprobleme bei der Aktualisierung von Microsoft SQL Server vermieden.
  
#### RMS mit SP2 kann keine Websites bereitstellen, deren Name einen Apostroph (') enthält
  
Wenn Sie versuchen, RMS mit SP2 auf einer Website bereitzustellen, deren Name einen Apostroph (') enthält, schlägt der Bereitstellungsvorgang fehl, und es wird eine Fehlermeldung wegen eines ungültigen Parameterseingeblendet. Damit RMS mit SP2 auf der Website bereitgestellt werden kann, müssen Sie den Apostroph aus dem Namen entfernen.
  
#### Aktivieren von ASP.NET Version 1.1 auf Servern, auf denen eine 64-Bit-Version von Windows Server 2003 ausgeführt wird
  
Im Abschnitt mit den Systemanforderungen in der RMS-Hilfe wird beschrieben, wie Sie nach der Installation der Internetinformationsdienste (Internet Information Services, IIS) .NET Framework 1.1 installieren und ASP.NET 1.1 aktivieren können. Wenn .NET Framework 1.1 vor IIS installiert wird, wird ASP.NET 1.1 nicht in den Webdiensterweiterungen aufgeführt, und die dokumentierte Vorgehensweise ist nicht hilfreich. Wurde IIS vor der Installation von .NET Framework 1.1 installiert, geben Sie in einer Eingabeaufforderung den folgenden Befehl ein, um ASP.NET zu aktivieren:
  
**%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis.exe -i -enable**
  
Wenn Sie eine neuere Version als .NET Framework 1.1 verwenden, ersetzen Sie in diesem Befehl das **-i** durch **-ir**, damit keine vorhandenen IIS-Skriptzuordnungen geändert werden.
  
#### Der lokalen „groupexpansion“-Pipeline muss ein Remote-RMS-Dienstkonto für die Gesamtstruktur hinzugefügt werden.
  
Es wurde eine Sicherheitslücke geschlossen, durch die der Eintrag „BUILTIN\\users“ aus der ACL in der „groupexpansion“-Pipeline entfernt wird. Dies kann die gesamtstrukturübergreifende Gruppenerweiterung zerstören. Gehen Sie zum Lösen des Problems folgendermaßen vor:
  
**Fügen Sie der Remotegesamtstruktur ein RMS-Dienstkonto hinzu.**  
1.  Wechseln Sie in „Gesamtstruktur1“, wobei „Gesamtstruktur1“ der RMS-Stammcluster in der ersten Gesamtstruktur ist, zu „inetpub\\wwwroot\\\_wmcs“.
  
2.  Klicken Sie mit der rechten Maustaste auf den Ordner **GroupExpansion**, und wählen Sie **Eigenschaften**.
  
3.  Klicken Sie im Fenster **GroupExpansion-Eigenschaften** auf die Registerkarte **Sicherheit**, fügen Sie den Eintrag für *Gesamtstruktur2\\RMS-Dienstkonto* hinzu (z. B. „rmil31\\rmsvc“), wobei „Gesamtstruktur2“ der RMS-Stammcluster in der zweiten Gesamtstruktur ist.
  
4.  Klicken Sie auf **OK**.
  
5.  Klicken Sie auf **Ausführen**, geben Sie **iisreset** ein, und klicken Sie auf**OK**.
  
#### Die Aktualisierung von .NET Framework kann zu Datenverlust führen
  
Wenn die .NET Framework (CLR) Version 1.1 aktualisiert wird, nachdem RMS installiert und bereitgestellt wurde, werden die vroots so eingestellt, dass sie .NET Framework Version 2.0 nutzen. In diesem Fall werden keine Informationen in die Protokollierungsdatenbank geschrieben. Dies führt zu Datenverlust. Halten Sie sich an eine der folgenden Vorgehensweisen:
  
-   Aktualisieren Sie zunächst .NET Framework, bevor Sie RMS installieren und bereitstellen.  
-   Stellen Sie die vroots so ein, dass sie 1.1 verwenden, nachdem .NET Framework aktualisiert wurde.
  
Dokumentationsänderungen in dieser Version  
------------------------------------------
  
Im Folgenden finden Sie eine Liste der Themen, die in dieser Version geändert wurden:
  
-   So vertrauen Sie Passport-basierten Rechtekontozertifikaten ([http://go.microsoft.com/fwlink/?LinkId=70369](http://go.microsoft.com/fwlink/?linkid=70369))  
-   Softwareanforderungen für RMS ([http://go.microsoft.com/fwlink/?LinkId=70371](http://go.microsoft.com/fwlink/?linkid=70371))  
-   So stellen Sie den RMS-Client bereit ([http://go.microsoft.com/fwlink/?LinkId=70373](http://go.microsoft.com/fwlink/?linkid=70373))  
-   RMS-Installation mithilfe einer Eingabeaufforderung ([http://go.microsoft.com/fwlink/?LinkId=70374](http://go.microsoft.com/fwlink/?linkid=70374))  
-   Kerntabellen der Konfigurationsdatenbank ([http://go.microsoft.com/fwlink/?LinkId=70375](http://go.microsoft.com/fwlink/?linkid=70375))  
-   Zertifizierungstabellen der Konfigurationsdatenbank ([http://go.microsoft.com/fwlink/?LinkId=70376](http://go.microsoft.com/fwlink/?linkid=70376))  
-   Protokollierungstabellen der Konfigurationsdatenbank ([http://go.microsoft.com/fwlink/?LinkId=70377](http://go.microsoft.com/fwlink/?linkid=70377))  
-   Evaluieren von Skalierungsanforderungen ([http://go.microsoft.com/fwlink/?LinkId=70378](http://go.microsoft.com/fwlink/?linkid=70378))  
-   Sichern der RMS-Bereitstellung ([http://go.microsoft.com/fwlink/?LinkId=70379](http://go.microsoft.com/fwlink/?linkid=70379))  
-   Aktivieren des Außerbetriebsetzungsdienstes ([http://go.microsoft.com/fwlink/?LinkId=70380](http://go.microsoft.com/fwlink/?linkid=70380))  
-   Planen für externe RMS-Benutzer ([http://go.microsoft.com/fwlink/?LinkId=70381](http://go.microsoft.com/fwlink/?linkid=70381))  
-   Aktivieren der RMS-Serverunterstützung für mobile Geräte und Serverdienste ([http://go.microsoft.com/fwlink/?LinkId=70382](http://go.microsoft.com/fwlink/?linkid=70382))
  
#### Copyright
  
*Die in diesem Dokument enthaltenen Angaben entsprechen dem Wissensstand der Microsoft Corporation zu den beschriebenen Problemen zum Zeitpunkt der Veröffentlichung. Microsoft muss auf veränderte Marktbedingungen reagieren und ist daher weder in der Lage noch dazu verpflichtet, die Richtigkeit der dargelegten Informationen über das Datum der Veröffentlichung hinaus zu garantieren.*
  
*Dieses Dokument dient lediglich zu Informationszwecken. MICROSOFT ÜBERNIMMT KEINE AUSDRÜCKLICHE, KONKLUDENTE ODER GESETZLICHE GEWÄHRLEISTUNG FÜR DIE INFORMATIONEN IN DIESEM DOKUMENT.*
  
*Die Benutzer sind verpflichtet, sich an alle geltenden Urheberrechtsgesetze zu halten. Unabhängig von der Anwendbarkeit der geltenden Urheberrechtsgesetze darf ohne ausdrückliche schriftliche Genehmigung der Microsoft Corporation kein Teil dieses Dokuments für beliebige Zwecke vervielfältigt, in einem Datenempfangssystem gespeichert oder darin eingelesen werden oder übertragen werden, unabhängig davon, auf welche Art und Weise oder mit welchen Mitteln (elektronisch, mechanisch, durch Fotokopieren, Aufzeichnen usw.) dies geschieht.*
  
*Es ist möglich, dass Microsoft Patente bzw. angemeldete Patente, Marken, Urheberrechte oder sonstige geistige Eigentumsrechte besitzt, die sich auf den fachlichen Inhalt dieses Dokuments beziehen. Das Bereitstellen dieses Dokuments gibt Ihnen jedoch keinen Anspruch auf diese Patente, Marken, Urheberrechte oder auf sonstiges geistiges Eigentum, es sei denn, dies wird ausdrücklich in schriftlichen Lizenzverträgen von Microsoft eingeräumt.*
  
*Die in den Beispielen verwendeten Firmen, Organisationen, Produkte, Domänennamen, E-Mail-Adressen, Logos, Personen, Orte und Ereignisse sind frei erfunden, soweit nichts anderes angegeben ist. Jede Ähnlichkeit mit bestehenden Firmen, Organisationen, Produkten, Domänennamen, E-Mail-Adressen, Logos, Personen, Orten oder Ereignissen ist rein zufällig.*
  
*© 2006 Microsoft Corporation. Alle Rechte vorbehalten.*
  
*Active Directory, Microsoft, MS-DOS, Visual Studio, Windows, Windows Server, SQL Server und Windows NT sind Marken oder eingetragene Marken der Microsoft Corporation in den USA und/oder in anderen Ländern.*
  
*Andere in diesem Dokument aufgeführte Produkt- und Firmennamen sind möglicherweise Marken der jeweiligen Eigentümer.*
