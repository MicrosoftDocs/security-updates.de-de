---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6'
Title: '2007 Microsoft Office-Sicherheitshandbuch auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6'
ms:assetid: 'ae3203f0-f0eb-426b-9deb-a1faea298982'
ms:contentKeyID: 20075607
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443663(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch Bedrohungen und Gegenmaßnahmen
========================================================================

### Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6

Veröffentlicht: 11. Nov 2007

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgeführt.

##### Auf dieser Seite

[](#ecd)[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)

### Informationen zu Benutzerrichtlinieneinstellungen

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle enthalten, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung sowie die empfohlene Konfiguration für EC- und SSLF-Umgebungen aufführt.

### E-Mail als Nur-Text lesen

Betrifft: **Outlook**

Diese Einstellung bestimmt, ob Outlook 2007 alle E-Mail-Nachrichten zum Lesen im Nur-Text-Format darstellt.

#### Sicherheitsrisiko

Outlook 2007 kann E-Mail-Nachrichten und andere Elemente in drei Formaten darstellen: Nur-Text-, Rich-Text- (RTF) und HTML-Format. Standardmäßig stellt Outlook E-Mail-Nachrichten in dem Format dar, in dem sie empfangen wurden.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, wird das Kontrollkästchen **Standardnachrichten im Nur-Text-Format lesen** im Bereich **E-Mail-Sicherheit** im Vertrauensstellungscenter aktiviert, und Benutzer können diese Einstellung nicht ändern. Diese Option ändert lediglich die Art und Weise, in der E-Mail-Nachrichten angezeigt werden. Die ursprüngliche Nachricht wird nicht in das Nur-Text-Format konvertiert.

Die Einstellung kann zum Schutz vor potenziellen neuartigen Angriffsformen verwendet werden, die auf das RTF- oder HTML-Format abzielen.

**Tabelle 1.192: E-Mail als Nur-Text lesen**

 
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
<td style="border:1px solid black;">CCE-791</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung zwingt Outlook 2007, alle Nachrichten im Nur-Text-Format anzuzeigen, was möglicherweise zu Beeinträchtigungen für Benutzer führt, die Nachrichten im HTML- oder RTF-Format empfangen. Inlinegrafiken in der Nachricht werden nicht angezeigt. Der Text formatierter Nachrichten kann verzerrt oder unlesbar werden.
  
### Signierte E-Mail als Nur-Text lesen
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, ob Outlook 2007 alle digital signierten E-Mail-Nachrichten zum Lesen im Nur-Text-Format darstellt.
  
#### Sicherheitsrisiko
  
Outlook 2007 kann E-Mail-Nachrichten und andere Elemente in drei Formaten darstellen: Nur-Text-, Rich-Text- (RTF) und HTML-Format. Standardmäßig stellt Outlook digital signierte E-Mail-Nachrichten in dem Format dar, in dem sie empfangen wurden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird das Kontrollkästchen **Standardnachrichten im Nur-Text-Format lesen** im Bereich **E-Mail-Sicherheit** im Vertrauensstellungscenter aktiviert, und Benutzer können diese Einstellung nicht ändern. Diese Option ändert lediglich die Art und Weise, in der E-Mail-Nachrichten angezeigt werden. Die ursprüngliche Nachricht wird nicht in das Nur-Text-Format konvertiert.
  
Die Einstellung kann zum Schutz vor potenziellen neuartigen Angriffsformen verwendet werden, die auf das RTF- oder HTML-Format abzielen.
  
**Tabelle 1.193: Signierte E-Mail als Nur-Text lesen**

 
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
<td style="border:1px solid black;">CCE-1456</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung zwingt Outlook 2007, signierte Nachrichten im Nur-Text-Format anzuzeigen, was möglicherweise zu Beeinträchtigungen für Benutzer führt, die signierte Nachrichten im HTML- oder RTF-Format empfangen. Inlinegrafiken in der Nachricht werden nicht angezeigt. Der Text formatierter Nachrichten kann verzerrt oder unlesbar werden.
  
### Smarttags in Excel erkennen
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Excel 2007 bestimmte Datentypen in Arbeitsmappen mit Smarttags kennzeichnet.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Die Einstellung „Smarttags erkennen“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Excel 2007\\Verschiedenes“ funktioniert nicht wie vorgesehen und beeinträchtigt die Konfiguration der Einstellung „Smarttags in Excel erkennen“, wenn diese verwendet wird. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103492).
  
#### Sicherheitsrisiko
  
Excel 2007 kann bestimmte Datentypen in Arbeitsmappen erkennen und automatisch mit Smarttags kennzeichnen, die zusätzliche Informationen oder Aktionen zur Verfügung stellen. Um die Erkennung von Smarttags in Excel zu aktivieren, klicken Sie auf die Schaltfläche **Microsoft Office** und dann auf **Excel-Optionen**, **Dokumentprüfung** und **AutoKorrektur-Optionen**. Aktivieren Sie dann das Kontrollkästchen **Daten mit Smarttags beschriften**, und wählen Sie aus, welche Erkennung aktiviert werden soll. Wenn die Smarttagerkennung aktiviert ist, kann Excel Daten, Kalendersymbole, Personennamen und geografische Überschriften erkennen sowie Aktionen bereitstellen, die Benutzer in externen Anwendungen wie Outlook und Microsoft MapPoint 2006 durchführen können.
  
In einigen Situationen kann die Aktivierung der Erkennung von Smarttags in Excel dazu führen, dass nicht autorisierte Personen Zugriff auf vertrauliche Daten erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, können Benutzer Excel 2007 nicht für die Erkennung von Smarttags konfigurieren.
  
**Tabelle 1.194: Erkennung von Smarttags in Excel**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | AutoKorrektur-Optionen... (Excel, Word, PowerPoint und Access)\Smarttags</td>
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
<td style="border:1px solid black;">CCE-1074</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die daran gewöhnt sind, in Excel-Arbeitsmappen mit Smarttags zu arbeiten. Die Smarttagerkennung ist in Excel 2007 standardmäßig nicht aktiviert. Deshalb sollten die meisten Benutzer von dieser Einstellung nicht betroffen sein.
  
### Für Grafikdarstellung auf VML vertrauen
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen GIF- oder PNG-Kopien von VML-Grafiken speichern, wenn Dokumente als Webseiten gespeichert werden.
  
#### Sicherheitsrisiko
  
Beim Speichern von Dokumenten als Webseiten können Excel 2007, PowerPoint 2007 und Word 2007 vektorbasierte Grafiken im VML-Format (Vector Markup Language) speichern, sodass Internet Explorer diese in jeder Auflösung gut darstellen kann.
  
Beim Speichern von VML-Grafiken speichern 2007 Office-Anwendungen standardmäßig zudem Kopien der Grafiken in einem Standardraster-Dateiformat (GIF oder PNG) zur Verwendung in Browsern, die VML nicht anzeigen können. Wenn das Kontrollkästchen **Für Grafikdarstellung in Browsern auf VML vertrauen** im Dialogfeld **Weboptionen** aktiviert ist, speichern Anwendungen keine Rasterkopien von VML-Grafiken. Das bedeutet, dass diese Grafiken in Browsern, die nicht von Microsoft stammen, nicht dargestellt werden können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, wird das Kontrollkästchen **Für Grafikdarstellung in Browsern auf VML vertrauen** im Dialogfeld **Weboptionen** in Excel 2007, PowerPoint 2007 und Word 2007 nicht aktiviert, und Benutzer können die Einstellung nicht ändern.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Ist die Einstellung **aktiviert**, generieren 2007 Office-Anwendungen beim Speichern von Dokumenten als Webseiten keine alternativen Dateien für VML-Grafiken, was die Anzeige der Grafiken für Webseitenleser erschweren kann.
  
**Tabelle 1.195: Für Grafikdarstellung in Browsern auf VML vertrauen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…\Browser</td>
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
<td style="border:1px solid black;">CCE-1438</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für EC- und SSLF-Umgebungen ist **Deaktiviert**, was dazu führen kann, dass als Webseiten gespeicherte Dokumente mehr Speicherplatz auf dem Datenträger belegen, wenn sowohl VML- als auch rasterbasierte Grafiken gespeichert werden. Ansonsten sollten die empfohlenen Einstellungen keine Nutzbarkeitsprobleme für Benutzer verursachen.
  
### Als Ebene 1 blockierte Dateierweiterungen entfernen
  
Betrifft: **Outlook**
  
Mit dieser Einstellung können Administratoren Anlagetypen (die nach Dateinamenerweiterung aufgelistet sind) aus der Liste der als Ebene 1 blockierten Dateierweiterungen entfernen.
  
#### Sicherheitsrisiko
  
Schädlicher Code wird oft per E-Mail verbreitet. Einige Viren können Kopien von sich selbst an andere Personen im Adressbuch oder der Kontaktliste des Opfers senden. Diese potenziell schädlichen Dateien beeinträchtigen möglicherweise die Computer unwissender Empfänger.
  
#### Gegenmaßnahme
  
Outlook 2007 verwendet zwei Sicherheitsebenen, um den Zugriff von Benutzern auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Dateien mit bestimmten Erweiterungen können als Ebene 1 (Benutzer können die Datei nicht anzeigen) oder Ebene 2 (Benutzer können die Datei öffnen, nachdem sie auf den Datenträger gespeichert wurde) kategorisiert werden. Benutzer können ohne Einschränkung Dateien jeden Typs öffnen, der nicht als Ebene 1 oder Ebene 2 kategorisiert ist.
  
Standardmäßig klassifiziert Outlook eine Reihe von potenziell schädlichen Dateitypen (wie EXE, REG und VBS) als Ebene 1 und blockiert den Empfang von Dateien mit diesen Erweiterungen durch Benutzer. (Die vollständige Liste von [Anlagedateitypen, die von Outlook 2007 gesperrt werden](http://technet2.microsoft.com/office/en-us/library/bc667b4c-1645-42be-8dc0-af56dc11ef5b1033.mspx), finden Sie auf Microsoft TechNet.)
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren mindestens eine der Erweiterungen in der Standardliste außer Kraft setzen, indem sie diese in das angezeigte Textfeld eingeben. Daraufhin werden die Erweiterungen effektiv aus der Liste entfernt. Mehrere Erweiterungen können durch ein Semikolon getrennt werden.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Wenn aus der Standardliste für Ebene 1 Erweiterungen entfernt werden, können Benutzer potenziell gefährliche Dateien öffnen, was die Sicherheit bedeutend verringern kann.
  
**Tabelle 1.196: Als Ebene 1 blockierte Dateierweiterungen entfernen**

 
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
<td style="border:1px solid black;">CCE-1631</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für EC- und SSLF-Umgebungen ist **Deaktiviert**. Alle bereits in der Liste enthaltenen Erweiterungen werden ignoriert, sodass Outlook 2007 den Zugriff darauf erneut blockiert. Diese Konfiguration könnte Benutzer beeinträchtigen, die für gewöhnlich derartige Dateien versenden und empfangen.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Sie können Exchange-Sicherheitsformulareinstellungen auch konfigurieren, indem Sie die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Outlook 2007\\Sicherheit\\Sicherheitsformulareinstellungen\\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.
  
### Als Ebene 2 blockierte Dateierweiterungen entfernen
  
Betrifft: **Outlook**
  
Mit dieser Einstellung können Administratoren Anlagetypen (die nach Dateinamenerweiterung aufgelistet sind) aus der Liste der als Ebene 2 blockierten Erweiterungen entfernen.
  
#### Sicherheitsrisiko
  
Schädlicher Code wird oft per E-Mail verbreitet. Einige Viren können Kopien von sich selbst an andere Personen im Adressbuch oder der Kontaktliste des Opfers senden. Diese potenziell schädlichen Dateien beeinträchtigen möglicherweise die Computer unwissender Empfänger.
  
Outlook 2007 verwendet zwei Sicherheitsebenen, um den Zugriff von Benutzern auf Dateien einzuschränken, die E-Mail-Nachrichten oder anderen Elementen angehängt sind. Dateien mit bestimmten Erweiterungen können als Ebene 1 (Benutzer können die Datei nicht anzeigen) oder Ebene 2 (Benutzer können die Datei öffnen, nachdem sie auf den Datenträger gespeichert wurde) kategorisiert werden. Benutzer können ohne Einschränkung Dateien jeden Typs öffnen, der nicht als Ebene 1 oder Ebene 2 kategorisiert ist.
  
Standardmäßig klassifiziert Outlook eine Reihe von potenziell schädlichen Dateitypen als Ebene 1. (Die vollständige Liste finden Sie in der Liste der [Anlagedateitypen, die von Outlook 2007 gesperrt werden](http://technet2.microsoft.com/office/en-us/library/bc667b4c-1645-42be-8dc0-af56dc11ef5b1033.mspx).) Outlook klassifiziert standardmäßig keine Dateitypen als Ebene 2, deshalb ist diese Einstellung allein genommen nicht besonders nützlich. Falls Erweiterungen in der Liste der Ebene 2 enthalten sind, wurden diese in der Regel über die Einstellung „Als Ebene 2 zu blockierende Dateierweiterungen hinzufügen“ eingefügt, über die sie wieder entfernt werden können.
  
Die von Outlook verwendeten kombinierten Listen mit blockierten und eingeschränkten Dateierweiterungen werden eigentlich durch Zusammenlegung verschiedener Richtlinien aufgestellt. Wenn eine Computerrichtlinie eine Erweiterung als Ebene 2 klassifiziert, könnte die Erweiterung in einigen Situationen mithilfe dieser Einstellung aus der Liste entfernt werden. Wie bei den Erweiterungen der Ebene 1 erleichtert das Entfernen von Einschränkungen für potenziell gefährliche Erweiterungen Benutzern allerdings das Öffnen gefährlicher Dateien, wodurch sich die Sicherheit deutlich verringern kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, werden keine Erweiterungen aus der Liste der Ebene 2 entfernt, unabhängig davon, wie sie der Liste hinzugefügt wurden.
  
**Tabelle 1.197: Als Ebene 2 blockierte Dateierweiterungen entfernen**

 
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
<td style="border:1px solid black;">CCE-1556</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### S/MIME-Bestätigung anfordern, wenn mit S/MIME signiert
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 S/MIME-Bestätigungsanforderungen mit Nachrichten versendet, die mit S/MIME signiert wurden.
  
#### Sicherheitsrisiko
  
Wenn Benutzer digital signierte E-Mail-Nachrichten versenden, können sie gleichzeitig S/MIME-Bestätigungsanforderungen senden. S/MIME-Bestätigungen bestätigen, dass Nachrichten unverändert empfangen wurden, und können Informationen darüber enthalten, wer die Nachrichten geöffnet hat und wann sie geöffnet wurden.
  
Standardmäßig versendet Outlook 2007 nur dann S/MIME-Bestätigungsanforderungen mit signierten Nachrichten, wenn Benutzer die Option im Bereich **E-Mail-Sicherheit** des Vertrauensstellungscenters oder im Dialogfeld **Sicherheitseigenschaften** für einzelne Nachrichten aktivieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, fordert Outlook 2007 S/MIME-Bestätigungen an, wenn das Programm mit S/MIME signierte Nachrichten versendet, und Benutzer können diese Einstellung nicht ändern.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Ist die Einstellung **deaktiviert**, fordert Outlook beim Versenden signierter Nachrichten nicht automatisch S/MIME-Bestätigungen an, aber Benutzer können dennoch Bestätigungsanforderungen in einzelne Nachrichten einfügen.
  
**Tabelle 1.198: S/MIME-Bestätigung anfordern, wenn mit S/MIME signiert**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-153</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn ein Benutzer eine Nachricht mit einer S/MIME-Bestätigungsanforderung sendet, wird die Bestätigung als Nachricht in den Posteingang des Benutzers übermittelt. Die Aktivierung dieser Einstellung führt dazu, dass Benutzer für jede versendete signierte Nachricht eine S/MIME-Bestätigung erhalten, es sei denn, die Empfänger können keine Bestätigungen generieren oder entscheiden sich gegen das Versenden der Bestätigung. Diese Konfiguration verursacht bei einigen Benutzern möglicherweise einen deutlichen Anstieg des E-Mail-Aufkommens.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Wenn die Einstellung „Alle E-Mail-Nachrichten signieren“ aktiviert ist, wie es bei der SSLF-Konfiguration der Fall ist, kann die Aktivierung dieser Einstellung die E-Mail-Infrastruktur erheblich belasten. Berücksichtigen Sie Ihre Anforderungen und Fähigkeiten, bevor Sie beide Einstellungen aktivieren.
  
### SuiteB-Algorithmen sind für S/MIME-Vorgänge erforderlich
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, ob Outlook 2007 für S/MIME-Vorgänge die Suite-B-Algorithmen der NSA verwenden muss.
  
#### Sicherheitsrisiko
  
Outlook 2007 implementiert Suite B, einen Satz kryptografischer Algorithmen für symmetrische Verschlüsselung, Hashing, digitale Signaturen und den Schlüsselaustausch, der 2005 von der National Security Agency (NSA) angekündigt wurde, einer Abteilung des amerikanischen Verteidigungsministeriums. Die Suite-B-Protokolle können verwendet werden, um die amerikanischen Regierungsstandards für die Verarbeitung geheimer und nicht geheimer Informationen zu erfüllen.
  
Standardmäßig kann Outlook jeden verfügbaren Algorithmus für S/MIME-Vorgänge wie Verschlüsselung, Signaturen usw. verwenden. Unternehmen, die Geschäfte mit der US-Regierung unterhalten und nicht die Suite-B-Algorithmen für S/MIME-Vorgänge verwenden, riskieren eine Verletzung der US-Regierungsvorschriften für die Verarbeitung vertraulicher Daten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, verwendet Outlook 2007 für S/MIME-Vorgänge nur Suite-B-Algorithmen. Folgende Algorithmen werden für Suite B eingesetzt:
  
-   **Symmetrische Verschlüsselung**: Advanced Encryption Standard (AES) mit Schlüsselgrößen von 128 und 256 Bit  
-   **Nachrichtenhash**: Secure Hash Algorithm (SHA-256 und SHA-384)  
-   **Schlüsselübereinstimmung**: Elliptic-Curve Menezes-Qu-Vanstone (ECMQV), Elliptic Curve Diffie-Hellman (ECDH)  
-   **Digitale Signaturen**: Elliptic-Curve Digital Signature Algorithm (ECDSA)
  
**Tabelle 1.199: SuiteB-Algorithmen sind für S/MIME-Vorgänge erforderlich**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1658</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, müssen Sie sich vergewissern, dass der vollständige, oben aufgelistete Satz Verschlüsselungsstandards und Algorithmen bereitgestellt wird und für die Benutzer in Ihrem Unternehmen verfügbar ist. Andernfalls werden sie einige S/MIME-Vorgänge nicht abschließen können.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Weitere Informationen über Suite B finden Sie in den [Fakten zur NSA Suite-B-Kryptografie (in englischer Sprache)](http://www.nsa.gov/ia/industry/crypto_suite_b.cfm).
  
### Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein
  
Betrifft: **Access, Excel, InfoPath, PowerPoint, Word**
  
Diese Einstellung steuert, ob Add-Ins für die angegebenen 2007 Office-Anwendungen von einem vertrauenswürdigen Herausgeber digital signiert sein müssen.
  
#### Sicherheitsrisiko
  
Standardmäßig führen 2007 Office-Anwendungen keine Überprüfung der digitalen Signatur von Anwendungs-Add-Ins durch, bevor sie diese öffnen. Wenn ein gefährliches Add-In geladen wird, können die Computer von Benutzern beschädigt oder die Datensicherheit beeinträchtigt werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, überprüfen die angegebenen Anwendungen vor dem Laden die digitale Signatur für jedes Add-In. Wenn ein Add-In nicht digital signiert ist oder die Signatur nicht von einem vertrauenswürdigen Herausgeber stammt, deaktiviert die Anwendung das Add-In und benachrichtigt den Benutzer.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Microsoft bietet vier Zertifikate für die 2007 Office-Version an, die Sie der Liste vertrauenswürdiger Herausgeber hinzufügen können. Diese Zertifikate müssen der Liste vertrauenswürdiger Herausgeber hinzugefügt werden, wenn Sie digitale Signaturen von einem vertrauenswürdigen Herausgeber für alle Add-Ins verlangen. Wenn Sie die Zertifikate nicht der Liste vertrauenswürdiger Herausgeber hinzufügen und digitale Signaturen von einem vertrauenswürdigen Herausgeber für alle Add-Ins verlangen, werden Benutzern bei der Verwendung verschiedener Anwendungen und Anwendungsfunktionen möglicherweise Benachrichtigungen in der Statusleiste und in Dialogfeldern angezeigt. Diese Benachrichtigungen werden angezeigt, weil einige Anwendungen integrierte Add-Ins verwenden, die mit der 2007 Office-Version ausgeliefert werden. Wenn die Zertifikate für diese Add-Ins nicht der Liste vertrauenswürdiger Herausgeber hinzugefügt werden und Benutzer die Add-Ins aufrufen, werden die Add-Ins deaktiviert und die Benutzer aufgefordert, sie zu aktivieren. Die Zertifikate von Microsoft haben die Namen „Mscert01.cer“, „Mscert02.cer“, „Mscert03.cer“ und „Mscert04.cer“ und können von der Microsoft-Website heruntergeladen werden.
  
**Tabelle 1.200: Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein**

 
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
<td style="border:1px solid black;">Access: CCE-1476Excel: CCE-1524InfoPath: CCE-1157PowerPoint: CCE-1107Word: CCE-1562</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann Beeinträchtigungen für Benutzer verursachen, die mit Add-Ins arbeiten, die nicht von vertrauenswürdigen Herausgebern signiert sind. Diese Benutzer müssen entweder signierte Versionen der Add-Ins erwerben oder die Verwendung der Add-Ins einstellen.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Die 2007 Office-Version speichert Zertifikate für vertrauenswürdige Herausgeber in der Aufstellung der vertrauenswürdigen Herausgeber von Internet Explorer. In früheren Versionen von Office wurden Informationen zu Zertifikaten für vertrauenswürdige Herausgeber (insbesondere den Zertifikatfingerabdruck) in einer speziellen Office-Aufstellung der vertrauenswürdigen Herausgeber gespeichert. Die 2007 Office-Version liest weiterhin Informationen zu Zertifikaten für vertrauenswürdige Herausgeber aus der Office-Aufstellung der vertrauenswürdigen Herausgeber, schreibt aber keine Informationen in diese Aufstellung.
  
Wenn Sie also eine Liste vertrauenswürdiger Herausgeber in einer früheren Version von Office erstellt und ein Upgrade auf die 2007 Office-Version durchgeführt haben, wird Ihre Liste vertrauenswürdiger Herausgeber weiterhin erkannt. Aber alle Zertifikate vertrauenswürdiger Herausgeber, die Sie der Liste hinzufügen, werden in der Aufstellung vertrauenswürdiger Herausgeber in Internet Explorer gespeichert.
  
Weitere Informationen über vertrauenswürdige Herausgeber finden Sie in der folgenden Dokumentation:
  
-   Microsoft Office Online-Artikel „[Hinzufügen, Entfernen oder Anzeigen eines vertrauenswürdigen Herausgebers](http://office.microsoft.com/en-us/help/ha100341381033.aspx)“.  
-   Knowledge Base-Artikel „[So wird's gemacht: Verwendung von Richtlinien für Softwareeinschränkung in Windows Server 2003](http://support.microsoft.com/kb/324036)“.  
-   Microsoft TechNet-Artikel „[Schutz vor nicht autorisierter Software mit Richtlinien für Softwareeinschränkung](http://go.microsoft.com/fwlink/?linkid=98671)“.  
-   Kapitel 6 „[Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/technet/security/prodtech/windowsxp/secwinxp/default.mspx)“ im Windows XP-Sicherheitshandbuch im Microsoft TechNet.
  
### Erforderliche Zertifizierungsstelle
  
Betrifft: **Outlook**
  
Mit dieser Einstellung können Administratoren eine erforderliche Zertifizierungsstelle festlegen, die Outlook 2007 für die Verschlüsselung und für digitale Signaturen verwendet.
  
#### Sicherheitsrisiko
  
Standardmäßig vertraut Outlook 2007 allen Zertifizierungsstellen, die durch Zertifikate in der Aufstellung vertrauenswürdiger Stammzertifizierungsstellen auf den Computern von Benutzern vertreten sind. In Umgebungen, die eine starke Sicherheit erfordern, sollten Administratoren eventuell die digitalen Zertifikate von Benutzern für S/MIME-Vorgänge wie Verschlüsselung, digitale Signaturen usw. kontrollieren, indem sie eine erforderliche Zertifizierungsstelle zur Verwendung in Outlook festlegen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren eine erforderliche Zertifizierungsstelle angeben, indem sie einen definierten X.509-Namen in das bereitgestellte Textfeld eingeben. Der Name muss exakt dem X.509-Zertifikatformat entsprechen. Zum Beispiel:
  
    CN = WoodgroveBankCA, DC = WoodgroveBank, DC = com
  
**Tabelle 1.201: Erforderliche Zertifizierungsstelle**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1498</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung sollte für Benutzer keine wesentlichen Beeinträchtigungen verursachen, wenn Stammzertifikate für die erforderliche Zertifizierungsstelle auf ihren Computern installiert sind.
  
### Kalenderdetails, die von Benutzern veröffentlicht werden können, einschränken
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, welche Kalenderdetails Outlook 2007-Benutzer an den Microsoft Office Outlook-Kalenderfreigabedienst veröffentlichen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer ihre Kalender für ausgewählte andere Benutzer freigeben, indem sie diese beim Microsoft Office Outlook-Kalenderfreigabedienst veröffentlichen. Benutzern stehen drei Optionen für die Anzeige der Details zur Verfügung:
  
-   **Nur Verfügbarkeit**. Autorisierte Besucher sehen, ob die Zeit des Benutzers als „Frei“, „Gebucht“, „Mit Vorbehalt“ oder „Abwesend“ markiert ist, Themen oder Details von Kalenderelementen werden nicht angezeigt.  
-   **Eingeschränkte Details**. Autorisierte Besucher können nur die Verfügbarkeit des Benutzers und den Betreff von Kalenderelementen sehen. Sie können keine Details von Kalenderelementen anzeigen. Optional können Benutzer festlegen, dass Besucher das Vorhandensein von privaten Elementen sehen können.  
-   **Alle Details**. Autorisierte Besucher können alle Details von Kalenderelementen sehen. Optional können Benutzer festlegen, dass Besucher von privaten Elementen sehen und auf Anlagen innerhalb von Kalenderelementen zugreifen können.
  
Wenn Benutzer eingeschränkte oder alle Details veröffentlichen können, kann dies zur Folge haben, dass nicht autorisierte Personen Zugang zu vertraulichen Daten in diesen Kalendern erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Detailstufen zur Auswahl zur Verfügung:
  
-   **Alle Optionen sind verfügbar**. Diese Detailstufe ist die Standardkonfiguration.  
-   **Deaktiviert „Alle Details“**.  
-   **Deaktiviert „Alle Details“ und „Eingeschränkte Details“**.
  
**Tabelle 1.202: Kalenderdetails, die von Benutzern veröffentlicht werden können, einschränken**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Kalenderoptionen\Microsoft Office Online-Freigabedienst</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Alle Optionen sind verfügbar)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Deaktiviert „Alle Details“ und „Eingeschränkte Details“)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1641</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Auswahl der Einstellungen **Deaktiviert „Alle Details“** oder **Deaktiviert „Alle Details“ und „Eingeschränkte Details“** könnte zu Beeinträchtigungen für Outlook 2007-Benutzer führen, die sich auf die Möglichkeit verlassen, Details ihrer Termine beim Microsoft Office Outlook-Kalenderfreigabedienst zu veröffentlichen. Diese Benutzer werden Termindetails über andere Methoden an Außenstehende weitergeben müssen.
  
### Hochlademethode einschränken
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 automatisch Kalenderupdates an Microsoft Office Online hochladen kann.
  
#### Sicherheitsrisiko
  
Wenn Benutzer ihre Kalender über den Microsoft Office Outlook-Kalenderfreigabedienst auf Microsoft Office Online veröffentlichen, führt Outlook 2007 standardmäßig in regelmäßigen Abständen eine Online-Aktualisierung durch. Der Benutzer kann das verhindern, indem er auf **Erweitert** klickt und dann **Einzelupload: Aktualisierungen werden nicht hochgeladen** im Dialogfeld **Einstellungen des veröffentlichten Kalenders** aktiviert. Wenn Ihr Unternehmen Richtlinien für die Regelung der Verwendung externer Ressourcen wie Microsoft Office Online einsetzt, verstoßen Sie möglicherweise gegen diese Richtlinien, wenn Sie die automatische Veröffentlichung von Outlook-Kalenderaktualisierungen zulassen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, führt Outlook 2007 keine automatische Veröffentlichung von Kalenderaktualisierungen an Microsoft Office Online durch. Benutzer können ihre Kalender aber über die Option „Einzelupload“ manuell veröffentlichen.
  
**Tabelle 1.203: Hochlademethode einschränken**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Kalenderoptionen\Microsoft Office Online-Freigabedienst</td>
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
<td style="border:1px solid black;">CCE-1399</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die ihre Kalender beim Microsoft Office Outlook-Kalenderfreigabedienst veröffentlichen. Diese Benutzer müssen Ihre Kalender über die Option „Einzelupload“ manuell aktualisieren. Wenn Benutzer nicht regelmäßig veröffentlichen, können ihre Onlinekalender schnell nicht mehr aktuell sein.
  
### Abrufen von Zertifikatsperrlisten
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, wie Outlook 2007 Zertifikatsperrlisten abruft, um die Gültigkeit von Zertifikaten zu überprüfen.
  
#### Sicherheitsrisiko
  
Zertifikatsperrlisten sind Listen mit digitalen Zertifikaten, die von ihren Zertifizierungsstellen gesperrt wurden, normalerweise weil die Zertifikate nicht ordnungsgemäß ausgestellt oder die damit verbundenen privaten Schlüssel beschädigt wurden.
  
Wenn Outlook 2007 ein Zertifikat mit einer URL bearbeitet, von der eine Zertifikatsperrliste heruntergeladen werden kann, ruft Outlook standardmäßig die Zertifikatsperrliste von der bereitgestellten URL ab, wenn Outlook online ist. Wird diese Konfiguration geändert wird, vertraut Outlook eventuell fälschlicherweise einem gesperrten Zertifikat, wodurch die Computer und Daten von Benutzern gefährdet sein können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren anhand von drei Optionen regeln, wie Outlook 2007 Zertifikatsperrlisten verwendet:
  
-   **Systemstandardwert verwenden**. Outlook verlässt sich auf den für das Betriebssystem konfigurierten Downloadzeitplan für die Zertifikatsperrliste.  
-   **Im Onlinemodus immer die Zertifikatsperrliste abrufen**. Diese Option ist die Standardkonfiguration in Outlook.  
-   **Zertifikatsperrliste nie abrufen**. Outlook unternimmt keinen Versuch, die Zertifikatsperrliste abzurufen, selbst wenn das Programm online ist. Diese Option kann die Sicherheit mindern.
  
**Tabelle 1.204: Abrufen von Zertifikatsperrlisten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie\Dialogfeld „Signaturstatus“</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">Outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Im Onlinemodus immer die Zertifikatsperrliste abrufen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Im Onlinemodus immer die Zertifikatsperrliste abrufen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-395</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte deshalb für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Im FIPS-kompatiblen Modus ausführen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 bei der Signierung und Verschlüsselung von Nachrichten FIPS-kompatible Algorithmen verwenden muss.
  
#### Sicherheitsrisiko
  
Outlook 2007 kann in einem Modus ausgeführt werden, der mit den Federal Information Processing Standards (FIPS) kompatibel ist, einem Standardsatz, der vom National Institute of Standards and Technology (NIST) zur Verwendung von nicht-militärischen Behörden und Auftragnehmern der US-amerikanischen Regierung veröffentlicht wurde.
  
Standardmäßig wird Outlook nicht im FIPS-kompatiblen Modus ausgeführt. Unternehmen, die Geschäfte mit der US-Regierung unterhalten und Outlook nicht im FIPS-kompatiblen Modus ausführen, riskieren eine Verletzung der Regierungsvorschriften für die Verarbeitung vertraulicher Daten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird Outlook 2007 in einem Modus ausgeführt, der mit dem FIPS 140-1-Standard für kryptografische Module kompatibel ist. Dieser Modus erfordert die Verwendung des SHA-1-Algorithmus für das Signieren und von 3DES für das Verschlüsseln.
  
**Tabelle 1.205: Im FIPS-kompatiblen Modus ausführen**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1018</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung schränkt die Algorithmen ein, die Outlook 2007 für die Signierung und Verschlüsselung von Nachrichten verwenden kann. Wenn Ihr Unternehmen verschiedene kryptografische Standards einhält, können Benutzer durch die Aktivierung des FIPS-kompatiblen Modus diese Standards möglicherweise nicht erfüllen.
  
Weitere Informationen über FIPS finden Sie in den [allgemeinen Informationen zu FIPS (möglicherweise in englischer Sprache)](http://www.itl.nist.gov/fipspubs/geninfo.htm).
  
### Programme ausführen
  
Betrifft: **PowerPoint**
  
Diese Einstellung steuert das Bestätigungsaufforderungs- und Aktivierungsverhalten für die Option **Programme ausführen** für interaktive Schaltflächen in PowerPoint 2007.
  
#### Sicherheitsrisiko
  
Über interaktive Schaltflächen können externe Programme aus PowerPoint 2007-Präsentationen heraus gestartet werden. Wenn eine böswillige Person einer Präsentation eine interaktive Schaltfläche hinzufügt, die ein gefährliches Programm startet, kann dadurch die Sicherheit des Computers und der Daten eines Benutzers erheblich beeinträchtigt werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren anhand von drei Optionen steuern, wie die Option „Programme ausführen“ funktioniert:
  
-   **Deaktivieren (keine Programme ausführen)**. Wenn Benutzer auf eine interaktive Schaltfläche klicken, der die Aktion „Programme ausführen“ zugewiesen ist, geschieht nichts. Diese Option setzt die Standardkonfiguration in PowerPoint 2007 durch.  
-   **Aktivieren (Bestätigung des Benutzers vor dem Ausführen)**. Wenn Benutzer auf eine interaktive Schaltfläche klicken, der die Aktion „Programme ausführen“ zugewiesen ist, verlangt PowerPoint vor der Ausführung des Programms eine Bestätigung des Benutzers.  
-   **Alle aktivieren (Ausführen ohne Bestätigung)**. Wenn Benutzer auf eine interaktive Schaltfläche klicken, der die Aktion „Programme ausführen“ zugewiesen ist, führt PowerPoint das Programm automatisch ohne Bestätigungsaufforderung aus.
  
**Tabelle 1.206: Programme ausführen**

 
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
<td style="border:1px solid black;">Aktivieren (Deaktivieren (keine Programme ausführen))</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktivieren (Deaktivieren (keine Programme ausführen))</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1649</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlenen Einstellungen für EC- und SSLF-Umgebungen aktivieren die Einstellung und konfigurieren das Dropdownmenü für **Deaktivieren (keine Programme ausführen)**. Diese Konfiguration führt zu Beeinträchtigungen für Benutzer, die Präsentationen erstellen oder verwenden möchten, in denen beim Klicken auf eine interaktive Schaltfläche externe Programme gestartet werden sollen. Diese Benutzer müssen während ihrer Präsentation externe Programme zum jeweiligen Zeitpunkt manuell starten.
  
### S/MIME-Interoperabilität mit externen Clients:
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 verschlüsselte Nachrichten selbst entschlüsselt oder sie zur Verarbeitung an ein externes Programm weitergibt.
  
#### Sicherheitsrisiko
  
In einigen Situationen kann es sein, dass Administratoren für die Verarbeitung der S/MIME-Nachrichtenentschlüsselung möglicherweise ein externes Programm, beispielsweise ein Add-In, einsetzen möchten. Wenn Ihr Unternehmen mit verschlüsselten Nachrichten arbeitet, die über die Entschlüsselungsfunktionalität in Outlook 2007 nicht ordnungsgemäß gehandhabt werden können, kann Outlook mit dieser Konfigurationseinstellung S/MIME-Nachrichten für die Entschlüsselung an ein externes Programm übergeben. Wenn allerdings kein autorisiertes externes Programm vorhanden ist, führt eine falsche Konfiguration dieser Einstellung möglicherweise dazu, dass nicht autorisierte und potenziell gefährliche Programme verschlüsselte Nachrichten verarbeiten und so die Sicherheit beeinträchtigen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen für die Konfiguration externer S/MIME-Clients zur Verfügung:
  
-   **Intern verarbeiten**. Outlook 2007 entschlüsselt alle S/MIME-Nachrichten selbst.  
-   **Extern verarbeiten**. Outlook übergibt alle S/MIME-Nachrichten an das konfigurierte externe Programm.  
-   **Soweit möglich verarbeiten**. Outlook 2007 versucht, alle S/MIME-Nachrichten selbst zu entschlüsseln. Wenn Outlook eine Nachricht nicht entschlüsseln kann, wird die Nachricht an das konfigurierte externe Programm übergeben. Diese Option ist die Standardkonfiguration.
  
**Tabelle 1.207: S/MIME-Interoperabilität mit externen Clients**

 
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
<td style="border:1px solid black;">Aktiviert (Intern verarbeiten)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1630</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Konfiguration für die SSLF-Umgebung ist **Intern verarbeiten**. Sie setzt die Standardkonfiguration in Outlook 2007 durch und dürfte deshalb für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen. Wenn Sie ein festgelegtes externes Programm haben, das Sie für die Verarbeitung von S/MIME-Nachrichten verwenden möchten, müssen Sie eine der zwei anderen Optionen aus dem Dropdownmenü auswählen.
  
### S/MIME-Kennworteinstellungen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, wie Outlook 2007 Kennwortinformationen für Schlüsselverwaltungsserver-Zertifikate erhält.
  
#### Sicherheitsrisiko
  
Der Schlüsselverwaltungsserver war ein Produkt, das vor Exchange 2000 SP2 in bestimmte Versionen von Microsoft Exchange Server integriert werden konnte. Benutzer mussten ein Kennwort bereitstellen, um vom Schlüsselverwaltungsserver ausgestellte Zertifikate für die Signierung oder Entschlüsselung von E-Mail-Nachrichten zu verwenden. Wenn Outlook 2007 per Eingabeaufforderung das richtige Kennwort verlangt, können Benutzer eine Zeitdauer in Minuten angeben, für die Outlook das Kennwort zwischenspeichert. Benutzer werden während der angegebenen Zeitdauer nicht kontinuierlich aufgefordert, das Kennwort erneut einzugeben.
  
Standardmäßig merkt sich Outlook Schlüsselverwaltungsserver-Kennwörter 30 Minuten lang. Benutzer können diesen Wert auf eine beliebige Dauer bis 300 Minuten ändern. Je länger die vom Benutzer angegebene Zeitdauer ist, umso höher ist die Wahrscheinlichkeit, dass eine nicht autorisierte Person den Computer des Benutzers verwenden kann, um auf vertrauliche Informationen zuzugreifen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren die Standarddauer in Minuten für das Zwischenspeichern von Schlüsselverwaltungsserver-Kennwörtern in Outlook sowie die maximal von Benutzern anzugebende Anzahl von Minuten ändern. Jeder Wert muss einer ganzen Zahl zwischen 1 und 2.147.483.647 entsprechen.
  
**Tabelle 1.208: S/MIME-Kennworteinstellungen**

 
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
<td style="border:1px solid black;">Aktiviert (1)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1163, CCE-1445, CCE-1582</td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Konfiguration ist **Aktiviert**, wobei sowohl für die Standardzeit als auch die maximale Zeit der Wert 1 festgelegt werden sollte (der minimale Wert, den die Einstellung ermöglicht). Mit dieser Konfiguration speichert Outlook Kennwörter für den Schlüsselverwaltungsserver eine Minute lang zwischen, und Benutzer können diesen Wert nicht auf eine längere Zeitdauer ändern. Wenn Benutzer oft Schlüsselverwaltungsserver-Zertifikate für die Signierung und Entschlüsselung von E-Mail-Nachrichten verwenden, führt diese Konfiguration möglicherweise zu erheblichen Beeinträchtigungen, da sie ihre Kennwörter häufig erneut eingeben müssen.
  
### S/MIME-Bestätigungsanforderungen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert die Handhabung von S/MIME-Bestätigungsanforderungen in Outlook 2007.
  
#### Sicherheitsrisiko
  
Eingehende signierte oder verschlüsselte Nachrichten können S/MIME-Bestätigungsanforderungen enthalten. S/MIME-Bestätigungen stellen sicher, dass Nachrichten unverändert empfangen werden. Sie können außerdem Informationen darüber enthalten, wer die Nachricht geöffnet hat und wann.
  
Wenn Benutzer Nachrichten mit angehängten Bestätigungsanforderungen öffnen, fordert Outlook 2007 sie standardmäßig auf zu entscheiden, ob dem Absender eine Bestätigung mit Informationen über die Identität des Benutzers, der die Nachricht geöffnet hat, und den Zeitpunkt des Öffnens gesendet werden soll. Der Benutzer kann die Nachricht auch öffnen, wenn Outlook die Bestätigung nicht senden kann.
  
In einigen Situationen führt die Aktivierung des automatischen Versendens von Bestätigungsanforderungen in Outlook möglicherweise dazu, dass nicht autorisierte Personen Zugriff auf vertrauliche Informationen erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen für die Handhabung von S/MIME-Bestätigungsanforderungen in Outlook 2007 zur Verfügung:
  
-   **Nachricht öffnen, wenn Bestätigung nicht gesendet werden kann**  
-   **Nachricht nicht öffnen, wenn Bestätigung nicht gesendet werden kann**  
-   **Vor dem Senden der Bestätigung immer auffordern**  
-   **Nie S/MIME-Bestätigungen senden**
  
**Tabelle 1.209: S/MIME-Bestätigungsanforderungen**

 
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
<td style="border:1px solid black;">Aktiviert (Nie S/MIME-Bestätigungen senden)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1613</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Konfiguration für die SSLF-Umgebung ist **Nie S/MIME-Bestätigungen senden**. Die Konfiguration wirkt sich nicht darauf aus, ob ein Benutzer E-Mail-Nachrichten öffnen und lesen kann. Jedoch erhalten Personen, die Nachrichten mit angehängter Bestätigungsanforderung an Benutzer senden, die von dieser Einstellung betroffen sind, nicht die angeforderten S/MIME-Bestätigungen, was zu Verwirrung führen kann. Denken Sie daran, Benutzer über diese Einstellung zu informieren, sodass sie E-Mail-Absendern mitteilen können, keine Bestätigung auf ihre Anforderung zu erwarten.
  
### Zusätzliche zum Verwalten von Formeln erforderliche Daten speichern
  
Betrifft: **Excel**
  
Diese Einstellung steuert, ob Excel 2007 ausgeblendete Daten für die Erhaltung von Formeln speichert, wenn eine Arbeitsmappe als eine Webseite gespeichert wird, die Microsoft Office Web Components (OWC) verwendet, was in Excel 2007 veraltet ist.
  
#### Sicherheitsrisiko
  
Microsoft Office Web Components (OWC) ist eine Sammlung von COM-Steuerelementen (Component Object Model), die von älteren Microsoft Office-Versionen für das Veröffentlichen von Tabellenkalkulationen, Diagrammen und Datenbanken im Web sowie für die Anzeige der veröffentlichten Komponenten im Web verwendet wird. OWC wurde in der 2007 Office-Version durch verbesserte Webfunktionen für die Office-Desktopanwendungen und Microsoft Windows SharePoint Services ersetzt. Unternehmen, die derzeit die Veröffentlichung von Daten im Web über OWC unterstützen und noch nicht bereit sind, auf neuere Veröffentlichungsmethoden umzusteigen, können OWC von Microsoft herunterladen und sie weiterhin mit 2007 Microsoft Office-Anwendungen verwenden.
  
Wenn Benutzer Arbeitsmappen als Webseiten speichern, die OWC verwenden, behält Excel standardmäßig Formeldaten mit externen Verweisen bei, die nicht im ausgewählten zu veröffentlichenden Bereich liegen. Das vergrößert die Dateien und kann in einigen Fällen das Risiko einer Offenlegung von vertraulichen Daten steigern. Der Benutzer kann diese Funktionalität ändern, indem er das Kontrollkästchen **Zusätzliche ausgeblendete Daten speichern, um Formeln zu erhalten** auf der Registerkarte **Allgemein** im Dialogfeld **Weboptionen** deaktiviert (verfügbar über den Bereich **Erweitert** im Dialogfeld **Excel-Optionen**). Wenn das Kontrollkästchen deaktiviert wird, ersetzt Excel 2007 die Formel durch berechnete Werte, wodurch sich die Dateigröße verringert.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, können Benutzer keine ausgeblendeten Daten zur Erhaltung von Formeln speichern, wenn sie eine Arbeitsmappe als eine Webseite veröffentlichen, die OWC verwendet.
  
**Tabelle 1.210: Zusätzliche zum Verwalten von Formeln erforderliche Daten speichern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Erweitert\Weboptionen…\Allgemein</td>
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
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1277</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Deaktiviert**. Wenn Benutzer Excel 2007-Daten auf Webseiten veröffentlichen, die OWC verwenden, können Sie diese Einstellung möglicherweise nicht deaktivieren, ohne Beeinträchtigungen zu verursachen. Erwägen Sie, auf die Verwendung von OWC zu verzichten und stattdessen ausschließlich Excel 2007 für die Veröffentlichung von Tabellenkalkulationsdaten im Web zu verwenden. Wenn Benutzer Daten nur mithilfe von Excel 2007 auf Webseiten veröffentlichen und keine Kompatibilität mit früheren Versionen von Microsoft Office aufrechterhalten müssen, sollten Sie eine Deaktivierung dieser Einstellung in Betracht ziehen, um die Größe von Dateien zu verringern und ihre Übertragung und Freigabe zu vereinfachen.
  
Wenn Benutzer keine Daten auf Webseiten veröffentlichen, müssen Sie diese Einstellung nicht konfigurieren.
  
### Excel-Dateien speichern unter
  
Betrifft: **Excel**
  
Diese Einstellung steuert das Standarddateiformat für das Speichern von Arbeitsmappen in Excel 2007.
  
#### Sicherheitsrisiko
  
Standardmäßig speichert Excel 2007 neue Arbeitsmappen im Office Open XML-Format mit der Dateierweiterung XLSX. Für Benutzer, die Excel 2000 mit Service Pack 3, Excel 2002 mit Service Pack 3 und Excel 2003 mit mindestens Service Pack 1 ausführen, stellt Microsoft das Compatibility Pack für 2007 Office System bereit, mit dem diese Versionen von Excel XLSX-Dateien öffnen und speichern können. Wenn einige Benutzer im Unternehmen das Compatibility Pack nicht installieren können oder Versionen von Excel ausführen, die älter als Excel 2000 mit Service Pack 3 sind, können diese Benutzer nicht auf Excel-Dateien zugreifen, die im XLSX-Format gespeichert sind.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren das Standarddateiformat für Excel 2007 optional wie folgt einrichten:
  
-   **Excel-Arbeitsmappe (\*.xlsx)**. Diese Option ist die Standardkonfiguration in Excel 2007.  
-   **Excel-Arbeitsmappe mit Makros (\*.xlsm)**  
-   **Excel-Binärarbeitsmappe (\*.xlsx)**  
-   **Webseite (\*.htm; \*.html)**  
-   **Excel 97-2003-Arbeitsmappe (\*.xls)**  
-   **Excel 5.0/95-Arbeitsmappe (\*.xls)**
  
Benutzer können auswählen, ob sie Arbeitsmappen in einem anderen Dateiformat als dem Standardformat speichern möchten.
  
**Tabelle 1.211: Excel-Dateien speichern unter**

 
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
<td style="border:1px solid black;">Aktiviert – Excel-Arbeitsmappe (*.xlsx).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1039</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung sieht **Excel-Arbeitsmappe (\*.xlsx)** als Standarddateiformat für das Speichern von Arbeitsmappen vor. Die Konfiguration setzt die Standardkonfiguration in Excel 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Die Aktivierung dieser Einstellung und die Auswahl eines anderen Formats als Standardformat für Excel 2007 verhindert nicht, dass Benutzer Dateien in anderen Formaten speichern können.
  
### Dateien in diesem Format speichern
  
Betrifft: **PowerPoint, Word**
  
Diese Einstellung kontrolliert das Standarddateiformat für das Speichern von Dateien in den angegebenen Anwendungen.
  
#### Sicherheitsrisiko
  
Standardmäßig speichern PowerPoint 2007 und Word 2007 neue Dateien im Office Open XML-Format: PowerPoint-Dateien haben die Dateierweiterung PPTX, Word-Dateien die Dateierweiterung DOCX. Für Benutzer, die frühere Versionen von PowerPoint und Word ausführen, bietet Microsoft das Compatibility Pack für 2007 Office System an, mit dem Benutzer Office Open XML-Dateien öffnen und speichern können. Wenn einige Benutzer in Ihrem Unternehmen das Compatibility Pack nicht installieren können oder Versionen von PowerPoint und Word ausführen, die älter als Microsoft Office 2000 mit Service Pack 3 sind, können diese Benutzer möglicherweise nicht auf Office Open XML-Dateien zugreifen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung in PowerPoint 2007 **aktiviert** ist, können Administratoren das Standarddateiformat der Anwendung optional wie folgt festlegen:
  
-   **PowerPoint-Präsentation (\*.pptx):** Diese Option ist die Standardkonfiguration in PowerPoint 2007.  
-   **PowerPoint-Präsentation mit Makros (\*.pptm)**  
-   **PowerPoint 97-2003-Präsentation (\*.ppt)**
  
Wenn diese Einstellung in Word 2007 **aktiviert** ist, können Administratoren das Standarddateiformat der Anwendung optional wie folgt festlegen:
  
-   **Word-Dokument (\*.docx):** Diese Option ist die Standardkonfiguration.  
-   **Webseite in einer Datei (\*.mht)**  
-   **Webseite (\*.htm; \*.html)**  
-   **Webseite, gefiltert (\*.htm, \*.html)**  
-   **Rich-Text-Format (\*.rtf)**  
-   **Nur-Text (\*.txt)**  
-   **Word 6.0/95 (\*.doc)**  
-   **Word 6.0/95 - Chinesisch (vereinfacht) (\*.doc)**  
-   **Word 6.0/95 - Chinesisch (traditionell) (\*.doc)**  
-   **Word 6.0/95 - Japanisch (\*.doc)**  
-   **Word 6.0/95 - Koreanisch (\*.doc)**  
-   **Word 97-2002 und Word 6.0/95 – RTF**  
-   **Word 5.1 für Macintosh (\*.mcw)**  
-   **Word 5.0 für Macintosh (\*.mcw)**  
-   **Word 2.x für Windows (\*.doc)**  
-   **Works 4.0 für Windows (\*.wps)**  
-   **WordPerfect 5.x für Windows (\*.doc)**  
-   **WordPerfect 5.1 für DOS (\*.doc)**  
-   **Word 2007-Dokument mit Makros (\*.docm)**  
-   **Word 2007-Vorlage ohne Makros (\*.dotx)**  
-   **Word 2007-Vorlage mit Makros (\*.dotm)**  
-   **Word 97-2003-Dokument (\*.doc)**  
-   **Word 97-2003-Vorlage (\*.dot)**  
-   **Flache XML-Dokument (\*.xml)**
  
Benutzer können Präsentationen oder Dokumente auch in einem anderen Dateiformat als dem Standardformat speichern.
  
**Tabelle 1.212: Dateien in diesem Format speichern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Speichern
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Speichern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">[PowerPoint] Aktiviert (PowerPoint-Präsentation (*.pptx))
[Word] Aktiviert (Word-Dokument (*.docx))</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">PowerPoint: CCE-1719Word: CCE-1656</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlenen Einstellungen für die SSLF-Umgebung erzwingen die Standardkonfiguration in PowerPoint 2007 und Word 2007 und sollte deshalb für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Die Aktivierung dieser Einstellung und die Auswahl eines anderen Formats als das Standardformat für Word 2007 und PowerPoint 2007 verhindert nicht, dass Benutzer Dateien in anderen Formaten speichern.
  
### Sicherheitseinstellung für Makros
  
Betrifft: **Outlook**
  
Diese Einstellung steuert die Sicherheitsstufe für Makros in Excel 2007.
  
#### Sicherheitsrisiko
  
Um Benutzer vor gefährlichem Code zu schützen, werden bei der Standardkonfiguration für Outlook 2007 alle Makros deaktiviert, die nicht vertrauenswürdig sind, darunter nicht signierte Makros, Makros mit abgelaufenen oder ungültigen Signaturen und Makros mit gültigen Signaturen von Herausgebern, die nicht in der Liste vertrauenswürdiger Herausgeber aufgeführt sind. Die Standardkonfiguration lässt außerdem zu, das Makros, die von vertrauenswürdigen Herausgebern signiert sind, automatisch und ohne Benachrichtigung an den Benutzer ausgeführt werden. Das führt möglicherweise dazu, dass gefährlicher Code ausgeführt wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen für die Handhabung von Makros in Outlook 2007 zur Verfügung:
  
-   **Immer warnen**. Diese Option entspricht der Option **Warnungen für alle Makros** im Bereich **Makrosicherheit** des Outlook-Vertrauensstellungscenters. Outlook deaktiviert alle Makros, die nicht von einem vertrauenswürdigen Speicherort aus geöffnet werden, selbst wenn die Makros von einem vertrauenswürdigen Herausgeber signiert sind. Für jedes deaktivierte Makro zeigt Outlook ein Dialogfeld mit einer Sicherheitswarnung an, das Informationen über das Makro und seine digitale Signatur (wenn vorhanden) enthält. Benutzer können das Makro dann entweder aktivieren oder deaktiviert lassen.  
-   **Nie warnen, alle deaktivieren**. Diese Option entspricht der Option **Keine Warnungen und alle Makros deaktivieren** im Vertrauensstellungscenter. Outlook deaktiviert alle Makros, die nicht von vertrauenswürdigen Speicherorten aus geöffnet werden und gibt keine Benachrichtigung an Benutzer aus.  
-   **Warnung für signierte, nicht signierte deaktivieren**. Diese Option entspricht der Option **Warnungen für signierte Makros. Alle nicht signierten Makros sind deaktiviert** im Vertrauensstellungscenter. Outlook verarbeitet Makros wie folgt:
  
    -   Wenn ein Makro von einem vertrauenswürdigen Herausgeber digital signiert ist, kann das Makro ausgeführt werden, wenn der Benutzer dem Herausgeber bereits vertraut hat.  
    -   Wenn ein Makro eine gültige Signatur von einem Herausgeber hat, dem der Benutzer nicht vertraut hat, lässt das Dialogfeld mit der Sicherheitswarnung für das Makro den Benutzer auswählen, ob das Makro für die aktuelle Sitzung aktiviert oder deaktiviert oder der Herausgeber der Liste vertrauenswürdiger Herausgeber hinzugefügt werden soll, sodass es in Zukunft ohne Aufforderung an den Benutzer ausgeführt wird.  
    -   Wenn ein Makro keine gültige Signatur besitzt, deaktiviert Outlook das Makro, ohne eine Bestätigung des Benutzers anzufordern, es sei denn, es wird von einem vertrauenswürdigen Speicherort aus geöffnet.
  
    Diese Option ist die Standardkonfiguration in Outlook 2007.
  
-   **Keine Sicherheitsüberprüfung**. Diese Option entspricht der Option **Keine Sicherheitsüberprüfung für Makros (nicht empfohlen)** im Vertrauensstellungscenter. Outlook führt alle Makros aus, ohne den Benutzer zur Bestätigung aufzufordern. Diese Konfiguration führt dazu, dass die Computer von Benutzern anfällig für potenziell schädlichen Code werden, und ist nicht empfehlenswert.
  
**Tabelle 1.213: Sicherheitseinstellungen für Makros**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Warnung für signierte, nicht signierte deaktivieren)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Nie warnen, alle deaktivieren)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1030</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Nie warnen, alle deaktivieren**. Diese Konfiguration führt dazu, dass Outlook 2007-Benutzer alle Vorteile der von Makros bereitgestellten Funktionalität verlieren. Benutzer, die von Makros profitieren möchten, können die Makros an einem vertrauenswürdigen Speicherort installieren. Das funktioniert allerdings nur, wenn die Option **Alle vertrauenswürdigen Speicherorte deaktivieren** nicht auf **Aktiviert** gesetzt ist.
  
### Alle signierten Nachrichten als Klartext senden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 signierte Nachrichten als signierte Nachrichten in Klartext versendet.
  
#### Sicherheitsrisiko
  
Wenn Benutzer E-Mail-Nachrichten mit ihrer digitalen Signatur signieren und dann versenden, verwendet Outlook 2007 standardmäßig den privaten Schlüssel der Signatur, um die digitale Signatur zu verschlüsseln, versendet die Nachrichten aber in Klartext, wenn sie nicht separat verschlüsselt werden. Wenn Benutzer diese Funktion ändern, indem sie die Option **Signierte Nachrichten als Klartext senden** im Bereich **E-Mail-Sicherheit** des Vertrauensstellungscenters deaktivieren, können alle Empfänger, die nicht auf das digitale Zertifikat des Absenders zugreifen oder dieses benutzen können, die E-Mail-Nachrichten nicht lesen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird die Option **Signierte Nachrichten als Klartext senden** im Bereich **E-Mail-Sicherheit** im Vertrauensstellungscenter aktiviert. Outlook 2007-Benutzer können diese Einstellung nicht ändern.
  
**Tabelle 1.214: Alle signierten Nachrichten als Klartext senden**

 
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
<td style="border:1px solid black;">CCE-14</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Eingabeaufforderung für das ItemProperty-Steuerelement festlegen
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, was geschieht, wenn Benutzer Steuerelemente zu einem benutzerdefinierten Outlook 2007-Formular hinzufügen und die Steuerelemente dann direkt an eines der Adressinformationsfelder binden.
  
#### Sicherheitsrisiko
  
Wenn ein Steuerelement in einem benutzerdefinierten Outlook 2007-Formular direkt an eines der Adressinformationsfelder gebunden wird, kann der Formularcode indirekt den Wert des Adressinformationsfelds abrufen, indem er die Eigenschaft „Wert“ des Steuerelements erhält. Wenn das benutzerdefinierte Formular von einem böswilligen oder unerfahrenen Benutzer erstellt wurde, erhalten nicht autorisierte Personen möglicherweise Zugriff auf vertrauliche Daten.
  
Standardmäßig gibt Outlook eine Eingabeaufforderung an den Benutzer aus, wenn dieser ein Steuerelement an ein Adressinformationsfeld bindet.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren anhand von vier Optionen steuern, wie sich Outlook beim Öffnen eines benutzerdefinierten Formulars verhalten soll, das ein Steuerelement enthält, das an ein Adressinformationsfeld gebunden ist:
  
-   **Eingabeaufforderung für Benutzer**  
-   **Automatisch genehmigen**  
-   **Automatisch ablehnen**  
-   **Benutzer basierend auf der Computersicherheit auffordern**
  
**Tabelle 1.215: Eingabeaufforderung für das ItemProperty-Steuerelement festlegen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Benutzerdefinierte Formularsicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Automatisch ablehnen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1586</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Sie können Exchange-Sicherheitsformulareinstellungen auch konfigurieren, indem Sie die Einstellung „Outlook-Sicherheitsmodus“ in „Benutzerkonfiguration\\Administrative Vorlagen\\Klassische administrative Vorlage (ADM)\\Microsoft Office Outlook 2007\\Sicherheit\\Sicherheitsformulareinstellungen\\Microsoft Office Outlook 2007-Sicherheit“ aktivieren und **Outlook-Sicherheitsgruppenrichtlinie verwenden** aus der Dropdownliste auswählen.
  
### Maximale Onlinestatusebene für einen Personennamen festlegen
  
Betrifft: **Outlook**
  
Mit dieser Einstellung können Administratoren steuern, wie viele Anwesenheitsinformationen Benutzer für Kontakte und E-Mail-Empfänger sehen können, wenn sie ein kompatibles Instant Messaging-Clientprogramm ausführen.
  
#### Sicherheitsrisiko
  
Outlook 2007 kann Anwesenheitsinformationen für Kontakte und E-Mail-Empfänger anzeigen, wenn Benutzer ein kompatibles Instant Messaging-Clientprogramm wie Microsoft Office Communicator oder Windows Live Messenger ausführen. Diese Informationen werden als Symbol angezeigt, das neben dem Namen der Personen angezeigt wird und zeigt, ob diese aktuell für Kommunikationszwecke verfügbar sind. Wenn Benutzer auf das Symbol klicken, wird ein Menü angezeigt, über das sie weitere Informationen finden und andere Aktionen durchführen können, etwa das Versenden einer Nachricht. Outlook kann Anwesenheitsinformationen an verschiedenen Stellen anzeigen, beispielsweise in den Kontakten, im Adressbuch und in den Benachrichtigungsfeldern eingehender und ausgehender E-Mail-Nachrichten.
  
Standardmäßig zeigt Outlook Anwesenheitsinformationen an verschiedenen Stellen an. Benutzer, die ein kompatibles Instant Messaging-Clientprogramm ausführen, können diese Konfiguration ändern, indem sie auf **Extras**, **Optionen** und die Registerkarte **Weitere** klicken und dann die unter **Personennamen** aufgelisteten Optionen ändern. Wenn Benutzer den Onlinestatus und weitere Anwesenheitsdetails von anderen sehen können, sind in einigen Situationen möglicherweise die Privatsphäre oder vertrauliche Daten gefährdet.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen zur Verfügung, mit denen sie die Konfiguration von Anwesenheitsindikatoren in Outlook 2007 durch Benutzer regeln können:
  
-   **Nicht zulassen**. Anwesenheitsindikatoren werden an keiner Stelle in Outlook angezeigt, und Benutzer können diese Konfiguration nicht ändern. In der Benutzeroberfläche sind beide Optionen unter **Personennamen** nicht verfügbar.  
-   **Überall zulassen, außer in den Feldern „An“ und „CC“**. Benutzer können auswählen, ob sie Anwesenheitsindikatoren in Outlook anzeigen möchten, können diese aber nicht in den Feldern „An“ und „CC“ von E-Mail-Nachrichten anzeigen. In der Benutzeroberfläche ist das Kontrollkästchen **Onlinestatus neben einem Personennamen anzeigen** verfügbar und kann von Benutzern aktiviert oder deaktiviert werden. Das Kontrollkästchen **Onlinestatus nur dann in den Feldern „An“ und „Cc“ anzeigen, wenn der Mauszeiger auf einen Personnamen zeigt** ist aktiviert und ausgeblendet.  
-   **Überall zulassen**. Benutzer erhalten die vollständige Kontrolle über die Optionen für die Anzeige von Anwesenheitsinformationen. In der Benutzeroberfläche ist das Kontrollkästchen **Onlinestatus neben einem Personennamen anzeigen** verfügbar und kann von Benutzern aktiviert oder deaktiviert werden. Wenn dieses Kontrollkästchen aktiviert ist, wird auch das Kontrollkästchen **Onlinestatus nur dann in den Feldern „An“ und „Cc“ anzeigen, wenn der Mauszeiger auf einen Personnamen zeigt** verfügbar.  
-   **Anwesenheit überall zulassen, bei Bedarf mit Exchange-RPCs**. Wie bei der Option **Überall zulassen** erhalten Benutzer die vollständige Kontrolle über die Optionen für die Anzeige von Anwesenheitsinformationen. Darüber hinaus verwendet Outlook für das Abrufen von Anwesenheitsinformationen Remoteprozeduraufrufe an den Exchange-Server, wenn Outlook im Exchange-Cache-Modus mit einem Offlineadressbuch (OAB) ausgeführt wird und Anwesenheitsinformationen lokal nicht verfügbar sind. Diese Option stellt Benutzern die genauesten Anwesenheitsinformationen zur Verfügung, steigert aber das Netzwerkverkehrsaufkommen. Standardmäßig verwendet Outlook keine Exchange-RPCs zum Abrufen von Anwesenheitsinformationen, wenn das Programm im Exchange-Cache-Modus ausgeführt wird.
  
**Tabelle 1.216: Maximale Onlinestatusebene für einen Personennamen festlegen**

 
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
<td style="border:1px solid black;">Aktiviert (Nicht zulassen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1596</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung von **Nicht zulassen** verhindert, dass Outlook 2007 Anwesenheitsindikatoren anzeigt. Benutzern wird es dadurch möglicherweise erschwert, andere zu kontaktieren oder deren Verfügbarkeit sicherzustellen. Die anderen Optionen dürften für die meisten Benutzer keine größeren Nutzbarkeitsprobleme verursachen.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Diese Einstellung wird außer Kraft gesetzt, wenn die Einstellung „Onlinestatus für Personennamen anzeigen“ aktiviert ist. Die Einstellung „Onlinestatus für Personennamen anzeigen“ konfiguriert Anwesenheitsoptionen für alle betroffenen Benutzer und verhindert, dass Benutzer diese ändern können. Weitere Informationen zu dieser Einstellung finden Sie unter dem entsprechenden Eintrag in diesem Handbuch.
  
### Nachrichtenformat festlegen
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt das Standardnachrichtenformat in Outlook 2007.
  
#### Sicherheitsrisiko
  
Standardmäßig werden neue E-Mail-Nachrichten in Outlook 2007 im HTML-Format formatiert. Wenn Benutzer Nachrichten an Empfänger mit E-Mail-Programmen senden, die HTML-Nachrichten nicht korrekt anzeigen können, gehen beim Versenden von Nachrichten in diesem Format möglicherweise Informationen verloren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren für E-Mail-Nachrichten in Outlook 2007 HTML, Rich Text oder Nur-Text als Standardformat einrichten. Benutzer können beim Verfassen von Nachrichten ein anderes Format als das Standardformat auswählen.
  
**Tabelle 1.217: Nachrichtenformat festlegen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\E-Mail-Format\Internetformatierung\Nachrichtenformat</td>
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
<td style="border:1px solid black;">Aktiviert (Nur-Text)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1526</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert nicht, dass Outlook 2007-Benutzer ein anderes Format als das Standardformat verwenden können, und sollte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Ausführungseingabeaufforderung für Outlook-Objektmodell „Benutzerdefinierte Aktionen“ festlegen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 vor der Ausführung einer benutzerdefinierten Aktion eine Bestätigungsaufforderung für Benutzer ausgibt.
  
#### Sicherheitsrisiko
  
Benutzerdefinierte Aktionen fügen Outlook 2007 Funktionen hinzu, die als Teil einer Regel ausgelöst werden können. Unter anderem können benutzerdefinierte Aktionen erstellt werden, die Nachrichten auf eine Weise beantworten, die programmgesteuerte Schutzmaßnahmen des Outlook-Objektmodells beim Senden umgeht.
  
Wenn Outlook oder ein anderes Programm eine benutzerdefinierte Aktion mithilfe des Outlook-Objektmodells initiiert, werden Benutzer standardmäßig aufgefordert zu entscheiden, ob sie die Aktion zulassen oder ablehnen. Wenn diese Konfiguration geändert wird, kann schädlicher Code das Outlook-Objektmodell nutzen, um vertrauliche Daten abzurufen oder die Sicherheit von Daten und Computerressourcen anderweitig zu gefährden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren anhand von vier Optionen steuern, wie sich Outlook bei der Ausführung einer benutzerdefinierten Aktion verhält, die das Outlook-Objektmodell verwendet:
  
-   **Eingabeaufforderung für Benutzer**  
-   **Automatisch genehmigen**  
-   **Automatisch ablehnen**  
-   **Benutzer basierend auf der Computersicherheit auffordern**. Diese Option setzt die Standardkonfiguration in **Outlook** durch.
  
**Tabelle 1.218: Ausführungseingabeaufforderung für Outlook-Objektmodell „Benutzerdefinierte Aktionen“ festlegen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen\Benutzerdefinierte Formularsicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzer basierend auf der Computersicherheit auffordern)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Automatisch ablehnen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1436</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Automatisch ablehnen**. Sie verhindert, dass Outlook 2007 benutzerdefinierte Aktionen ausführt, die das Outlook-Objektmodell verwenden. Wenn sich Benutzer auf derartige Aktionen verlassen, müssen Sie möglicherweise alternative Methoden für die Bereitstellung dieser Funktionalität finden.
  
### Alle E-Mail-Nachrichten signieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 digitale Signaturen für alle ausgehenden E-Mail-Nachrichten verlangt.
  
#### Sicherheitsrisiko
  
Standardmäßig erfordert Outlook 2007 keine digitalen Signaturen für ausgehende Nachrichten. Wenn Ihr Unternehmen das Signieren von E-Mail-Nachrichten anhand von Richtlinien festgelegt hat, um die Authentizität der Nachrichten zu sichern, verstoßen die Benutzer möglicherweise gegen diese Richtlinien, wenn Sie das Versenden nicht signierter Nachrichten zulassen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, erfordert Outlook 2007 für alle ausgehenden Nachrichten vor dem Versenden eine digitale Signatur.
  
**Tabelle 1.219: Alle E-Mail-Nachrichten signieren**

 
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
<td style="border:1px solid black;">CCE-1639</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann deutliche Beeinträchtigungen für Outlook 2007-Benutzer verursachen, die nicht über gültige Signaturen für das Signieren von E-Mail-Nachrichten verfügen. Diese Benutzer können erst dann E-Mail-Nachrichten versenden, wenn sie digitale Signaturen erhalten haben.
  
### Signaturwarnung
  
Betrifft: **Outlook**
  
Diese Einstellung bestimmt, wie Outlook 2007 Benutzer vor Nachrichten mit ungültigen digitalen Signaturen warnt.
  
#### Sicherheitsrisiko
  
Wenn Benutzer E-Mail-Nachrichten mit ungültigen digitalen Signaturen öffnen, zeigt Outlook 2007 standardmäßig ein Warndialogfeld an. Benutzer können entscheiden, ob sie zukünftig vor ungültigen Signaturen gewarnt werden möchten.
  
Wenn Benutzer bei ungültigen Signaturen keine Benachrichtigung erhalten, können sie eine betrügerische Signatur, die von einer böswilligen Person versendet wurde, möglicherweise nicht erkennen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren anhand von drei Optionen steuern, wie Outlook 2007 Benutzer vor ungültigen Signaturen warnt:
  
-   **Benutzer entscheidet, ob er gewarnt werden möchte**. Diese Option setzt die Standardkonfiguration durch.  
-   **Immer wegen ungültigen Signaturen warnen**.  
-   **Nie bei ungültigen Signaturen warnen**.
  
**Tabelle 1.220: Signaturwarnung**

 
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
<td style="border:1px solid black;">Aktiviert – Immer wegen ungültigen Signaturen warnen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert – Immer wegen ungültigen Signaturen warnen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-700</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt möglicherweise zu Beeinträchtigungen für Outlook 2007-Benutzer, die viele mit ungültigen Signaturen signierte Nachrichten erhalten. Diesen Benutzern wird bei jedem Öffnen einer solchen Nachricht ein Warndialogfeld angezeigt.
  
### Makro standardmäßig in „Persönliche Makroarbeitsmappe“ speichern
  
Betrifft: **Excel**
  
Diese Einstellung bestimmt den Standardspeicherort für das Speichern von Arbeitsmappen in Excel 2007.
  
#### Sicherheitsrisiko
  
Das Dialogfeld **Makro aufzeichnen** enthält ein Dropdownmenü, über das Benutzer auswählen können, ob das neue Makro in der aktuellen Arbeitsmappe, einer neuen Arbeitsmappe oder der persönlichen Makroarbeitsmappe (Personal.xlsb) gespeichert werden soll, einer verborgenen Arbeitsmappe, die bei jedem Start von Excel 2007 geöffnet wird.
  
Standardmäßig zeigt Excel das Dialogfeld **Makro aufzeichnen** mit bereits aktivierter Option **Diese Arbeitsmappe** im Dropdownmenü an. Wenn ein Benutzer ein Makro in der aktiven Arbeitsmappe speichert und diese an andere Benutzer verteilt, wird das Makro zusammen mit der Arbeitsmappe weitergegeben. Bei versehentlicher oder absichtlicher Auslösung des Makros besteht möglicherweise ein Sicherheitsrisiko für die Daten in der Arbeitsmappe.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, zeigt Excel 2007 das Dialogfeld **Makro aufzeichnen** mit bereits aktivierter Option **Persönliche Makroarbeitsmappe** im Dropdownmenü an. Benutzer können weiterhin eine der anderen zwei Optionen im Dropdownmenü aktivieren.
  
**Tabelle 1.221: Makro standardmäßig in „Persönliche Makroarbeitsmappe“ speichern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">excel12.adm</td>
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
<td style="border:1px solid black;">CCE-1246</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert nicht, dass Benutzer einen anderen Speicherort für das Speichern von Makros auswählen, deshalb wird sie für die meisten Benutzer kaum zu wesentlichen Beeinträchtigungen führen.
  
### Menüelement für externe Signaturdienste unterdrücken
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Outlook 2007 das Menüelement **Signaturdienste hinzufügen** anzeigt.
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer **Signaturdienste hinzufügen** (aus dem Dropdownmenü **Signaturzeile** auf der Registerkarte **Einfügen** der Multifunktionsleiste in Excel 2007, PowerPoint 2007 und Word 2007) aktivieren, um eine Liste von Signaturdienstanbietern auf der [Microsoft Office](http://office.microsoft.com/)-Website anzuzeigen. Wenn Ihr Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Signaturanbieter oder Office Marketplace verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn Sie zulassen, dass sie auf das Menüelement **Signaturdienste hinzufügen** zugreifen können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, zeigt Outlook 2007 das Menüelement **Signaturdienste hinzufügen** nicht im Dropdownmenü **Signaturzeile** an.
  
**Tabelle 1.222: Menüelement für externe Signaturdienste unterdrücken**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Signatur</td>
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
<td style="border:1px solid black;">CCE-1220</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert das Hinzufügen eines Signaturdiensts von Microsoft Office Online durch Benutzer, sollte aber ansonsten für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Office-Signaturanbieter unterdrücken
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer Word 2007-Dokumenten und Excel 2007-Arbeitsmappen eine Microsoft Office-Standardsignaturzeile hinzufügen können.
  
#### Sicherheitsrisiko
  
Digitale Signaturen stellen die Authentizität, Integrität und Nichtabstreitbarkeit elektronischer Dokumente sicher. In Excel 2007 und Word 2007 können Benutzer einem Dokument gleichzeitig mit der digitalen Signatur sichtbare Darstellungen ihrer Signaturen hinzufügen. Die Möglichkeit, digitale Signaturen durch die Verwendung von Signaturzeilen in 2007 Office-Dokumenten aufzunehmen, ermöglicht Unternehmen die Verwendung papierloser Signierungsvorgänge für Dokumente wie Verträge oder andere Vereinbarungen.
  
Standardmäßig bieten Excel 2007 und Word 2007 zwei Arten von Signaturzeilen an, die als „Microsoft Office-Signaturzeile“ und „Stempelsignaturzeile“ bezeichnet werden. Die für die Benutzer verfügbare(n) Option(en) sind je nach Bearbeitungssprache(n) unterschiedlich, die bei der Installation für die Anwendung konfiguriert wurde(n).
  
-   Die Microsoft Office-Signaturzeile zeigt den Buchstaben „X“ an, gefolgt von einer horizontalen Linie, eine vertraute Konvention für handschriftliche Signaturzeilen.  
-   Die Stempelsignaturzeile ist nur für Benutzer der Sprachversionen Vereinfachtes Chinesisch, Traditionelles Chinesisch, Japanisch oder Koreanisch der 2007 Microsoft Office-Version verfügbar sowie für Benutzer, die das Microsoft Office Project Multi Language Pack 2007 für eine dieser Sprachen installiert haben. Diese Signaturzeile zeigt ein Quadrat an, eine Konvention in Ländern, in denen Gummiidentitätsstempel (die in Japan und Südkorea als *Hanko* bezeichnet werden) für das Signieren von Dokumenten verwendet werden.
  
Bei beiden Arten von Signaturzeilen kann der Signierende seinen Namen, seinen Titel und seine E-Mail-Adresse angeben. Wenn keine Art von Signaturzeile angemessen ist, können Sie Office-Anwendungen Signaturprodukte von Drittanbietern hinzufügen, die verschiedene Anforderungen erfüllen.
  
Wenn Benutzer nicht die richtige Signaturzeile zur Auswahl haben, können sie Dokumente möglicherweise nicht digital signieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen für die Aktivierung der 2007 Office-Standardsignaturzeilen zur Verfügung:
  
-   **Westlich und Ostasiatisch aktivieren**. Sowohl die **Microsoft Office-Signaturzeile** als auch die **Stempelsignaturzeile** sind über das Dropdownmenü **Signaturzeile** auf der Registerkarte **Einfügen** der Multifunktionsleiste verfügbar.  
-   **Standard Westlich unterdrücken**. Benutzer können Dokumenten die Microsoft Office-Signaturzeile nicht hinzufügen.  
-   **Standard Ostasiatisch unterdrücken**. Benutzer können Dokumenten die Stempelsignaturzeile nicht hinzufügen.  
-   **Westlich und Ostasiatisch unterdrücken**. Keine der Standardsignaturzeilen ist verfügbar. Diese Einstellung tritt nur in Kraft, wenn mindestens ein anderer gültiger Signaturanbieter installiert ist.
  
**Tabelle 1.223: Office-Signaturanbieter unterdrücken**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Signatur</td>
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
<td style="border:1px solid black;">CCE-1572</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die optimale Auswahl für diese Einstellung hängt von den Richtlinien und Standards des jeweiligen Unternehmens ab. Ein Unternehmen kann entscheiden, die Office-Standardsignaturzeilen zu unterdrücken, um die Nutzung einer benutzerdefinierten Signaturzeile durchzusetzen, die den bestimmten Anforderungen des Unternehmens entspricht. (Ein Unternehmen kann beispielsweise eine Signaturzeile implementieren, die einen stärkeren Hashalgorithmus als SHA1 verwendet, der von den Standardsignaturzeilen benutzt wird.)
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Diese Einstellung betrifft nur sichtbare Signaturzeilen in Excel 2007-Arbeitsmappen und Word 2007-Dokumenten. Sie wirkt sich nicht auf Möglichkeit aus, dass Benutzer Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen und Word 2007-Dokumenten unsichtbare digitale Signaturen hinzufügen können.
  
### Outlook-RSS-Feeds mit der gemeinsamen Feedliste synchronisieren
  
Betrifft: **Outlook**
  
Diese Einstellung legt fest, ob Outlook 2007 die gemeinsame Feedliste abonniert, die mehreren RSS-Clients zur Verfügung gestellt wird.
  
#### Sicherheitsrisiko
  
Die gemeinsame Feedliste ist eine hierarchische Sammlung von RSS-Feeds, die Clients wie Outlook 2007, die Feedliste in Internet Explorer 7 und die Minianwendung für Feedschlagzeilen der Windows Vista-Sidebar abonnieren können.
  
Wenn Outlook eine sehr große Feedliste abonniert, können die Leistung und die Verfügbarkeit beeinträchtigt werden, insbesondere wenn Outlook für das Herunterladen vollständiger RSS-Nachrichtentexte konfiguriert ist oder die Feedliste nicht regelmäßig automatisch archiviert wird.
  
Standardmäßig verwaltet Outlook seine eigenen Feedlisten und abonniert nicht automatisch RSS-Feeds, die der gemeinsamen Feedliste hinzugefügt werden.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, abonniert Outlook 2007 automatisch RSS-Feeds, die in Internet Explorer hinzugefügt werden, und Outlook RSS-Feeds werden mit der gemeinsamen Feedliste synchronisiert, sodass sie in Internet Explorer verfügbar sind. Achten Sie darauf, dass Drittanbieteranwendungen außer Internet Explorer der gemeinsamen Feedliste Feeds hinzufügen können und Outlook diese bei Aktivierung dieser Einstellung ebenfalls abonniert.
  
**Tabelle 1.224: Outlook-RSS-Feeds mit der gemeinsamen Feedliste synchronisieren**

 
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
<td style="border:1px solid black;">Outlk12.adm</td>
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
<td style="border:1px solid black;">CCE-1131</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die auf die gemeinsame Feedliste für gewöhnlich in Outlook zugreifen. Benutzer haben weiterhin Zugriff auf die gemeinsame Feedliste über Internet Explorer 7 und andere Clientprogramme. Die Deaktivierung dieser Einstellung verhindert nicht, dass Benutzer eine separate Abonnementliste für RSS-Feeds in Outlook 2007 unterhalten.
  
### Zugriff auf Visual Basic-Projekt vertrauen
  
Betrifft: **Excel, PowerPoint, Word**
  
Diese Einstellung steuert, ob Automatisierungsclients wie Microsoft Visual Studio 2005 Tools for the Microsoft Office System (VSTO) auf das Visual Basic for Applications-Projektsystem in den angegebenen Anwendungen zugreifen können.
  
#### Sicherheitsrisiko
  
VSTO-Projekte erfordern Zugriff auf das Visual Basic for Applications-Projektsystem in Excel 2007, PowerPoint 2007 und Word 2007, selbst wenn die Projekte Visual Basic for Applications nicht verwenden. Die Entwurfszeitunterstützung für Steuerelemente sowohl in Visual Basic- als auch C\#-Projekten hängt in Word und Excel vom Visual Basic for Applications-Projektsystem ab.
  
Standardmäßig lassen Excel, Word und PowerPoint nicht zu, dass Automatisierungsclients einen programmgesteuerten Zugriff auf VBA-Projekte erhalten. Benutzer können dies aktivieren, indem sie die Option **Zugriff auf das VBA-Projektobjektmodell vertrauen** im Bereich **Makroeinstellungen** des Vertrauensstellungscenters aktivieren. Das bedeutet allerdings, dass Makros in allen vom Benutzer geöffneten Dokumenten auf die Visual Basic-Kernobjekte, -methoden und -eigenschaften zugreifen können, was ein potenzielles Sicherheitsrisiko darstellt.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, wird das Kontrollkästchen **Zugriff auf das VBA-Projektobjektmodell vertrauen** deaktiviert, und Benutzer können diese Einstellung nicht ändern.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Durch die Deaktivierung dieser Einstellung können VSTO-Projekte in der ausgewählten Anwendung nicht richtig mit dem VBA-Projektsystem interagieren.
  
**Tabelle 1.225: Zugriff auf Visual Basic-Projekt vertrauen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">excel12.adm, ppt12.adm, word12.adm</td>
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
<td style="border:1px solid black;">Excel: CCE-862PowerPoint: CCE-68Word: CCE-703</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Excel 2007, Word 2007 und PowerPoint 2007 durch und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### E-Mail von Kontakten vertrauen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 beim Filtern von Junk-E-Mail E-Mail-Nachrichten von Absendern aus der Kontaktliste von Benutzern analysiert.
  
#### Sicherheitsrisiko
  
Standardmäßig werden E-Mail-Adressen in den Kontaktlisten von Benutzern beim Filtern von Junk-E-Mail als sichere Absender angesehen. Wenn diese Konfiguration geändert wird, können E-Mail-Nachrichten von Benutzerkontakten fälschlicherweise als Junk-E-Mail klassifiziert werden und wichtige Informationen verloren gehen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird das Kontrollkästchen **Meine Kontakte sind auch vertrauenswürdige Absender** auf der Registerkarte **Sichere Absender** des Dialogfelds **Junk-E-Mail-Optionen** aktiviert, und Benutzer können diese Einstellung nicht ändern.
  
**Tabelle 1.226: E-Mail von Kontakten vertrauen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Junk-E-Mail</td>
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
<td style="border:1px solid black;">CCE-1117</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Option „Smarttag für Personennamen aktivieren“ deaktivieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Smarttags für Personennamen in Outlook 2007 angezeigt werden.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103514).
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer das Smarttag „Personennamen“ aktivieren, sodass 2007 Office-Anwendungen Namen von Personen erkennen und mit Smarttagindikatoren markieren. Die Auswahl eines Smarttags führt dazu, dass die Anwendung Daten über die Person aus Active Directory abruft, sofern dies möglich ist. In einigen Situationen führt diese Funktionalität möglicherweise dazu, dass nicht autorisierte Personen Zugriff auf vertrauliche Daten erhalten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, markiert Outlook 2007 die Namen von Personen nicht mit Smarttagindikatoren.
  
**Tabelle 1.227: Option „Smarttag für Personennamen aktivieren“ deaktivieren**

 
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
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1648</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die sich auf Smarttags für Personennamen verlassen. Allerdings sind Smarttags in Outlook 2007 standardmäßig deaktiviert und werden in der 2007 Office-Version nicht so stark verwendet wie in früheren Versionen. Beeinträchtigungen sollten in den meisten Situationen minimal sein.
  
### RSS-Feature deaktivieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob die RSS-Aggregationsfunktion in Outlook 2007 deaktiviert ist.
  
#### Sicherheitsrisiko
  
Standardmäßig können Benutzer aus Outlook 2007 heraus RSS-Feeds abonnieren und RSS-Elemente wie E-Mail-Nachrichten lesen. Wenn Ihr Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie RSS-Feeds verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn sie in Outlook RSS-Feeds abonnieren können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, wird die RSS-Aggregationsfunktion in Outlook 2007 deaktiviert.
  
**Tabelle 1.228: RSS-Funktion deaktivieren**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1620</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu einigen Beeinträchtigungen für Benutzer führen, die RSS-Feeds normalerweise in Outlook 2007 lesen. Sie wirkt sich nicht auf die Leistung anderer RSS-Clients wie Internet Explorer 7 aus.
  
### Blockierung des automatischen Downloads von verknüpften Bildern aufheben
  
Betrifft: **PowerPoint**
  
Diese Einstellung bestimmt, ob PowerPoint 2007 automatisch Links aus externen Quellen herunterlädt.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Bilder in PowerPoint 2007-Präsentationen einfügen, können Sie die Option **Mit Datei verknüpfen** anstelle von **Einfügen** auswählen. Dann wird das Bild durch einen Link zu einer Datei auf einem Datenträger dargestellt, statt in die Präsentationsdatei selbst eingebettet zu werden.
  
Wenn PowerPoint eine Präsentation öffnet, stellt das Programm standardmäßig keine verknüpften Bilder dar, die auf einem anderen Computer gespeichert sind, es sei denn, die Präsentation selbst ist an einem vertrauenswürdigen Speicherort gespeichert (wie im Vertrauensstellungscenter konfiguriert). Wenn diese Konfiguration geändert wird, lädt PowerPoint beliebige Bilder, die an Remotespeicherorten gespeichert wurden, was ein Sicherheitsrisiko darstellt.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, lädt PowerPoint 2007 keine Bilder, die an Remotespeicherorten gespeichert sind.
  
![](images/Dd443663.note(de-de,TechNet.10).gif)**Hinweis:**
  
Wenn diese Einstellung **aktiviert** ist, lädt PowerPoint 2007 Bilder, die an Remotespeicherorten gespeichert sind, was möglicherweise die Sicherheit verringert.
  
**Tabelle 1.229: Blockierung des automatischen Downloads von verknüpften Bildern aufheben**

 
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
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1451</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in PowerPoint 2007 durch und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Hyperlinks unterstreichen
  
Betrifft: **Access**
  
Diese Einstellung steuert, ob Hyperlinks in Access 2007-Tabellen, -Abfragen, -Formularen und -Berichten unterstrichen sind.
  
#### Sicherheitsrisiko
  
Standardmäßig unterstreicht Access 2007 Hyperlinks, die in Tabellen, Abfragen, Formularen und Berichten angezeigt werden. Wenn diese Konfiguration geändert wird, klicken Benutzer möglicherweise ohne sich dessen bewusst zu sein auf gefährliche Hyperlinks, was ein Sicherheitsrisiko bedeuten kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, unterstreicht Access 2007 alle Hyperlinks in Tabellen, Abfragen, Formularen und Berichten, wenn diese erstellt werden, und setzt alle Konfigurationsänderungen auf den Computern von Benutzern außer Kraft.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Die Aktivierung oder Deaktivierung dieser Einstellung führt nicht zu der ordnungsgemäßen Deaktivierung des Kontrollkästchens **Hyperlinks unterstreichen** im Dialogfeld **Weboptionen** in Access 2007, wodurch Benutzer fälschlicherweise davon ausgehen könnten, dass die Option weiterhin durch den Benutzer konfigurierbar bleibt. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103507).
  
**Tabelle 1.230: Hyperlinks unterstreichen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Anwendungseinstellungen\Weboptionen…\Allgemein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm</td>
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
<td style="border:1px solid black;">CCE-1395</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in Access 2007 durch und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Automatische Verknüpfungen beim Öffnen aktualisieren
  
Betrifft: **Word**
  
Diese Einstellung steuert, ob Word 2007 bei jedem Öffnen eines Dokuments automatisch Inhalte aktualisiert, die mit anderen Dateien verknüpft sind.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Dokumente öffnen, aktualisiert Word 2007 standardmäßig automatisch alle Verknüpfungen zu externen Inhalten wie Grafiken, Excel-Arbeitsblättern und PowerPoint-Folien. Der Benutzer kann die automatische Aktualisierung deaktivieren, indem er auf die **Microsoft Office-Schaltfläche** und dann auf **Word-Optionen** und **Erweitert** klickt, zum Bereich **Allgemein** navigiert und das Kontrollkästchen **Automatische Verknüpfungen beim Öffnen aktualisieren** deaktiviert.
  
Wenn Word für das automatische Aktualisieren von Verknüpfungen beim Öffnen von Dokumenten konfiguriert ist, kann sich der Dokumentinhalt ohne Wissen des Benutzers ändern, was möglicherweise ein Risiko für wichtige Informationen darstellt.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, führt Word 2007 beim Öffnen von Dokumenten keine automatische Aktualisierung von Verknüpfungen zu externen Inhalten durch. Benutzer können verknüpfte Inhalte weiterhin manuell aktualisieren, indem sie mit der rechten Maustaste auf das verknüpfte Objekt klicken und **Verknüpfung aktualisieren** auswählen. Alternativ können Benutzer auch auf die **Microsoft Office-Schaltfläche** klicken, auf **Vorbereiten** zeigen und dann auf **Verknüpfungen mit Dateien bearbeiten** klicken.
  
**Tabelle 1.231: Automatische Verknüpfungen beim Öffnen aktualisieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Erweitert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">word12.adm</td>
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
<td style="border:1px solid black;">CCE-1249</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die mit Word 2007-Dokumenten arbeiten, die externe Inhalte enthalten. Ziehen Sie in Betracht, Ihren Benutzern die Methoden für das manuelle Aktualisieren von Verknüpfungen zu zeigen.
  
### URL für S/MIME-Zertifikate
  
Betrifft: **Outlook**
  
Diese Einstellung stellt eine URL bereit, unter der Outlook 2007-Benutzer S/MIME-Zertifikate erhalten können.
  
#### Sicherheitsrisiko
  
Wenn Benutzer auf die Option **Digitale ID anfordern** im Bereich **E-Mail-Sicherheit** des Vertrauensstellungscenters klicken, öffnet Outlook 2007 eine Seite auf der Microsoft Office Online-Website, auf der sie S/MIME-Zertifikate für die Verschlüsselung und Signierung erhalten können. Wenn Ihr Unternehmen Richtlinien für die Regelung der Verwendung externer Ressourcen wie Office Online einsetzt, führt diese Konfiguration möglicherweise dazu, dass Benutzer gegen diese Richtlinien verstoßen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren eine URL eingeben, unter der Benutzer S/MIME-Zertifikate erhalten können. Die URL kann die drei Variablen *%1*, *%2* und *%3* enthalten, die durch den Namen des Benutzers, die E-Mail-Adresse bzw. die Sprache ersetzt werden. Wenn Benutzer auf **Digitale ID anfordern** klicken, werden sie an die bereitgestellte URL weitergeleitet.
  
**Tabelle 1.232: URL für S/MIME-Zertifikate**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-677</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Vergewissern Sie sich, dass die bereitgestellte URL auf eine gültige Site mit Informationen darüber verweist, wie Benutzer digitale IDs erhalten können. Andernfalls werden wahrscheinlich die Desktopsupportanfragen steigen.
  
### Unicode-Format beim Ziehen von E-Mail-Nachrichten in das Dateisystem verwenden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob E-Mail-Nachrichten, die von Outlook 2007 zum Dateisystem gezogen werden, im Unicode- oder ANSI-Format gespeichert werden.
  
#### Sicherheitsrisiko
  
Wenn Benutzer E-Mail-Nachrichten von Outlook 2007 in ein Windows Explorer-Fenster oder auf ihren Desktop ziehen, erstellt Outlook standardmäßig eine MSG-Datei, die das systemeigene Zeichencodierungsformat für das konfigurierte Gebietsschema verwendet (das so genannte „ANSI“-Format). Wenn diese Einstellung **aktiviert** ist, verwendet Outlook bei der Erstellung der Nachrichtendatei den Unicode-Zeichencodierungsstandard, wodurch Sonderzeichen in der Nachricht erhalten bleiben.
  
Unicode-Text ist aber anfällig für Homografieangriffe, bei denen Zeichen durch andere, ähnlich aussehende Zeichen ersetzt werden. Der kyrillische Buchstabe „a“ (U+0430) wirkt in vielen Schriftarten identisch mit dem lateinischen Buchstaben „a“ (U+0061), ist aber tatsächlich ein anderes Zeichen. Homografie kann in „Phishingangriffen“ verwendet werden, um Opfer davon zu überzeugen, betrügerische Websites zu besuchen und vertrauliche Daten einzugeben.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, werden E-Mail-Nachrichten, die von Outlook 2007 zum Dateisystem gezogen werden, im ANSI-Format gespeichert.
  
**Tabelle 1.233: Unicode-Format beim Ziehen von E-Mail-Nachrichten in das Dateisystem verwenden**

 
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1287</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Einstellungen für VBA-Makrowarnung
  
Betrifft: **Access, Excel, PowerPoint, Word**
  
Diese Einstellung steuert, wie die angegebenen Anwendungen Benutzer warnen, wenn Visual Basic for Applications (VBA)-Makros vorhanden sind.
  
#### Sicherheitsrisiko
  
Wenn Benutzer in den angegebenen Anwendungen Dateien öffnen, die VBA-Makros enthalten, öffnen die Anwendungen die Dateien standardmäßig mit deaktivierten Makros und zeigen in der Vertrauensstellungsleiste eine Warnung mit dem Hinweis an, dass Makros vorhanden sind und diese deaktiviert wurden. Benutzer können die Dateien bei Bedarf prüfen und bearbeiten, aber keine deaktivierte Funktionalität verwenden, solange sie nicht auf der Vertrauensstellungsleiste auf **Optionen** klicken und die entsprechende Aktion auswählen. Wenn Benutzer gefährliche Makros aktivieren, werden möglicherweise ihre Computer beeinträchtigt oder vertrauliche Daten offengelegt.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen zur Verfügung, um festzulegen, wie die angegebene Anwendung den Benutzer vor Makros warnt:
  
-   **Vertrauensstellungsleistenwarnung für alle Makros**. Die Anwendung zeigt die Vertrauensstellungsleiste für alle Makros an, unabhängig davon, ob diese signiert sind oder nicht. Diese Option setzt die Standardkonfiguration in der 2007 Office-Version durch.  
-   **Vertrauensstellungsleistenwarnung nur für digital signierte Makros (nicht signierte Makros werden deaktiviert)**. Die Anwendung zeigt die Vertrauensstellensleiste für digital signierte Makros an und lässt den Benutzer entscheiden, ob er diese aktiviert oder deaktiviert. Alle nicht signierten Makros werden deaktiviert, und Benutzer werden nicht benachrichtigt.  
-   **Keine Warnungen für alle Makros, aber alle Makros deaktivieren**. Die Anwendung deaktiviert alle Makros, unabhängig davon, ob diese signiert sind oder nicht, und gibt keine Benachrichtigung an den Benutzer aus.  
-   **Keine Sicherheitsüberprüfung für Makros (nicht empfohlen)**. Alle Makros werden aktiviert, unabhängig davon, ob sie signiert sind oder nicht. Diese Option kann die Sicherheit deutlich verringern, weil sie die Ausführung von gefährlichem Code ermöglicht, ohne dass dieser erkannt wird.
  
**Tabelle 1.234: Einstellungen für VBA-Makrowarnung**

 
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
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit\Vertrauensstellungscenter
Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Sicherheit\Vertrauensstellungscenter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">access12.adm, excel12.adm, ppt12.adm, word12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Vertrauensstellungsleistenwarnung für alle Makros)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Vertrauensstellungsleistenwarnung nur für digital signierte Makros (nicht signierte Makros werden deaktiviert))</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">Access: CCE-427Excel: CCE-649PowerPoint: CCE-567 Word: CCE-659</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Vertrauensstellungsleistenwarnung nur für digital signierte Makros (nicht signierte Makros werden deaktiviert)**. Diese Konfiguration führt dazu, dass Dokumente und Vorlagen, die nicht signierte Makros enthalten, alle von diesen Makros bereitgestellte Funktionalität verlieren. Um diesen Funktionalitätsverlust zu verhindern, können Benutzer die Makros an einem vertrauenswürdigen Speicherort installieren, es sei denn, die Option **Alle vertrauenswürdigen Speicherorte deaktivieren** ist auf **Aktiviert** gesetzt. Wenn Ihr Unternehmen keine offiziell genehmigten Makros verwendet, überlegen Sie, ob Sie für eine höhere Sicherheit die Option **Keine Warnungen für alle Makros, aber alle Makros deaktivieren** auswählen sollten.
  
![](images/Dd443663.important(de-de,TechNet.10).gif)**Wichtig:**
  
Wenn **Vertrauensstellungsleistenwarnung nur für digital signierte Makros (nicht signierte Makros werden deaktiviert)** aktiviert ist, können Benutzer nicht signierte Access 2007-Datenbanken nicht öffnen.
  
Beachten Sie auch, dass die 2007 Office-Version Zertifikate für vertrauenswürdige Herausgeber in der Aufstellung der vertrauenswürdigen Herausgeber von Internet Explorer speichert. In früheren Versionen von Office wurden Informationen zu Zertifikaten für vertrauenswürdige Herausgeber (insbesondere den Zertifikatfingerabdruck) in einer speziellen Office-Aufstellung der vertrauenswürdigen Herausgeber gespeichert. Die 2007 Office-Version liest weiterhin Informationen zu Zertifikaten für vertrauenswürdige Herausgeber aus der Office-Aufstellung der vertrauenswürdigen Herausgeber, schreibt aber keine Informationen in diese Aufstellung.
  
Wenn Sie also eine Liste vertrauenswürdiger Herausgeber in einer früheren Version von Office erstellt und ein Upgrade auf die 2007 Office-Version durchgeführt haben, wird Ihre Liste vertrauenswürdiger Herausgeber weiterhin erkannt. Aber alle Zertifikate vertrauenswürdiger Herausgeber, die Sie der Liste hinzufügen, werden in der Aufstellung vertrauenswürdiger Herausgeber in Internet Explorer gespeichert.
  
Weitere Informationen über vertrauenswürdige Herausgeber finden Sie in der folgenden Dokumentation:
  
-   Microsoft Office Online-Artikel „[Hinzufügen, Entfernen oder Anzeigen eines vertrauenswürdigen Herausgebers](http://office.microsoft.com/en-us/help/ha100341381033.aspx)
  
-   Knowledge Base-Artikel „[So wird's gemacht: Verwendung von Richtlinien für Softwareeinschränkung in Windows Server 2003](http://support.microsoft.com/kb/324036)
  
-   Microsoft TechNet-Artikel „[Schutz vor nicht autorisierter Software mit Richtlinien für Softwareeinschränkung](http://go.microsoft.com/fwlink/?linkid=98671)
  
-   Kapitel 6 „[Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/technet/security/prodtech/windowsxp/secwinxp/default.mspx) im Windows XP-Sicherheitshandbuch im Microsoft TechNet.
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))  
-   Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6  
-   [Sicherheitseinstellungen für Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenmaßnahmen:%20sicherheitseinstellungen%20in%202007%20office%20system)
  
|                                  |                                                                                                                                                                                                                                                                                                                                                                              |  
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [Zum Seitenanfanq](#mainsection) | [![](images/Dd443663.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))7 von 8[![](images/Dd443663.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10)) |
