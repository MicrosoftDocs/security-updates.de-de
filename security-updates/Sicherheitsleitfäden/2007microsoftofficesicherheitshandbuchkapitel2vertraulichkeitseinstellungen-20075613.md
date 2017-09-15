---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 2: Vertraulichkeitseinstellungen'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 2: Vertraulichkeitseinstellungen'
ms:assetid: '5204bf0f-65b9-403e-9d94-958dbd1553e1'
ms:contentKeyID: 20075613
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443670(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch
=========================================

Kapitel 2: Vertraulichkeitseinstellungen
----------------------------------------

Verffentlicht: 11. Nov 2007

Vertraulichkeitseinstellungen tragen zur Minderung von Bedrohungen fr Informationen bei, die weder ffentlich noch privat bekannt gemacht werden sollten, z. B. E-Mail-Korrespondenz, Projektplanungsinformationen, Entwurfsspezifikationen, Finanzdaten, Kundendaten sowie persnliche bzw. private Daten.

Die 2007 Microsoft Office-Version bietet eine Reihe von Technologien und Einstellungen, mit denen sich Bedrohungen fr vertrauliche Informationen mindern lassen. Diese Technologien und Einstellungen werden nach den jeweils geminderten Bedrohungen in drei Hauptgruppen unterteilt.

-   **Datenschutzoptionen**. Diese Optionen tragen zum Schutz von persnlichen und privaten Informationen bei, darunter in Dateien enthaltene verborgene Informationen sowie ber ein Netzwerk bermittelte Daten.
-   **Verschlsselungseinstellungen**. Diese Einstellungen tragen zum Schutz von Daten bei, die in Dokumenten, Prsentationen und Tabellenkalkulationen erstellt und gespeichert wurden.
-   **Einstellungen zur Verwaltung von Informationsrechten (IRM)**. Diese Einstellungen helfen, per E-Mail gesendete Informationen zu schtzen.

![](images/Dd443670.important(de-de,TechNet.10).gif)**Wichtig:**

Neben der Bercksichtigung der in diesem Kapitel erluterten Einstellungen sollten Sie zudem sicherstellen, dass Ihre Computer zu jedem Zeitpunkt mit den neuesten Sicherheitspatches von Microsoft aktualisiert sind. Ein effektives Patchmanagement trgt entscheidend zur Verbesserung der Sicherheit in Unternehmen bei.

##### Auf dieser Seite

[Mindern von Bedrohungen fr den Datenschutz](#exd)
[Schutz von Informationen durch Verschlsselung](#esaac)
[Schutz von Informationen durch IRM](#eldac)

Mindern von Bedrohungen fr den Datenschutz
------------------------------------------

Zu Bedrohungen fr den Datenschutz gehren jegliche Bedrohungen oder Angriffsmethoden, die persnliche bzw. private Informationen ohne Zustimmung oder Wissen des Benutzers offenlegen. Bedrohungen fr den Datenschutz gefhrden die Vertraulichkeit von Daten, da persnliche und private Informationen in der Regel als vertraulich angesehen werden.

Bedrohungen fr den Datenschutz knnen mit verschiedenen Angriffsmethoden ausgenutzt werden. Bei den gngigsten Angriffsmethoden wird oftmals versucht, auf als Metadaten bezeichnete Dokumentdaten zuzugreifen. Zu Metadaten gehren beispielsweise Informationen wie Name des Autors, Name des Unternehmens, Bearbeitungszeit oder Versionsnummer des Dokuments. Jeder, der Zugriff auf das Dokument hat, kann auch auf die Metadaten zugreifen, sofern diese nicht aus einem Dokument entfernt wurden.

Bedrohungen fr den Datenschutz knnen ebenfalls ausgenutzt werden, wenn ein Dokument vertrauliche Daten enthlt, sei es im Text, in den Grafiken oder in zustzlichem Inhalt wie Kommentaren, Revisionen, Anmerkungen, benutzerdefinierten XML-Daten, verborgenem Text, Wasserzeichen sowie Kopf- und Fuzeileninformationen. Wenn diese zustzlichen Informationen nicht aus einem Dokument entfernt werden, hat jeder, der Zugriff auf das Dokument hat, ebenfalls Zugriff auf diese Inhalte.

Bisweilen besteht die Mglichkeit, durch Aktivieren oder Verwenden verschiedener Anwendungsfunktionen private Informationen offenzulegen. Diese Funktionen werden zwar nicht als Angriffsmethoden angesehen, sie knnen jedoch persnliche oder private Informationen, die das Unternehmen als vertraulich bzw. geschtzt einstuft, zugnglich machen. Wenn Sie beispielsweise zulassen, dass die 2007 Office-Version automatisch Updates fr das Onlinehilfesystem herunterldt, kann die IP-Adresse Ihres Computers offengelegt werden. Diese knnte als persnliche bzw. private Information angesehen werden.

Die meisten Unternehmen sind Bedrohungen fr den Datenschutz ausgesetzt und mchten eine aktive Rolle dabei spielen, die Offenlegung privater oder persnlicher Informationen zu steuern.

Weitere Informationen zum Datenschutz finden Sie in den [Datenschutzbestimmungen fr das 2007 Microsoft Office System](http://office.microsoft.com/en-us/products/fx101153491033.aspx).

Standardmig trgt die 2007 Office-Version zur Minderung verschiedener Bedrohungen fr den Datenschutz bei. Zu den Standardeinstellungen gehren die folgenden:

-   **Dokumentinspektor ist aktiviert**. Dokumentinspektor ist ein neues Tool, mit dem Benutzer Bedrohungen fr den Datenschutz mindern knnen, und zwar durch Entfernen von Metadaten, Revisionen, Kommentaren, benutzerdefinierten XML-Tags und anderen potenziell privaten und persnlichen Inhalten aus Dokumenten.

    ![](images/Dd443670.note(de-de,TechNet.10).gif)**Hinweis:**
    Dokumentinspektor ist erweiterbar und kann programmgesteuert gendert werden, um den Datenschutzanforderungen des Unternehmens durch Erstellen benutzerdefinierter Inspektormodule gerecht zu werden. Weitere Informationen finden Sie auf MSDN im Artikel ber das [Anpassen des Dokumentinspektors von 2007 Office System](http://go.microsoft.com/fwlink/?linkid=78577) (mglicherweise in englischer Sprache).

-   **Metadaten werden in einem verschlsselten Dokument geschtzt**. Wenn Benutzer Dokumente mithilfe der Kennwortschutzfunktion verschlsseln, werden die Metadaten im Dokument ebenfalls verschlsselt. Diese Einstellung gilt nur fr Dateien im Office Open XML-Format.
-   **Die Option zur Teilnahme am Programm zur Verbesserung der Benutzerfreundlichkeit ist standardmig deaktiviert**. Das Programm zur Verbesserung der Benutzerfreundlichkeit ermglicht Microsoft ein automatisches und anonymes Sammeln von Daten von den Benutzercomputern, beispielsweise die von der Software generierten Fehlermeldungen, die in den Computern installierte Hardware, ob beim Ausfhren von Microsoft-Software Schwierigkeiten auftreten und ob Hardware und Software gut und schnell reagieren.
-   **Die Option zum regelmigen Download einer Datei, mit der Systemprobleme bestimmt werden knnen, ist standardmig deaktiviert**. Diese Einstellung ermglicht Computern das Empfangen von Updates, mit denen die Anwendungszuverlssigkeit verbessert werden kann. Dabei wird erkannt, wenn Computer abstrzen oder instabil werden und das Microsoft Office-Diagnosetool ausgefhrt, um mglicherweise gefundene Probleme zu diagnostizieren und zu reparieren. Weiterhin wird Microsoft durch diese Einstellung ermglicht, Benutzer zum Senden von Fehlerberichten fr bestimmte Arten von angezeigten Fehlermeldungen aufzufordern.

In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich Bedrohungen fr den Datenschutz verringern lassen. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.

**Tabelle 2.1. Hilfreiche Sicherheitseinstellungen zur Minderung von Bedrohungen fr den Datenschutz**

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
<td style="border:1px solid black;"><p>Automatisches Empfangen kleiner Updates zur Verbesserung der Zuverlssigkeit</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Steuerelementbloggen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Auf bekannte Lsungen berprfen deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Herunterladen von ClipArt und Medien vom Client und von der Office Online-Website deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Befehle deaktivieren</p></td>
<td style="border:1px solid black;"><p>Office Access 2007, Excel 2007, InfoPath 2007, PowerPoint 2007 und Word 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Vom Kunden bermittelte Vorlagendownloads von Office Online deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Dokumentinformationsbereich deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Einschlieen von Dokumenteigenschaften in PDF- und XPS-Ausgabe deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Herunterladen von Vorlagen vom Client und von der Office Online-Website deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Schulungskursdownloads von der Office Online-Website deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Programm zur Verbesserung der Benutzerfreundlichkeit aktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ausgeblendeten Text</p></td>
<td style="border:1px solid black;"><p>Office Word 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Ausgeblendete Markups anzeigen</p></td>
<td style="border:1px solid black;"><p>Office PowerPoint 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Onlineinhaltoptionen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Hindert Benutzer am Hochladen von Dokumentvorlagen an die Office Online-Community.</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
</tbody>  
</table>
  
### Richtlinien zur Minderung von Bedrohungen fr den Datenschutz
  
Zur Minderung von Bedrohungen fr den Datenschutz in Ihrem Unternehmen sollten Sie die folgenden Richtlinien befolgen:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Einstellungen zur Minderung von Bedrohungen fr den Datenschutz innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Verwenden Sie Dateisystem- und Netzwerkzugriffssicherheit, um den unbefugten Zugriff auf Dokumente zu verhindern.  
-   Verschlsseln Sie Dokumente, die vertrauliche Informationen enthalten. Durch die Dokumentverschlsselung werden auch die mit dem Dokument verknpften Metadaten verschlsselt.  
-   Erwgen Sie vor dem Senden von Dokumenten an einen Empfnger den Einsatz von Dokumentinspektor, um Metadaten, Revisionen, Kommentare, benutzerdefinierte XML-Tags oder verborgene Dokumente zu entfernen. Diese Richtlinien sind nur erforderlich, wenn die Elemente vertrauliche Daten enthalten, die Empfnger nicht sehen sollen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Schutz von Informationen durch Verschlsselung  
---------------------------------------------
  
Die 2007 Office-Version bietet verschiedene Einstellungen, mit denen Sie die Art und Weise der Dokumentverschlsselung ndern knnen, wenn Benutzer die Verschlsselungsfunktion verwenden. Die Verschlsselungsfunktion ist nur in Office Access 2007, Office Excel 2007, Office PowerPoint 2007 und Office Word 2007 verfgbar.
  
Durch Verschlsselung lassen sich eine Vielzahl von Bedrohungen und Angriffsmethoden fr Dokumente mindern. Dokumentbedrohungen beinhalten Zugriffsversuche auf die Dokumente des Unternehmens bzw. die darin enthaltenen Informationen durch unbefugte Benutzer. Nicht autorisierter Zugriff auf Dokumente kann einen Verlust vertraulicher Daten die Dokumentdaten sind nicht lnger geschtzt sowie den Verlust von Inhalten zur Folge haben.
  
Die Dokumente der meisten Unternehmen sind Bedrohungen ausgesetzt, doch viele Unternehmen ergreifen keine ausreichenden Manahmen, um diese Bedrohungen zu mindern, da die Bedrohung entweder als minimal angesehen wird oder die Verwaltungskosten zum Verringern von Bedrohungen als zu hoch erachtet werden. Diese Auffassungen fhren oft zu unsicheren Praktiken und Situationen, beispielsweise den folgenden:
  
-   Die Netzwerksicherheitsarchitektur des Unternehmens kann Eindringlinge und Angreifer nicht vom Zugriff auf das interne Netzwerk abhalten. Dadurch erhht sich das Risiko, dass bswillige Benutzer Zugriff auf Unternehmensdokumente erlangen.  
-   Das Unternehmen hindert Benutzer nicht daran, proprietre Dokumente ber das Internet zu senden, zu empfangen oder freizugeben, beispielsweise Finanzdaten, Projektplne, Prsentationen oder Zeichnungen.  
-   Das Unternehmen hindert Benutzer nicht daran, Laptopcomputer mit ffentlichen Netzwerken zu verbinden. Dadurch erhht sich das Risiko eines Zugriffs nicht identifizierbarer Angreifer auf die Dokumente, die auf den Laptopcomputern von Benutzern gespeichert sind.  
-   Das Unternehmen hindert Benutzer nicht daran, Dokumente mit proprietren Informationen aus dem Bro zu entfernen.  
-   Es besteht die Mglichkeit, dass unbefugte Angreifer oder Eindringlinge Zugriff auf Dokumente mit proprietren Informationen erlangen.
  
In der 2007 Office-Version werden Dokumente nicht standardmig verschlsselt, und es gibt keine administrativen Einstellungen, die eine Verschlsselung von Dokumenten erzwingen. Sie knnen Bedrohungen fr Dokumente jedoch mindern, indem Benutzer fr die folgenden Anwendungen die Kennwortschutzfunktion zum Verschlsseln von Dokumenten verwenden: Office Excel 2007, Office PowerPoint 2007, Office Word 2007 und Datenbanken in Office Access 2007. Standardmig werden fr diese Anwendungen die folgenden Einstellungen verwendet, wenn Benutzer ein Dokument oder eine Datenbank verschlsseln:
  
-   Fr Office Access 2007-Datenbanken (.accdb) und Office Open XML-Dokumente auf dem Windows XP Professional-Betriebssystem ist der Kryptografiedienstanbieter (Cryptographic Service Provider, CSP) Microsoft Enhanced RSA und AES Cryptographic Provider. Der Kryptografiealgorithmus ist AES-128, und die Lnge des kryptografischen Schlssels betrgt 128 Bit.  
-   Fr Office Access 2007-Datenbanken und Office Open XML-Dokumente auf dem Windows Vista-Betriebssystem ist der CSP Microsoft Enhanced RSA und AES Cryptographic Provider. Der Kryptografiealgorithmus ist AES-128, und die Lnge des kryptografischen Schlssels betrgt 128 Bit.  
-   Excel-, PowerPoint- und Word-Dokumente, die im Office 97-2003-Format gespeichert sind, verwenden die Office 97/2000-kompatible Verschlsselungsmethode, eine proprietre Verschlsselungsmethode namens RC-40 40 Bit, die ber die Registrierung angepasst werden kann.
  
    ![](images/Dd443670.note(de-de,TechNet.10).gif) **Hinweis:**  
    AES-128 kann ber eine Registrierungseinstellung auf 256 Bit erhht werden.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich die Verschlsselung konfigurieren lsst. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 2.2. Hilfreiche Sicherheitseinstellungen fr die Konfiguration von Verschlsselung**

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
<td style="border:1px solid black;"><p>Kennwort zum ffnen der Benutzeroberflche deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RPC-Verschlsselung aktivieren</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Alle E-Mail-Nachrichten verschlsseln</p></td>
<td style="border:1px solid black;"><p>Office Outlook 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Verschlsselungstyp fr kennwortgeschtzte Office 97-2003-Dateien</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Verschlsselungstyp fr kennwortgeschtzte Office Open XML-Dateien</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Dokumentmetadaten fr kennwortgeschtzte Dateien schtzen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
</tbody>  
</table>
  
### Richtlinien zur Verwendung der Verschlsselung
  
Beachten Sie beim Einsatz von Verschlsselung in Ihrem Unternehmen die folgenden Richtlinien:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass Verschlsselungseinstellungen innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Verschlsseln Sie Dokumente, die vertrauliche Informationen enthalten.  
-   Bewerten Sie die verschiedenen Verschlsselungsalgorithmen, um zu bestimmen, welche fr Ihr Unternehmen geeignet sind. Fr unterschiedliche Dokumenttypen und Empfnger sind mglicherweise verschiedene Algorithmen angemessen.  
-   Erwgen Sie eine Verschlsselung von Dokumenten, die nicht ffentlich verfgbar sein sollten, aber ber ffentliche Netzwerke wie das Internet bertragen werden.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
Schutz von Informationen durch IRM  
----------------------------------
  
Die 2007 Office-Version stellt eine Reihe von Einstellungen fr die Verwaltung von Informationsrechten (Information Rights Management, IRM) zur Verfgung, mit denen sich vertrauliche Daten in Dokumenten schtzen lassen. IRM ist eine persistente Technologie auf Dateiebene, die Berechtigungen und Autorisierung einsetzt, um das Drucken, bermitteln oder Kopieren vertraulicher Daten durch nicht autorisierte Personen zu verhindern. Wenn der Zugriff auf ein Dokument oder eine Nachricht mithilfe dieser Technologie eingeschrnkt wird, werden diese Nutzungseinschrnkungen als Teil des Dateiinhalts mit dem Dokument bzw. der E-Mail weitergegeben.
  
IRM hilft IT-Managern bei der Durchsetzung bestehende Unternehmensrichtlinien in Bezug auf Dokumentvertraulichkeit, Workflow und E-Mail-Aufbewahrung. Fr CEOs und Sicherheitsbeauftragte reduziert IRM das Risiko, dass wichtige Unternehmensinformationen in die Hnde unbefugter Personen fallen, sei es durch Zufall, Gedankenlosigkeit oder bswillige Absicht. Auerdem werden in Windows Rights Management Server smtliche Rechte und Nutzungsdaten aller durch IRM geschtzten Dokumente protokolliert. Dadurch erhalten Sie Beweismaterial, mit dem die Einhaltung von Vorschriften zum Schutz vertraulicher Finanz- und Betriebsdaten nachgewiesen werden kann. Weiterhin wird ein Autorisierungsweg bereitgestellt, anhand dessen sich feststellen lsst, wer Zugriff auf bestimmte Informationen hatte, wann auf sie zugegriffen wurde usw.
  
Mithilfe von IRM-Untersttzung in der 2007 Office-Version knnen Bedrohungen fr die Vertraulichkeit von Dokumenten gemindert werden, indem die folgenden beiden Grundvoraussetzungen erfllt werden:
  
-   **Zugriffseinschrnkung fr vertrauliche Informationen**. IRM schtzt vertrauliche Informationen vor unbefugtem Zugriff und unbefugter Wiederverwendung. Unternehmen verlassen sich auf Firewalls, Schutzmanahmen fr eine sichere Anmeldung und andere Netzwerktechnologien, um vertrauliches geistige Eigentum zu schtzen. Eine grundlegende Einschrnkung dieser Technologien ist, dass autorisierte Benutzer oder schdliche, vom Benutzer ausgefhrte Software, die Informationen an unbefugte Personen weitergeben knnen. Diese Einschrnkung fhrt mglicherweise zu einer potenziellen Verletzung von Sicherheitsrichtlinien.  
-   **Schutz von Informationen**. Information Worker arbeiten oft mit vertraulichen Daten. Durch Einsatz von IRM brauchen sich diese Mitarbeiter nicht auf die Diskretion von anderen zu verlassen, um zu gewhrleisten, dass vertrauliche Daten das Unternehmen nicht verlassen. IRM schrnkt die Mglichkeiten von Benutzern ein, vertrauliche Informationen weiterzuleiten, zu kopieren oder zu drucken, da diese Funktionen in Dokumenten und Nachrichten mit eingeschrnkten Berechtigungen deaktiviert werden.
  
Ein Einsatz von IRM in Ihrem Unternehmen erfordert in der Regel Zugriff auf einen Rechteverwaltungsserver, auf dem Microsoft Windows Rights Management Services (RMS) fr Windows Server 2003 oder hher ausgefhrt wird. (IRM kann auch durch Verwendung von Microsoft Windows Live ID zur Authentifizierung von Berechtigungen eingesetzt werden.) Die Berechtigungen werden mithilfe von Authentifizierung durchgesetzt, normalerweise mit Active Directory. Wenn Active Directory nicht implementiert ist, knnen Benutzer mithilfe von Windows Live ID authentifiziert werden (die berprfung von Rechten und Nutzung ist allerdings nicht verfgbar, wenn die ffentliche RMS-Option ber Microsoft Windows Live ID verwendet wird).
  
Obwohl IRM in die 2007 Office-Version integriert ist, muss die erforderliche RMS-Clientsoftware separat installiert und konfiguriert werden, um mit RMS fr Windows Server 2003 oder hher bzw. mit dem Windows Live ID-Dienst im Internet zu funktionieren. Sie knnen den [Microsoft Windows Rights Management Services-Client](http://go.microsoft.com/fwlink/?linkid=76880) herunterladen, um Benutzern ein Ausfhren von Anwendungen zu ermglichen, durch die Rechte auf der Basis von RMS-Technologien eingeschrnkt werden.
  
Microsoft Office muss nicht installiert sein, um geschtzte Dokumente und Nachrichten lesen zu knnen. Das Rechteverwaltungs-Add-On fr Microsoft Internet Explorer (ein kostenloser Download von Microsoft) ermglicht Microsoft Windows-Benutzern mit den entsprechenden Berechtigungen das Lesen von E-Mail-Nachrichten und einigen Dokumenten mit eingeschrnkten Berechtigungen ohne Verwendung von Office-Software.
  
Standardmig sind Dokumente in der 2007 Office-Version nicht durch IRM geschtzt, und es gibt keine administrativen Einstellungen, mit denen Sie Benutzer zum Schtzen von Dokumenten mit IRM zwingen knnen. Sie knnen jedoch die Berechtigungsrichtlinien erstellen, die in Office-Anwendungen angezeigt werden. Beispielsweise knnten Sie eine Berechtigungsrichtlinie mit dem Namen **Firma (vertraulich)** aufstellen, die besagt, dass Dokumente oder E-Mail-Nachrichten nur von Benutzern innerhalb der Unternehmensdomne geffnet werden knnen. Wenn Benutzer eine solche Richtlinie implementieren (durch Klicken auf **Firma (vertraulich)** in der Office-Benutzeroberflche), wird das Dokument gem der Berechtigungsrichtlinie **Firma (vertraulich)** geschtzt. Sie knnen eine beliebige Anzahl von Berechtigungsrichtlinien erstellen.
  
In der folgenden Tabelle sind eine Reihe von 2007 Office-Einstellungen aufgefhrt, mit denen sich IRM konfigurieren lsst. Weitere Informationen zu spezifischen Einstellungen finden Sie im begleitenden Handbuch *Bedrohungen und Gegenmanahmen*.
  
**Tabelle 2.3. Hilfreiche Sicherheitseinstellungen fr die Konfiguration von IRM**

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
<td style="border:1px solid black;"><p>Benutzer mit frheren Versionen von Office knnen mit Browsern lesen...</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Gruppen in Office immer erweitern, wenn die Berechtigung fr Dokumente eingeschrnkt wird</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzer mssen zum berprfen der Berechtigung immer eine Verbindung herstellen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft Passport-Dienste fr Inhalt mit eingeschrnkter Berechtigung deaktivieren</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Verwaltung von Informationsrechten (IRM)</p></td>
<td style="border:1px solid black;"><p>Office InfoPath 2007</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer knnen nie Gruppen angeben, wenn die Berechtigung fr Dokumente eingeschrnkt wird</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzer knnen Berechtigungen fr Inhalte, deren Rechte verwaltet werden, nicht ndern</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Dokumentmetadaten fr Office Open XML-Dateien, deren Rechte verwaltet werden, schtzen</p></td>
<td style="border:1px solid black;"><p>2007 Office System</p></td>
</tr>  
</tbody>  
</table>
  
### Richtlinien zum Schutz von Informationen mit IRM
  
Beachten Sie die folgenden Richtlinien, um Informationen in Ihrem Unternehmen mit IRM zu schtzen:
  
-   Gewhrleisten Sie mithilfe der Gruppenrichtlinie, dass IRM-Einstellungen innerhalb des gesamten Unternehmens durchgesetzt werden.  
-   Schtzen Sie vertrauliche Informationen in E-Mail-Nachrichten, indem Sie Benutzer am Drucken, Kopieren, ndern und Weiterleiten dieser Informationen hindern.  
-   Schtzen Sie Office-Dokumente auf Benutzer- oder Gruppenbasis, je nach den vom Anwendungsbesitzer definierten Rechten.  
-   Verwenden Sie Dokumentablaufdaten. Nach Ablauf des Datums kann das Dokument lediglich vom Dokumentbesitzer geffnet werden.  
-   Verlassen Sie sich nicht darauf, dass IRM einen absoluten Schutz fr vertrauliche Daten bereitstellt. Benutzer knnen nach wie vor Informationen verbal weitergeben, handschriftlich kopieren bzw. fotografieren und diese an nicht befugte Benutzer weitergeben.
  
##### In diesem Beitrag
  
-   [berblick](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))  
-   [Kapitel 1: Sicherheit in der 2007 Office-Version](https://technet.microsoft.com/de-de/library/b9767904-ac34-4263-89e7-3c3e82eff607(v=TechNet.10))  
-   Kapitel 2: Vertraulichkeitseinstellungen  
-   [Kapitel 3: Integrittseinstellungen](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10))  
-   [Kapitel 4: Verfgbarkeitseinstellungen](https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10))  
-   [Kapitel 5: Entwerfen und Implementieren von Sicherheitseinstellungen](https://technet.microsoft.com/de-de/library/6de5a362-72f8-4937-84ef-54ec91e040e6(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um ber Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%c2%a0microsoft%20office-sicherheitshandbuch)
  
|                                                  |                                                                                                                                                                                                                                                                                                                                                                              |  
|--------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443670.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/b9767904-ac34-4263-89e7-3c3e82eff607(v=TechNet.10))3 von 6[![](images/Dd443670.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10)) |
