---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Sicherheitseinstellungen für Computerrichtlinien'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Sicherheitseinstellungen für Computerrichtlinien'
ms:assetid: 'e5d2501b-a96b-4c69-b912-59ad22c30503'
ms:contentKeyID: 20075612
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443669(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen
=========================================================================

### Sicherheitseinstellungen für Computerrichtlinien

Veröffentlicht: 11. Nov 2007

Die Computerrichtlinieneinstellungen im folgenden Abschnitt sind nach Namen aufgeführt.

##### Auf dieser Seite

[Informationen zu Computerrichtlinieneinstellungen](#ecd)

Informationen zu Computerrichtlinieneinstellungen
-------------------------------------------------

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle verfügbar, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung, die empfohlene Konfiguration für EC- und SSLF-Umgebungen sowie zugehörige CCE-Bezeichner (Common Configuration Enumeration) aufführt.

#### Binden an Objekt

Betrifft: **2007 Office System**

Diese Einstellung bestimmt, ob Microsoft® Internet Explorer® beim Öffnen von URLs, die von einer 2007 Office-Anwendung übergeben werden, typische Sicherheitsüberprüfungen von Microsoft ActiveX®-Steuerelementen vornimmt.

![](images/Dd443669.important(de-de,TechNet.10).gif) Wichtig:

Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103493).

##### Sicherheitsrisiko

Internet Explorer führt eine Reihe von Sicherheitsüberprüfungen durch, bevor ein ActiveX-Steuerelement initialisiert wird. Ein Steuerelement wird nicht initialisiert, wenn das Kill Bit für das Steuerelement in der Registrierung eingestellt ist oder wenn die Sicherheitseinstellungen für die Zone, in der sich das Steuerelement befindet, eine Initialisierung nicht zulassen.

Diese Funktionalität kann separat für Instanzen von Internet Explorer gesteuert werden, die durch 2007 Office-Anwendungen gestartet werden (z. B., wenn ein Benutzer auf einen Link in einem Office-Dokument klickt oder eine Menüoption auswählt, durch die eine Webseite geladen wird). Ein Sicherheitsrisiko könnte auftreten, wenn ein Laden potenziell gefährlicher Steuerelemente zugelassen wird.

##### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, können Kontrollkästchen für eine oder mehrere 2007 Office-Anwendungen ausgewählt werden, die in einer Liste aufgeführt sind. Internet Explorer wendet typische Sicherheitsüberprüfungen für alle in Webseiten eingebetteten ActiveX-Objekte an, die von den ausgewählten Anwendungen geöffnet werden.

**Tabelle 2.1. Binden an Objekt**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen\IE-Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1669, CCE-1691, CCE-1338, CCE-1717, CCE-1488, CCE-1638, CCE-1647, CCE-1294</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zu den spezifischen Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Ein Aktivieren dieser Einstellung kann Beeinträchtigungen für Benutzer verursachen, die Webseiten mit potenziell gefährlichen ActiveX-Steuerelementen von 2007 Office-Anwendungen aus öffnen. Da jedoch betroffene Steuerelemente normalerweise standardmäßig blockiert werden, wenn Webseiten mit Internet Explorer geöffnet werden, dürften für die meisten Benutzer keine größeren Nutzbarkeitsprobleme auftreten.
  
### Popups blockieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Internet Explorer beim Öffnen von URLs, die von einer 2007 Office-Anwendung übergeben werden, Popupfenster blockiert.
  
![](images/Dd443669.important(de-de,TechNet.10).gif) Wichtig:
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103494).
  
#### Sicherheitsrisiko
  
Die Popupblocker-Funktion in Internet Explorer kann zum Blockieren der Anzeige unerwünschter Popup- und Popunderfenster verwendet werden. Diese Funktionalität kann separat für Instanzen von Internet Explorer gesteuert werden, die durch 2007 Office-Anwendungen gestartet werden (z. B., wenn ein Benutzer auf einen Link in einem Office-Dokument klickt oder eine Menüoption auswählt, durch die eine Webseite geladen wird). Wenn der Popupblocker deaktiviert ist, könnten störende und potenziell gefährliche Popupfenster geladen werden und zu einem Sicherheitsrisiko führen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Kontrollkästchen für eine oder mehrere 2007 Office-Anwendungen ausgewählt werden, die in einer Liste aufgeführt sind. Internet Explorer wendet diese Popupblocker-Funktion auf alle Webseiten an, die von den ausgewählten Anwendungen geöffnet werden.
  
**Tabelle 2.2. Popups blockieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen\IE-Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1152, CCE-1566, CCE-1077, CCE-1606, CCE-1738, CCE-1262, CCE-1663, CCE-1544</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zu den spezifischen Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Das Aktivieren dieser Einstellung kann Beeinträchtigungen für Benutzer verursachen, die Webseiten mit Popupfenstern von 2007 Office-Anwendungen aus öffnen. Popupfenster können von Vorteil sein und sind manchmal sogar erforderlich, damit bestimmte Webseiten funktionieren. Um diese Popupfenster anzuzeigen, muss der Benutzer die betroffenen Webseiten der Liste **Zugelassene Sites** im Dialogfeld **Popupblockereinstellungen** von Internet Explorer hinzufügen.
  
### Paketreparatur deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer die Möglichkeit haben, beschädigte Office Open XMP-Dokumente zu reparieren.
  
#### Sicherheitsrisiko
  
Wenn eine 2007 Office-Anwendung entdeckt, dass ein Office Open XML-Dokument beschädigt ist, hat der Benutzer standardmäßig die Möglichkeit, das beschädigte Dokument zu reparieren.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, versuchen 2007 Office-Anwendungen nicht, beschädigte Office Open XML-Dokumente zu reparieren. Diese Einstellung kann zum Schutz gegen theoretische Zero-Day-Angriffe eingesetzt werden, die auf die Paketreparaturfunktion abzielen und möglicherweise bedeuten können, dass ein Angreifer Office Open XML-Paketdateien umfunktioniert.
  
**Tabelle 2.3. Paketreparatur deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen</td>
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
<td style="border:1px solid black;">CCE-933</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Konfiguration lautet **Aktiviert**, was bedeutet, dass 2007 Office-Benutzer nicht in der Lage sind, beschädigte Office Open XML-Paketdateien selbst zu reparieren. Wenn Benutzer versuchen, beschädigte Dateien zu öffnen, ist hierzu Administratorhilfe erforderlich.
  
### Benutzername und Kennwort deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Internet Explorer URLs mit Benutzerinformationen öffnet, die von einer 2007 Office-Anwendung übergeben werden.
  
![](images/Dd443669.important(de-de,TechNet.10).gif) Wichtig:
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103499).
  
#### Sicherheitsrisiko
  
Der Uniform Resource Locator (URL)-Standard ermöglicht, dass Benutzerauthentifizierungen in Form von http://benutzername:kennwort@beispiel.com in URLs aufgenommen werden können. Ein böswilliger Benutzer könnte diese URL-Syntax zum Erstellen eines Hyperlinks verwenden, der scheinbar eine legitime Website öffnet, tatsächlich aber eine betrügerische (gefälschte) Website öffnet. Zum Beispiel scheint die URL http://www.wingtiptoys.com@beispiel.com die Website http://www.wingtiptoys.com zu öffnen. Tatsächlich aber öffnet sie http://beispiel.com. Internet Explorer blockiert normalerweise alle URLs mit dieser Syntax, um Benutzer vor solchen Angriffen zu schützen.
  
Diese Funktionalität kann separat für Instanzen von Internet Explorer gesteuert werden, die durch 2007 Office-Anwendungen gestartet werden (z. B., wenn ein Benutzer auf einen Link in einem Office-Dokument klickt oder eine Menüoption auswählt, durch die eine Webseite geladen wird). Wenn Benutzernamen und Kennwörter in URLs zugelassen werden, könnten Benutzer auf gefährliche Webseiten geleitet werden, die möglicherweise ein Sicherheitsrisiko darstellen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Kontrollkästchen für eine oder mehrere 2007 Office-Anwendungen ausgewählt werden, die in einer Liste aufgeführt sind. Internet Explorer blockiert alle URLs mit Benutzerauthentifizierungsinformationen, die von den ausgewählten Anwendungen geöffnet werden.
  
**Tabelle 2.4. Benutzername und Kennwort deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen\IE-Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1563, CCE-1215, CCE-1484, CCE-1629, CCE-1762, CCE-1660, CCE-1057, CCE-1285</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zu den spezifischen Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Das Aktivieren dieser Einstellung kann Beeinträchtigungen für Benutzer verursachen, die URLs mit Benutzerauthentifizierungsinformationen von einer 2007 Office-Anwendung aus öffnen. Da solche URLs standardmäßig blockiert sind, wenn Internet Explorer Webseiten auf normale Weise öffnet, dürften für die meisten Benutzer jedoch keine größeren Nutzbarkeitsprobleme auftreten.
  
### VBA für Office-Anwendungen deaktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Anwendungen außer Microsoft Office Access™ 2007 Microsoft Visual Basic® for Applications (VBA) verwenden können.
  
#### Sicherheitsrisiko
  
Standardmäßig können die meisten Office-Anwendungen, einschließlich Microsoft Office Excel® 2007, Outlook® 2007, PowerPoint® 2007 und Word 2007 Visual Basic for Applications (VBA)-Code ausführen, der den Anwendungsbetrieb anpasst und automatisiert. VBA könnte ebenfalls von unerfahrenen oder böswilligen Entwicklern zum Erstellen von schädlichem Code verwendet werden, der die Computer von Benutzern beschädigen bzw. die Vertraulichkeit, Integrität oder Verfügbarkeit von Daten beeinträchtigen kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können die 2007-Versionen von Excel, Outlook, PowerPoint, Publisher, SharePoint® Designer und Word keinen VBA-Code ausführen. Bei Aktivieren dieser Einstellung werden weder VBA-Code noch VBA-Dateien auf dem Computer des Benutzers installiert bzw. davon entfernt.
  
![](images/Dd443669.note(de-de,TechNet.10).gif) **Hinweis:**
  
Diese Einstellung hat keine Auswirkungen auf Access 2007.
  
**Tabelle 2.5. VBA für Office-Anwendungen deaktivieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen</td>
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
  
Wenn diese Einstellung **aktiviert** ist, funktioniert VBA-Code in 2007 Office-Anwendungen nicht (mit Ausnahme von Access). Falls in Ihrem Unternehmen unbedingt Dokumente mit VBA-Code verwendet werden müssen, können Sie diese Einstellung möglicherweise nicht aktivieren.
  
### InfoPath APTCA Assembly-Positivliste
  
Betrifft: **InfoPath**
  
Diese Einstellung ermöglicht es Administratoren, eine Liste von Assemblys im globalen Assemblycache (Global Assembly Cache, GAC) zu konfigurieren, die von Microsoft Office InfoPath® 2007 aufgerufen werden können.
  
#### Sicherheitsrisiko
  
Der GAC enthält freigegebene Assemblys, die von anderen Anwendungen aufgerufen werden können. Wenn eine Anwendung voll vertrauenswürdig ist, kann sie auf jede Assembly im GAC zugreifen. Wenn eine Anwendung teilweise vertrauenswürdig ist, kann sie lediglich auf Assemblys im GAC zugreifen, für die das Attribut „AllowPartiallyTrustedCallersAttribute“ (APTCA) festgelegt ist.
  
Ein böswilliger Benutzer könnte versuchen, ein InfoPath 2007-Formular zu erstellen, das auf eine Assembly mit dem APTCA-Attribut zugreift, aber das nicht für die Verwendung mit InfoPath-Formularen bestimmt ist.
  
Zum Schutz gegen einen solchen Angriff kann die Geschäftslogik eines InfoPath-Formulars Assemblys im Global Assembly Cache (GAC) nur aufrufen, wenn zwei Bedingungen erfüllt sind:
  
-   Für die Assembly ist das Attribut „Allow Partially Trust Callers Attribute“ (APTCA) festgelegt.
  
-   Die Assembly ist in der Liste zugelassener Elemente (Positivliste) für die APTCA-Assembly aufgeführt. Standardmäßig ist diese Liste leer.
  
    ![](images/Dd443669.note(de-de,TechNet.10).gif) **Hinweis:**
  
    Die Standardfunktionalität kann durch Deaktivieren der Gruppenrichtlinieneinstellung „InfoPath APTCA Assembly-Positivlistenerzwingung“ geändert werden, der nächsten in diesem Handbuch beschriebenen Einstellung. Microsoft empfiehlt jedoch eindringlich, dass die Positivlistenerzwingung unbedingt aktiviert werden sollte.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren der APTCA-Assembly-Positivliste Einträge hinzufügen. Um der Positivliste eine neue Assembly hinzuzufügen, fügen Sie einen neuen Zeichenfolgenwert hinzu, der dem APTCA-Schlüssel entspricht. Das Feld **Wertname** sollte dem öffentlichen Schlüsseltoken für die Assembly entsprechen, und das Feld **Wertdaten** sollte „1“ entsprechen, damit InfoPath 2007 das Laden der Assembly erlaubt. Wenn das Feld **Wertdaten** nicht „1“ ist, kann die Assembly nicht geladen werden.
  
**Tabelle 2.6. InfoPath APTCA Assembly-Positivliste**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007 (Computer)\Sicherheit</td>
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
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1169</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Durch diese Einstellung ändert sich die Standardkonfiguration nicht. Sie dürfte also keine Auswirkungen auf die Nutzbarkeit haben. Wenn ein InfoPath 2007-Formular Assemblys im GAC verwenden muss, müssen Sie sicherstellen, dass für die Assemblys das ACPTA-Attribut eingestellt ist und dass sie der Positivliste hinzugefügt wurden.
  
### InfoPath APTCA Assembly-Positivlistenerzwingung
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob InfoPath 2007 Assemblys aufrufen kann, die nicht in der Liste zulässiger Elemente (Positivliste) für die APTCA-Assembly enthalten sind.
  
#### Sicherheitsrisiko
  
Standardmäßig kann die Geschäftslogik eines InfoPath 2007-Formulars nur Assemblys des globalen Assemblycache (GAC) aufrufen, die in der APTCA-Assembly-Positivliste enthalten sind. Wenn diese Konfiguration geändert wird, können Formulare jede Assembly im GAC aufrufen, für die das Attribut APTCA (Allow Partially Trust Callers Attribute) festgelegt ist. Diese Konfiguration könnte es böswilligen Entwicklern ermöglichen, auf Assemblys im GAC zuzugreifen, die nicht für die Verwendung von InfoPath-Formularen bestimmt sind.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können InfoPath 2007-Formulare keine Assemblys aufrufen, die nicht in der APTCA-Assembly-Positivliste enthalten sind, und sie überschreibt alle Konfigurationsänderungen auf dem lokalen Computer.
  
**Tabelle 2.7. InfoPath APTCA Assembly-Positivlistenerzwingung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007 (Computer)\Sicherheit</td>
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
<td style="border:1px solid black;">CCE-1739</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung setzt die Standardkonfiguration durch und dürfte daher keine Auswirkungen auf die Nutzbarkeit haben. Wenn ein InfoPath 2007-Formular Assemblys im GAC verwenden muss, müssen Sie sicherstellen, dass für die Assemblys das ACPTA-Attribut festgelegt ist und dass sie in der Liste zulässiger Elemente (Positivliste) aufgeführt sind.
  
### URL navigieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Internet Explorer versucht, fehlerhafte URLs zu laden, die von 2007 Office-Anwendungen übergeben werden.
  
![](images/Dd443669.important(de-de,TechNet.10).gif) Wichtig:
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103502).
  
#### Sicherheitsrisiko
  
Zum Schutz des Benutzers vor Angriffen versucht Internet Explorer in der Regel nicht, fehlerhafte URLs zu laden. Diese Funktionalität kann separat für Instanzen von Internet Explorer gesteuert werden, die durch 2007 Office-Anwendungen gestartet werden (z. B., wenn ein Benutzer auf einen Link in einem Office-Dokument klickt oder eine Menüoption auswählt, durch die eine Webseite geladen wird). Wenn Internet Explorer versucht, eine fehlerhafte URL zu laden, könnte in bestimmten Fällen ein Sicherheitsrisiko auftreten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Kontrollkästchen für eine oder mehrere 2007 Office-Anwendungen ausgewählt werden, die in einer Liste aufgeführt sind. Internet Explorer blockiert alle fehlerhaften URLs, die von den ausgewählten Anwendungen übergeben werden.
  
**Tabelle 2.8. URL navigieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen\IE-Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1034, CCE-1435, CCE-1708, CCE-808, CCE-1650, CCE-1223, CCE-1764, CCE-1769</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zu den spezifischen Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Durch Aktivieren dieser Einstellung werden legitime URLs nicht blockiert. Sie dürfte daher keine Nutzbarkeitsprobleme für Benutzer von 2007 Office verursachen.
  
### Gespeichert von URL
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Internet Explorer die von 2007 Office-Anwendungen übergegeben URLs auf „Mark of the Web“ (MOTW)-Kommentare evaluiert.
  
![](images/Dd443669.important(de-de,TechNet.10).gif) Wichtig:
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103503).
  
#### Sicherheitsrisiko
  
Wenn Internet Explorer eine Webseite aus einer UNC-Freigabe lädt, die einen „Mark of the Web“ (MOTW)-Kommentar enthält, dass die Seite von einer Site im Internet gespeichert wurde, führt Internet Explorer die Seite in der Regel in der Internetsicherheitszone aus und nicht in der weniger stark eingeschränkten lokalen Intranetsicherheitszone. Diese Funktionalität kann separat für Instanzen von Internet Explorer gesteuert werden, die durch 2007 Office-Anwendungen gestartet werden (z. B., wenn ein Benutzer auf einen Link in einem Office-Dokument klickt oder eine Menüoption auswählt, durch die eine Webseite geladen wird). Wenn Internet Explorer die Seite nicht auf MOTW evaluiert, könnte es zur Ausführung von potenziell schädlichem Code kommen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Kontrollkästchen für eine oder mehrere 2007 Office-Anwendungen ausgewählt werden, die in einer Liste aufgeführt sind. Internet Explorer evaluiert alle URLs auf MOTW-Kommentare, die von den ausgewählten Anwendungen übergeben werden.
  
**Tabelle 2.9. Gespeichert von URL**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Computerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System (Computer)\Sicherheitseinstellungen\IE-Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">office12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (excel.exe, powerpnt.exe, pptview.exe, winword.exe, outlook.exe, spDesign.exe, msaccess.exe)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-IDs</strong></td>
<td style="border:1px solid black;">CCE-1193, CCE-1352, CCE-928, CCE-1576, CCE-1100, CCE-1232, CCE-1774, CCE-906</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zu den spezifischen Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Das Aktivieren dieser Einstellung kann zur Folge haben, dass manche in UNC-Freigaben gespeicherte Webseiten beim Öffnen von 2007 Office-Anwendungen aus in einer eingeschränkteren Sicherheitszone ausgeführt werden als dies der Fall wäre, wenn diese Einstellung deaktiviert bzw. nicht konfiguriert wäre. Bei einer Seite mit einem MOTW-Kommentar, der angibt, dass sie von einer Internetsite gespeichert wurde, kann jedoch angenommen werden, dass sie ursprünglich für die Ausführung in der Internetzone entworfen wurde. Daher dürften für die meisten Benutzer keine größeren Nutzbarkeitsprobleme auftreten.
  
![](images/Dd443669.note(de-de,TechNet.10).gif) **Hinweis:**
  
Weitere Informationen zur Verwendung von „Mark of the Web“ zum Steuern der Sicherheitszone, in der Internet Explorer Webseiten ausführt, finden Sie im Artikel [Mark of the Web](http://msdn2.microsoft.com/en-us/library/ms537628.aspx) in der MSDN Library (möglicherweise in englischer Sprache).
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))  
-   Sicherheitseinstellungen für Computerrichtlinien
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenmaßnahmen)
  
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><div>
<a href="#mainsection"></a><a href="#mainsection">Zum Seitenanfanq</a>
</div></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10)"><img src="https://msdn.microsoft.com/de-de/Dd443674.pageLeft(de-de,TechNet.10).gif" /></a> 8 von 8 </td>
</tr>
</tbody>
</table>
