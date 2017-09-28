---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien'
ms:assetid: 'f3af8a5d-5067-4add-917b-f7ab8cdca16c'
ms:contentKeyID: 20075619
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443676(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen
=========================================================================

### Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3

Veröffentlicht: 11. Nov 2007

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgeführt.

#### Auf dieser Seite

[](#ecd)[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)
Informationen zu Benutzerrichtlinieneinstellungen
-------------------------------------------------

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle enthalten, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung sowie die empfohlene Konfiguration für EC- und SSLF-Umgebungen aufführt.

### Standarddateiformat

Betrifft: **Access**

Diese Einstellung steuert, ob neue Datenbankdateien im aktuellen Microsoft Office Access™ 2007-Format oder in einem von früheren Access-Versionen verwendeten Format erstellt werden.

#### Sicherheitsrisiko

Wenn Benutzer neue Datenbankdateien erstellen, speichert Access 2007 diese standardmäßig im aktuellen Access 2007-Format. Benutzer können diese Funktionalität ändern, indem sie auf die Office-Schaltfläche und dann auf **Access-Optionen** klicken und ein Dateiformat aus der Liste **Standarddateiformat** auswählen.

Eine neue Datenbank, die in einem ungeeigneten Format erstellt wurde, kann möglicherweise von einigen Benutzern nicht geöffnet oder verwendet werden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Administratoren angeben, ob neue Datenbankdateien standardmäßig im Access 2007- oder im Access 2002–2003-Format erstellt werden. Benutzer haben die Möglichkeit, die Standardeinstellung weiterhin außer Kraft zu setzen und beim Speichern von Dateien ein bestimmtes Format auszuwählen, können die Standardeinstellung aber nicht selbst über das Dialogfeld **Access-Optionen** einrichten.

![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn diese Einstellung **deaktiviert** ist, stehen Benutzern im Dialogfeld **Access-Optionen** drei Standarddateiformate zur Auswahl: Access 2000, Access 2002–2003 und Access 2007. Administratoren können mit dieser Einstellung entweder das Access 2002–2003- oder das Access 2007-Format, aber nicht das Access 2000-Format als Standardformat festlegen.

**Tabelle 1.80: Standarddateiformat**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Access 2007)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Access 2007)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1260</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert nicht, dass Benutzer ein anderes Dateiformat für eine neue Access-Datenbank auswählen. Sie sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft Excel Open XML-Arbeitsmappen erzwungen wird
  
Betrifft: **Excel**
  
Diese Einstellung steuert, ob verschlüsselte Makros in Open XML-Arbeitsmappen vor dem Öffnen mit Antivirensoftware überprüft werden müssen.
  
#### Sicherheitsrisiko
  
Wenn eine Office Open XML-Arbeitsmappe mit Rechten verwaltet wird oder kennwortgeschützt ist, werden alle in die Arbeitsmappe eingebetteten Makros gemeinsam mit den restlichen Inhalten der Arbeitsmappe verschlüsselt.
  
Standardmäßig werden diese verschlüsselten Makros deaktiviert, wenn sie nicht direkt vor dem Laden von Antivirensoftware überprüft werden. Wenn diese Standardkonfiguration geändert wird, verlangt Excel 2007 vor dem Laden verschlüsselter Makros keine Überprüfung. Excel verarbeitet die Makros entsprechend der Angaben in den Makrosicherheitseinstellungen von 2007 Office System. Dadurch werden möglicherweise unbemerkt Makroviren geladen, was zu einem Datenverlust oder einer verringerten Anwendungsfunktionalität führen kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, deaktiviert Excel 2007 verschlüsselte Makros, bis sie auf Viren überprüft wurden.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, kann die Sicherheit durch die Verwendung verschlüsselter, nicht auf Viren überprüfter Makros deutlich verringert werden. Mit Ausnahme von besonderen Situationen, in denen eine Echtzeitprüfung von Arbeitsmappendateien nicht möglich ist, sollte diese Einstellung **deaktiviert** werden.
  
**Tabelle 1.81: Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft Excel Open XML-Arbeitsmappen erzwungen wird**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">excel12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1308</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Excel 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft PowerPoint Open XML-Präsentationen erzwungen wird
  
Betrifft: **PowerPoint**
  
Diese Einstellung steuert, ob verschlüsselte Makros in Open XML-Präsentationen vor dem Öffnen mit Antivirensoftware überprüft werden müssen.
  
#### Sicherheitsrisiko
  
Wenn eine Office Open XML-Präsentation mit Rechten verwaltet wird oder kennwortgeschützt ist, werden alle in die Präsentation eingebetteten Makros gemeinsam mit den restlichen Inhalten der Präsentation verschlüsselt. Standardmäßig werden diese verschlüsselten Makros deaktiviert, wenn sie nicht direkt vor dem Laden von Antivirensoftware überprüft werden.
  
Wenn diese Einstellung **deaktiviert** ist, verlangt PowerPoint 2007 vor dem Laden verschlüsselter Makros keine Überprüfung. PowerPoint verarbeitet die Makros entsprechend der Angaben in den Makrosicherheitseinstellungen von 2007 Office System. Dadurch werden möglicherweise unbemerkt Makroviren geladen, was zu einem Datenverlust oder einer verringerten Anwendungsfunktionalität führen kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, deaktiviert PowerPoint 2007 verschlüsselte Makros, bis sie auf Viren überprüft wurden.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **deaktiviert** ist, kann die Sicherheit durch die Verwendung verschlüsselter, nicht auf Viren überprüfter Makros deutlich verringert werden. Mit Ausnahme von besonderen Situationen, in denen eine Echtzeitprüfung von Präsentationsdateien nicht möglich ist, sollte diese Einstellung **aktiviert** werden.
  
**Tabelle 1.82: Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft PowerPoint Open XML-Präsentationen erzwungen wird**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">ppt12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1142</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in PowerPoint 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft Word Open XML-Dokumenten erzwungen wird
  
Betrifft: **Word**
  
Diese Einstellung steuert, ob verschlüsselte Makros in Open XML-Dokumenten vor dem Öffnen mit Antivirensoftware überprüft werden müssen.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103498).
  
#### Sicherheitsrisiko
  
Wenn ein Office Open XML-Dokument mit Rechten verwaltet wird oder kennwortgeschützt ist, werden alle in das Dokument eingebetteten Makros gemeinsam mit den restlichen Inhalten des Dokuments verschlüsselt. Standardmäßig werden diese verschlüsselten Makros deaktiviert, wenn sie nicht direkt vor dem Laden von Antivirensoftware überprüft werden.
  
Wenn die Standardkonfiguration geändert wird, verlangt Word 2007 vor dem Laden verschlüsselter Makros keine Überprüfung. Word verarbeitet die Makros entsprechend der Angaben in den Makrosicherheitseinstellungen von 2007 Office System. Dadurch werden möglicherweise unbemerkt Makroviren geladen, was zu einem Datenverlust oder einer verringerten Anwendungsfunktionalität führen kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, deaktiviert Word 2007 verschlüsselte Makros, bis sie auf Viren überprüft werden.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **deaktiviert** ist, kann die Sicherheit durch die Verwendung verschlüsselter, nicht auf Viren überprüfter Makros deutlich verringert werden. Mit Ausnahme von besonderen Situationen, in denen eine Echtzeitprüfung von Dokumentdateien nicht möglich ist, sollte diese Einstellung **aktiviert** werden.
  
**Tabelle 1.83: Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft Word Open XML-Dokumenten erzwungen wird**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1280</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Word 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### DFÜ-Optionen
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, wie Outlook eine Verbindung zu DFÜ-Konten herstellt.
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer eine Verbindung zu ihren E-Mail-Servern über DFÜ-Netzwerke herstellen, wenn ihre Konten entsprechend konfiguriert sind. DFÜ-Verbindungen werden häufig von mobilen Benutzern verwendet, die sich von Remotestandorten mit dem Internet verbinden müssen. Remoteverbindungen unterliegen in der Regel nicht denselben Einschränkungen wie Unternehmensnetzwerkumgebungen und sind deshalb möglicherweise anfälliger für Angriffe.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren unter drei Optionen für Outlook 2007 eine oder mehrere Optionen auswählen:
  
-   **Vor dem Wechsel der DFÜ-Verbindung warnen**. Outlook zeigt eine Warnmeldung an, bevor ein Benutzer zu einer anderen als der bestehenden DFÜ-Verbindung wechselt.
  
-   **Verbindung nach dem Senden, Empfangen oder Aktualisieren trennen**. Outlook trennt die Verbindung nach Beenden einer manuellen Senden/Empfangen-Aktion durch den Benutzer automatisch.
  
-   **Bei einer Übermittlung im Hintergrund automatisch wählen**. Outlook wählt automatisch bei Durchführung einer Senden/Empfangen-Aktion im Hintergrund. Outlook sendet und empfängt E-Mail-Nachrichten, ohne ein Dialogfeld zu öffnen. Der Benutzer kann Outlook-Funktionen während der Senden/Empfangen-Aktion weiterhin verwenden.
  
**Tabelle 1.84: DFÜ-Optionen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\E-Mail-Setup</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">Outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Vor dem Wechsel der DFÜ-Verbindung warnen, Verbindung nach dem Senden, Empfangen oder Aktualisieren trennen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Vor dem Wechsel der DFÜ-Verbindung warnen, Verbindung nach dem Senden, Empfangen oder Aktualisieren trennen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1093, CCE-1599, CCE-1621, CCE-1269</td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die empfohlene Einstellung ist **Aktiviert** mit aktivierten Kontrollkästchen **Vor dem Wechsel der DFÜ-Verbindung warnen** und **Verbindung nach dem Senden, Empfangen oder Aktualisieren trennen**. Diese Konfiguration soll die Zeitdauer, für die der Computer eines Benutzers eine DFÜ-Verbindung unnötigerweise aufrechterhält, so kurz wie möglich halten und sicherstellen, dass der Computer nicht ohne Wissen des Benutzers online geht oder bleibt. Für die meisten Benutzer verursacht diese Einstellung vermutlich keine Nutzbarkeitsprobleme.
  
### Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung verhindert, dass 2007 Office-Benutzer auf Updates, Add-Ins und Patches auf der Office Online-Website zugreifen.
  
#### Sicherheitsrisiko
  
Mit dem Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website können Benutzer sicherstellen, dass ihre Computer auf dem neuesten Stand bleiben und mit den aktuellen Sicherheitspatches ausgestattet sind. Um aber sicherzugehen, dass Updates getestet sind und auf eine einheitliche Weise zugewiesen werden, führen viele Unternehmen Updates bevorzugt über einen zentralisierten Mechanismus wie Microsoft Systems Center oder Windows Server Update Services ein.
  
Standardmäßig können Benutzer Updates, Add-Ins und Patches von der Office Online Website herunterladen, um eine reibungslose und sichere Ausführung ihrer 2007 Office-Anwendungen zu gewährleisten. Wenn das Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Office Online verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn das Herunterladen von Updates zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird 2007 Office-Benutzern der Zugriff auf Updates, Add-Ins und Patches von der Office Online-Website verwehrt.
  
**Tabelle 1.85: Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">Office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1379</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für EC-Umgebungen ist **Nicht konfiguriert**. Diese Einstellung wirkt sich nicht auf die Funktionsweise für den Benutzer aus. Für SSLF-Umgebungen sorgt dagegen die Einstellung **Aktiviert** dafür, dass 2007 Office-Benutzern der Zugriff auf Updates, Add-Ins und Patches auf der Office Online-Website verwehrt wird. Wenn Sie die Einstellung aktivieren, sollten Sie sich vergewissern, dass Benutzer Sicherheitsupdates über einen alternativen Mechanismus wie Windows Server Update Services erhalten.
  
### Alle ActiveX-Steuerelemente deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung bestimmt, ob ActiveX-Steuerelemente deaktiviert werden.
  
#### Sicherheitsrisiko
  
Ein ActiveX-Steuerelement kann ein einfaches Textfeld oder ein komplexeres Objekt sein, beispielsweise eine spezielle Symbolleiste, ein vollständiges Dialogfeld oder eine kleine Anwendung. ActiveX-Steuerelemente werden auf Websites und in Anwendungen verwendet. ActiveX-Steuerelemente sind keine eigenständigen Programme und werden in einem Hostprogramm wie Internet Explorer und Microsoft Office-Programmen ausgeführt. ActiveX-Steuerelemente sind allerdings sehr leistungsstark, denn als COM-Objekte (Component Object Model) haben sie einen uneingeschränkten Zugriff auf den Computer, auf dem sie ausgeführt werden. ActiveX-Steuerelemente können auf das lokale Dateisystem zugreifen und die Registrierungseinstellungen des Betriebssystems ändern. Wenn ein Angreifer ein ActiveX-Steuerelement umfunktioniert, um einen Computer zu übernehmen, kann dies erhebliche Auswirkungen zur Folge haben.
  
Standardmäßig können Benutzer die Vertrauensebene für ActiveX-Steuerelemente im Vertrauensstellungscenter der 2007-Versionen von Microsoft Access, PowerPoint, Word und Excel einrichten. Die Standardkonfiguration lädt keine nicht vertrauenswürdigen ActiveX-Steuerelemente, sondern fordert den Benutzer über die Statusleiste auf zu entscheiden, ob das Steuerelement ausgeführt werden soll.
  
Wenn Benutzer sich für eine Ausführung aller Steuerelemente ohne Eingabeaufforderung und Einschränkung entscheiden, kann ein gefährliches Steuerelement ihre Computer gefährden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, initialisieren 2007 Office-Anwendungen keine ActiveX-Steuerelemente von nicht vertrauenswürdigen Standorten und geben keine Benachrichtigung über die Deaktivierung von ActiveX-Steuerelementen an den Benutzer aus.
  
**Tabelle 1.86: Alle ActiveX-Steuerelemente deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">Office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1242</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
ActiveX-Steuerelemente können zusätzliche Funktionalität in Dokumenten bereitstellen, sodass ihre Deaktivierung die Funktionalität für Benutzer verringern kann. Sie sollten Benutzer darüber informieren, dass diese Einstellung deaktiviert ist, da sie von der Anwendung nicht über die Deaktivierung von ActiveX-Steuerelementen benachrichtigt werden. Sie sollten sich vor der Aktivierung dieser Einstellung außerdem vergewissern, dass keine unternehmenswichtigen Funktionen durch ActiveX-Steuerelemente bereitgestellt werden.
  
### Alle Anwendungs-Add-Ins deaktivieren
  
Betrifft: **Access, Excel, InfoPath, PowerPoint, Word**
  
Diese Einstellung deaktiviert alle Add-Ins für die 2007-Versionen der angegebenen Office-Anwendungen.
  
#### Sicherheitsrisiko
  
Angreifer können Add-Ins für die Durchführung böswilliger oder schädlicher Aktionen wie das Verbreiten von Viren ausnutzen. Benutzer können über das Vertrauensstellungscenter Einschränkungen für Add-Ins festlegen. Beispielsweise können alle Add-Ins deaktiviert oder eine Signatur von einem vertrauenswürdigen Herausgeber verlangt werden.
  
Standardmäßig ist die Ausführung installierter und registrierter Add-Ins ohne Benachrichtigung an den Benutzer zugelassen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, sind alle Add-Ins für die 2007-Versionen der angegebenen Office-Anwendungen deaktiviert.
  
**Tabelle 1.87: Alle Anwendungs-Add-Ins deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Anwendungseinstellungen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, inf12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">Access: CCE-1238 Excel: CCE-1251 InfoPath: CCE-1135 PowerPoint: CCE-1204 Word: CCE-1681</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt möglicherweise zu erheblichen Beeinträchtigungen für Benutzer, die mit Add-Ins arbeiten. Wenn Benutzer für die 2007-Versionen der angegebenen Office-Anwendungen unternehmenswichtige Add-Ins installiert haben, können Sie diese Einstellung möglicherweise nicht aktivieren.
  
Aufgrund der Vielfalt dieser Einstellung führt der GPOAccelerator sowohl für die EC- als auch die SSLF-Umgebung keine Konfiguration durch. Die Einstellung „Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein“ ist für die SSLF-Umgebung aktiviert und sollte einen effektiven Schutz vor schädlichen Add-Ins bieten.
  
### Alle Benachrichtigungen für Vertrauensstellungsleiste aus Sicherheitsgründen deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen Benutzer bei Erkennung potenziell unsicherer Funktionen oder Inhalte benachrichtigen oder ob solche Funktionen und Inhalte automatisch ohne Benachrichtigung deaktiviert werden.
  
#### Sicherheitsrisiko
  
Die Statusleiste in 2007 Office-Anwendungen wird für die Identifizierung von Sicherheitsproblemen wie nicht signierte Makros oder potenziell unsichere Add-Ins verwendet. Werden solche Probleme erkannt, deaktiviert die Anwendung die unsicheren Funktionen oder Inhalte und zeigt oben im aktiven Fenster die Statusleiste an. Die Statusleiste informiert den Benutzer über die Art des Sicherheitsproblems und stellt ihm in einigen Fällen die Option bereit, die potenziell unsicheren Funktionen oder Inhalte zu aktivieren. Diese Aktivierung kann den Computer des Benutzers beschädigen.
  
Wenn eine 2007 Office-Anwendung ein Sicherheitsproblem erkennt, wird standardmäßig die Statusleiste angezeigt. Diese Konfiguration kann allerdings von Benutzern im Vertrauensstellungscenter geändert werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, zeigen 2007 Office-Anwendungen in der Statusleiste Informationen über automatisch blockierte Inhalte an.
  
**Tabelle 1.88: Alle Benachrichtigungen für Vertrauensstellungsleiste aus Sicherheitsgründen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1486</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung ändert die Standardkonfiguration nicht und dürfte daher keine Nutzbarkeitsprobleme verursachen.
  
### Alle vertrauenswürdigen Speicherorte deaktivieren
  
Betrifft: **Access, Excel, PowerPoint, Word**
  
Mit dieser Einstellung können Administratoren alle vertrauenswürdigen Speicherorte in den 2007-Versionen der angegebenen Office-Anwendungen deaktivieren.
  
#### Sicherheitsrisiko
  
Im Vertrauensstellungscenter angegebene vertrauenswürdige Speicherorte werden für die Festlegung von Dateispeicherorten verwendet, die als sicher betrachtet werden. Inhalte, Code und Add-Ins können mit minimalen Sicherheitsmaßnahmen aus vertrauenswürdigen Speicherorten geladen werden, ohne dass der Benutzer eine Eingabeaufforderung zur Genehmigung erhält. Wenn eine gefährliche Datei von einem vertrauenswürdigen Speicherort geöffnet wird, unterliegt sie nicht den Standardsicherheitsmaßnahmen und kann den Computer oder die Daten von Benutzern gefährden.
  
Standardmäßig werden die Dateien an vertrauenswürdigen (im Vertrauensstellungscenter angegebenen) Speicherorten als sicher betrachtet.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, werden alle vertrauenswürdigen Speicherorte in den 2007-Versionen der angegebenen Anwendungen ignoriert. Dazu zählen alle vertrauenswürdigen Speicherorte, die während des Office-Setups eingerichtet, über die Gruppenrichtlinie an Benutzer bereitgestellt oder von Benutzern selbst hinzugefügt wurden.
  
**Tabelle 1.89: Alle vertrauenswürdigen Speicherorte deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Anwendungseinstellungen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter\Vertrauenswürdige Speicherorte</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">Access: CCE-1520 Excel: CCE-1449 PowerPoint: CCE-782 Word: CCE-1637</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für EC-Umgebungen entspricht der Standardkonfiguration und sollte deshalb keine Nutzbarkeitsprobleme verursachen. Die empfohlene Einstellung für SSLF-Umgebungen dagegen deaktiviert vertrauenswürdige Speicherorte. Wenn unternehmenswichtige Gründe für den Zugriff auf einige Dateien in einer vertrauenswürdigeren Umgebung vorliegen, verursacht die Deaktivierung vertrauenswürdiger Speicherorte vermutlich Nutzbarkeitsprobleme.
  
### Alle Benutzeranpassungen der Symbolleiste für den Schnellzugriff deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer die Symbolleiste für den Schnellzugriff in den Anwendungen anpassen können, die diese verwenden.
  
#### Sicherheitsrisiko
  
Die Symbolleiste für den Schnellzugriff bietet 2007 Office-Benutzern einen komfortablen Zugriff auf häufig verwendete Befehle wie **Speichern** und **Rückgängig**.
  
Standardmäßig können Benutzer in den 2007-Versionen von Microsoft Access, Excel, Outlook (nur in den Fenstern zum Verfassen und Lesen von Nachrichten), PowerPoint und Word die Symbolleiste für den Schnellzugriff anpassen, indem sie Befehle hinzufügen oder entfernen. Durch das Laden von Vorlagen können ebenfalls Befehle hinzugefügt oder entfernt werden.
  
Ein Angreifer oder ein in einer Vorlage enthaltener Code kann die Symbolleiste für den Schnellzugriff möglicherweise ändern und die Nutzbarkeit beeinträchtigen. Der Symbolleiste können außerdem Verknüpfungen zu Makros mit schädlichem Code hinzugefügt werden. Auch wenn Sie andere Sicherheitsmaßnahmen treffen können, um die Ausführung von schädlichem Code zu verhindern, gewährleistet das Verhindern von Änderungen an der Symbolleiste für den Schnellzugriff eine gleichbleibende Funktionsweise für den Benutzer.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer und Vorlagen keine Änderungen an der Symbolleiste für den Schnellzugriff vornehmen.
  
**Tabelle 1.90: Alle Benutzeranpassungen der Symbolleiste für den Schnellzugriff deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Globale Optionen\Anpassen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-582, CE-1291, CCE-1326, CCE-1330, CCE-1335, CCE-1229</td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die empfohlene Einstellung entspricht der Standardkonfiguration und sollte sich deshalb nicht auf die Nutzbarkeit auswirken. Ziehen Sie die Aktivierung dieser Einstellung in spezifischen Situationen in Betracht, beispielsweise bei einer Bereitstellung an unbeaufsichtigte Kioske.
  
### Automatisches Wiederveröffentlichen deaktivieren
  
Betrifft: **Excel**
  
Mit dieser Einstellung können Administratoren die automatische Wiederveröffentlichungsfunktion in Excel 2007 deaktivieren.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Excel-Daten auf einer statischen Webseite veröffentlichen und die Funktion für das automatische Wiederveröffentlichen aktivieren, speichert Excel 2007 bei jedem Speichern der Arbeitsmappe eine Kopie der Daten an die Webseite. Wenn sich die Seite auf einem Webserver befindet, kann jede Person mit Zugriff auf die Seite nach jedem Speichervorgang die aktualisierten Daten sehen. Das führt möglicherweise zu einer unerwünschten Weitergabe vertraulicher oder falscher Informationen.
  
Wenn die Funktion für die automatische Wiederveröffentlichung aktiviert ist, wird standardmäßig bei jedem Speichern einer veröffentlichten Arbeitsmappe ein Meldungsdialogfeld angezeigt. Über dieses Dialogfeld kann der Benutzer die Funktion für das automatische Wiederveröffentlichen zeitweilig oder dauerhaft deaktivieren oder die Option **Diese Meldung nicht mehr anzeigen** aktivieren, damit das Dialogfeld nicht bei jedem Speichervorgang angezeigt wird. Wenn der Benutzer die Option **Diese Meldung nicht mehr anzeigen** aktiviert, veröffentlicht Excel die Daten weiterhin nach jedem Speichervorgang neu, ohne den Benutzer zu informieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, ist die Funktion für das automatische Wiederveröffentlichen deaktiviert. In diesem Fall müssen Excel 2007-Benutzer Daten manuell im Internet veröffentlichen.
  
**Tabelle 1.91: Automatisches Wiederveröffentlichen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Speichern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">excel12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1295</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn die Verwendung der Funktion zum automatischen Wiederveröffentlichen eine unternehmenswichtige Anforderung ist, können Sie die Einstellung möglicherweise nicht deaktivieren. In den meisten Situationen sollten Benutzer Daten aber auch manuell im Internet veröffentlichen können.
  
### „Auf bekannte Lösungen überprüfen“ deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung verhindert, dass die Microsoft Office-Diagnose Microsoft-Server auf Lösungen für Abstürze überprüft.
  
#### Sicherheitsrisiko
  
Die Microsoft Office-Diagnose sammelt bei Computerabstürzen relevante Diagnosedaten und fordert Benutzer auf, diese Daten an Microsoft zu übermitteln. Benutzer werden an eine Webseite weitergeleitet, die Informationen über den Absturz und, wenn möglich, Ratschläge zur Problemlösung und Vermeidung zukünftiger Abstürze bereitstellt. Alle Daten werden anonym an Microsoft übertragen und enthalten in Übereinstimmung mit den [Datenschutzbestimmungen](http://office.microsoft.com/en-us/products/fx101129941033.aspx) von Microsoft keine personenbezogenen Daten. Einige Unternehmen legen aber möglicherweise über Sicherheitsrichtlinien fest, dass Informationen über ihre Computer unter keinen Umständen extern übermittelt werden können.
  
Wenn eine 2007 Office-Anwendung abstürzt, gibt die Microsoft Office-Diagnose standardmäßig eine Eingabeaufforderung für Benutzer aus und stellt dann eine Verbindung zu Servern von Microsoft her, um Informationen über den Absturz zu übertragen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stellt die Office-Diagnosefunktion keine Verbindung zu den Servern von Microsoft her, um Informationen zu übertragen.
  
**Tabelle 1.92: „Auf bekannte Lösungen überprüfen“ deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Office-Diagnose</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1634</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn Sie eine Verbindung mit Servern von Microsoft für die Übertragung von Informationen über einen Absturz verhindern, erhalten Benutzer möglicherweise keine Informationen über Probleme. Solche Situationen können die Anzahl der Supportanfragen von Benutzern steigern, die ihre Probleme dann intern lösen müssen.
  
### Herunterladen von ClipArt und Medien vom Client und von der Office Online-Website deaktivieren
  
Betrifft: **2007 Office System**
  
Mit dieser Einstellung können Administratoren verhindern, dass 2007 Office-Benutzer ClipArt und andere Medien von Microsoft Office Online herunterladen.
  
#### Sicherheitsrisiko
  
Über Microsoft Office Online können Benutzer ClipArt und andere Medien wie Fotos, Filme und Sounds entweder über den Arbeitsbereich „ClipArt“ in Excel 2007, InfoPath 2007, Outlook 2007, PowerPoint 2007 und Word 2007 oder durch Aufrufen der Office Online-Website unter office.microsoft.com herunterladen.
  
Einige Unternehmen regeln möglicherweise über Sicherheitsrichtlinien, dass Benutzer Inhalte nur aus internen Quellen herunterladen können.
  
Standardmäßig ist der Download von Inhalten von der Office Online-Website für Benutzer zugelassen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer weder über die 2007 Office-Anwendungen noch durch Aufrufen der Office Online-Website ClipArt und andere Medien von Office Online herunterladen.
  
**Tabelle 1.93: Herunterladen von ClipArt und Medien vom Client und von der Office Online-Website deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1458</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn Benutzer keine Inhalte von Office Online herunterladen können, haben sie nur dann Zugriff auf ClipArt und andere Medien, wenn diese an einen zentralen Speicherort innerhalb des Unternehmens heruntergeladen und intern zur Verfügung gestellt werden.
  
### Befehle deaktivieren
  
Betrifft: **Access, Excel, InfoPath, PowerPoint, Word**
  
Mit dieser Einstellung können Administratoren bestimmte Befehle in den 2007-Versionen der angegebenen Office-Anwendungen deaktivieren.
  
#### Sicherheitsrisiko
  
Als funktionsreiche Produktivitätsanwendungen beinhalten die 2007 Microsoft Office-Anwendungen einige Befehle, die von unerfahrenen oder böswilligen Benutzern missbraucht werden können, um die Sicherheit zu beeinträchtigen, einen Datenverlust zu verursachen oder Computer zu beschädigen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren bestimmte Befehle in der Benutzeroberfläche der ausgewählten Anwendung deaktivieren.
  
Die Aktivierung dieser Einstellung im Ordner **Vordefiniert** für die ausgewählte Anwendung stellt eine vordefinierte Liste von Befehlen zur Verfügung, die Administratoren selektiv in der Benutzeroberfläche der Anwendung deaktivieren können. Die meisten Befehle in dieser Liste beziehen sich auf Funktionen, die eine relativ hohe potenzielle Auswirkung auf die Sicherheit haben können, darunter Makros, das Anpassen von Anwendungen, das Versenden von E-Mail-Nachrichten und so weiter.
  
Administratoren können im Ordner **Benutzerdefiniert** für die ausgewählten Anwendungen jeden Befehl mit einer Befehlsleisten-ID deaktivieren, einschließlich von Befehlen, die nicht in den vordefinierten Listen enthalten sind.
  
**Tabelle 1.94: Befehle deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, inf12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">Access: CCE-1370, CCE-1268, CCE-1400, CCE-1440, CCE-581, CCE-1480, CCE-1489, CCE-1392, CCE-1414, CCE-1418, CCE-1405, CCE-1550
Excel: CCE-1469, CCE-1473, CCE-1499, CCE-1024, CCE-1530, CCE-1120, CCE-1252, CCE-1151, CCE-1301, CCE-1310, CCE-1213, CCE-1362, CCE-1156, CCE-1429
InfoPath: CCE-1065, CCE-1361, CCE-1096, CCE-1391, CCE-1519, CCE-1523, CCE-1171, CCE-1457, CCE-1426, CCE-805, CCE-1453, CCE-1351, CCE-620, CCE-1017
PowerPoint: CCE-1327, CCE-1723, CCE-1366, CCE-1679, CCE-1173, CCE-1714, CCE-1485, CCE-1687, CCE-1709, CCE-1463
Word: CCE-1659, CCE-1329, CCE-1632, CCE-1425, CCE-1196, CCE-936, CCE-1354, CCE-1125, CCE-1742, CCE-1782, CCE-1306, CCE-1548</td>
</tr>
</tbody>
</table>
 

Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.

#### Auswirkung

Die Deaktivierung von Befehlen in den 2007-Versionen von Microsoft Office-Anwendungen kann die Funktionalität der Anwendungen entsprechend verringern. Berücksichtigen Sie vor der Deaktivierung von Befehlen die Anforderungen der Benutzer und wägen Sie diese gegen die Sicherheitsanforderungen des Unternehmens ab.

### Vom Kunden übermittelte Vorlagendownloads von Office Online deaktivieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob 2007 Office-Benutzer von der Community bereitgestellte Vorlagen von Office Online herunterladen können.

![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**

Aufgrund eines Problems, das in einigen Fällen zu einem Absturz von Office-Anwendungen führen kann, wenn Benutzer eine von Kunden bereitgestellte Vorlage herunterladen möchten und diese Einstellung aktiviert ist, legt der GPOAccelerator sowohl für EC- als auch SSLF-Umgebungen **Nicht konfiguriert** fest. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103506).

#### Sicherheitsrisiko

Benutzer von Excel 2007, PowerPoint 2007 und Word 2007 können Vorlagen aus dem Communitybereich der Microsoft Office Online-Website herunterladen, indem Sie auf **Neu** im Menü **Microsoft Office** klicken.

Standardmäßig können Benutzer von Microsoft Office-Benutzern weltweit bereitgestellte Communityvorlagen sowie von Microsoft und seinen Partnern entworfene Vorlagen herunterladen. Alle an Office Online hochgeladenen Vorlagen werden auf Viren und ihre Gültigkeit überprüft, bevor sie zum Download bereitgestellt werden. Das bedeutet, dass sie zunächst für eine bestimmte Anzahl Tage auf der Office Online-Website verfügbar sein und eine bestimmte Anzahl von Malen heruntergeladen werden müssen. (Darüber hinaus versetzt Office Online wichtige Vorlagen gelegentlich in einen vertrauenswürdigen Status, damit die besten Vorlagen von möglichst vielen Personen gesehen werden.)

Das Vertrauensstellungssystem soll sicherstellen, dass nur hochwertige Vorlagen zum Download über Office angeboten werden. Dennoch kann Microsoft nicht garantieren, dass die Vorlagen frei von Viren und Fehlern sind. Die Sicherheitsrichtlinien eines Unternehmens verhindern möglicherweise den Download von durch die Community bereitgestellten Vorlagen durch Benutzer.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Benutzer keine von der Community bereitgestellten Vorlagen von Office Online herunterladen. Der Zugriff auf Vorlagen, die von Microsoft und seinen Partnern veröffentlicht werden, ist nicht betroffen. (Wie bereits erwähnt, konfiguriert der GPOAccelerator die Einstellung aufgrund eines Fehlers, der zu Anwendungsabstürzen führen kann, allerdings nicht. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103506).)

**Tabelle 1.95: Vom Kunden übermittelte Vorlagendownloads von Office Online deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1533</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt zu geringen Beeinträchtigungen für 2007 Office-Benutzer, die von der Community bereitgestellte Vorlagen von Office Online herunterladen. Diese Benutzer werden über ihre Webbrowser auf die Office Online-Website zugreifen müssen, um von der Community bereitgestellte Vorlagen herunterzuladen.
  
### Dokumentinformationsbereich deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Excel 2007-, PowerPoint 2007- und Word 2007-Benutzer Dokumentinformationen im Dokumentinformationsbereich anzeigen können.
  
#### Sicherheitsrisiko
  
Der Dokumentinformationsbereich ersetzt das modale Dialogfeld **Eigenschaften** in früheren Versionen von Excel, PowerPoint und Word und ermöglicht Benutzern die Anzeige und Bearbeitung von Metadaten, die dem Dokument zugeordnet sind.
  
2007 Office-Entwickler können benutzerdefinierte Dokumentinformationsbereiche erstellen, um verschiedene für das Dokument oder das Unternehmen relevante Informationen aufzuzeichnen. Wenn diese Metadaten als vertraulich betrachtet werden, kann die Datensicherheit gefährdet sein, wenn ein Zugriff auf den Dokumentinformationsbereich durch Benutzer zugelassen wird.
  
Standardmäßig können Benutzer den Dokumentinformationsbereich anzeigen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, werden Formulare und Steuerelemente im Dokumentinformationsbereich nicht angezeigt. Wenn Benutzer den Bereich öffnen, wird er selbst zwar angezeigt, ist aber leer.
  
**Tabelle 1.96: Dokumentinformationsbereich deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Dokumentinformationsbereich</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1546</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Der GPOAccelerator führt standardmäßig keine Konfiguration für diese Einstellung für EC- oder SSLF-Umgebungen durch. Ziehen Sie die Aktivierung dieser Einstellung in besonderen Situationen in Betracht, die zusätzliche Sicherheitsmaßnahmen für die Metadaten von Dokumenten erfordern.
  
### Dynamisches Zwischenspeichern der Formularvorlage in InfoPath-E-Mail-Formularen deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob Vorlagen, die mit in InfoPath 2007 erstellten E-Mail-Formularen versendet werden, lokal zwischengespeichert werden.
  
#### Sicherheitsrisiko
  
Standardmäßig speichert InfoPath 2007 Formularvorlagen zwischen, wenn sie an ein E-Mail-Element angehängt sind, das als InfoPath-E-Mail-Formular erkannt wird. Wenn Benutzer Formulare ausfüllen, die mit einer eingeschränkten Sicherheitsstufe geöffnet werden, verwendet InfoPath die zwischengespeicherte Version der versendeten Vorlage statt einer veröffentlichten Version.
  
Um das Ausfüllen eines veröffentlichten Formulars durch Benutzer zu umgehen, kann ein Angreifer eine alternative Version des Formulars per E-Mail versenden, die Daten als Teil eines Phishingangriffs an den Absender zurücksenden würde und dazu eingesetzt werden könnte, Zugriff auf vertrauliche Daten zu erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, speichert InfoPath 2007 nicht die an das E-Mail-Element angehängte Formularvorlage, sondern die Formularvorlage vom veröffentlichten Speicherort zwischen.
  
**Tabelle 1.97: Dynamisches Zwischenspeichern der Formularvorlage in InfoPath-E-Mail-Formularen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1236</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung erfordert, dass eingeschränkte Formulare veröffentlicht werden müssen, anstatt nur per E-Mail versendet zu werden. Benutzer können Formulare weiterhin per E-Mail senden, allerdings muss die Formularvorlage am veröffentlichten Speicherort zur Verfügung stehen.
  
### E-Mail-Formulare in der Sicherheitszone „Voll vertrauenswürdig“ deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob InfoPath 2007 voll vertrauenswürdige E-Mail-Formulare öffnen kann.
  
#### Sicherheitsrisiko
  
InfoPath stellt drei Sicherheitsstufen für Formularvorlagen bereit: „Eingeschränkt“, „Domäne“ und „Voll vertrauenswürdig“. Die Sicherheitsstufen bestimmen, ob eine Formularvorlage auf Daten in anderen Domänen oder auf Dateien und Einstellungen auf Ihrem Computer zugreifen kann. Voll vertrauenswürdige Formulare haben die Sicherheitsstufe „Voll vertrauenswürdig“ und können auf Dateien und Einstellungen auf den Computern von Benutzern zugreifen. Die Formularvorlage für diese Formulare muss mit einem vertrauenswürdigen Stammzertifikat digital signiert oder auf dem Computer eines Benutzers installiert sein.
  
Standardmäßig kann InfoPath 2007 voll vertrauenswürdige E-Mail-Formulare öffnen. Wenn ein Angreifer ein gefährliches, voll vertrauenswürdiges E-Mail-Formular sendet, könnte dieses möglicherweise den Computer eines Benutzers beeinträchtigen oder dem Angreifer Zugriff auf vertrauliche Daten verschaffen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer voll vertrauenswürdige E-Mail-Formulare nicht öffnen. Stattdessen müssen diese Formulare in InfoPath 2007 geöffnet werden.
  
**Tabelle 1.98: E-Mail-Formulare in der Sicherheitszone „Voll vertrauenswürdig“ deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1567</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt möglicherweise zu einigen Beeinträchtigungen für Benutzer, die mit voll vertrauenswürdigen E-Mail-Formularen arbeiten. Um auf diese Formulare zugreifen zu können, müssen Benutzer veröffentlichte Versionen dieser Formulare in InfoPath 2007 öffnen.
  
### E-Mail-Formulare in der Sicherheitszone „Internet“ deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob aus dem Internet stammende E-Mail-Formulare geöffnet werden können.
  
#### Sicherheitsrisiko
  
InfoPath 2007-E-Mail-Formulare können von einem externen Angreifer entworfen und als Teil eines Phishingversuchs über das Internet versendet werden. Benutzer füllen solche Formulare möglicherweise aus und stellen dem Angreifer so vertrauliche Daten bereit.
  
Standardmäßig können aus dem Internet stammende Formulare zwar geöffnet werden, die Formulare können aber nicht auf Inhalte zugreifen, die in einer anderen Domäne gespeichert sind.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer E-Mail-Formulare aus dem Internet nicht öffnen.
  
**Tabelle 1.99: E-Mail-Formulare in der Sicherheitszone „Internet“ deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1170</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer aus dem Internet versendete E-Mail-Formulare nicht öffnen. Stattdessen müssen diese Formulare veröffentlicht und in InfoPath 2007 geöffnet werden.
  
### E-Mail-Formulare in der Sicherheitszone „Intranet“ deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob aus dem lokalen Intranet des Benutzers stammende E-Mail-Formulare geöffnet werden können.
  
#### Sicherheitsrisiko
  
InfoPath-E-Mail-Formulare können von einem internen Angreifer entworfen und über das lokale Intranet versendet werden. Benutzer füllen solche Formulare möglicherweise aus und stellen dem Angreifer so vertrauliche Daten bereit.
  
Standardmäßig können aus dem lokalen Intranet des Benutzers stammende E-Mail-Formulare geöffnet werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer E-Mail-Formulare aus dem lokalen Intranet nicht öffnen.
  
**Tabelle 1.100: E-Mail-Formulare in der Sicherheitszone „Intranet“ deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1316</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer aus dem lokalen Intranet versendete E-Mail-Formulare nicht öffnen. Stattdessen müssen diese Formulare veröffentlicht und in InfoPath 2007 geöffnet werden.
  
### E-Mail-Formulare deaktivieren, die mit der eingeschränkten Sicherheitsstufe ausgeführt werden
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob E-Mail-Formulare geöffnet werden können, die auf der Sicherheitsstufe für eingeschränkten Zugriff ausgeführt werden.
  
#### Sicherheitsrisiko
  
Mit der Sicherheitsstufe für eingeschränkten Zugriff ausgeführte InfoPath 2007-Formulare können nur auf Daten zugreifen, die in den Formularen gespeichert sind. Ein böswilliger Benutzer könnte jedoch ein E-Mail-Formular versenden, das mit der Sicherheitsstufe für eingeschränkten Zugriff ausgeführt wird, und versuchen, auf von Benutzern bereitgestellte vertrauliche Daten zuzugreifen.
  
Standardmäßig kann InfoPath 2007 E-Mail-Formulare öffnen, die mit der Sicherheitsstufe für eingeschränkten Zugriff ausgeführt werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer E-Mail-Formulare, die mit der Sicherheitsstufe für eingeschränkten Zugriff ausgeführt werden, nicht öffnen. Normalerweise wird diese Einstellung nur aktiviert, wenn Sie das Öffnen von E-Mail-Formularen vollständig verhindern möchten. Das bedeutet, dass die folgenden Einstellungen ebenfalls aktiviert werden müssten.
  
-   E-Mail-Formulare in der Sicherheitszone „Voll vertrauenswürdig“ deaktivieren
  
-   E-Mail-Formulare in der Sicherheitszone „Internet“ deaktivieren
  
-   E-Mail-Formulare in der Sicherheitszone „Intranet“ deaktivieren
  
**Tabelle 1.101: E-Mail-Formulare deaktivieren, die mit der eingeschränkten Sicherheitsstufe ausgeführt werden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1518</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer E-Mail-Formulare, die mit der Sicherheitsstufe für eingeschränkten Zugriff ausgeführt werden, nicht öffnen. Diese Formulare müssen veröffentlicht und in InfoPath 2007 geöffnet werden.
  
### Vollzugriff voll vertrauenswürdiger Lösungen auf den Computer deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob InfoPath 2007-Benutzer voll vertrauenswürdige Formulare öffnen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können InfoPath 2007-Benutzer auswählen, ob sie die Ausführung vertrauenswürdiger Formulare auf ihren Computern zulassen. Die Sicherheitsstufe „Voll vertrauenswürdig“ lässt den Zugriff auf lokale Systemressourcen wie COM-Komponenten oder Dateien auf den Computern von Benutzern durch Formulare zu und unterdrückt bestimmte Sicherheitsaufforderungen. Sie kann nur mit Formularen verwendet werden, die auf den Computern von Benutzern installiert sind oder eine mit einem vertrauenswürdigen Stammzertifikat digital signierte Vorlage verwenden.
  
Wie bei jedem Sicherheitsmodell, das vertrauenswürdigen Entitäten einen Betrieb mit geringeren Sicherheitskontrollmechanismen ermöglicht, könnte ein als voll vertrauenswürdig gekennzeichnetes Formular mit schädlichen Inhalten die Informationssicherheit gefährden oder die Computer von Benutzern beeinträchtigen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können InfoPath 2007-Benutzer als voll vertrauenswürdig gekennzeichnete Formulare nicht ausführen. Diese Konfiguration entspricht der Deaktivierung des Kontrollkästchens **Ausführung vollständig vertrauenswürdiger Formulare auf diesem Computer zulassen** in der Kategorie **Vertrauenswürdige Herausgeber** des Vertrauensstellungscenters.
  
**Tabelle 1.102: Vollzugriff voll vertrauenswürdiger Lösungen auf den Computer deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1114</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer als voll vertrauenswürdig gekennzeichnete Formulare nicht ausführen, selbst wenn diese nicht auf geschützte Systemressourcen zugreifen. Falls unternehmenswichtige Prozesse von der Ausführung voll vertrauenswürdiger InfoPath 2007-Formulare abhängen, können Sie diese Einstellung möglicherweise nicht aktivieren.
  
### Hyperlinkwarnungen deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen Benutzer über unsichere Hyperlinks benachrichtigen.
  
#### Sicherheitsrisiko
  
Unsichere Hyperlinks sind Links, die möglicherweise ein Sicherheitsrisiko darstellen, wenn Benutzer darauf klicken. Das Klicken auf einen unsicheren Link kann die Sicherheit vertraulicher Daten gefährden oder Computer von Benutzern beschädigen.
  
Zu den von 2007 Office als unsicher betrachteten Links zählen ausführbare Dateien, TIFF-Dateien und Microsoft Document Imaging (MDI)-Dateien. Darüber hinaus gelten Links als unsicher, die als unsicher betrachtete Protokolle verwenden, darunter msn, nntp, mms, outlook und stssync.
  
Standardmäßig benachrichtigen 2007 Office-Anwendungen Benutzer über unsichere Hyperlinks und deaktivieren diese, bis sie von den Benutzern aktiviert werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, können Hyperlinkwarnungen mit keinerlei Mitteln unterdrückt werden. 2007 Office-Benutzer werden über unsichere Links benachrichtigt und müssen diese manuell aktivieren, um sie benutzen zu können.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn die Einstellung **aktiviert** ist, werden Warnungen über unsichere Hyperlinks für alle Benutzer unterdrückt. Dadurch wird die Sicherheit möglicherweise wesentlich verringert. Mit Ausnahme von besonderen Umständen sollte diese Einstellung **deaktiviert** werden.
  
**Tabelle 1.103: Hyperlinkwarnungen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1623</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung entspricht der Standardkonfiguration und dürfte daher keine Nutzbarkeitsprobleme verursachen.
  
### Hyperlinks zu Webvorlagen über den Befehl „Neu“ im Menü „Datei“ und in Aufgabenbereichen deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer in 2007 Office-Anwendungen Hyperlinks zu Vorlagen auf Office Online folgen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer Vorlagen von Microsoft Office Online direkt in 2007 Office-Anwendungen herunterladen. In Access, Excel, PowerPoint und Word können Benutzer Vorlagen herunterladen, indem Sie auf die **Microsoft Office-Schaltfläche** und dann auf **Neu** klicken und eine der unter **Microsoft Office Online** oder **Aus Microsoft Office Online** aufgelisteten Kategorien auswählen. In InfoPath können Benutzer die Office Online-Vorlagendownloadseite öffnen, indem sie auf **Datei**, **Eine Formularvorlage entwerfen** und dann auf **Formulare auf Office Online** klicken.
  
Einige Unternehmen verfügen möglicherweise über Richtlinien, die das Herunterladen von Inhalten aus externen Quellen wie Office Online nicht zulassen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer Hyperlinks zu Vorlagen auf Office Online in 2007 Office-Anwendungen nicht folgen.
  
**Tabelle 1.104: Hyperlinks zu Webvorlagen über den Befehl „Neu“ im Menü „Datei“ und in Aufgabenbereichen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1166</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung ändert die Standardkonfiguration und verhindert, dass 2007 Office-Benutzer direkt auf Vorlagen von Office Online zugreifen können. Wenn Benutzer einen Zugriff auf einige dieser Vorlagen benötigen, müssen Sie diese innerhalb Ihres Unternehmens verfügbar machen.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Die Aktivierung dieser Einstellung verhindert nicht, dass Benutzer über ihren Webbrowser Vorlagen von der Office Online-Website herunterladen. Weitere Informationen über das Verhindern von Vorlagendownloads über Webbrowser finden Sie unter „Herunterladen von Vorlagen vom Client und von der Office Online-Website deaktivieren“ in diesem Handbuch.
  
### Einschließen von Dokumenteigenschaften in PDF- und XPS-Ausgabe deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Dokumentmetadaten in PDF- und XPS-Dokumenten gespeichert werden können.
  
#### Sicherheitsrisiko
  
Wenn die Add-Ins „Microsoft - Speichern als PDF“ oder „Microsoft - Speichern als XPS“ für 2007 Microsoft Office-Programme installiert sind, werden Dokumenteigenschaften standardmäßig als Metadaten gespeichert, wenn Benutzer Dateien über die Befehle **PDF oder XPS** oder **Als PDF oder XPS veröffentlichen** in Access 2007, Excel 2007, InfoPath 2007, PowerPoint 2007 und Word 2007 speichern. Das ist nur dann nicht der Fall, wenn die Option **Dokumenteigenschaften** im Dialogfeld **Optionen** deaktiviert ist. Wenn diese Metadaten vertrauliche Daten enthalten, kann das Speichern der Metadaten mit der Datei die Sicherheit gefährden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, werden Metadaten mit Dokumenteigenschaften nicht an PDF- und XPS-Dateien exportiert.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn die Einstellung **deaktiviert** ist, werden Metadaten mit Dokumenteigenschaften immer mit PDF- und XPS-Dateien gespeichert, und Benutzer können diese Einstellung nicht außer Kraft setzen. Diese Konfiguration kann die Sicherheit gefährden, wenn die Metadaten vertrauliche Daten enthalten.
  
**Tabelle 1.105: Einschließen von Dokumenteigenschaften in PDF- und XPS-Ausgabe deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Add-Ins „Microsoft - Speichern als PDF“ und „Microsoft - Speichern als XPS“</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1643</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer Metadaten mit Dokumenteigenschaften nicht an PDF- und XPS-Dateien exportieren. Wenn einige Benutzer diese Funktionalität als Teil eines unternehmenswichtigen Prozesses benötigen, kann die Einstellung für diese Benutzer möglicherweise nicht aktiviert werden.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Unabhängig von der Aktivierung dieser Einstellung sollten Sie in Betracht ziehen, die Benutzer über den Dokumentinspektor zu informieren. Der Dokumentinspektor hilft, vertrauliche Daten in Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen und Word 2007-Dokumenten zu finden und daraus zu entfernen. Weitere Informationen über den Dokumentinspektor finden Sie unter [Entfernen von ausgeblendeten Daten und persönlichen Informationen aus Office-Dokumenten](http://office.microsoft.com/en-us/help/ha100375931033.aspx).
  
### E-Mail-Formulare von InfoPath in Outlook deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob Outlook 2007 InfoPath-E-Mail-Formulare direkt oder als Anlage darstellt.
  
#### Sicherheitsrisiko
  
Angreifer können durch Versenden von InfoPath-E-Mail-Formularen versuchen, sich Zugriff auf vertrauliche Informationen zu verschaffen. Je nach Vertrauensstufe der Formulare kann außerdem ein automatischer Zugriff auf andere Daten möglich sein.
  
Standardmäßig verwendet Outlook 2007 die InfoPath-E-Mail-Formularfunktion zur Darstellung von Formularen in Outlook. Benutzer können diese Formulare dann direkt in Outlook ausfüllen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stellt Outlook 2007 InfoPath-Formulare in Form von E-Mail-Nachrichten mit Anlagen dar. Alle spezifischen Verhaltensweisen von InfoPath-E-Mail-Formularen werden in Outlook deaktiviert.
  
**Tabelle 1.106: E-Mail-Formulare von InfoPath in Outlook deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1265</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, stellt Outlook 2007 das Formular nicht direkt dar. Diese Konfiguration erfordert, dass Benutzer das Formular als Anlage öffnen, und verhindert, dass Benutzer Formularinformationen in einer Ordneransicht sehen, die die Formularverwaltungsfunktionalität in Outlook verringert. Sie verhindert jedoch nicht, dass Benutzer von Outlook auf InfoPath-Formulare zugreifen und diese ausfüllen.
  
### Internetfaxfeature deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung bestimmt, ob Benutzer in 2007 Office-Anwendungen auf die Internetfaxfunktion zugreifen können.
  
#### Sicherheitsrisiko
  
Excel 2007-, PowerPoint 2007- und Word 2007-Benutzer können mit der Internetfaxfunktion Dokumente über einen Internetfaxdienst-Anbieter an Faxempfänger senden. Wenn das Unternehmen über Richtlinien für die Regelung von Zeit, Ort oder Art und Weise des Faxversands verfügt, trägt diese Einstellung möglicherweise dazu bei, dass Benutzer diese Richtlinien umgehen.
  
Standardmäßig können 2007 Office-Benutzer die Internetfaxfunktion verwenden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Benutzer keine Internetfaxe versenden, und das Menüelement **Internetfax** wird aus dem Untermenü **Senden** des Microsoft Office-Menüs entfernt.
  
**Tabelle 1.107: Internetfaxfunktion deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Dienste\Fax</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1061</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn die Internetfaxfunktion für das Versenden von Faxen in Ihrem Unternehmen verwendet wird, führt die Aktivierung dieser Einstellung dazu, dass Benutzer diese Funktionalität verlieren. In solchen Situationen müssen Sie sicherstellen, dass Benutzern, die Faxe versenden müssen, ein anderer Mechanismus bereitgestellt wird.
  
### Microsoft Passport-Dienste für Inhalt mit eingeschränkter Berechtigung deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer geschützte Inhalte öffnen können, die mit einem authentifizierten Windows Live™ ID-Konto (früher Microsoft .NET Passport) erstellt wurden.
  
#### Sicherheitsrisiko
  
Die Funktion zur Verwaltung von Informationsrechten der 2007 Microsoft Office-Version ermöglicht Einzelpersonen und Administratoren die Angabe von Zugriffsberechtigungen für Word 2007-Dokumente, Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen und Outlook 2007-E-Mail-Nachrichten. Diese Funktion trägt dazu bei, das Drucken, Weiterleiten oder Kopieren vertraulicher Daten durch nicht autorisierte Personen zu verhindern. Benutzer schützen Inhalte mit digitalen Zertifikaten, die sie über die Windows-Rechteverwaltungsdienste (RMS) oder ein Windows Live ID-Konto (früher Microsoft .NET Passport) erhalten.
  
Wenn ein Benutzer eine mit einer Windows Live ID erstellte Datei öffnet, deren Rechte verwaltet werden, stellt die Anwendung standardmäßig eine Verbindung zu einem Lizenzierungsserver her, um die Anmeldeinformationen des Benutzers zu überprüfen und eine Lizenz herunterzuladen, die die Zugriffsberechtigungen des Benutzers auf die Datei bestimmt. Wenn das Unternehmen über Richtlinien für die Regelung des Zugriffs auf externe Dienste wie Windows Live ID verfügt, lässt diese Funktion möglicherweise zu, dass Benutzer gegen diese Richtlinien verstoßen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer geschützte Inhalte, die mit einem Windows Live™ ID-Konto erstellt wurden, nicht öffnen.
  
**Tabelle 1.108: Microsoft Passport-Dienste für Inhalt mit eingeschränkter Berechtigung deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1237</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie verhindert, dass Benutzer geschützte Inhalte öffnen, die mit einem Windows Live ID-Konto erstellt wurden. Wenn Benutzer aus unternehmenswichtigen Gründen mit geschützten Inhalten dieser Art arbeiten müssen, kann diese Einstellung möglicherweise nicht aktiviert werden, ohne wesentliche Beeinträchtigungen zu verursachen. Benutzer, die nicht mit geschützten Inhalten arbeiten, sind von dieser Einstellung nicht betroffen.
  
### Öffnen von Lösungen in der Sicherheitszone „Internet“ deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob Benutzer InfoPath 2007-Lösungen aus einer Quelle in der Sicherheitszone „Internet“ öffnen können.
  
#### Sicherheitsrisiko
  
Angreifer können mithilfe von auf Websites im Internet veröffentlichten InfoPath 2007-Lösungen versuchen, Zugriff auf vertrauliche Daten von Benutzern zu erhalten.
  
Standardmäßig können Benutzer InfoPath-Lösungen öffnen, die keinen verwalteten Code von Quellen aus der Sicherheitszone „Internet“ enthalten, wie es im Dialogfeld **Internetoptionen** in Internet Explorer festgelegt ist.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, zeigt InfoPath 2007 eine Fehlermeldung an, wenn Benutzer versuchen, Lösungen aus der Sicherheitszone „Internet“ zu öffnen.
  
**Tabelle 1.109: Öffnen von Lösungen in der Sicherheitszone „Internet“ deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1105</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer keine InfoPath 2007-Lösungen öffnen, die sich in der Sicherheitszone „Internet“ befinden. Falls unternehmenswichtige Gründe für den Zugriff auf diese Lösungen durch Benutzer vorliegen, kann diese Einstellung entweder nicht aktiviert werden, oder die Websites mit der entsprechenden Lösung muss der Zone der vertrauenswürdigen Sites oder der lokalen Intranetzone hinzugefügt werden.
  
### Bestätigungs-Assistenten bei der ersten Ausführung deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzern bei der ersten Ausführung einer 2007 Microsoft Office-Anwendung ein Bestätigungs-Assistent angezeigt wird.
  
#### Sicherheitsrisiko
  
Standardmäßig wird der Bestätigungs-Assistent bei der ersten Ausführung einer 2007 Microsoft Office-Anwendung angezeigt. Benutzer erhalten so die Möglichkeit, sich für internetbasierte Dienste anzumelden, die die Nutzung von Office optimieren. Zu diesen Diensten zählen beispielsweise Microsoft Update, das Programm zur Verbesserung der Benutzerfreundlichkeit, die Office-Diagnose und die Online-Hilfe. Wenn das Unternehmen über Richtlinien für die Regelung der Verwendung solcher externen Ressourcen verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn die Anmeldung bei diesen Diensten zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird der Bestätigungs-Assistent bei der ersten Ausführung einer 2007 Microsoft Office-Anwendung nicht angezeigt.
  
**Tabelle 1.110: Bestätigungs-Assistenten bei der ersten Ausführung deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Datenschutz\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1615</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie verhindert, dass sich Benutzer bei den oben aufgelisteten Diensten anmelden können. Dadurch erhalten Benutzer allerdings keine aktuellen Programmupdates, Sicherheitskorrekturen und Hilfeinhalte. Wenn Sie diese Einstellung aktivieren, müssen Sie den Benutzern Updates über andere Methoden bereitstellen.
  
### Kennwort zum Öffnen der Benutzeroberfläche deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer Dokumenten Kennwörter hinzufügen können.
  
#### Sicherheitsrisiko
  
Wenn 2007 Office-Benutzer einem Dokument ein Kennwort hinzufügen, können andere Benutzer das Dokument nicht öffnen. Diese Funktion bietet eine zusätzliche Schutzstufe für Dokumente, die bereits durch Zugriffssteuerungslisten geschützt sind. Außerdem stellt sie ein Mittel für den Schutz von Dokumenten bereit, die nicht durch Sicherheitsmaßnahmen auf Dateiebene geschützt sind.
  
Standardmäßig können Benutzer Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen und Word 2007-Dokumenten Kennwörter hinzufügen, indem sie im Dialogfeld **Speichern** oder **Speichern unter** auf **Extras** und dann auf **Allgemeine Optionen** klicken und ein entsprechendes Kennwort für das Öffnen oder Ändern der Dokumente eingeben. Wenn diese Konfiguration geändert wird, können Benutzer keine Kennwörter im Dialogfeld **Allgemeine Optionen** eingeben, sodass Dokumente nicht durch ein Kennwort geschützt werden können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, werden die Kennwortfelder im Dialogfeld **Allgemeine Optionen** von 2007 Office-Anwendungen aktiviert und können nicht von Benutzern deaktiviert werden.
  
**Tabelle 1.111: Kennwort zum Öffnen der Benutzeroberfläche deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">Office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1083</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlenen Einstellungen erzwingen die Standardkonfiguration und wirken sich deshalb nicht auf Nutzbarkeit aus. Normalerweise sollten Sie diese Einstellung nicht aktivieren, weil Benutzer andernfalls ihren 2007 Office-Dateien keine Kennwörter hinzufügen können. Wenn Sie aber sicherstellen möchten, dass nur andere Methoden für den Schutz von Dateien verwendet werden, können Sie die Aktivierung dieser Einstellung in Betracht ziehen.
  
### Senden der Formularvorlage mit E-Mail-Formularen deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob Benutzer Formatvorlagen gemeinsam mit InfoPath 2007-E-Mail-Formularen versenden können.
  
#### Sicherheitsrisiko
  
Standardmäßig lässt InfoPath 2007 beim Versenden von E-Mail-Formularen das Anhängen von Formularvorlagen zu. Wenn Benutzer in E-Mail-Formularen enthaltene Formularvorlagen öffnen können, statt eine zwischengespeicherte und zuvor veröffentliche Version verwenden zu müssen, kann ein Angreifer eine schädliche Formularvorlage mit dem E-Mail-Formular versenden und sich Zugriff auf vertrauliche Daten verschaffen.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Die Formularvorlage wird nur dann direkt geöffnet, wenn das Formular mit einer eingeschränkten Sicherheitsstufe geöffnet wird. Andernfalls ist die Anlage tatsächlich ein Link zum veröffentlichten Speicherort.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer Formularvorlagen nicht als Anlage an E-Mail-Nachrichten von InfoPath 2007 versenden.
  
**Tabelle 1.112: Senden der Formularvorlage mit E-Mail-Formularen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1210</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, müssen Formularvorlagen vor Verwendung eines bestimmten Formulars an einem Netzwerkspeicherort veröffentlicht oder von Benutzern installiert werden. Diese Konfiguration wirkt sich möglicherweise auf die Nutzbarkeit aus, insbesondere wenn Sie häufig Einzelexemplare von Formularen verwenden.
  
### Senden von InfoPath 2003-Formularen als E-Mail-Formulare deaktivieren
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, wie mit InfoPath 2003 kompatible Formulare per E-Mail versendet werden.
  
#### Sicherheitsrisiko
  
Ein Angreifer kann mit InfoPath 2003-Formularen darauf abzielen, die Sicherheit eines Unternehmens zu gefährden. InfoPath 2003 hat keinen Veröffentlichungsspeicherort für E-Mail-Formulare geschrieben, was bedeutete, dass Formulare ohne einen entsprechenden veröffentlichten Speicherort geöffnet werden konnten.
  
Standardmäßig sendet InfoPath 2007 alle Formulare mithilfe der InfoPath-E-Mail-Formulare-Integration per E-Mail. Das gilt auch für Formulare, die im InfoPath 2003-Dateiformat erstellt wurden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, kann InfoPath 2007 keine mit InfoPath 2003 kompatiblen Formulare als integrierte E-Mail-Formulare versenden.
  
**Tabelle 1.113: Senden von InfoPath 2003-Formularen als E-Mail-Formulare deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\E-Mail-Formulare von InfoPath</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-884</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist und das Unternehmen InfoPath 2003-Formulare verwendet, können diese Formulare erst dann per E-Mail verteilt werden, wenn sie zu InfoPath 2007-Formulare aktualisiert wurden.
  
### Tastenkombinationen deaktivieren
  
Betrifft: **Access, Excel, InfoPath, PowerPoint, Word**
  
Mit dieser Einstellung können Administratoren bestimmte Tastenkombinationen in den angegebenen Office-Anwendungen deaktivieren.
  
#### Sicherheitsrisiko
  
Anwendungen in der 2007 Microsoft Office-Version verfügen über zahlreiche Tastenkombinationen, die Benutzern die Durchführung von Befehlen ohne Verwendung der Maus ermöglichen. Einige Angriffe können mithilfe von Tastenkombinationen ausgelöst werden und die Sicherheit wichtiger Informationen oder der Computerumgebung gefährden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren bestimmte Tastenkombinationen in den angegebenen Office-Anwendungen deaktivieren.
  
Die Aktivierung dieser Einstellung im Ordner „Vordefiniert“ für die angegebene Anwendung stellt eine vordefinierte Liste von Tastenkombinationen zur Verfügung, die Administratoren selektiv in der Benutzeroberfläche der Anwendung deaktivieren können. Die meisten Befehle in dieser Liste beziehen sich auf Funktionen, die möglicherweise eine starke Auswirkung auf die Sicherheit haben, darunter Makros, Hyperlinks und die Funktion „Suchen“.
  
Administratoren können im Ordner „Benutzerdefiniert“ für die angegebenen Anwendungen alle Tastenkombinationen deaktivieren, auch solche, die nicht in den vordefinierten Listen enthalten sind. Wenn ein von einer bestimmten Tastenkombination ausgelöster Angriff ermittelt wird, kann die Tastenkombination mit dieser Einstellung zeitweilig deaktiviert werden, bis das Problem durch einen Softwarepatch oder ein Update der Antivirensignatur behoben werden kann.
  
**Tabelle 1.114: Tastenkombinationen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Elemente in Benutzeroberfläche deaktivieren\Vordefiniert
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Elemente in Benutzeroberfläche deaktivieren\(Vordefiniert|Benutzerdefiniert)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, inf12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">Access: CCE-1075, CCE-709, CCE-1502
Excel: CCE-1182, CCE-1525, CCE-1547, CCE-1300
InfoPath: CCE-1021, CCE-1299, CCE-1197
PowerPoint: CCE-1467, CCE-1740, CCE-1780, CCE-1661
Word: CCE-1716, CCE-1597, CCE-1689, CCE-1570, CCE-1720</td>
</tr>
</tbody>
</table>
 

#### Auswirkung

Die Verwendung dieser Einstellungen zur Deaktivierung von Tastenkombinationen kann zu Beeinträchtigungen für Benutzer führen, die sich auf die betroffenen Tastenkombinationen verlassen. Ziehen Sie die Auswirkung auf die Umgebung in Betracht, bevor Sie Tastenkombinationen deaktivieren, besonders wenn es sich um beliebte Tastenkombinationen handelt. Denken Sie insbesondere darüber nach, ob Sie die Einstellungen „Benutzerdefiniert“ vielleicht nur in Reaktion auf spezifische und bekannte Bedrohungen verwenden sollten.

### Folienaktualisierung deaktivieren

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob Benutzer Folien in einer Präsentation mit ihren Gegenstücken in einer PowerPoint 2007-Folienbibliothek verknüpfen können.

#### Sicherheitsrisiko

PowerPoint 2007-Benutzer können Folieninhalte freigeben und wiederverwenden, indem sie einzelne Foliendateien an einem zentralen Speicherort in einer Folienbibliothek auf einem Server speichern, auf dem Office SharePoint Server 2007 läuft. Mit der Folienaktualisierungsfunktion können Benutzer eine Folie in einer Präsentation auf dem Computer eines Benutzers mit der Originalfolie verknüpfen, die sich in der Folienbibliothek auf dem Server befindet.

Jedes Mal, wenn ein Benutzer eine Präsentation mit einer freigegebenen Folie öffnet, gibt PowerPoint 2007 standardmäßig eine Benachrichtigung an den Benutzer aus, wenn die Folie aktualisiert wurde. Der Benutzer kann dann die Aktualisierung ignorieren, der veralteten Folie eine neue Folie anhängen oder die veraltete Folie durch die aktualisierte Folie ersetzen. In einigen Situationen kann das Aktualisieren einer Folie in einer Präsentation aus einer externen Quelle wie einer Folienbibliothek möglicherweise dazu führen, dass wichtige Informationen verloren gehen. Ein Angreifer könnte die Daten in der Folienbibliothek ändern, was sich auf Integrität aller Folienpräsentationen auswirkt, die von dieser Bibliothek abhängen.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, kann PowerPoint 2007 den Status einer Folie in einer Folienbibliothek nicht überprüfen, wenn eine Präsentation mit Folienaktualisierungsdaten geöffnet wird.

**Tabelle 1.115: Folienaktualisierung deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">ppt12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1731</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie verhindert, dass PowerPoint 2007-Benutzer Folienbibliotheken auf Folienaktualisierungen überprüfen können. Benutzer, die mit Folienbibliotheken verknüpfte Folien verwenden, müssen andere Mechanismen für die Aktualisierung der Folien in ihren Präsentationen verwenden. Benutzer, die nicht mit Folienbibliotheken arbeiten, sind von dieser Einstellung nicht betroffen.
  
### Manifestverwendung von SmartDocument aktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen eine Manifestdatei für das XML-Erweiterungspaket mit einem SmartDocument laden können.
  
#### Sicherheitsrisiko
  
Ein XML-Erweiterungspaket ist die Gruppe von Dateien, die ein SmartDocument in Excel 2007 und Word 2007 darstellt. Die für ein SmartDocument erforderliche Logik wird über ein XML-Erweiterungspaket bereitgestellt, für das eine oder mehrere Komponenten zusammengestellt werden. Diese Komponenten können beliebige Datentypen enthalten, darunter XML-Schemas, XSLTs (Extensible Stylesheet Language Transforms), DLLs (Dynamic Link Libraries) und Bilddateien sowie zusätzliche XML-, HTML-, Word-, Excel- und Textdateien.
  
Die Schlüsselkomponente zur Erstellung eines XML-Erweiterungspakets ist die Erstellung einer Manifestdatei für das XML-Erweiterungspaket. Mit der Erstellung dieser Datei geben Sie die Speicherorte aller Dateien, aus denen das XML-Erweiterungspaket zusammengestellt ist, sowie die erforderlichen Informationen an, die 2007 Office anweisen, wie die Dateien für das SmartDocument eingerichtet werden sollen. Das XML-Erweiterungspaket kann außerdem Informationen über die erforderliche Einrichtung von Dateien enthalten, beispielsweise wie ein vom XML-Erweiterungspaket erfordertes COM-Objekt installiert und registriert werden soll.
  
XML-Erweiterungspakete können verwendet werden, um schädlichen Code zu initialisieren und zu laden. Dadurch kann die Stabilität eines Computers beeinträchtigt und ein Datenverlust verursacht werden.
  
Standardmäßig können 2007 Office-Anwendungen eine Manifestdatei für das XML-Erweiterungspaket mit einem SmartDocument laden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Anwendungen keine XML-Erweiterungspakete mit SmartDocuments laden.
  
**Tabelle 1.116: Manifestverwendung von SmartDocument deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\SmartDocuments (Word, Excel)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-903</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Benutzer mit SmartDocuments arbeiten können. Wenn unternehmenswichtige SmartDocuments in Ihrem Unternehmen verwendet werden, ist die Deaktivierung dieser Einstellung möglicherweise nicht durchführbar.
  
### Herunterladen von Vorlagen vom Client und von der Office Online-Website deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer Dokumentvorlagen von Microsoft Office Online entweder über die Office Online-Website oder direkt in 2007 Office-Anwendungen herunterladen können.
  
#### Sicherheitsrisiko
  
Benutzer der 2007 Office-Version können Vorlagen von der Microsoft Office Online-Website herunterladen, indem sie im Menü „Microsoft Office“ oder „Datei“ in einigen Office-Anwendungen auf **Neu** klicken oder mit einem Webbrowser die Office Online-Website aufrufen. Vorlagen werden von Microsoft und Quellen in der Community bereitgestellt und können aktive Inhalte enthalten.
  
Einige Unternehmen regeln möglicherweise über Sicherheitsrichtlinien, dass Benutzer Inhalte nur aus internen Quellen herunterladen können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer Dokumentvorlagen von Office Online weder über 2007 Office-Anwendungen noch einen Webbrowser herunterladen.
  
**Tabelle 1.117: Herunterladen von Vorlagen vom Client und von der Office Online-Website deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1233</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung ändert die Standardkonfiguration und verhindert, dass Benutzer direkt auf Vorlagen von Office Online zugreifen können. Wenn Benutzer einen Zugriff auf einige dieser Vorlagen benötigen, müssen Sie diese innerhalb Ihres Unternehmens verfügbar machen.
  
### Abrufen veröffentlichter Hyperlinks vom Office Server durch den Office-Client deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen Office-Server abfragen können, um Listen veröffentlichter Links abzurufen.
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer von 2007 Office-Anwendungen Links zu Microsoft Office SharePoint Server-Sites in diesen Anwendungen sehen und verwenden. Administratoren konfigurieren veröffentlichte Links in Office-Anwendungen während der anfänglichen Bereitstellung und können Links im Rahmen des normalen Betriebsablaufs hinzufügen oder ändern. Diese Links werden beim Öffnen und Speichern von Dokumenten in diesen Anwendungen auf der Registerkarte **Meine SharePoint-Websites** der Dialogfelder **Öffnen**, **Speichern** und **Speichern unter** angezeigt. Links können gezielt erstellt werden, sodass sie nur für Benutzer angezeigt werden, die Mitglied bestimmter Zielgruppen sind.
  
Wenn sich eine böswillige Person Zugriff auf die Liste veröffentlichter Links verschafft, könnte sie die Links so verändern, dass sie auf nicht genehmigte Websites verweisen. Dadurch können vertrauliche Daten gefährdet werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Anwendungen einen Office-Server nicht nach veröffentlichten Links abfragen.
  
**Tabelle 1.118: Abrufen veröffentlichter Hyperlinks vom Office Server durch den Office-Client deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Servereinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1545</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer die Liste veröffentlichter Links nicht verwenden, um Dateien direkt in 2007 Office-Anwendungen zu öffnen und zu speichern. Das beeinträchtigt möglicherweise die Verwendung von SharePoint Server für die Zusammenarbeit an Dokumenten.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Diese Einstellung betrifft speziell Microsoft Office SharePoint Server. Die Windows SharePoint Services (WSS) sind nicht betroffen.
  
### Schulungskursdownloads von der Office Online-Website deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer Schulungs- und Übungsmaterialien von Microsoft Office Online herunterladen können.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103520).
  
#### Sicherheitsrisiko
  
Office Online bietet einen Schulungsbereich mit Dokumenten und Vorlagen für Schulungszwecke.
  
Einige Unternehmen verfügen möglicherweise über Sicherheitsrichtlinien, die den Zugriff auf Dokumente und Vorlagen aus externen Quellen verhindern.
  
Standardmäßig können Benutzer ausgewählter 2007 Office-Anwendungen Dokumente und Vorlagen aus dem Schulungsbereich der Microsoft Office Online-Website herunterladen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Benutzer keine Schulungsmaterialien von Office Online herunterladen.
  
**Tabelle 1.119: Schulungskursdownloads von der Office Online-Website deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1528</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung aktiviert ist, können Benutzer nicht auf Dokumente und Vorlagen im Schulungsbereich von Office Online zugreifen. Wenn Benutzer im Unternehmen Zugriff auf diese Dokumente und Vorlagen benötigen, müssen Sie diese intern zur Verfügung stellen.
  
### Benachrichtigung für Vertrauensstellungsleiste für nicht signierte Anwendungs-Add-Ins deaktivieren
  
Betrifft: **Access, Excel, InfoPath, PowerPoint, Word**
  
Diese Einstellung steuert, ob die angegebenen 2007 Office-Anwendungen Benutzer benachrichtigen, wenn nicht signierte Anwendungs-Add-Ins geladen werden, oder ob solche Add-Ins automatisch und ohne Benachrichtigung deaktiviert werden.
  
#### Sicherheitsrisiko
  
Wenn eine Anwendung so konfiguriert ist, dass alle Add-Ins von einem vertrauenswürdigen Herausgeber signiert sein müssen, werden standardmäßig alle von der Anwendung geladenen nicht signierten Add-Ins deaktiviert. Die Anwendung zeigt in diesem Fall oben im aktiven Fenster die Vertrauensstellungsleiste an. Die Vertrauensstellungsleiste enthält eine Meldung, die den Benutzer über das nicht signierte Add-In informiert.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, deaktivieren Anwendungen nicht signierte Add-Ins automatisch, ohne den Benutzer zu informieren.
  
**Tabelle 1.120: Benachrichtigung für Vertrauensstellungsleiste für nicht signierte Anwendungs-Add-Ins deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Anwendungseinstellungen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, inf12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">Access: CCE-1423
Excel: CCE-1422
InfoPath: CCE-1434
PowerPoint: CCE-743
Word: CCE-1333</td>
</tr>
</tbody>
</table>
 

#### Auswirkung

Diese Einstellung wird nur angewendet, wenn die 2007 Office-Anwendung so konfiguriert ist, dass alle Add-Ins von einem vertrauenswürdigen Herausgeber signiert sein müssen. Standardmäßig können Benutzer diese Voraussetzung in der Kategorie **Add-Ins** des Vertrauensstellungscenters für die Anwendung selbst konfigurieren. Um diese Voraussetzung zu erzwingen, müssen Sie die Einstellung **Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein** in der Gruppenrichtlinie aktivieren, damit Benutzer die Einstellung nicht selbst ändern können.

### Benutzeroberflächenerweiterung von Dokumenten und Vorlagen deaktivieren

Betrifft: **2007 Office System**

Diese Einstellung steuert, ob 2007 Office-Anwendungen einen in einem Dokument oder einer Vorlage enthaltenen benutzerdefinierten Benutzeroberflächencode laden.

#### Sicherheitsrisiko

Entwickler können in der 2007 Office-Version die Benutzeroberfläche mit Anpassungscode erweitern, der in einem Dokument oder einer Vorlage enthalten ist. Wenn der Anpassungscode von einem unerfahrenen oder böswilligen Entwickler geschrieben wurde, könnte er die Zugänglichkeit oder die Verfügbarkeit wichtiger Anwendungsbefehle einschränken. Darüber hinaus könnten Befehle hinzugefügt werden, die Makros mit schädlichem Code starten.

Standardmäßig laden 2007 Office-Anwendungen beim Öffnen eines Dokuments oder einer Vorlage jeden darin enthaltenen Anpassungscode für die Benutzeroberfläche.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Anwendungen in Dokumenten oder Vorlagen enthaltenen Benutzeroberflächen-Anpassungscode nicht laden.

![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**

Die Aktivierung dieser Einstellung verhindert nicht, dass Vorlagen Änderungen an der Symbolleiste für den Schnellzugriff vornehmen.

**Tabelle 1.121: Benutzeroberflächenerweiterung von Dokumenten und Vorlagen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Globale Optionen\Anpassen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-630, CCE-1154, CCE-1410, CCE-1432, CCE-1198, CCE-929</td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Entwickler Dokumente und Vorlagen für die Erweiterung der Benutzeroberfläche verwenden können. Einige Unternehmen erweitern die Benutzeroberfläche, um die Benutzerproduktivität zu steigern. Wenn das Unternehmen eine modifizierte Benutzeroberfläche verwendet, können Sie diese Einstellung möglicherweise nicht aktivieren. Manchmal ist nur für bestimmte Teams in einem Unternehmen eine veränderte Benutzeroberfläche erforderlich, sodass Sie die Einstellung für den Rest des Unternehmens aktivieren können.
  
### Benutzeranpassungen der Symbolleiste für den Schnellzugriff über die Benutzeroberfläche deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer die Symbolleiste für den Schnellzugriff über die Benutzeroberfläche der Anwendung anpassen können.
  
#### Sicherheitsrisiko
  
Die Symbolleiste für den Schnellzugriff wird in der Titelleiste des Fensters angezeigt und bietet Benutzern einen komfortablen Zugriff auf häufig verwendete Befehle wie „Speichern“ und „Rückgängig“. Wie bei den meisten konventionellen Symbolleisten in 2007 Office-Anwendungen können Benutzer die Symbolleiste für den Schnellzugriff anpassen, indem sie Befehle hinzufügen oder entfernen. Durch das Laden von Vorlagen können ebenfalls Befehle hinzugefügt oder entfernt werden.
  
Wenn Sie in Umgebungen, in denen mehrere Benutzer eine einzige Desktopumgebung gemeinsam nutzen (wie bei einem Kiosk), zulassen, dass Benutzer der Symbolleiste für den Schnellzugriff Schaltflächen hinzufügen oder aus dieser entfernen können, kann es zu Beeinträchtigungen für andere Benutzer kommen.
  
Standardmäßig wird die Symbolleiste für den Schnellzugriff in den 2007-Versionen von Access, Excel, Outlook (nur in den Fenstern zum Verfassen und Lesen von Nachrichten), PowerPoint und Word in der Titelleiste des Fensters neben der Microsoft Office-Schaltfläche angezeigt.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer die Symbolleiste für den Schnellzugriff nicht ändern, indem sie die Registerkarte **Anpassung** im Dialogfeld „Optionen“ der Anwendung benutzen oder mit der rechten Maustaste auf die Symbolleiste für den Schnellzugriff klicken. Vorlagen, die der Symbolleiste Befehle hinzufügen oder Befehle aus dieser entfernen, sind nicht betroffen.
  
**Tabelle 1.122: Benutzeranpassungen der Symbolleiste für den Schnellzugriff über die Benutzeroberfläche deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Globale Optionen\Anpassen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1344, CCE-723, CCE-1384, CCE-1159, CCE-1146, CCE-1542</td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Benutzer die Symbolleiste für den Schnellzugriff für ihre eigenen Zwecke anpassen, wodurch eventuell die Produktivität beeinträchtigt werden könnte.
  
Der GPOAccelerator konfiguriert diese Einstellung standardmäßig weder für EC- noch für SSLF-Umgebungen. Ziehen Sie die Aktivierung dieser Einstellung in spezifischen Situationen in Betracht, beispielsweise bei einer Bereitstellung an unbeaufsichtigte Kioske.
  
### Benutzereinträge in Serverliste deaktivieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer bei der Einrichtung eines Besprechungsarbeitsbereichs der Liste von SharePoint-Servern Einträge hinzufügen können.
  
#### Sicherheitsrisiko
  
Wenn Benutzer die Adressen von im Unternehmen nicht genehmigten Servern manuell eingeben, verwenden sie möglicherweise Server, die den Anforderungen an die Informationssicherheit des Unternehmens nicht entsprechen, sodass vertraulich Daten gefährdet sein können.
  
Bei der Erstellung eines Arbeitsbereichs können Benutzer standardmäßig einen Server aus einer von Administratoren bereitgestellten Standardliste auswählen oder die Adresse eines nicht aufgelisteten Servers manuell eingeben.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren zwei Optionen zur Verfügung, über die sie festlegen, ob Outlook 2007-Benutzer der Liste veröffentlichter Server Einträge hinzufügen können:
  
-   **Veröffentlichungsstandard, andere zulassen**. Diese Option ist die Standardkonfiguration in Outlook 2007.
  
-   **Veröffentlichungsstandard, andere nicht zulassen**. Diese Option verhindert, dass Benutzer Server in die Standardliste veröffentlichter Server einfügen können.
  
**Tabelle 1.123. Benutzereinträge in Serverliste deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Besprechungsarbeitsbereich</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Veröffentlichungsstandard, andere nicht zulassen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1041</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Veröffentlichungsstandard, andere nicht zulassen**. Wenn für Benutzer im Unternehmen eine legitime Notwendigkeit besteht, andere Server als die in der veröffentlichten Serverliste zu verwenden, müssen sie sich an den Administrator wenden.
  
### VBA für Office-Anwendungen deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen außer Access Microsoft Visual Basic® for Applications (VBA) verwenden können.
  
#### Sicherheitsrisiko
  
VBA könnte ebenfalls von unerfahrenen oder böswilligen Entwicklern zum Erstellen von schädlichem Code verwendet werden, der die Computer von Benutzern beschädigen bzw. die Vertraulichkeit, Integrität oder Verfügbarkeit von Daten beeinträchtigen kann.
  
Standardmäßig können die meisten 2007 Office-Anwendungen einschließlich Excel, Outlook, PowerPoint, Word und Access Visual Basic® for Applications (VBA)-Code ausführen, der Anwendungsvorgänge anpasst und automatisiert.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können die 2007-Versionen von Excel, Outlook, PowerPoint, Publisher, SharePoint Designer und Word keinen VBA-Code ausführen. VBA-bezogener Code oder entsprechende Dateien werden auf den Computern von Benutzern weder installiert noch davon entfernt.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Die Einstellung wirkt sich nicht auf VBA in Access 2007 aus. Da InfoPath 2007 kein VBA verwendet, ist die Anwendung von dieser Einstellung ebenfalls nicht betroffen.
  
**Tabelle 1.124: VBA für Office-Anwendungen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-116</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn wichtige Geschäftsprozesse von VBA-Code abhängig sind, der in Excel, Outlook, PowerPoint, Publisher, SharePoint Designer oder Word ausgeführt wird, müssen Sie entweder Alternativen zu diesen Geschäftsprozessen entwickeln oder können diese Einstellung nicht aktivieren.
  
### Anlagen der Ebene 1 anzeigen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 potenziell gefährliche Anlagen blockiert, die als Ebene 1 festgelegt sind.
  
#### Sicherheitsrisiko
  
Um Benutzer vor Viren und anderen schädlichen Dateien zu schützen, verwendet Outlook 2007 zwei Sicherheitsebenen, die als Ebene 1 und Ebene 2 festgelegt sind, um den Zugriff auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Potenziell schädliche Dateien können nach ihrer Dateierweiterung als diese zwei Ebenen klassifiziert werden. Alle anderen Dateitypen werden als sicher betrachtet.
  
Standardmäßig blockiert Outlook den Zugriff auf Dateien der Ebene 1 vollständig und erfordert vor dem Öffnen von Dateien der Ebene 2, dass Benutzer diese auf dem Datenträger speichern. Wenn diese Konfiguration geändert wird, können Benutzer potenziell gefährliche Anlagen öffnen. Das kann ihre Computer beeinträchtigen oder die Vertraulichkeit, Integrität und Verfügbarkeit von Daten gefährden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, werden Anlagen der Ebene 1 unter keinen Umständen angezeigt.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer Zugriff auf Anlagen vom Dateityp der Ebene 1 erhalten, indem sie die Anlagen wie bei Anlagen der Ebene 2 zuerst auf dem Datenträger speichern und dann öffnen. Diese Funktion kann die Sicherheit deutlich verringern.
  
**Tabelle 1.125: Anlagen der Ebene 1 anzeigen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1296</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die vollständige Liste der standardmäßig als Ebene 1 klassifizierten Dateitypen finden Sie in der Liste der [Anlagedateitypen, die von Outlook 2007 gesperrt werden](http://technet2.microsoft.com/office/en-us/library/bc667b4c-1645-42be-8dc0-af56dc11ef5b1033.mspx).
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Zur Anwendung dieser Einstellung müssen Sie außerdem die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Outlook 2007\\Sicherheit\\Sicherheitsformulareinstellungen\\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und die Option **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.
  
### Onlinestatus für Personennamen anzeigen
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, an welcher Stelle Benutzer Anwesenheitsinformationen für Kontakte und E-Mail-Empfänger sehen, wenn sie ein kompatibles Instant Messaging-Clientprogramm ausführen.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103517).
  
#### Sicherheitsrisiko
  
Outlook 2007 kann Anwesenheitsinformationen für Kontakte und E-Mail-Empfänger anzeigen, wenn Benutzer ein kompatibles Instant Messaging-Clientprogramm wie Microsoft Office Communicator oder Windows Live Messenger ausführen. Anwesenheitsinformationen werden als Symbol neben dem Namen der Personen angezeigt. Das Symbol zeigt an, ob diese Personen aktuell für Kommunikationszwecke verfügbar sind. Wenn Benutzer auf das Symbol klicken, wird ein Menü angezeigt, über das sie weitere Informationen finden und andere Aktionen durchführen können, etwa das Versenden einer Nachricht. Outlook kann Anwesenheitsinformationen an verschiedenen Stellen anzeigen, beispielsweise in den Kontakten, im Adressbuch und in den Benachrichtigungsfeldern eingehender und ausgehender E-Mail-Nachrichten.
  
Standardmäßig zeigt Outlook Anwesenheitsinformationen an verschiedenen Stellen an. Wenn Benutzer den Onlinestatus und weitere Anwesenheitsdetails von anderen sehen können, sind in einigen Fällen möglicherweise die Privatsphäre oder sensible Daten gefährdet.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen für die Konfiguration von Anwesenheitsindikatoren in Outlook 2007 zur Verfügung:
  
-   **Nie**. Anwesenheitsindikatoren werden an keiner Stelle in Outlook angezeigt.
  
-   **Überall, außer in den Feldern „An“ und „CC“**. Outlook zeigt Anwesenheitsindikatoren an verschiedenen Stellen wie den Kontakten und im Adressbuch an. In den Feldern „An“ und „CC“ von E-Mail-Nachrichten werden sie nur dann angezeigt, wenn der Mauszeiger auf den Namen einer Person zeigt.
  
-   **Überall**. Anwesenheitsindikatoren werden an allen möglichen Stellen in Outlook angezeigt, einschließlich der Felder **An** und **Cc** von eingegangenen Nachrichten. Diese Option ist die Standardkonfiguration in Outlook 2007.
  
**Tabelle 1.126: Onlinestatus für Personennamen anzeigen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Weitere\Personennamen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Nie)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1604</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung von **Nie** verhindert, dass Outlook 2007 Anwesenheitsindikatoren anzeigt. Benutzern wird es dadurch möglicherweise erschwert, andere zu kontaktieren oder deren Verfügbarkeit zu ermitteln. Die anderen Optionen werden für die meisten Benutzer vermutlich keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Die Aktivierung dieser Einstellung setzt die Einstellung „Maximale Onlinestatusebene für einen Personennamen festlegen“ außer Kraft, sodass Administratoren einschränken können, inwieweit Benutzer die Art und Weise der Onlinestatusanzeige ändern können. Weitere Informationen finden Sie im Eintrag für die Einstellung „Maximale Onlinestatusebene für einen Personennamen festlegen“ in diesem Handbuch.
  
### Bilder und externen Inhalt in HTML-E-Mail anzeigen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 nicht vertrauenswürdige Bilder und externe Inhalte in HTML-E-Mail-Nachrichten herunterlädt, ohne dass sich der Benutzer ausdrücklich für den Download entscheidet.
  
#### Sicherheitsrisiko
  
Böswillige E-Mail-Absender können HTML-Nachrichten mit eingebetteten *Webbeacons* versenden. Webbeacons sind Bilder und andere Inhalte von externen Servern, die verfolgen können, ob bestimmte Empfänger die Nachrichten öffnen. Durch Anzeige einer E-Mail-Nachricht mit einem Webbeacon wird bestätigt, dass die E-Mail-Adresse des Empfängers gültig ist, wodurch der Empfänger anfällig für zusätzliche Spam-Nachrichten und schädliche E-Mails wird.
  
Standardmäßig lädt Outlook nur dann externe Inhalte in HTML-E-Mail-Nachrichten und RSS-Elementen herunter, wenn die Inhalte als sicher betrachtet werden. Folgende Inhalte können in Outlook 2007 als sicher konfiguriert werden:
  
-   Inhalte in E-Mail-Nachrichten von Absendern und an Empfänger, die in den Listen der sicheren Absender und der sicheren Empfänger definiert sind
  
-   Inhalte von Websites aus der Internet Explorer-Sicherheitszone „Vertrauenswürdige Sites“
  
-   Inhalte von RSS-Elementen
  
-   Inhalte aus SharePoint-Diskussionsrunden
  
Benutzer können steuern, welche Inhalte als sicher betrachtet werden, indem sie die Optionen im Bereich **Automatischer Download** des Vertrauensstellungscenters ändern. Wenn die Standardblockierungskonfiguration von Outlook im Vertrauensstellungscenter oder über eine andere Methode außer Kraft gesetzt wird, zeigt Outlook externe Inhalte in allen HTML-E-Mail-Nachrichten an, auch solchen, die Webbeacons enthalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, lädt Outlook 2007 nur dann automatisch Inhalte von externen Servern herunter, wenn der Absender in der Liste der sicheren Absender aufgeführt ist. Empfänger können sich auf der Basis einzelner Nachrichten entscheiden, ob externe Inhalte von nicht vertrauenswürdigen Absendern heruntergeladen werden.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Gehen Sie bei der Konfiguration dieser Einstellung sorgfältig vor. Der Name dieser Einstellung und ihre Beschreibung in der ADM-Datei implizieren, dass die Einstellung automatische Downloads blockiert, obwohl tatsächlich das Gegenteil der Fall ist. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103523).
  
**Tabelle 1.127: Bilder und externen Inhalt in HTML-E-Mail anzeigen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen für den automatischen Download von Bildern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1133</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Anlagenvorschau in Outlook nicht zulassen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer Anlagen in E-Mail-Nachrichten in einer Vorschau anzeigen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer bestimmte Arten von E-Mail-Anlagen im Nachrichtenfenster oder im Lesebereich in einer Vorschau anzeigen, indem sie auf das Symbol für die Anlage klicken. Benutzer können Outlook 2007-Elemente, Word-Dokumente, PowerPoint-Präsentationen, Excel-Arbeitsblätter, Microsoft Visio®-Zeichnungen, Bilddateien und Textdateien in einer Vorschau anzeigen. Um Benutzer vor schädlichem Code zu schützen, werden in Anlagen eingebettete aktive Inhalte (wie Skripts, Makros und ActiveX-Steuerelemente) während einer Vorschau deaktiviert.
  
Wenn ein Sicherheitsrisiko ermittelt wird, das sich auf mindestens eine der angegebenen Dateien bezieht, können Sie das Unternehmen mithilfe dieser Einstellung vor Angriffen schützen, indem sie die Vorschau solcher Dateien durch Benutzer so lange verhindern, bis ein Sicherheitspatch verfügbar ist.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Benutzer Anlagen in Outlook 2007 nicht in einer Vorschau anzeigen. Stattdessen müssen Benutzer je nach Sicherheitseinstellungen die Anlage in der entsprechenden Anwendung anzeigen. Diese Konfiguration kann als Schutz vor theoretischen zukünftigen Zero-Day-Angriffen verwendet werden, die auf bestimmte Dateitypen abzielen.
  
**Tabelle 1.128: Anlagenvorschau in Outlook nicht zulassen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\E-Mail-Optionen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1192</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie kann zu geringen Beeinträchtigungen für Benutzer führen, die für gewöhnlich die Vorschaufunktion für Anlagen in Outlook 2007 verwenden. Diese Benutzer müssen Anlagen nun in ihren Standardanwendungen öffnen, um sie anzuzeigen.
  
### Das Erstellen, Beantworten oder Weiterleiten von Signaturen für E-Mail-Nachrichten nicht zulassen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer E-Mail-Signaturen definieren und verwenden können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer Signaturen in E-Mail-Nachrichten erstellen und verwenden. Benutzer können Nachrichten Signaturen manuell hinzufügen, aber auch Outlook so konfigurieren, dass Signaturen automatisch neuen Nachrichten, Antworten oder weitergeleiteten Nachrichten bzw. allen drei Nachrichtentypen hinzugefügt werden. Signaturen beinhalten in der Regel Details wie den Namen, den Titel, die Telefonnummern und den Standort des Benutzers. Wenn das Unternehmen über Richtlinien für die Regelung der Verteilung dieser Art von Informationen verfügt, kann die Verwendung von Signaturen dazu führen, dass einige Benutzer unabsichtlich gegen diese Richtlinien verstoßen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer Signaturen nicht automatisch an neue Nachrichten, Antworten oder weitergeleitete Nachrichten anhängen. Sie verhindert auch, dass Benutzer auf die Registerkarte **E-Mail-Signatur** des Dialogfelds für****Signaturen und Briefpapier zugreifen können, um Signaturen manuell hinzuzufügen.
  
**Tabelle 1.129: Das Erstellen, Beantworten oder Weiterleiten von Signaturen für E-Mail-Nachrichten nicht zulassen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\E-Mail-Format</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1419</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung entspricht der Standardkonfiguration von Outlook 2007 und sollte sich deshalb nicht auf die Nutzbarkeit auswirken.
  
### Ordner in anderen als Standardspeichern können nicht als Ordnerhomepages festgelegt werden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer Ordnerhomepages für Ordner in anderen Speichern als Standardspeichern definieren können.
  
#### Sicherheitsrisiko
  
Outlook 2007 ermöglicht Benutzern die Festlegung von Webseiten als Homepages für persönliche oder öffentliche Ordner. Wenn ein Benutzer auf einen Ordner klickt, zeigt Outlook die Homepage an, die der Benutzer diesem zugewiesen hat. Mit dieser Funktion können Sie leistungsfähige Anwendungen für öffentliche Ordner erstellen. Allerdings können in die Webseiten auch Skripts eingefügt werden, die auf das Outlook-Objektmodell zugreifen und Benutzer Sicherheitsrisiken aussetzen.
  
Standardmäßig lässt Outlook nicht zu, dass Benutzer Ordnerhomepages für Ordner in anderen Speichern als Standardspeichern definieren können. Wenn diese Konfiguration geändert wird, können Benutzer gefährliche Ordnerhomepages für Outlook-Datendateien (.pst) und andere nicht dem Standard entsprechende Speicher erstellen und darauf zugreifen, wodurch die Sicherheit der Benutzerdaten gefährdet wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer Ordnerhomepages für Ordner in anderen Speichern als Standardspeichern weder erstellen noch darauf zugreifen. Sie setzt alle Konfigurationsänderungen auf den Computern der Benutzer außer Kraft.
  
![](images/Dd443676.note(de-de,TechNet.10).gif) **Hinweis:**
  
Wenn diese Einstellung **deaktiviert** ist, können Benutzer Ordnerhomepages für Ordner in anderen als Standardspeichern erstellen und darauf zugreifen, auch wenn u. U. andere Einstellungen eine korrekte Funktionsweise der Seiten verhindern.
  
**Tabelle 1.130: Ordner in anderen als Standardspeichern können nicht als Ordnerhomepages festgelegt werden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Weitere\Erweitert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1494</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Weitere Informationen finden im Artikel über das [Konfigurieren der Sicherheit für Outlook 2007-Ordnerhomepages](http://technet2.microsoft.com/office/en-us/library/4cbc696f-72e6-4f57-970f-91dc568797111033.mspx?mfr=true) (möglicherweise in englischer Sprache).
  
### Outlook-Objektmodellskripts können nicht für öffentliche Ordner ausgeführt werden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 Skripts ausführt, die mit benutzerdefinierten Formularen oder Ordnerhomepages für öffentliche Ordner verknüpft sind.
  
#### Sicherheitsrisiko
  
Ordner können in Outlook 2007 mit benutzerdefinierten Formularen oder Ordnerhomepages verknüpft werden, die Skripts beinhalten, die auf das Outlook-Objektmodell zugreifen. Diese Skripts können den Ordnern und den darin enthaltenen Elementen Funktionen hinzufügen, doch stellen gefährliche Skripts auch ein Sicherheitsrisiko dar.
  
Standardmäßig ermöglicht Outlook die Ausführung von Skripts in benutzerdefinierten Formularen oder Ordnerhomepages für öffentliche Ordner. Wenn Benutzer bei der Verwendung öffentlicher Ordner unabsichtlich gefährliche Skripts ausführen, sind ihre Computer oder Daten möglicherweise gefährdet.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, kann Outlook 2007 keine mit öffentlichen Ordnern verknüpften Skripts ausführen. Die Aktivierung setzt außerdem alle Konfigurationsänderungen auf den Computern der Benutzer außer Kraft.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **deaktiviert** ist, führt Outlook automatisch alle mit benutzerdefinierten Formularen oder Ordnerhomepages für öffentliche Ordner verknüpften Skripts aus. Das kann die Sicherheit bedeutend verringern.
  
**Tabelle 1.131: Outlook-Objektmodellskripts können nicht für öffentliche Ordner ausgeführt werden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Weitere\Erweitert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1560</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn das Unternehmen benutzerdefinierte Formulare oder öffentliche Ordnerhomepages verwendet, die Skripts enthalten, kann die Aktivierung dieser Einstellung deren Funktionalität verringern oder sie unbrauchbar machen. Erwägen Sie, die öffentlichen Ordner des Unternehmens im Hinblick auf betroffene Elemente zu untersuchen, bevor Sie diese Einstellung aktivieren.
  
### Outlook-Objektmodellskripts können nicht für freigegebene Ordner ausgeführt werden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 Skripts ausführt, die mit benutzerdefinierten Formularen oder Ordnerhomepages für freigegebene Ordner verknüpft sind.
  
#### Sicherheitsrisiko
  
Ordner können in Outlook 2007 mit benutzerdefinierten Formularen oder Ordnerhomepages verknüpft werden, die Skripts beinhalten, die auf das Outlook-Objektmodell zugreifen. Diese Skripts können den Ordnern und den darin enthaltenen Elementen Funktionen hinzufügen, doch stellen gefährliche Skripts auch ein Sicherheitsrisiko dar.
  
Standardmäßig lässt Outlook die Ausführung von Skripts in benutzerdefinierten Formularen oder Ordnerhomepages für freigegebene Ordner nicht zu. Wenn diese Konfiguration geändert wird, führen Benutzer möglicherweise bei der Verwendung freigegebener Ordner unabsichtlich gefährliche Skripts aus, die ihre Computer oder Daten gefährden können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, kann Outlook 2007 keine mit freigegebenen Ordnern verknüpften Skripts ausführen. Die Aktivierung setzt außerdem alle Konfigurationsänderungen auf den Computern der Benutzer außer Kraft.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **deaktiviert** ist, führt Outlook automatisch alle Skripts aus, die mit benutzerdefinierten Formularen oder Ordnerhomepages für freigegebene Ordner verknüpft sind. Das kann die Sicherheit bedeutend verringern.
  
**Tabelle 1.132: Outlook-Objektmodellskripts können nicht für freigegebene Ordner ausgeführt werden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Weitere\Erweitert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1529</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Benutzer können Ordnerberechtigungen nicht ändern
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer die Zugriffsberechtigungen für von ihnen kontrollierte Ordner ändern können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer die Berechtigungen für Ordner unter ihrer Kontrolle über die Registerkarte **Berechtigungen** des Dialogfelds **Eigenschaften** für den Ordner oder durch Versenden einer Freigabenachricht ändern. Wenn Benutzer die Berechtigungen für einen von ihnen kontrollierten Ordner ändern, können vertrauliche Daten in den im Ordner gespeicherten Elementen möglicherweise gefährdet sein, wenn nicht autorisierte Personen darauf Zugriff erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer die Berechtigungen für Ordner nicht ändern. Die Einstellungen auf der Registerkarte **Berechtigungen** werden deaktiviert. Die Aktivierung dieser Einstellung wirkt sich nicht auf vorhandene Berechtigungen aus.
  
**Tabelle 1.133: Benutzer können Ordnerberechtigungen nicht ändern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\Exchange</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1303</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie verhindert, dass Outlook 2007-Benutzer von ihnen kontrollierte Ordner für andere freigeben können. Benutzer, die Ordner freigeben möchten, müssen sich für die erforderliche Änderung an den Administrator wenden.
  
### E-Mail-Adresse nicht mit der Adresse von verwendeten Zertifikaten vergleichen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 die E-Mail-Adresse des Benutzers mit der Adresse des für das Signieren verwendeten Zertifikats vergleicht.
  
#### Sicherheitsrisiko
  
Wenn ein Benutzer eine Nachricht signiert, vergleicht Outlook 2007 standardmäßig die E-Mail-Adresse des Benutzers mit dem für das Signieren verwendeten Zertifikat. Die E-Mail-Adresse des Benutzers muss entweder im Feld für den Antragsteller oder den alternativen Antragsteller des Zertifikats angezeigt werden. Andernfalls lässt Outlook nicht zu, dass der Benutzer die Nachricht mit diesem Zertifikat signiert.
  
Wenn diese Konfiguration geändert wird, können Benutzer Nachrichten versenden, die mit Zertifikaten signiert sind, die nicht ihren E-Mail-Adressen entsprechen. Das führt möglicherweise zu Problemen, wenn der Empfänger versucht, die Nachricht zu lesen oder die Signatur zu überprüfen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, überprüft Outlook 2007, ob die E-Mail-Adresse des Benutzers mit dem für das Signieren verwendeten Zertifikat übereinstimmt.
  
**Tabelle 1.134: E-Mail-Adresse nicht mit der Adresse von verwendeten Zertifikaten vergleichen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-316</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Schaltfläche „In GAL veröffentlichen“ nicht anzeigen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer E-Mail-Zertifikate in der globale Adressenliste (GAL) veröffentlichen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer ihre E-Mail-Zertifikate über den Bereich **E-Mail-Sicherheit** des Vertrauensstellungscenters in der globalen Adressenliste veröffentlichen. Wenn das Unternehmen über Richtlinien für die Regelung der Verwendung von digitalen Zertifikaten für das Signieren und Verschlüsseln von E-Mail-Nachrichten verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn das Veröffentlichen von Zertifikaten zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird die Schaltfläche **In GAL veröffentlichen** im Bereich **E-Mail-Sicherheit** des Vertrauensstellungscenters nicht angezeigt.
  
**Tabelle 1.135: Schaltfläche „In GAL veröffentlichen“ nicht anzeigen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-345</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Outlook 2007-Benutzer E-Mail-Zertifikate in der globalen Adressenliste (GAL) veröffentlichen. Benutzer, die ein neues oder aktualisiertes Zertifikat veröffentlichen müssen, sollten sich an einen Administrator wenden.
  
### Verteilerlisten nicht erweitern
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer beim Adressieren von E-Mail-Nachrichten Verteilerlisten erweitern können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer beim Hinzufügen einer Verteilerliste in die Felder **An**, **Cc** oder **Bcc** einer E-Mail-Nachricht oder anderer Elemente diese Verteilerliste erweitern, um die E-Mail-Adressen aller Personen in der Liste zu sehen. Wenn das Unternehmen Verteilerlisten verwendet, deren Mitgliedschaft unter Verschluss steht, kann die Erweiterung der Verteilerlisten durch Benutzer ein Sicherheitsrisiko darstellen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer Verteilerlisten nicht erweitern.
  
**Tabelle 1.136: Verteilerlisten nicht erweitern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1565</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Aktiviert**. Sie verhindert, dass Outlook 2007-Benutzer Verteilerlisten bei der Adressierung von E-Mail-Nachrichten erweitern können. Benutzer, die die Zusammensetzung einer Verteilerliste sehen möchten, müssen deren Eintrag in der globalen Adressenliste überprüfen, um zu sehen, ob die Konfiguration ein Anzeigen der Listenmitgliedschaft zulässt.
  
### Internetkalenderintegration nicht in Outlook einschließen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Benutzer Kalender im Internet veröffentlichen und abonnieren können.
  
#### Sicherheitsrisiko
  
Benutzer können mit der Internetkalenderfunktion in Outlook 2007 Kalender online veröffentlichen (über das webcal://-Protokoll) und von anderen veröffentlichte Kalender abonnieren. Wenn Benutzer einen Internetkalender abonnieren, fragt Outlook den Kalender in regelmäßigen Zeitabständen ab und lädt alle Änderungen herunter, sobald sie veröffentlicht wurden.
  
Standardmäßig lässt Outlook zu, dass Benutzer Internetkalender abonnieren. Wenn das Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Internetkalender verfügt, führt die Verwendung dieser Funktion möglicherweise dazu, dass Benutzer gegen diese Richtlinien verstoßen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, werden alle Internetkalenderfunktionen in Outlook 2007 deaktiviert.
  
**Tabelle 1.137: Internetkalenderintegration nicht in Outlook einschließen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\Internetkalender</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1461</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die Internetkalender in Outlook 2007 abonnieren. Diese Benutzer müssen eine andere Methode für den Zugriff auf Internetkalenderdaten verwenden.
  
### Herunterladen von Inhalt von sicheren Zonen nicht zulassen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 beim Anzeigen von Nachrichten automatisch Inhalte aus sicheren Zonen herunterlädt.
  
#### Sicherheitsrisiko
  
Standardmäßig lädt Outlook 2007 automatisch Inhalte von Sites herunter, die per Definition auf der Registerkarte **Sicherheit** des Dialogfelds **Internetoptionen** in Internet Explorer als sicher betrachtet werden. Bei dieser Konfiguration könnten Benutzer unabsichtlich Webbeacons herunterladen, die ihre Identität an Spammer und andere böswillige Personen weitergeben.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, lädt Outlook 2007 Inhalte aus sicheren Zonen nicht automatisch herunter. Empfänger können sich auf der Basis einzelner Nachrichten entscheiden, ob externe Inhalte von nicht vertrauenswürdigen Absendern heruntergeladen werden.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Beachten Sie, dass diese Einstellung „umgekehrt“ funktioniert. Trotz des Namens verhindert die Deaktivierung der Einstellung den Download von Inhalten aus sicheren Zonen, und die Aktivierung der Einstellung lässt den Download zu. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103510).
  
**Tabelle 1.138: Herunterladen von Inhalt von sicheren Zonen nicht zulassen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen für den automatischen Download von Bildern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1347</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung kann zu einigen Beeinträchtigungen für Outlook 2007-Benutzer führen, die E-Mail-Nachrichten mit Inhalten aus sicheren Zonen empfangen, da sie den Inhalt für jede Nachricht einzeln herunterladen müssen.
  
### Keine Eingabeaufforderung zu Anlagen der Ebene 1 beim Schließen eines Elements
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 vor dem Schließen eines Elements mit einer unsicheren Anlage, die bei erneutem Öffnen des Elements blockiert wird, eine Warnung anzeigt.
  
#### Sicherheitsrisiko
  
Um Benutzer vor Viren und anderen schädlichen Dateien zu schützen, verwendet Outlook 2007 zwei Sicherheitsebenen, die als Ebene 1 und Ebene 2 festgelegt sind, um den Zugriff von Benutzern auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Standardmäßig blockiert Outlook den Zugriff auf Dateien der Ebene 1 vollständig und erfordert vor dem Öffnen von Dateien der Ebene 2, dass Benutzer diese auf dem Datenträger speichern. Potenziell schädliche Dateien können nach ihrer Dateierweiterung als diese zwei Ebenen klassifiziert werden. Alle anderen Dateitypen werden als sicher betrachtet.
  
Beim Schließen eines Elements, dem eine Datei der Ebene 1 angehängt wurde, warnt Outlook den Benutzer standardmäßig, dass die Nachricht eine potenziell unsichere Anlage enthält und der Benutzer beim späteren Öffnen des Elements möglicherweise nicht auf die Anlage zugreifen kann. (Zu einem solchen Ablauf der Ereignisse kann es kommen, wenn ein Benutzer einen Nachrichtenentwurf schließt, den er später weiter bearbeiten möchte.) Wenn diese Konfiguration geändert wird, zeigt Outlook beim Schließen des Elements durch den Benutzer keine Warnung an, blockiert aber dennoch die unsichere Anlage, wenn der Benutzer die Nachricht später öffnet. Diese Funktion kann dazu führen, dass Benutzer den Zugriff auf wichtige Daten verlieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, gibt Outlook 2007 vor dem Schließen von Elementen mit Anlagen der Ebene 1 eine Warnung für den Benutzer aus und setzt alle Konfigurationsänderungen auf den Computern von Benutzern außer Kraft.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, zeigt Outlook keine Warnung an, wenn Benutzer Elemente mit Anlagen der Ebene 1 schließen. Das führt möglicherweise zu einem Datenverlust.
  
**Tabelle 1.139: Keine Eingabeaufforderung zu Anlagen der Ebene 1 beim Schließen eines Elements**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1569</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Zur Anwendung dieser Einstellung müssen Sie außerdem die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Outlook 2007\\Sicherheit\\Sicherheitsformulareinstellungen\\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und die Option **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.
  
### Keine Eingabeaufforderung zu Anlagen der Ebene 1 beim Senden eines Elements
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 vor dem Versenden eines Elements mit einer unsicheren Anlage, die beim Öffnen durch einen Empfänger blockiert wird, eine Warnung anzeigt.
  
#### Sicherheitsrisiko
  
Um Benutzer vor Viren und anderen schädlichen Dateien zu schützen, verwendet Outlook 2007 zwei Sicherheitsebenen, die als Ebene 1 und Ebene 2 festgelegt sind, um den Zugriff auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Standardmäßig blockiert Outlook den Zugriff auf Dateien der Ebene 1 vollständig und erfordert vor dem Öffnen von Dateien der Ebene 2, dass Benutzer diese auf dem Datenträger speichern. Potenziell schädliche Dateien können nach ihrer Dateierweiterung als diese zwei Ebenen klassifiziert werden. Alle anderen Dateitypen werden als sicher betrachtet.
  
Beim Versenden eines Elements, dem eine Datei der Ebene 1 angehängt wurde, warnt Outlook Benutzer standardmäßig, dass die Meldung eine potenziell unsichere Anlage enthält, auf die der Empfänger möglicherweise nicht zugreifen kann. Wenn diese Konfiguration geändert wird, zeigt Outlook beim Versenden solcher Elemente keine Warnung an, was dazu führen kann, dass Benutzer den Zugriff auf wichtige Daten verlieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, gibt Outlook 2007 vor dem Versenden von Elementen mit Anlagen der Ebene 1 eine Warnung für den Benutzer aus und setzt alle Konfigurationsänderungen auf den Computern von Benutzern außer Kraft.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, zeigt Outlook keine Warnung an, wenn ein Benutzer ein Element mit einer Anlage der Ebene 1 versendet. Das gefährdet möglicherweise die Daten des Benutzers.
  
**Tabelle 1.140: Keine Eingabeaufforderung zu Anlagen der Ebene 1 beim Senden eines Elements**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Anlagensicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1652</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443676.important(de-de,TechNet.10).gif) **Wichtig:**
  
Zur Anwendung dieser Einstellung müssen Sie außerdem die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Outlook 2007\\Sicherheit\\Sicherheitsformulareinstellungen\\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und die Option **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.
  
### Nicht zum Konvertieren älterer Datenbanken auffordern
  
Betrifft: **Access**
  
Diese Einstellung steuert, ob Access 2007 Benutzer auffordert, ältere Datenbanken beim Öffnen zu konvertieren.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Datenbanken öffnen, die im Access 97-Dateiformat erstellt wurden, fordert Access 2007 sie standardmäßig auf, die Datenbank in ein neueres Dateiformat zu konvertieren. Benutzer können entscheiden, ob sie die Datenbank konvertieren oder im älteren Format belassen möchten.
  
Wenn diese Konfiguration geändert wird, behält Access Datenbanken im Access 97-Format unverändert bei. Access informiert den Benutzer, dass die Datenbank im älteren Format gespeichert ist, stellt dem Benutzer aber keine Option zur Konvertierung der Datenbank bereit. Einige in neueren Versionen von Access eingeführte Funktionen sind nicht verfügbar, und der Benutzer kann keine Entwurfsänderungen an der Datenbank durchführen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, fordert Access 2007 Benutzer auf, Datenbanken im Access 97-Format in ein neueres Dateiformat zu konvertieren.
  
**Tabelle 1.141: Nicht zum Konvertieren älterer Datenbanken auffordern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1510</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Access 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Option „Weiter“ in Dialogfeldern mit Verschlüsselungswarnungen nicht bereitstellen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer E-Mail-Nachrichten senden können, nachdem eine Verschlüsselungswarnung angezeigt wurde.
  
#### Sicherheitsrisiko
  
Wenn Outlook 2007-Benutzer beim Versuch, eine Nachricht zu versenden, ein verschlüsselungsrelevantes Dialogfeld sehen, können sie entscheiden, die Warnung zu bestätigen und die Nachricht trotzdem zu versenden. Wenn Benutzer nach der Anzeige eines Verschlüsselungsfehlers Nachrichten senden, können Empfänger diese wahrscheinlich nicht lesen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, enthalten die Warndialogfelder keine Schaltfläche **Weiter**, was bedeutet, dass Benutzer den Sendevorgang vollständig abbrechen müssen. Diese Konfiguration kann dazu beitragen, das Versenden unnötiger, nicht lesbarer Nachrichten zu vermeiden.
  
**Tabelle 1.142: Option „Weiter“ in Dialogfeldern mit Verschlüsselungswarnungen nicht bereitstellen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1511</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeinträchtigungen für Outlook 2007-Benutzer führen, die versuchen, Nachrichten mit Verschlüsselungsfehlern zu versenden. In den meisten Fällen würden allerdings auch die Fehler selbst Beeinträchtigungen verursachen, wenn das Versenden zugelassen wäre.
  
### Datenextrahierungsoptionen beim Öffnen beschädigter Arbeitsmappen nicht anzeigen
  
Betrifft: **Excel**
  
Diese Einstellung steuert, ob Excel 2007 Benutzern vor Beginn eines Vorgangs zum Öffnen und Reparieren eine Liste von Datenextrahierungsoptionen präsentiert wird.
  
#### Sicherheitsrisiko
  
Wenn Benutzer eine beschädigte Arbeitsmappe mit dem Befehl „Öffnen und reparieren“ öffnen möchten, fragt Excel 2007 standardmäßig, ob Daten extrahiert oder repariert werden sollen. Falls Zellen mit Formeln vorhanden sind, werden Benutzer außerdem aufgefordert, entweder die Inhalte in Werte zu konvertieren oder die Formeln wiederherzustellen. Wenn sich Benutzer anstelle des Reparierens der Arbeitsmappe für das Extrahieren von Daten entscheiden, können wichtige Formeln, Formatierungen und VBA-Code unnötig verloren gehen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, öffnet Excel 2007 die Datei mithilfe eines sicheren Ladeprozesses und fordert den Benutzer nicht auf, sich zwischen dem Reparieren und dem Extrahieren von Daten zu entscheiden.
  
**Tabelle 1.143: Datenextrahierungsoptionen beim Öffnen beschädigter Arbeitsmappen nicht anzeigen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Datenwiederherstellung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">excel12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1094</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Excel 2007-Benutzer auswählen können, wie Arbeitsmappen wiederhergestellt werden. Das führt möglicherweise zu mehr Desktopsupportanfragen.
  
### Dokumentinformationsbereich für Signal übertragende Elemente der Benutzeroberfläche
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer eine Sicherheitswarnung sehen, wenn sie benutzerdefinierte Dokumentinformationsbereiche öffnen, die eine Bedrohung durch Webbeacons enthalten.
  
#### Sicherheitsrisiko
  
InfoPath 2007 kann für die Erstellung von benutzerdefinierten Dokumentinformationsbereichen verwendet werden, die Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen und Word 2007-Dokumenten angehängt werden können.
  
Ein böswilliger Benutzer kann einen Webbeacon in ein InfoPath-Formular einfügen, das zur Erstellung eines benutzerdefinierten Dokumentinformationsbereichs verwendet wird. Beim Öffnen des Formulars kann über Webbeacons ein externer Server kontaktiert werden. Das Formular kann Informationen sammeln, oder von Benutzern eingegebene Daten können an einen externen Server gesendet werden, sodass Benutzer anfällig für weitere Angriffe werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen zur Verfügung, über die sie steuern können, wann Benutzer eine Eingabeaufforderung zu Bedrohungen durch Webbeacons erhalten:
  
-   Benutzeroberfläche nie anzeigen
  
-   Benutzeroberfläche immer anzeigen
  
-   Benutzeroberfläche anzeigen, falls sich XSN in der Internetzone befindet
  
**Tabelle 1.144: Dokumentinformationsbereich für Signal übertragende Elemente der Benutzeroberfläche**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Dokumentinformationsbereich</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzeroberfläche anzeigen, falls sich XSN in der Internetzone befindet)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzeroberfläche immer anzeigen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1505</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die EC-Umgebung ist **Benutzeroberfläche anzeigen, falls sich XSN in der Internetzone befindet**. Sie kann Beeinträchtigungen für Benutzer verursachen, die oft solche Dokumente öffnen. Um diese Beeinträchtigungen zu vermeiden, sollten Sie sich vergewissern, dass sich die XSN-Dateien für die Dokumentinformationsbereiche in einer sichereren Zone befinden.
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Benutzeroberfläche immer anzeigen**. Sie kann Beeinträchtigungen für Benutzer verursachen, die oft Dokumente mit benutzerdefinierten Dokumentinformationsbereichen öffnen.
  
### Vollständigen Text von Artikeln als HTML-Anlagen herunterladen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 automatisch den vollständigen Text von RSS-Einträgen als HTML-Anlagen herunterlädt.
  
#### Sicherheitsrisiko
  
Viele RSS-Feeds verwenden Nachrichten, die eine kurze Zusammenfassung einer längeren Nachricht oder eines Artikels mit einem Link zum vollständigen Inhalt enthalten. Benutzer können Outlook 2007 für einen automatischen Download der verknüpften Inhalte als Nachrichtenanlagen für einzelne RSS-Feeds konfigurieren. Wenn ein Feed oft aktualisiert wird oder in der Regel sehr lange Nachrichten enthält und nicht regelmäßig automatisch archiviert wird, kann das Herunterladen vollständiger Artikel dazu führen, dass der betroffene Nachrichtenspeicher sehr umfangreich wird. Das wiederum kann sich auf die Leistung von Outlook auswirken.
  
Standardmäßig führt Outlook beim Abrufen von Feeds keinen automatischen Download des vollständigen Texts von RSS-Einträgen durch.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, lädt Outlook 2007 den vollen Text von RSS-Einträgen nicht automatisch als Anlagen herunter.
  
**Tabelle 1.145: Vollständigen Text von Artikeln als HTML-Anlagen herunterladen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Kontoeinstellungen\RSS-Feeds</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1311</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen. Die Deaktivierung dieser Einstellung verursacht möglicherweise geringfügige Beeinträchtigungen für Benutzer, die für gewöhnlich in Outlook 2007 Artikel als HTML-Anlagen lesen. Diese Benutzer müssen auf den Link **Artikel anzeigen** klicken, um solche Artikel im Standardwebbrowser zu öffnen.
  
#### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))  
-   Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))  
-   [Sicherheitseinstellungen für Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenmaßnahmen:%20sicherheitseinstellungen%20in%202007%20office%20system)
  
|                                                  |                                                                                                                                                                                                                                                                                                                                                                                |  
|--------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443676.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10)) 4 von 8 [![](images/Dd443676.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10)) |
