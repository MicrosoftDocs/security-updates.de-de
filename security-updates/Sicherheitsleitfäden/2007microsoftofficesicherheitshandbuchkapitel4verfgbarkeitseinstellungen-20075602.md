---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch:Kapitel 4: Verfügbarkeitseinstellungen'
Title: '2007 Microsoft Office-Sicherheitshandbuch:Kapitel 4: Verfügbarkeitseinstellungen'
ms:assetid: 'fe08a815-c260-4218-aea7-3f2f8447f81c'
ms:contentKeyID: 20075602
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443658(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch
=========================================

### Kapitel 4: Verfügbarkeitseinstellungen

Veröffentlicht: 11. Nov 2007

Mithilfe von Verfgbarkeitseinstellungen lassen sich Bedrohungen wichtiger Unternehmensdaten und -prozesse verringern. Bswillige Benutzer knnten Angriffe auf die Verfgbarkeit solcher Daten und Prozesse ausfhren und dabei Microsoft ActiveX-Steuerelemente, externe Links zu Datenquellen, Add-Ins und Microsoft Visual Basic for Applications (VBA)-Makros ausnutzen.

Ein bswilliger Benutzer knnte beispielsweise einen Hyperlink zu einer externen Tabellenkalkulation ausnutzen, indem er die externe Tabellenkalkulation durch eine andere ersetzt, die falsche Daten enthlt bzw. beschdigt ist. Ebenso knnte ein bswilliger Benutzer ein ActiveX-Steuerelement, das auf Unternehmensdaten in einer Datenbank zugreift, durch ein Steuerelement ersetzen, das eine Verknpfung zu einer manipulierten Datenbank herstellt.

Die 2007 Microsoft Office-Version bietet eine Reihe von Technologien und Einstellungen zum Verringern von Bedrohungen der Verfgbarkeit. Diese Technologien und Einstellungen lassen sich aufgrund der Bedrohungsarten und Angriffsmethoden in sechs Hauptgruppen einteilen.

-   **VBA-Makroeinstellungen** ermglichen ein Steuern der Ausfhrung von Makros, wenn diese in Dokumenten, E-Mail-Mitteilungen, Prsentationen und Tabellenkalkulationen enthalten sind.
-   **Add-In-Einstellungen** ermglichen ein Steuern der Ausfhrung von Add-Ins.
-   **ActiveX-Steuerelementeinstellungen** ermglichen ein Steuern der Ausfhrung von ActiveX-Steuerelementen.
-   **Einstellungen fr externe Inhalte** ermglichen ein Steuern der Verknpfungen zu externen Inhaltsfunktionen in Dokumenten, Prsentationen und Tabellenkalkulationen.
-   **Dateiblockierungstechnologien** umfassen zahlreiche Einstellungen, mit denen Benutzer am ffnen oder Speichern bestimmter Dateitypen und Dateiformate gehindert werden knnen.
-   **Microsoft Internet Explorer-Funktionseinstellungen** tragen dazu bei, eine Reihe unterschiedlicher Internet Explorer-Funktionstypen vor einer Ausnutzung zu schtzen. Diese Einstellungen sind besonders ntzlich, wenn ein Dokument oder eine Anwendung Internet Explorer hostet.

![](images/Dd443658.important(de-de,TechNet.10).gif)**Wichtig:**

Neben der Bercksichtigung der in diesem Kapitel erluterten Einstellungen sollten Sie zudem sicherstellen, dass Ihre Computer zu jedem Zeitpunkt mit den neuesten Sicherheitspatches von Microsoft aktualisiert sind. Ein effektives Patchmanagement trgt entscheidend zur Verbesserung der Sicherheit in Unternehmen bei.

##### Auf dieser Seite

[Verringern von Bedrohungen ber VBA-Makros](#eyd)
[Mindern von Bedrohungen durch Add-Ins](#eng)
[Einstellungen zur Minderung von Bedrohungen durch ActiveX-Steuerelemente](#egac)
[Einstellungen zum Mindern von Bedrohungen durch externe Inhalte](#egbc)
[Dateiblockierungstechnologie](#egcc)
[Mindern von Bedrohungen durch Internet Explorer-Funktionen](#egdc)

Verringern von Bedrohungen ber VBA-Makros
-----------------------------------------

Mithilfe von VBA-Makroeinstellungen kann die Funktion von VBA-Makros gesteuert werden, wodurch sich das Risiko von Bedrohungen und Angriffsmethoden mindern lsst, die sich auf die Sicherheit und Verfgbarkeit von Unternehmensdaten und -prozessen auswirken.

Die VBA-Makrofunktionalitt wird in der Regel von Programmierern ausgenutzt, die schdlichen Code schreiben oder schdliche Programme zur Ausfhrung auf den Computern der Benutzer erstellen. Solche Makros werden oft ber Dokumente, E-Mail-Mitteilungen, Prsentationen und Tabellenkalkulationen verteilt.

VBA-Makros stellen fr Unternehmen jeder Gre ein potenzielles Risiko dar. Dieses potenzielle Risiko ist jedoch hher, wenn im Unternehmen Folgendes zugelassen wird:

-   Ausfhren von VBA-Makros
-   Empfangen von E-Mail-Anlagen
-   Gemeinsamer Zugriff auf Dokumente ber ein ffentliches Netzwerk, z. B. das Internet
-   ffnen von Dokumenten aus Quellen auerhalb des Unternehmens, beispielsweise von Kunden, Anbietern oder Partnern

Das Ausfhren vertrauenswrdiger Makros wird standardmig zugelassen. Zu vertrauenswrdigen Makros gehren Makros in Dateien, die an vertrauenswrdigen Speicherorten gespeichert sind, sowie Makros, die die folgenden Kriterien erfllen:

-   Das Makro wurde vom Entwickler mit einer digitalen Signatur versehen.
-   Die digitale Signatur ist gltig.
-   Die digitale Signatur ist aktuell (nicht abgelaufen).
-   Das mit der digitalen Signatur verbundene Zertifikat wurde von einer anerkannten Zertifizierungsstelle (Certification Authority, CA) ausgestellt.
-   Der Entwickler, der das Makro signiert hat, ist ein vertrauenswrdiger Herausgeber.

Das Ausfhren nicht vertrauenswrdiger Makros wird standardmig nicht zugelassen. Wenn in einer Datei ein nicht vertrauenswrdiges Makro entdeckt wird, wird in der Statusleiste eine Warnung angezeigt, dass die Datei ein potenziell schdliches Makro enthlt. Wenn der Benutzer auf die Statusleiste klickt, hat er die Wahl, das Makro zu aktivieren oder es deaktiviert zu belassen. Diese Funktionalitt unterscheidet sich von der in Office 2003, bei der unsignierte Makros deaktiviert wurden und der Benutzer nicht die Option erhielt, diese zu aktivieren.

In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen durch VBA-Makros mindern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.

**Tabelle 4.1. Sicherheitseinstellungen zur Minderung von Bedrohungen durch VBA-Makros**

 
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
<td style="border:1px solid black;">Makrosicherheitseinstellungen auf Makros, Add-Ins und SmartTags anwenden</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Automatisierungssicherheit</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bestimmen, ob das berprfen verschlsselter Makros in Microsoft Excel Open XML-Arbeitsmappen erzwungen wird</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bestimmen, ob das berprfen verschlsselter Makros in Microsoft PowerPoint Open XML-Prsentationen erzwungen wird</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bestimmen, ob das berprfen verschlsselter Makros in Microsoft Word Open XML-Dokumenten erzwungen wird</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alle Benachrichtigungen fr Vertrauensstellungsleiste aus Sicherheitsgrnden deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Befehle deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Excel 2007, PowerPoint 2007, InfoPath 2007, Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Tastenkombinationen deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Excel 2007, PowerPoint 2007, InfoPath 2007, Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Benachrichtigung fr Vertrauensstellungsleiste fr nicht signierte Anwendungs-Add-Ins deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Excel 2007, PowerPoint 2007, InfoPath 2007, Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VBA fr Office-Anwendungen deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Excel-Dateien speichern unter</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sicherheitseinstellung fr Makros</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Makro standardmig in Persnliche Makroarbeitsmappe speichern</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zugriff auf Visual Basic-Projekt vertrauen</td>
<td style="border:1px solid black;">Office Excel 2007, PowerPoint 2007, Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Einstellungen fr VBA-Makrowarnung</td>
<td style="border:1px solid black;">Office Access 2007, Excel 2007, PowerPoint 2007, Word 2007</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Mindern von Bedrohungen durch Add-Ins  
-------------------------------------
  
Add-Ins bieten zustzliche Funktionalitt wie benutzerdefinierte Befehle und besondere Funktionen fr die 2007 Microsoft Office-Programme. COM-Add-Ins beispielsweise knnen in einem oder mehreren Office-Programmen ausgefhrt werden. COM-Add-Ins (die die Dateinamenerweiterungen .dll oder .exe aufweisen) verwenden Automatisierungs-Add-Ins, Anwendungs-Add-Ins (.wll, .xll, .xlam), XML-Erweiterungspakete, XML-Stylesheets, Smarttags usw.
  
Mithilfe von Add-In-Einstellungen kann die Funktionsweise von Add-Ins gesteuert werden, wodurch sich das Risiko von Bedrohungen und Angriffsmethoden mindern lsst, die sich auf die Sicherheit und Verfgbarkeit von Unternehmensdaten und -prozessen auswirken.
  
Wie bei VBA-Makros werden Add-Ins in der Regel von Programmierern ausgenutzt, die schdlichen Code schreiben oder schdliche Programme zur Ausfhrung auf den Computern der Benutzer erstellen. Add-Ins werden normalerweise ber Dynamic Link Library-Dateien (.dll) und Excel-Add-In-Dateien (.xll und .xlam) verteilt.
  
Add-Ins stellen fr Unternehmen jeder Gre ein potenzielles Risiko dar. Das potenzielle Risiko ist jedoch grer, wenn das Unternehmen Benutzer nicht am Ausfhren und Installieren von Add-Ins hindert. Standardmig kann jedes installierte und registrierte Add-In ohne Benutzereingriff oder Warnung ausgefhrt werden. Zu den installierten und registrierten Add-Ins gehren beispielsweise die folgenden:
  
-   COM-Objekte (Component Object Model)  
-   Smarttags  
-   Automatisierungsprogramme  
-   RTD-Server (RealTimeData)  
-   Anwendungs-Add-Ins (zum Beispiel WLL-, XLL- und XLAM-Dateien)  
-   XML-Erweiterungspakete  
-   XML-Stylesheets
  
Diese Standardfunktionalitt entspricht der Auswahl der Einstellung **Allen installierten Add-Ins und Vorlagen** vertrauen aus frheren Versionen des Microsoft Office-Systems.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen durch Add-Ins mindern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 4.2. Sicherheitseinstellungen zur Minderung von Bedrohungen durch Add-Ins**

 
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
<td style="border:1px solid black;">Makrosicherheitseinstellungen auf Makros, Add-Ins und SmartTags anwenden</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Vertrauenswrdige Add-Ins konfigurieren</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Alle Anwendungs-Add-Ins deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Office Excel 2007, Office InfoPath 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alle Benachrichtigungen fr Vertrauensstellungsleiste aus Sicherheitsgrnden deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Benachrichtigung fr Vertrauensstellungsleiste fr nicht signierte Anwendungs-Add-Ins deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Office Excel 2007, Office InfoPath 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anwendungs-Add-Ins mssen von einem vertrauenswrdigen Herausgeber signiert sein</td>
<td style="border:1px solid black;">Office Access 2007, Office Excel 2007, Office InfoPath 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
</tbody>
</table>
  
### Richtlinien zum Mindern von Bedrohungen durch Add-Ins
  
Beachten Sie die folgenden Richtlinien, um Bedrohungen durch Add-Ins zu verringern:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr Add-Ins innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Ziehen Sie in Betracht, es zur Auflage zu machen, dass alle Add-Ins von einem vertrauenswrdigen Herausgeber signiert sein mssen.  
-   Steuern Sie mithilfe des Office-Anpassungstoolkits, welche Herausgeber in der Liste vertrauenswrdiger Herausgeber enthalten sind.  
-   Erwgen Sie den Einsatz von Desktopsicherheitskontrollmechanismen, wie das Einschrnken von Benutzerberechtigungen fr das Betriebssystem, um Benutzer an der Installation von Add-Ins zu hindern.  
-   Wenn in einer Umgebung besonders hohe Sicherheitsanforderungen vorliegen, sollten Sie ein Deaktivieren aller Add-Ins in Erwgung ziehen. Diese Konfiguration wirkt sich mglicherweise auf die Nutzbarkeit aus, bietet aber uerst hohe Sicherheit.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Einstellungen zur Minderung von Bedrohungen durch ActiveX-Steuerelemente  
------------------------------------------------------------------------
  
Mithilfe von Einstellungen fr ActiveX-Steuerelemente kann die Funktionsweise von ActiveX-Steuerelementen gesteuert werden. Hierdurch lassen sich Risiken durch Bedrohungen und Angriffsmethoden verringern, die sich auf die Verfgbarkeit von Unternehmensdaten und -prozessen auswirken.
  
ActiveX-Steuerelemente werden in der Regel von Programmierern ausgenutzt, die schdlichen Code schreiben oder schdliche Programme zur Ausfhrung auf den Computern der Benutzer erstellen. Solche Steuerelemente werden oft ber Dokumente, E-Mail-Mitteilungen, Prsentationen und Tabellenkalkulationen verteilt.
  
ActiveX-Steuerelemente stellen fr Unternehmen jeder Gre ein potenzielles Risiko dar. Dieses potenzielle Risiko ist jedoch hher, wenn im Unternehmen Folgendes zugelassen wird:
  
-   Ausfhren von ActiveX-Steuerelementen  
-   Installieren von ActiveX-Steuerelementen  
-   Herunterladen von ActiveX-Steuerelementen
  
Bei der Standardeinstellung fr ActiveX-Steuerelemente knnen diese auf vier verschiedene Arten ausgefhrt werden, abhngig von den Eigenschaften des ActiveX-Steuerelements sowie den Eigenschaften des Dokuments, in dem das Steuerelement enthalten ist.
  
-   Wenn in der Registrierung ein Kill Bit fr ein ActiveX-Steuerelement festgelegt ist, wird das Steuerelement nicht geladen und kann unter keinen Umstnden geladen werden. Ein Kill Bit ist eine Funktion, mit der verhindert wird, dass Steuerelemente mit bekannten Exploits geladen werden.  
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das kein VBA-Projekt enthlt, und das ActiveX-Steuerelement als Sicher fr Initialisierung (Safe for Initialization, SFI) gekennzeichnet ist, wird das ActiveX-Steuerelement im abgesicherten Modus unter minimalen Einschrnkungen geladen (also mit permanenten Werten). Die Statusleiste wird nicht angezeigt, und der Benutzer sieht keine Informationen zum Vorhandensein von ActiveX-Steuerelementen in den Dokumenten. Alle ActiveX-Steuerelemente im Dokument mssen als SFI markiert sein, damit keine Mitteilung in der Statusleiste generiert wird.  
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das kein VBA-Projekt enthlt, und das Dokument ActiveX-Steuerelemente enthlt, die als unsicher fr die Initialisierung (Unsafe for Initialization, UFI) gekennzeichnet sind, wird der Benutzer in der Statusleiste darber informiert, dass ActiveX-Steuerelemente deaktiviert wurden. Wenn der Benutzer auf die Statusleiste klickt, wird ein Dialogfeld angezeigt, in dem der Benutzer die Mglichkeit hat, die ActiveX-Steuerelemente zu aktivieren. Wenn der Benutzer die ActiveX-Steuerelemente aktiviert, werden alle ActiveX-Steuerelemente (als SFI und UFI gekennzeichnete) unter minimalen Einschrnkungen geladen (also mit permanenten Werten).  
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das auch ein VBA-Projekt enthlt, wird in der Statusleiste eine Mitteilung angezeigt, dass ActiveX-Steuerelemente deaktiviert wurden. Wenn der Benutzer auf die Statusleiste klickt, wird er in einem Dialogfeld gefragt, ob die ActiveX-Steuerelemente aktiviert werden sollen. Aktiviert der Benutzer die ActiveX-Steuerelemente, werden alle ActiveX-Steuerelemente (als SFI und UFI gekennzeichnete) unter minimalen Einschrnkungen geladen (also mit permanenten Werten).
  
In der folgenden Tabelle sind die 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen durch ActiveX-Steuerelemente verringern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch Bedrohungen und Gegenmanahmen.
  
**Tabelle 4.3. Sicherheitseinstellungen zum Mindern von Bedrohungen durch ActiveX-Steuerelemente**

 
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
<td style="border:1px solid black;">ActiveX-Steuerelementinitialisierung</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Alle ActiveX-Steuerelemente deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Alle Benachrichtigungen fr Vertrauensstellungsleiste aus Sicherheitsgrnden deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Steuerelemente in Forms3 laden</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
</tbody>
</table>
  
### Richtlinien zur Minderung von Bedrohungen durch ActiveX-Steuerelemente
  
Beachten Sie die folgenden Richtlinien, um Bedrohungen durch ActiveX-Steuerelemente zu verringern:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr ActiveX-Steuerelemente innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Steuern Sie mithilfe des Office-Anpassungstoolkits, welche Herausgeber in der Liste vertrauenswrdiger Herausgeber enthalten sind.  
-   Lassen Sie Vorsicht walten, wenn Sie Dokumente mit ActiveX-Steuerelementen in vertrauenswrdigen Speicherorten ablegen. Diese Steuerelemente werden ohne Einschrnkungen und ohne Aufforderung an den Benutzer ausgefhrt.  
-   Wenn in einer Umgebung besonders hohe Sicherheitsanforderungen vorliegen, sollten Sie ein Deaktivieren aller ActiveX-Steuerelemente in Erwgung ziehen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Einstellungen zum Mindern von Bedrohungen durch externe Inhalte  
---------------------------------------------------------------
  
Mithilfe der Einstellungen fr externe Inhalte kann die Funktionsweise von Links zu externen Inhalten gesteuert werden. Hierdurch lassen sich Risiken durch Bedrohungen und Angriffsmethoden verringern, die sich auf die Verfgbarkeit von Unternehmensdaten und -prozessen auswirken.
  
Zu Bedrohungen ber externe Inhalte gehrt jede Angriffsmethode, bei der ein Dokument ber ein Intranet oder ein ffentliches Netzwerk wie das Internet mit einem anderen Dokument, einer Datenbank, einem Bild oder einer Website verknpft wird. Bedrohungen durch externe Inhalte werden in der Regel ber die folgenden Angriffsmethoden ausgenutzt:
  
-   Hyperlinks knnen ausgenutzt werden, indem Benutzer zu nicht vertrauenswrdigen Dokumenten oder Websites mit schdlichem Code oder Inhalt geleitet werden.  
-   Datenverbindungen knnen ausgenutzt werden, indem eine Verbindung zu beschdigten oder schdlichen Datenquellen oder Datenbanken hergestellt wird und Daten bswillig manipuliert oder extrahiert werden.  
-   Webbeacons ermglichen Angreifern ein Einbetten unsichtbarer Links in HTML-E-Mail-Nachrichten. Wenn ein Benutzer eine solche E-Mail-Nachricht ffnet, wird der Link aktiviert und ldt das Remotebild herunter. Dabei knnen Benutzerinformationen wie E-Mail-Adresse und IP-Adresse an den Remotecomputer gesendet werden.  
-   Paketobjekte sind eingebettete Objekte, die schdlichen Code ausfhren knnen.
  
Externe Inhalte stellen eine Bedrohung dar, wenn im Unternehmen folgende Praktiken gelten:
  
-   Benutzern wird uneingeschrnkter Zugriff auf ffentliche Netzwerke, z. B. das Internet, bereitgestellt.  
-   Der Empfang von E-Mail-Nachrichten, die eingebettete Bilder und HTML enthalten, durch Benutzer ist zugelassen.  
-   Die Verwendung von Datenverbindungen in Tabellenkalkulationen und anderen Dokumenten durch Benutzer ist zugelassen.
  
Standardmig trgt die 2007 Office-Version durch folgende Manahmen zur Abwehr von Bedrohungen bei:
  
-   Der Benutzer wird durch ein Dialogfeld mit einer Sicherheitswarnung darauf aufmerksam gemacht, dass er auf einen Link zu mglicherweise gefhrlichen Dateien klickt, darunter ausfhrbare Dateien, externe Office-Dokumente und Dateiverknpfungen zu TIF-Dateien.  
-   Der Benutzer wird durch ein Dialogfeld mit einer Sicherheitswarnung darauf aufmerksam gemacht, dass er auf einen Hyperlink klickt, der mglicherweise gefhrliche Protokolle verwendet. Bei unsicheren Protokollen handelt es sich um Protokolle, die Skripts oder Inhalt ausfhren, der potenziell unsicher ist. Zu diesen Protokollen gehren msn, nntp, mms, outlook und stssync.  
-   In PowerPoint sind Links zu externen Bilddateien deaktiviert, und in der Statusleiste wird erlutert, dass Referenzen zu externen Bildern blockiert wurden.  
-   In Excel sind Verbindungen zu externen Daten blockiert, und dem Benutzer wird die Statusleiste angezeigt.  
-   In Excel wird ein Dialogfeld mit einer Sicherheitswarnung angezeigt, wenn ein Benutzer ein automatisches Update fr eine Tabellenkalkulation ausfhrt, die Links zu Daten in anderen Tabellenkalkulationen enthlt.  
-   Wenn Benutzer die Blockierung eines Hyperlinks zu einem Office-Dokument aufheben, wird das Dokument innerhalb einer Office-Anwendung geffnet.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen durch externe Inhalte verringern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 4.4. Sicherheitseinstellungen zur Minderung von Bedrohungen durch externe Inhalte**

 
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
<td style="border:1px solid black;">Aktualisieren von automatischen Verknpfungen besttigen</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Profil automatisch basierend auf der primren SMTP-Adresse von Active Directory konfigurieren</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Automatisch Inhalt fr E-Mail von Personen in den Listen Sichere Absender und Sichere Empfnger herunterladen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Automatisches Empfangen kleiner Updates zur Verbesserung der Zuverlssigkeit</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr in InfoPath geffnete Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr in InfoPath-Editor-ActiveX geffnete Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Vertrauenswrdige Zonen blockieren</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verhalten der schrittweisen Aktualisierung von Windows SharePoint Services steuern</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Steuern des Verhaltens beim ffnen von Formularen in der Sicherheitszone Internet</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Steuern des Verhaltens beim ffnen von Formularen in der Sicherheitszone Intranet</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Steuern des Verhaltens beim ffnen von Formularen in der Sicherheitszone Vertrauenswrdige Sites</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Steuerelementbloggen</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DF-Optionen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Alle Benachrichtigungen fr Vertrauensstellungsleiste aus Sicherheitsgrnden deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Auf bekannte Lsungen berprfen deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Herunterladen von ClipArt und Medien vom Client und von der Office Online-Website deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Befehle deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Office Excel 2007, Office InfoPath 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Vom Kunden bermittelte Vorlagendownloads von Office Online deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hyperlinkwarnungen deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetfaxfeature deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Lsungen in der Sicherheitszone Internet deaktivieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Tastenkombinationen deaktivieren</td>
<td style="border:1px solid black;">Office Access 2007, Office Excel 2007, Office InfoPath 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herunterladen von Vorlagen vom Client und von der Office Online-Website deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Abrufen verffentlichter Hyperlinks vom Office Server durch den Office-Client deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Schulungskursdownloads von der Office Online-Website deaktivieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bilder und externen Inhalt in HTML-E-Mail anzeigen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herunterladen von Inhalt von sicheren Zonen nicht zulassen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Datenextrahierungsoptionen beim ffnen beschdigter Arbeitsmappen nicht anzeigen</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dokumentinformationsbereich fr Signal bertragende Elemente der Benutzeroberflche</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr E-Mail-Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hyperlinks in E-Mail-Nachrichten aktivieren</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internet in sichere Zonen fr den automatischen Download von Bildern einschlieen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Intranet in sichere Zonen fr den automatischen Download von Bildern einschlieen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internet- und Netzwerkpfade als Hyperlinks</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bilder von Webseiten laden, die nicht mit Excel erstellt wurden</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Onlineinhaltoptionen</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Blockierung des automatischen Downloads von verknpften Bildern aufheben</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Hyperlinks unterstreichen</td>
<td style="border:1px solid black;">Office Access 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Automatische Verknpfungen beim ffnen aktualisieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
</tbody>
</table>
  
### Richtlinien zur Verringerung von Bedrohungen ber externe Inhalte
  
Beachten Sie die folgenden Richtlinien, um Bedrohungen durch externe Inhalte zu verringern:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen zur Minderung von Bedrohungen durch externe Inhalte innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Fhren Sie Benutzerschulungen zu den Bedrohungen durch, die externe Inhalte fr ein Unternehmen darstellen knnen.  
-   Lassen Sie Vorsicht walten, wenn Sie Dokumente mit Links zu externen Inhalten in vertrauenswrdigen Speicherorten ablegen. Fr Dateien in vertrauenswrdigen Speicherorten werden keine Warnungen zu externen Inhalten in der Statusleiste angezeigt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Dateiblockierungstechnologie  
----------------------------
  
Die Microsoft Office Isolated Conversion Environment (MOICE)-Funktion und die Dateiblockierungsfunktionalitt in der 2007 Microsoft Office-Version sind so konzipiert, dass Kunden sich leichter vor Office-Dateien schtzen knnen, die mglicherweise schdliche Software enthalten, z. B. unaufgefordert aus bekannten oder unbekannten Quellen erhaltene Office-Dateien. MOICE bietet neue Risikominderungstechnologien, um bestimmte Microsoft Office-Datentypen zu konvertieren. Die Datenblockierungstechnologie stellt einen Mechanismus zur Verfgung, mit dem das ffnen bestimmter Office-Dateitypen gesteuert und blockiert werden kann.
  
MOICE verwendet den 2007 Microsoft Office System-Konverter, um Office 2003-Binrdokumente in das neuere Office Open XML-Format zu konvertieren. Wenn ein Benutzer ein Office 2003-Binrdokument ffnet, konvertiert MOICE es in das neue Office Open XML-Format und bergibt es dann zum ffnen an die entsprechende Anwendung. Zum Schutz gegen Sicherheitsrisiken, die whrend des Konvertierungsvorgangs auftreten knnen, wird MOICE mit einem eingeschrnkten Token ausgefhrt. Zusammenfassend gesagt, bietet MOICE einen Mechanismus, mit dem Kunden potenziell unsichere Office 2003-Binrdokumente vorverarbeiten knnen. Durch den Konvertierungsvorgang erhalten Kunden zustzliche Gewissheit, dass das Dokument als sicher angesehen werden kann.
  
Weitere Informationen zum Installieren und Aktivieren von MOICE finden Sie im Knowledge Base-Artikel 935865, [Beschreibung des Microsoft Office Isolated Conversion Environment-Updates fr das Compatibility Pack fr Word-, Excel- und PowerPoint 2007-Dateiformate](http://support.microsoft.com/kb/935865).
  
Die Dateiblockierungstechnologie umfasst eine Gruppe an Einstellungen, mit der Benutzer am ffnen oder Speichern bestimmter Dateitypen oder Dateiformate gehindert werden knnen. Mithilfe dieser Einstellungen lsst sich das Risiko von Zero-Day-Angriffen (Angriffe, die bisher unaufgedeckte oder nicht durch einen Patch behobene Sicherheitsrisiken ausnutzen) und anderen Bedrohungen und Angriffsmethoden verringern, die die Verfgbarkeit von Unternehmensdaten und -prozessen beeintrchtigen.
  
Wenn Benutzer versuchen, blockierte Dateitypen oder Dateiformate zu ffnen, evaluiert der Dateiblockierungsmechanismus die jeweilige Datei im Analysestadium (beim Laden der Datei), wodurch Dateityp und -format wesentlich genauer bestimmt werden knnen als durch einfaches berprfen der Dateinamenerweiterung. Aufgrund dieser Funktionalitt wirkt sich ein ndern der Dateinamenerweiterung einer Datei nicht auf den Blockierungsmechanismus aus. Wenn eine Datei beispielsweise im Office Word 2003-Binrformat mit einer DOC-Erweiterung gespeichert ist und Sie die Datei auf eine RTF-Erweiterung umbenennen, hindern die Einstellungen, die das ffnen von Word 2003-Binrdateien blockieren, den Benutzer am ffnen der Datei, obwohl diese eine RTF-Erweiterung aufweist.
  
Wenn Benutzer versuchen, Dateien mit einem blockierten Dateityp oder Dateiformat zu speichern, wird eine Fehlermeldung angezeigt, die besagt, dass versucht wird, eine Datei zu speichern, die vom Systemadministrator blockiert wurde. Die Fehlermeldung enthlt ebenfalls einen Link zum folgenden Knowledge Base-Artikel: [Fehlermeldung beim Versuch einen Dateityp zu ffnen oder zu speichern, der durch die Registrierungsrichtlinieneinstellungen in einem 2007 Office- oder Office 2003-Programm gesperrt wurde](http://go.microsoft.com/fwlink/?linkid=79656).
  
Durch die Dateiblockierungseinstellungen kann die Gefahr von Zero-Day-Angriffen verringert werden, die Sicherheitsrisiken ausnutzen. Dabei handelt es sich um eine besondere Art von Sicherheitsbedrohung, die mit einem Softwareupdate behoben werden kann, z. B. durch ein Microsoft-Sicherheitsbulletin oder ein Service Pack. Viele Angriffsmethoden knnen ein Sicherheitsrisiko darstellen, darunter:
  
-   Codeausfhrung von Remotestandorten aus  
-   Erhhung von Berechtigungen  
-   Offenlegung von Informationen
  
Bswillige Programmierer oder Benutzer knnen Sicherheitsrisiken durch eine Reihe von Sicherheitsangriffen ausnutzen. Bis zur Verffentlichung eines Sicherheitsbulletins oder eines Service Packs, durch das das Sicherheitsrisiko behandelt wird, stellt das Sicherheitsrisiko eine potenzielle Bedrohung fr das Unternehmen dar. Durch Implementieren der Dateiblockierungseinstellungen knnen Benutzer daran gehindert werden, bestimmte Dateien und Dateiformate zu ffnen, die ein Sicherheitsrisiko darstellen, bis ein Patch zur Behebung des Sicherheitsrisikos bereitgestellt wurde.
  
Standardmig knnen Benutzer alle Dateitypen und -formate ffnen und speichern. Die einzige Ausnahme liegt bei Dateien vor, die in einem Format lter als Word 6.0 gespeichert wurden. (Dateien, die mit einer Betaversion von Word 6.0 gespeichert wurden, werden als lter als das Word 6.0-Format angesehen und knnen standardmig nicht geffnet werden.)
  
In der folgenden Tabelle sind die 2007 Office-Einstellungen aufgefhrt, durch die sich Bedrohungen der Verfgbarkeit mithilfe von Dateiblockierungseinstellungen verringern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 4.5. Dateiblockierungseinstellungen zum Verringern von Bedrohungen der Verfgbarkeit**

 
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
<td style="border:1px solid black;">ffnen von Konvertern blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Binary 12-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Binrdateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Konvertern blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von DIF- und SYLK-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Dateien mit frherer Version als der folgenden blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer Excel 2007-Dateiformate blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von HTML- und XMLSS-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von HTML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen interner Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Open XML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Gliederungen blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer Excel 2007-Dateiformate ber das Compatibility Pack fr 2007 Office System und den Excel 2007-Konverter blockieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer PowerPoint 2007-Dateiformate ber das Compatibility Pack fr 2007 Office System und den PowerPoint 2007-Konverter blockieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer Word 2007-Dateiformate blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Vorabversionen neuer Word 2007-Dateiformate ber das Compatibility Pack fr 2007 Office System und den Word 97-2003/Open XML-Formatkonverter blockieren</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von RTF-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von Textdateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Word 2003-XML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ffnen von XLL-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von XML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von DIF- und SYLK-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von Binrdateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von Binary12-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von Konvertern blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von Grafikfiltern blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von HTML- und XMLSS-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von HTML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von Open XML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office PowerPoint 2007, Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von Gliederungen blockieren</td>
<td style="border:1px solid black;">Office PowerPoint 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von RTF-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Speichern von Textdateitypen blockieren</td>
<td style="border:1px solid black;">Office Excel 2007, Office Word 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Speichern von Word 2003-XML-Dateitypen blockieren</td>
<td style="border:1px solid black;">Office Word 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bestimmte Dateitypen als Anlagen fr Formulare blockieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dateien in diesem Format speichern</td>
<td style="border:1px solid black;">Office PowerPoint 2007, Office Word 2007</td>
</tr>
</tbody>
</table>
  
### Richtlinien zum Verwenden der Dateiblockierungstechnologie
  
Beachten Sie bei Verwendung der Dateiblockierungstechnologie die folgenden Richtlinien:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr die Dateiblockierung innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Wenn ein Dateityp in Ihrem Unternehmen nicht verwendet wird, sollten Sie Benutzer daran hindern, diesen Dateityp zu ffnen.  
-   Wenn ein Zero-Day-Exploit auftritt, bei dem ein bestimmter Dateityp verwendet wird, setzen Sie so lange die Dateiblockierung ein, um Benutzer am ffnen dieser Dateien zu hindern, bis ein Sicherheitspatch fr das Sicherheitsrisiko bereitgestellt werden kann.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Mindern von Bedrohungen durch Internet Explorer-Funktionen  
----------------------------------------------------------
  
Die 2007 Office-Version enthlt verschiedene Einstellungen, mit denen die sich Bedrohungen durch Internet Explorer verringern lassen. Diese Einstellungen werden als Internet Explorer-Funktionssteuerungseinstellungen bezeichnet und ermglichen ein Einschrnken des Internet Explorer-Verhaltens fr die einzelnen Anwendungen.
  
Bedrohungen durch Internet Explorer knnen auftreten, wenn eine Anwendung oder ein Dokument programmgesteuert Internet Explorer-Funktionalitt verwendet. Bedrohungen ber Internet Explorer stellen ein Risiko fr Anwendungen und Dokumente dar, da alle fr Internet Explorer bestehenden Bedrohungen gleichzeitig eine Bedrohung fr die Anwendung bzw. das Dokument sind, in denen Internet Explorer gehostet wird. Bedrohungen durch Internet Explorer drcken sich in zahlreichen Angriffsmethoden aus und knnen ber verschiedene Sicherheitsangriffe ausgenutzt werden. Beispiele fr diese Angriffsmethoden sind die Installation von ActiveX-Steuerelementen, MIME-Ermittlung, Zonenanhebung und die Installation von Add-Ons.
  
Internet Explorer stellt eine Bedrohung dar, wenn im Unternehmen folgende Praktiken gelten:
  
-   Die Ausfhrung von ActiveX-Steuerelementen, Add-Ins oder Makros, die Internet Explorer-Funktionalitt verwenden, durch Benutzer ist zugelassen.  
-   Es werden Office-Lsungen entwickelt und verteilt, die Internet Explorer-Funktionalitt beinhalten.
  
In der 2007 Office-Version knnen 15 Internet Explorer-Funktionssteuerungseinstellungen konfiguriert werden. Durch jede Einstellung wird eine besondere Art von Internet Explorer-Funktionalitt eingeschrnkt. Um die eingeschrnkte Funktionalitt fr eine bestimmte Einstellung zu aktivieren, mssen Sie die gewnschten Anwendungen dafr anmelden. Wenn eine Anwendung fr eine bestimmte Internet Explorer-Funktionsteuerungseinstellung angemeldet ist, wird das strker eingeschrnkte Verhalten der Einstellung durchgesetzt, wenn die Einstellung Internet Explorer hostet. Umgekehrt gilt: Wenn eine Anwendung fr eine bestimmte Internet Explorer-Funktionsteuerungseinstellung nicht angemeldet ist, wird das strker eingeschrnkte Verhalten der Einstellung nicht durchgesetzt, wenn die Einstellung Internet Explorer hostet.
  
Standardmig sind Office Outlook 2007 (Outlook.exe) und Office InfoPath 2007 (InfoPath.exe) fr alle 15 Internet Explorer-Funktionssteuerungseinstellungen angemeldet. Auerdem sind drei Office InfoPath 2007-Komponenten fr die 15 Internet Explorer-Funktionssteuerungseinstellungen angemeldet: Dokumentinformationsbereich, Workflowformulare und Drittanbieterhosting.
  
![](images/Dd443658.note(de-de,TechNet.10).gif) **Hinweis:**
  
Office InfoPath 2007 ist ein besonderer Fall und kann nicht fr einzelne Internet Explorer-Funktionssteuerungseinstellungen angemeldet bzw. abgemeldet werden. Sie knnen lediglich konfigurieren, welche Office InfoPath 2007-Komponenten fr die gesamte Gruppe von Internet Explorer-Funktionssteuerungseinstellungen angemeldet bzw. abgemeldet werden.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen durch Internet Explorer verringern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 4.6. Sicherheitseinstellungen zur Minderung von Bedrohungen durch Internet Explorer**

 
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
<td style="border:1px solid black;">Benutzer mit frheren Versionen von Office knnen mit Browsern lesen...</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr in InfoPath geffnete Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr in InfoPath-Editor-ActiveX geffnete Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Vertrauenswrdige Zonen blockieren</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">E-Mail-Formulare in der Sicherheitszone Voll vertrauenswrdig deaktivieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">E-Mail-Formulare in der Sicherheitszone Internet deaktivieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">E-Mail-Formulare in der Sicherheitszone Intranet deaktivieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ffnen von Lsungen in der Sicherheitszone Internet deaktivieren</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Herunterladen von Inhalt von sicheren Zonen nicht zulassen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Dokumentinformationsbereich fr Signal bertragende Elemente der Benutzeroberflche</td>
<td style="border:1px solid black;">2007 Office System</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Signal bertragende Elemente der Benutzeroberflche fr E-Mail-Formulare</td>
<td style="border:1px solid black;">Office InfoPath 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet in sichere Zonen fr den automatischen Download von Bildern einschlieen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Intranet in sichere Zonen fr den automatischen Download von Bildern einschlieen</td>
<td style="border:1px solid black;">Office Outlook 2007</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet- und Netzwerkpfade als Hyperlinks</td>
<td style="border:1px solid black;">Office Excel 2007</td>
</tr>
</tbody>
</table>
  
### Richtlinien zum Verringern von Bedrohungen ber Internet Explorer-Funktionen
  
Beachten Sie die folgenden Richtlinien, um Bedrohungen durch Internet Explorer-Funktionen zu verringern:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen fr Internet Explorer innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Vergewissern Sie sich, dass die im Windows Vista-Sicherheitshandbuch bzw. im Windows XP-Sicherheitshandbuch empfohlenen Internet Explorer-Einstellungen ebenfalls implementiert sind.  
-   Im [Handbuch zur Desktopsicherheit mit Internet Explorer 7](http://go.microsoft.com/fwlink/?linkid=100953) finden Sie weitere Informationen zum Schutz von Internet Explorer 7 (mglicherweise in englischer Sprache).
  
-   Machen Sie sich bewusst, dass andere Office-Anwendungen wie Office InfoPath 2007 Internet Explorer programmgesteuert hosten knnen.
  
    ![](images/Dd443658.note(de-de,TechNet.10).gif)**Hinweis:**
  
##### In diesem Beitrag
  
-   [berblick](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))  
-   [Kapitel 1: Sicherheit in der 2007 Office-Version](https://technet.microsoft.com/de-de/library/b9767904-ac34-4263-89e7-3c3e82eff607(v=TechNet.10))  
-   [Kapitel 2: Vertraulichkeitseinstellungen](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10))  
-   [Kapitel 3: Integrittseinstellungen](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10))  
-   Kapitel 4: Verfgbarkeitseinstellungen  
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
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443658.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10))5 von 6[![](images/Dd443658.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/6de5a362-72f8-4937-84ef-54ec91e040e6(v=TechNet.10)) |
