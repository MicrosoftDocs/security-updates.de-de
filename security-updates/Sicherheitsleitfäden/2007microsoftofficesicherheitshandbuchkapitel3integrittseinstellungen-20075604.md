---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 3: Integritätseinstellungen'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 3: Integritätseinstellungen'
ms:assetid: '1e5968df-c831-421f-99f1-3799520a7132'
ms:contentKeyID: 20075604
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443660(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch
=========================================

Kapitel 3: Integrittseinstellungen
----------------------------------

Verffentlicht: 11. Nov 2007

Integrittseinstellungen untersttzen Sie bei der Abwehr von Bedrohungen fr die Integritt von Unternehmensdaten und -prozessen. Bswillige Benutzer ben Angriffe auf die Integritt von Unternehmensressourcen aus, indem sie Dokumente, Prsentation und Tabellenkalkulationen beschdigen. Ein bswilliger Benutzer knnte beispielsweise ein Microsoft Visual Basic for Applications (VBA)-Makro oder ein Microsoft ActiveX-Steuerelement in einer Datei oder einer E-Mail-Nachricht zur Beeintrchtigung von Computern in Ihrem Unternehmen einsetzen. Ebenso knnte ein Angriff auf die Integritt Ihrer Unternehmensdaten oder -prozesse ausgebt werden, indem eine Datei durch eine hnliche Datei mit beschdigten Daten oder Informationen ersetzt wird.

Um die Risiken dieser Integrittsbedrohungen und Angriffsmethoden zu verringern, knnen Sie beweiserhebliche Vertrauensmechanismen implementieren. Dabei handelt es sich um Sicherheitstechnologien, die nachweisen, dass eine Datei oder Unternehmensressource vertrauenswrdig ist und nicht von einem unbefugten Benutzer gendert oder beschdigt wurde.

Die 2007 Microsoft Office-Version bietet verschiedene Einstellungen, mit denen Bedrohungen der Integritt gemindert werden knnen. Diese Einstellungen beziehen sich auf drei verschiedene Typen beweiserheblicher Vertrauensmechanismen:

-   **Liste vertrauenswrdiger Herausgeber**. Dieser Mechanismus ermglicht eine Unterscheidung zwischen vertrauenswrdigen und nicht vertrauenswrdigen Inhaltsherausgebern. Alle von Inhaltsherausgebern signierten Dateien, die nicht in der Liste vertrauenswrdiger Herausgeber aufgefhrt sind, werden als potenziell schdliche Inhalte angesehen.
-   **Vertrauenswrdige Speicherorte**. Dieser Mechanismus ermglicht die Unterscheidung von Ordnern, die Dateien aus vertrauenswrdigen Quellen enthalten. Eine Datei, die nicht an einem vertrauenswrdigen Speicherort gespeichert ist, wird als potenziell schdlicher Inhalt angesehen.
-   **Digitale Signaturen**. Dieser Mechanismus ermglicht es Benutzern, Dokumente, Prsentationen und Tabellenkalkulationen mit digitalen Signaturen zu versehen, durch die sich der Ersteller der Datei nachweisen lsst.

![](images/Dd443660.important(de-de,TechNet.10).gif) Wichtig:

Neben der Bercksichtigung der in diesem Kapitel erluterten Einstellungen sollten Sie zudem sicherstellen, dass Ihre Computer zu jedem Zeitpunkt mit den neuesten Sicherheitspatches von Microsoft aktualisiert sind. Ein effektives Patchmanagement trgt entscheidend zur Aufrechterhaltung der Sicherheit in Unternehmen bei.

##### Auf dieser Seite

[Einstellungen fr vertrauenswrdige Herausgeber](#eyd)
[Einstellungen fr vertrauenswrdige Speicherorte](#eng)
[Einstellungen fr digitale Signaturen](#e2gac)

Einstellungen fr vertrauenswrdige Herausgeber
---------------------------------------------

Mithilfe der Liste vertrauenswrdiger Herausgeber knnen Sie Inhaltsherausgeber bestimmen, denen Sie vertrauen. Bei einem Herausgeber handelt es sich um einen Entwickler, ein Softwareunternehmen oder ein Unternehmen, das Inhalte wie ActiveX-Steuerelemente, Add-Ins oder Makros erstellt und verteilt. Ein Herausgeber ist vertrauenswrdig, wenn sein digitales Zertifikat der Liste vertrauenswrdiger Herausgeber hinzugefgt wurde. Wenn eine Datei geffnet und ihr aktiver Inhalt durch ein digitales Zertifikat aus der Liste vertrauenswrdiger Herausgeber signiert wurde, wird der Inhalt als vertrauenswrdig und frei von Integrittsexploits angesehen.

Integrittsbedrohungen werden ber verschiedene Methoden ausgenutzt. Zu den hufigsten dieser Methoden gehrt die Verwendung schdlicher ActiveX-Steuerelemente, Add-Ins und VBA-Makos. Diese Technologien knnen von Programmierern ausgenutzt werden, die schdlichen Code schreiben bzw. schdliche Programme erstellen, die auf dem Computer eines Benutzers ausgefhrt werden. Integrittsbedrohungen stellen fr die meisten Unternehmen ein potenzielles Risiko dar, besonders aber fr Unternehmen, die Benutzern Folgendes ermglichen:

-   Ausfhren von ActiveX-Steuerelementen, Add-Ins und Makros
-   Empfangen von E-Mail-Anlagen
-   Gemeinsamer Zugriff auf Dokumente ber ein ffentliches Netzwerk, z. B. das Internet
-   ffnen von Dokumenten aus Quellen auerhalb des Unternehmens, beispielsweise von Kunden, Anbietern oder Partnern

Standardmig sind ActiveX-Steuerelemente und Makros, die von einem Herausgeber aus der Liste vertrauenswrdiger Herausgeber signiert wurden, aktiviert und werden ohne Warnung ausgefhrt, wenn die folgenden Bedingungen zutreffen:

-   Das ActiveX-Steuerelemente bzw. das Makro ist mit einer digitalen Signatur versehen.
-   Die digitale Signatur ist gltig.
-   Die digitale Signatur ist aktuell (nicht abgelaufen).
-   Das mit der digitalen Signatur verbundene Zertifikat wurde von einer anerkannten Zertifizierungsstelle (Certification Authority, CA) ausgestellt.

Standardmig knnen Anwendungs-Add-Ins ohne Signatur durch einen Herausgeber aus der Liste vertrauenswrdiger Herausgeber ausgefhrt werden. Wenn Sie festlegen mchten, dass diese signiert sein sollen, knnen Sie dies ber die Gruppenrichtlinie oder die Benutzeroberflche konfigurieren. Weitere Informationen finden Sie unter der Einstellung Anwendungs-Add-Ins mssen von einem vertrauenswrdigen Herausgeber signiert sein im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.

Standardmig sind keine vertrauenswrdigen Herausgeber in der Liste vertrauenswrdiger Herausgeber aufgefhrt. Die Liste vertrauenswrdiger Herausgeber ist jedoch aktiviert, und Benutzer knnen der Liste digitale Zertifikate fr alle Herausgeber hinzufgen, die als vertrauenswrdig eingestuft werden sollen.

Zum Hinzufgen von Zertifikaten zur Liste vertrauenswrdiger Herausgeber sollten Sie das Office-Anpassungstool (OAT) und nicht die Gruppenrichtlinie verwenden. Wenn beim Anpassen einer neuen Bereitstellung von 2007 Office bzw. beim Installieren von Updates fr vorhandene Installationen Zertifikate mithilfe des OAT hinzugefgt werden sollen, muss Ihnen das digitale Zertifikat (CER-Datei) des vertrauenswrdigen Herstellers vorliegen. Wenn es nicht mglich ist, das Zertifikat direkt vom Herausgeber zu beziehen, knnen Sie ein Zertifikat aus einer vom Herausgeber signierten Datei exportieren, etwa aus einer DLL-Datei (Dynamic Link Library) oder einer ausfhrbaren EXE-Datei.

Die folgende Liste enthlt eine 2007 Office-Einstellung, die Ihnen bei Verwendung und Konfiguration der Einstellung fr vertrauenswrdige Herausgeber behilflich sein kann. Weitere Informationen zu dieser Einstellung finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.

**Tabelle 3.1. Sicherheitseinstellungen fr vertrauenswrdige Herausgeber**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Name der Einstellung</th>
<th>Betrifft</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Anwendungs-Add-Ins mssen von einem vertrauenswrdigen Herausgeber signiert sein</p></td>
<td style="border:1px solid black;"><p>Office Access 2007, Excel 2007, InfoPath 2007, PowerPoint 2007, Word 2007</p></td>
</tr>  
</tbody>  
</table>
  
Die 2007 Office-Version speichert Zertifikate fr vertrauenswrdige Herausgeber in der Aufstellung der vertrauenswrdigen Herausgeber von Microsoft Internet Explorer. In frheren Versionen von Microsoft Office wurden Informationen zu Zertifikaten fr vertrauenswrdige Herausgeber (insbesondere der Zertifikatfingerabdruck) in einer speziellen Office-Aufstellung der vertrauenswrdigen Herausgeber gespeichert. Die 2007 Office-Version liest weiterhin Informationen zu Zertifikaten fr vertrauenswrdige Herausgeber aus der Office-Aufstellung der vertrauenswrdigen Herausgeber, schreibt aber keine Informationen in diese Aufstellung.
  
Wenn Sie also eine Liste vertrauenswrdiger Herausgeber in einer frheren Version von Office erstellt und ein Upgrade auf die 2007 Office-Version durchgefhrt haben, wird Ihre Liste vertrauenswrdiger Herausgeber weiterhin anerkannt. Jedoch werden alle Zertifikate vertrauenswrdiger Herausgeber, die Sie der Liste hinzufgen, in der Aufstellung vertrauenswrdiger Herausgeber in Internet Explorer gespeichert. Diese Funktionalitt ist fr alle Anwendungen gleich, die die Liste vertrauenswrdiger Herausgeber verwenden. Dazu gehren:
  
-   Microsoft Office Access 2007  
-   Microsoft Office Excel 2007  
-   Microsoft Office InfoPath 2007  
-   Microsoft Office Outlook 2007  
-   Microsoft Office PowerPoint 2007  
-   Microsoft Office Word 2007
  
Die meisten der Liste vertrauenswrdiger Herausgeber hinzugefgten Zertifikate gelten fr ActiveX-Steuerelemente, Add-Ins und Makros, die Ihr Unternehmen entwickelt oder von anderen Unternehmen als Microsoft erworben hat. Wenn alle Add-Ins von einem vertrauenswrdigen Herausgeber signiert sein mssen, sollten der Liste vertrauenswrdige Herausgeber auch Zertifikate von Microsoft hinzugefgt werden. Die Zertifikate von Microsoft haben die Namen Mscert01.cer, Mscert02.cer, Mscert03.cer und Mscert04.cer und knnen von der Microsoft-Website heruntergeladen werden. Wenn Sie die Einstellung Anwendungs-Add-Ins mssen von einem vertrauenswrdigen Herausgeber signiert sein aktivieren, ohne die Microsoft-Zertifikate zur Liste vertrauenswrdiger Hersteller hinzuzufgen, werden in der Statusleiste und in Dialogfeldern Meldungen angezeigt, wenn ein Benutzer Anwendungen und Anwendungsfunktionen verwendet, die Add-Ins aus der 2007 Office-Version verwenden.
  
### Richtlinien fr die Verwendung von Einstellungen fr vertrauenswrdige Herausgeber
  
Beachten Sie bei der Verwendung von Einstellungen fr vertrauenswrdige Herausgeber die folgenden Richtlinien:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr vertrauenswrdige Herausgeber innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Fgen Sie der Liste vertrauenswrdiger Herausgeber nur Herausgeber hinzu, denen unbedingt vertraut werden kann. ActiveX-Steuerelemente und Makros in Dokumenten knnen ohne Warnung ausgefhrt werden, wenn der jeweilige Herausgeber in der Liste vertrauenswrdiger Herausgeber aufgefhrt ist.  
-   Ziehen Sie in Betracht, es mithilfe der Gruppenlinie zur Auflage zu machen, dass alle Add-Ins von einem vertrauenswrdigen Herausgeber signiert sein mssen. In diesem Fall sollten Sie der Liste vertrauenswrdiger Herausgeber ebenfalls die Microsoft-Zertifikate fr integrierte Add-Ins hinzufgen.  
-   Fgen Sie der Liste vertrauenswrdiger Herausgeber Zertifikate mithilfe des Office-Anpassungstools (OAT) hinzu.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Einstellungen fr vertrauenswrdige Speicherorte  
----------------------------------------------
  
Die Funktion fr vertrauenswrdige Speicherorte in der 2007 Office-Version ermglicht es Ihnen, auf den Festplatten von Benutzercomputern bzw. auf Netzwerkfreigaben Ordner als vertrauenswrdige Dateiquellen zu bestimmen. Alle in vertrauenswrdigen Speicherorten abgelegten Dateien werden als vertrauenswrdig angesehen. Beim ffnen einer vertrauenswrdigen Datei wird der Inhalt als vertrauenswrdig und frei von Integrittsexploits betrachtet. Der gesamte Dateiinhalt wird aktiviert und ist aktiv, und der Benutzer wird nicht ber mglicherweise in der Datei enthaltene potenzielle Risiken informiert, z. B. unsignierte Makros, ActiveX-Steuerelemente oder Links zu Inhalten im Internet.
  
Wie bereits erwhnt knnen Integrittsbedrohungen ber verschiedene Methoden ausgenutzt werden. Zu den hufigsten Methoden gehrt die Verwendung schdlicher ActiveX-Steuerelemente, Add-Ins und VBA-Makros. Diese Technologien knnen von Programmierern ausgenutzt werden, die schdlichen Code schreiben bzw. schdliche Programme erstellen, die auf dem Computer eines Benutzers ausgefhrt werden. Integrittsbedrohungen stellen fr die meisten Unternehmen ein potenzielles Risiko dar, besonders aber fr Unternehmen, die Benutzern Folgendes ermglichen:
  
-   Ausfhren von ActiveX-Steuerelementen, Add-Ins und Makros  
-   Empfangen von E-Mail-Anlagen  
-   Gemeinsamer Zugriff auf Dokumente ber ein ffentliches Netzwerk, z. B. das Internet  
-   ffnen von Dokumenten aus externen Quellen, z. B. von Kunden, Anbietern oder Partnern.
  
In der folgenden Liste sind die Standardeinstellungen fr vertrauenswrdige Speicherorte aufgefhrt:
  
-   Vertrauenswrdige Speicherorte sind aktiviert, sodass Benutzer die Mglichkeit haben, solche Speicherorte zu erstellen.  
-   Netzwerkfreigaben knnen nicht als vertrauenswrdige Speicherorte bestimmt werden. Diese Einstellung kann jedoch vom Benutzer gendert werden.  
-   Benutzer knnen der Liste vertrauenswrdiger Speicherorte Ordner hinzufgen.  
-   Es kann eine Mischung aus benutzerdefinierten und richtliniendefinierten vertrauenswrdigen Speicherorten vorhanden sein.
  
Auerdem werden verschiedene Ordner auf Anwendungsbasis als vertrauenswrdige Speicherorte festgelegt. Die Standardordner fr die einzelnen Anwendungen sind in den folgenden Tabellen aufgefhrt.
  
![](images/Dd443660.note(de-de,TechNet.10).gif) Hinweis:  
Office InfoPath 2007 und Office Outlook 2007 verwenden keine vertrauenswrdigen Speicherorte.
  
**Tabelle 3.2. Vertrauenswrdige Standardspeicherorte fr Office Access 2007**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="33%" />  
<col width="33%" />  
<col width="33%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Vertrauenswrdige Standardspeicherorte</th>  
<th>Ordnerbeschreibung</th>  
<th>Vertrauenswrdige Unterordner</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Office12\ACCWIZ</p></td>
<td style="border:1px solid black;"><p>Assistentendatenbanken</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
</tbody>  
</table>
  
**Tabelle 3.3. Vertrauenswrdige Standardspeicherorte fr Office Excel 2007**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="33%" />  
<col width="33%" />  
<col width="33%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Vertrauenswrdige Standardspeicherorte</th>  
<th>Ordnerbeschreibung</th>  
<th>Vertrauenswrdige Unterordner</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Anwendungsvorlagen</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming\Microsoft\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Benutzervorlagen</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Office12\XLSTART</p></td>
<td style="border:1px solid black;"><p>Excel-StartUp</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming \Microsoft\Excel\XLSTART</p></td>
<td style="border:1px solid black;"><p>Benutzer-Startup</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Office12\STARTUP</p></td>
<td style="border:1px solid black;"><p>Office-Startup</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Office12\Bibliothek</p></td>
<td style="border:1px solid black;"><p>Add-Ins</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
</tbody>  
</table>
  
**Tabelle 3.4. Vertrauenswrdige Standardspeicherorte fr Office PowerPoint 2007**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="33%" />  
<col width="33%" />  
<col width="33%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Vertrauenswrdige Standardspeicherorte</th>  
<th>Ordnerbeschreibung</th>  
<th>Vertrauenswrdige Unterordner</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Anwendungsvorlagen</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming\Microsoft\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Benutzervorlagen</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming\Microsoft\Add-Ins</p></td>
<td style="border:1px solid black;"><p>Add-Ins</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Dokumentdesigns 12</p></td>
<td style="border:1px solid black;"><p>Anwendungsdesigns</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
</tbody>  
</table>
  
**Tabelle 3.5. Vertrauenswrdige Standardspeicherorte fr Office Word 2007**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="33%" />  
<col width="33%" />  
<col width="33%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Vertrauenswrdige Standardspeicherorte</th>  
<th>Ordnerbeschreibung</th>  
<th>Vertrauenswrdige Unterordner</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Programme\Microsoft Office\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Anwendungsvorlagen</p></td>
<td style="border:1px solid black;"><p>Zugelassen</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming\Microsoft\Vorlagen</p></td>
<td style="border:1px solid black;"><p>Benutzervorlagen</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzer\<em>&lt;benutzername&gt;</em>\Appdata\Roaming \Microsoft\Word\Startup</p></td>
<td style="border:1px solid black;"><p>Benutzer-Startup</p></td>
<td style="border:1px solid black;"><p>Nicht zugelassen</p></td>
</tr>  
</tbody>  
</table>
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit deren Hilfe Sie vertrauenswrdige Speicherorte verwenden und konfigurieren knnen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 3.6. Sicherheitseinstellungen fr vertrauenswrdige Speicherorte**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Name der Einstellung</th>  
<th>Betrifft</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Mischung aus Richtlinien- und Benutzerspeicherorten zulassen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Vertrauenswrdige Speicherorte, die sich nicht auf dem Computer befinden, zulassen</p></td>
<td style="border:1px solid black;"><p>Office Access 2007, Office Excel 2007, Office PowerPoint 2007, Office Word 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Alle vertrauenswrdigen Speicherorte deaktivieren</p></td>
<td style="border:1px solid black;"><p>Office Access 2007, Office Excel 2007, Office PowerPoint 2007, Office Word 2007</p></td>
</tr>  
</tbody>  
</table>
  
### Richtlinien zur Verwendung von Einstellungen fr vertrauenswrdige Speicherorte
  
Beachten Sie beim Verwenden der Einstellungen fr vertrauenswrdige Speicherorte die folgenden Richtlinien:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr vertrauenswrdige Speicherorte innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Gehen Sie beim Ablegen von Dateien in vertrauenswrdigen Speicherorten vorsichtig vor. Diese Dateien knnen aktive Inhalte enthalten, die aktiviert sind, und dem Benutzer wird keine Warnung dazu angezeigt. In bestimmten Situationen sollte erwogen werden, die Einstellungen fr vertrauenswrdige Speicherorte ganz zu deaktivieren.  
-   Verwenden Sie in vertrauenswrdigen Speicherorten Sicherheitseinstellungen auf Dateiebene.  
-   berprfen Sie die Quelle von Dateien in vertrauenswrdigen Speicherorten mithilfe digitaler Signaturen.  
-   Setzen Sie Verschlsselung ein, um unbefugte Benutzer am Anzeigen und ndern von Dateien in vertrauenswrdigen Speicherorten zu hindern.  
-   Vertrauenswrdige Speicherorte im Netzwerk bieten attraktive Ziele fr potenzielle Angreifer. Wenn Sie im Netzwerk vertrauenswrdige Speicherorte verwenden, befolgen Sie die Richtlinien auf den Seiten zur [Server- und Domnenisolation](http://technet.microsoft.com/en-us/network/bb545651.aspx) auf der Microsoft TechNet-Website.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
<span></span>  
Einstellungen fr digitale Signaturen  
------------------------------------
  
Die Funktion fr digitale Signaturen in der 2007 Office-Version ermglicht Benutzern ein digitales Signieren von Dokumenten, Prsentationen und Tabellenkalkulationen.
  
Auerdem knnen Dokumenten, Prsentationen und Tabellenkalkulationen digitale Signaturzeilen hinzugefgt werden, die Ihrem Unternehmen einen papierlosen Signaturprozess fr Dokumente wie Vertrge oder andere Vereinbarungen ermglichen. Eine digitale Signatur sieht wie ein normaler Signaturplatzhalter in einem Druckdokument aus (z. B. der Buchstabe X gefolgt von einer horizontalen Linie), funktioniert aber anders. Wenn eine Signaturzeile in ein Office-Dokument eingefgt wird, kann der Autor des Dokuments Informationen ber den vorgesehenen Signaturgeber sowie Anweisungen fr den Signaturgeber angeben. Wenn eine elektronische Kopie des Dokuments an den vorgesehenen Signaturgeber gesendet wird, sieht diese Person die Signaturlinie sowie eine Meldung, dass ihre Signatur angefordert wird. Der Signaturgeber klickt auf die Signaturzeile, um das Dokument digital zu signieren. Der Signaturgeber kann dann entweder eine Signatur eintippen, ein digitales Bild seiner Signatur auswhlen oder mithilfe der Freihandfunktionen auf einem Tablet PC eine Signatur schreiben. Wenn der Signaturgeber dem Dokument eine sichtbare Ausfhrung seiner Signatur hinzufgt, wird gleichzeitig eine digitale Signatur hinzugefgt, um die Identitt des Signaturgebers zu authentifizieren. Nach der digitalen Signierung wird das Dokument schreibgeschtzt, damit an seinem Inhalt keine nderungen vorgenommen werden knnen. Im Gegensatz zu Unterschriften auf Papier bieten digitale Signaturen einen Nachweis darber, was genau signiert wurde. Weiterhin kann bei digitalen Signaturen die Signatur in der Zukunft berprft werden.
  
Digitale Signaturen tragen zur Verringerung von Integrittsbedrohungen bei, da gewhrleistet wird, dass der Inhalt von Dokumenten, E-Mail-Nachrichten, Prsentationen und Tabellenkalkulation nach der Signatur nicht gendert oder manipuliert wurde. Durch digitale Signaturen knnen auch Bedrohungsrisiken im Bereich Authentizitt verringert werden, da sichergestellt ist, dass es sich wirklich um den Signaturgeber handelt. Weiterhin wird das Risiko der Nichtanerkennung gemindert, da der Ursprung des signierten Inhalts gewhrleistet ist. (Nichtanerkennung bedeutet in diesem Kontext, dass ein Signaturgeber jede Verbindung mit dem signierten Inhalt ablehnt.)
  
Um diese Bedrohungen zu verringern und die oben aufgefhrten Zusicherungen vorzunehmen, muss der Inhalt mit einer digitalen Signatur versehen sein, die die folgenden Kriterien erfllt:
  
-   Die digitale Signatur ist gltig.  
-   Das mit der digitalen Signatur verbundene Zertifikat ist aktuell (nicht abgelaufen).  
-   Der Signaturgeber oder das signaturgebende Unternehmen, auch als Herausgeber bezeichnet, mssen vertrauenswrdig sein.  
-   Das mit der digitalen Signatur verbundene Zertifikat wurde dem signaturgebenden Herausgeber von einer anerkannten Zertifizierungsstelle (Certification Authority, CA) zugestellt.
  
Die 2007 Office-Version ist in der Lage, diese Kriterien zu erkennen und warnt Benutzer im Falle eines Problems mit einer digitalen Signatur, wenn diese versuchen, ein Dokument, eine E-Mail-Nachricht, eine Prsentation oder eine Tabellenkalkulation zu signieren.
  
Standardmig enthalten Dokumente, E-Mail-Nachrichten, Prsentationen und Tabellenkalkulationen keine digitalen Signaturen bzw. Signaturzeilen und erfordern diese auch nicht. Es gibt auerdem keine Richtlinieneinstellungen, mit denen Sie Benutzer zum digitalen Signieren von Dokumenten, Prsentationen oder Tabellenkalkulationen zwingen knnen.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit deren Hilfe Sie digitale Signaturen verwenden und konfigurieren knnen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 3.7. Sicherheitseinstellungen fr digitale Signaturen**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th>Name der Einstellung</th>  
<th>Betrifft</th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Anlage sicherer temporrer Ordner</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>EKU-Filterung</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Beschriftung aller mit S/MIME signierter Nachrichten sicherstellen</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Schlsselverwendungsfilterung</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Legacyformatsignaturen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fehlende Zertifikatsperrlisten</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Fehlende Stammzertifikate</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fehler der Ebene 2 als Fehler, nicht als Warnungen, hher stufen</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>S/MIME-Besttigung anfordern, wenn mit S/MIME signiert</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Abrufen von Zertifikatsperrlisten</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Alle signierten Nachrichten als Klartext senden</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Alle E-Mail-Nachrichten signieren</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Signaturwarnung</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Menelement fr externe Signaturdienste unterdrcken</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Office-Signaturanbieter unterdrcken</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>URL fr S/MIME-Zertifikate</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
</tbody>  
</table>
  
### Richtlinien fr die Verwendung von Einstellungen fr digitale Signaturen
  
Beachten Sie beim Einsatz digitaler Signaturen in Ihrem Unternehmen die folgenden Richtlinien:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr digitale Signaturen innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Verwenden Sie digitale Signaturen in E-Mail-Nachrichten um zu besttigen, dass der Absender auch die Person ist, die er vorgibt zu sein, und dass die Nachricht whrend der bermittlung nicht gendert wurde.  
-   Setzen Sie digitale Signaturen fr andere Microsoft Office-Dokumente ein, wenn deren Ursprung sowie die Tatsache, dass sie seit der Signierung nicht gendert wurden, gewhrleistet werden sollen.  
-   Stellen Sie sicher, dass Benutzer in der berprfung digitaler Signaturen geschult werden.  
-   Ziehen Sie in Erwgung, Signaturen fr alle ausgehenden E-Mail-Nachrichten obligatorisch zu machen. Dazu bentigen alle Benutzer ein Signaturzertifikat einer vertrauenswrdigen Zertifizierungsstelle.
  
##### In diesem Beitrag
  
-   [berblick](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))  
-   [Kapitel 1: Sicherheit in der 2007 Office-Version](https://technet.microsoft.com/de-de/library/b9767904-ac34-4263-89e7-3c3e82eff607(v=TechNet.10))  
-   [Kapitel 2: Vertraulichkeitseinstellungen](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10))  
-   Kapitel 3: Integrittseinstellungen  
-   [Kapitel 4: Verfgbarkeitseinstellungen](https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10))  
-   [Kapitel 5: Entwerfen und Implementieren von Sicherheitseinstellungen](https://technet.microsoft.com/de-de/library/6de5a362-72f8-4937-84ef-54ec91e040e6(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um ber Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch)
  
|                                                  |                                                                                                                                                                                                                                                                                                                                                                              |  
|--------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443660.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10))4 von 6[![](images/Dd443660.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10)) |
