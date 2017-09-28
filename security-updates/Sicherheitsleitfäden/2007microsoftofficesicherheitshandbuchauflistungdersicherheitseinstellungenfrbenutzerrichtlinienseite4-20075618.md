---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4'
ms:assetid: '2324b4a2-1709-464a-ba66-7413a87d1188'
ms:contentKeyID: 20075618
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443675(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch Bedrohungen und Gegenmaßnahmen
========================================================================

Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 4
----------------------------------------------------------------------

Verffentlicht: 11. Nov 2007

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgefhrt.

##### Auf dieser Seite

[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)

Informationen zu Benutzerrichtlinieneinstellungen
-------------------------------------------------

Fr jede Einstellung werden neben einer Beschreibung auch Informationen ber die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwgungen bereitgestellt. Darber hinaus ist fr jede Einstellung eine Tabelle enthalten, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung sowie die empfohlene Konfiguration fr EC- und SSLF-Umgebungen auffhrt.

### EKU-Filterung

Betrifft: **2007 Office System**

Mit dieser Einstellung knnen Administratoren Werte fr die erweiterte Schlsselverwendung (EKU) angeben, die beim Filtern einer Liste digitaler Zertifikate fr die Signierung von Excel 2007-, PowerPoint 2007- und Word 2007-Dokumenten verwendet werden sollen.

#### Sicherheitsrisiko

Eine EKU-Erweiterung fr ein digitales Zertifikat ist eine Sammlung von mindestens einem Wert, die darauf hinweist, wie ein Zertifikat verwendet werden soll. Zu Beispielen fr EKU-Werte gehren die Smartcard-Anmeldung und die Clientauthentifizierung. Mithilfe der EKU-Filterung knnen Sie die Liste installierter Zertifikate filtern, die fr das digitale Signieren von Dokumenten verwendet werden knnen. Die gefilterte Liste wird angezeigt, wenn Benutzer versuchen, ein Zertifikat fr die digitale Signatur eines Dokuments auszuwhlen.

Standardmig ist die EKU-Filterung nicht aktiviert. Wenn die EKU-Filterung nicht verwendet wird, knnen Benutzer versehentlich oder mit bswilliger Absicht die falsche Art von Zertifikat fr das digitale Signieren eines Dokuments oder das berprfen einer Signatur verwenden. Dadurch wird mglicherweise die Datensicherheit gefhrdet oder eine berprfung der Signatur eines Dokuments unmglich gemacht.

#### Gegenmanahme

Wenn diese Einstellung **aktiviert** ist, knnen Administratoren eine Liste von Objektbezeichnern (OIDs) angeben, die akzeptable EKUs fr Zertifikate darstellen, die in Verbindung mit signierten Dokumenten verwendet werden. Fr ein Zertifikat mit dem verschlsselnden Dateisystembezeichner (1.3.6.1.4.1.311.10.3.4) lautet der Objektbezeichner 1.3.6.1.4.1.311.10.3.4. Die Liste angemessener OIDs ist je nach den bestimmten, im Unternehmen verwendeten Zertifikaten unterschiedlich.

Eine Liste von Objektbezeichnern, die der Microsoft-Kryptografie zugeordnet sind, finden Sie im Knowledge Base-Artikel 287547 [ber zur Microsoft-Kryptografie gehrige Objektbezeichner (maschinell bersetzter Artikel)](http://support.microsoft.com/kb/287547).

**Tabelle 1.146: EKU-Filterung**

 
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
<td style="border:1px solid black;">CCE-1167</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, sind 2007 Office-Benutzer eventuell eingeschrnkter darin, welche Zertifikate sie fr das digitale Signieren von Dokumenten verwenden knnen. Sie mssen sicherstellen, dass das EKU-Feld fr die Zertifikate ausgefllt wird, die Sie fr das digitale Signieren verwenden mchten.
  
### Signal bertragende Elemente der Benutzeroberflche fr E-Mail-Formulare
  
Betrifft: **InfoPath**
  
Diese Einstellung steuert, ob Benutzer gewarnt werden, wenn ein InfoPath-Formular eine Bedrohung durch Webbeacons enthlt.
  
#### Sicherheitsrisiko
  
Bswillige Benutzer knnen per E-Mail InfoPath-Formulare mit eingebetteten Webbeacons versenden, ber die verfolgt werden kann, wann Empfnger das Formular ffnen. Damit erhlt der Absender eine Besttigung, dass die E-Mail-Adressen der Empfnger gltig sind. Darber hinaus knnen zustzliche von dem Formular gesammelte oder von Benutzern eingegebene Informationen an externe Server bermittelt werden, sodass Benutzer anfllig fr weitere Angriffe werden.
  
Standardmig werden InfoPath 2007-Benutzer nur vor einer Bedrohung durch Webbeacons gewarnt, wenn das Formular aus dem Internet stammt.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen zur Verfgung, ber die sie steuern knnen, wann InfoPath 2007-Benutzer eine Eingabeaufforderung zu Bedrohungen durch Webbeacons erhalten:
  
-   Benutzeroberflche nie anzeigen  
-   Benutzeroberflche immer anzeigen  
-   Benutzeroberflche anzeigen, falls sich XSN in der Internetzone befindet
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn die Einstellung **Deaktiviert** oder **Aktiviert**|**Benutzeroberflche nie anzeigen** ausgewhlt wird, werden Benutzer nicht vor Bedrohungen durch Webbeacons gewarnt. Diese Konfiguration kann die Sicherheit wesentlich beeintrchtigen.
  
**Tabelle 1.147: Signal bertragende Elemente der Benutzeroberflche fr E-Mail-Formulare**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007 System\Verschiedenes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzeroberflche anzeigen, falls sich XSN in der Internetzone befindet)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Benutzeroberflche immer anzeigen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1212</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung fr die EC-Umgebung ndert die Standardkonfiguration nicht und sollte deshalb die Nutzbarkeit nicht beeintrchtigen. Wenn die empfohlene Einstellung fr die SSLF-Umgebung ausgewhlt wird, werden Benutzer vor potenziellen Bedrohungen durch Webbeacons gewarnt, auch wenn diese aus dem lokalen Intranet stammen. Es ist mglich, dass einige interne Formulare vollkommen legitim Signal bertragende Techniken verwenden. In diesem Fall sollten diese Formulare umgestaltet oder Benutzer ber die angezeigte Warnmeldung informiert werden.
  
### Programm zur Verbesserung der Benutzerfreundlichkeit aktivieren
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer am Programm zur Verbesserung der Benutzerfreundlichkeit von Microsoft Office teilnehmen und damit dazu beitragen knnen, Microsoft Office zu verbessern.
  
#### Sicherheitsrisiko
  
Wenn sich Benutzer fr die Teilnahme am Programm zur Verbesserung der Benutzerfreundlichkeit (CEIP, Customer Experience Improvement Program) entscheiden, senden 2007 Office-Anwendungen automatisch Informationen ber die Nutzung der Anwendungen an Microsoft. Diese Informationen werden mit anderen CEIP-Daten kombiniert, um Microsoft bei der Problemlsung und Verbesserung seiner Produkte und der am hufigsten von Kunden verwendeten Funktionen zu untersttzen. Die Funktion sammelt weder Benutzernamen, Adressen noch andere Informationen, mit denen Benutzer identifiziert werden knnen, mit Ausnahme der fr das Versenden der Daten verwendeten IP-Adresse.
  
Standardmig haben Benutzer die Mglichkeit, sich bei der ersten Ausfhrung einer Office-Anwendung fr die Teilnahme am Programm zur Verbesserung der Benutzerfreundlichkeit zu entscheiden. Wenn Ihr Unternehmen Richtlinien fr die Regelung der Verwendung externer Ressourcen wie das Programm zur Verbesserung der Benutzerfreundlichkeit einsetzt, verstoen Benutzer mglicherweise gegen diese Richtlinien, wenn die Teilnahme der Benutzer an dem Programm zugelassen wird.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, knnen 2007 Office-Benutzer nicht am Programm zur Verbesserung der Benutzerfreundlichkeit teilnehmen.
  
**Tabelle 1.148: Programm zur Verbesserung der Benutzerfreundlichkeit aktivieren**

 
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
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-184</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Das Programm zur Verbesserung der Benutzerfreundlichkeit sendet Daten automatisch und ohne Beeintrchtigung der Anwendungsnutzung an Microsoft, sodass die Option **Deaktiviert** keine Nutzbarkeitsprobleme fr 2007 Office-Benutzer verursacht.
  
### Hyperlinks in E-Mail-Nachrichten aktivieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Hyperlinks in mutmalichen Phishing-E-Mails in Outlook 2007 aktiviert sind.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Kurzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103500).
  
#### Sicherheitsrisiko
  
Der Junk-E-Mail-Filter von Outlook 2007 wertet jede eingehende Nachricht auf mgliche Spam- oder Phishinginhalte aus. Die Erkennung verdchtiger Nachrichten ist immer aktiviert.
  
Standardmig handhabt Outlook verdchtige Nachrichten auf zweierlei Weise:
  
-   Wenn der Junk-E-Mail-Filter eine Nachricht nicht als Spam, aber als Phishingversuch betrachtet, wird die Nachricht im Posteingang belassen, aber alle Links in der Nachricht werden deaktiviert, und der Benutzer kann die Funktionen Antworten und Allen antworten nicht verwenden. Darber hinaus werden alle Anlagen der verdchtigen Nachrichten blockiert.  
-   Wenn der Junk-E-Mail-Filter die Nachricht sowohl als Spam als auch Phishingversuch betrachtet, wird die Nachricht automatisch in den Junk-E-Mail-Ordner bermittelt. Jede in den Junk-E-Mail-Ordner bermittelte Nachricht wird in das Nur-Text-Format konvertiert, und alle Links werden deaktiviert. Darber hinaus werden die Funktionen Antworten und Allen antworten deaktiviert und alle Anlagen der Nachricht blockiert. Die Infoleiste benachrichtigt Benutzer ber diese Funktionalittsnderung. Wenn Benutzer sicher sind, dass eine Nachricht legitim ist, knnen sie auf die Infoleiste klicken und die Links in der Nachricht aktivieren.
  
Benutzer knnen die Handhabung von Phishingnachrichten in Outlook im Dialogfeld **Junk-E-Mail-Optionen** ndern, indem sie das Kontrollkstchen **Hyperlinks und sonstige Funktionen in Phishingnachrichten deaktivieren (empfohlen)** deaktivieren. Wenn dieses Kontrollkstchen deaktiviert ist, deaktiviert Outlook Links in mutmalichen Phishingnachrichten nur, wenn diese als Junk-E-Mail klassifiziert werden. Benutzer knnten auf diese Weise vertrauliche Informationen an schdliche Websites weitergeben.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, deaktiviert Outlook 2007 alle Links in mutmalichen Phishingnachrichten, selbst wenn diese nicht als Junk-E-Mail klassifiziert sind, und Benutzer knnen diese Einstellung nicht ndern.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn die Einstellung **aktiviert** ist, fhrt Outlook keine Deaktivierung von Links in mutmalichen Phishingnachrichten durch, die nicht auch als Junk-E-Mail klassifiziert sind. Diese Konfiguration kann die Sicherheit wesentlich verringern.
  
**Tabelle 1.149: Hyperlinks in E-Mail-Nachrichten aktivieren**

 
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
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1052</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in Outlook 2007 durch und sollte daher fr die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### RPC-Verschlsselung aktivieren
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 fr die Kommunikation mit Microsoft Exchange-Servern die RPC-Verschlsselung verwendet.
  
#### Sicherheitsrisiko
  
Standardmig ist der Kommunikationskanal fr Remoteprozeduraufrufe (RPCs) zwischen einem Outlook 2007-Clientcomputer und einem Exchange-Server nicht verschlsselt. Wenn eine bswillige Person den Netzwerkdatenverkehr zwischen Outlook und dem Server mithrt, kann sie mglicherweise auch auf vertrauliche Informationen zugreifen.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, verwendet Outlook 2007 fr die Kommunikation mit Microsoft Exchange-Servern die RPC-Verschlsselung.
  
![](images/Dd443675.note(de-de,TechNet.10).gif) **Hinweis:**
  
Die RPC-Verschlsselung verschlsselt nur Daten, die vom Outlook-Clientcomputer zum Exchange-Server transportiert werden. Sie bietet keine Verschlsselung fr die Nachrichten selbst, whrend diese ber das Internet bertragen werden.
  
**Tabelle 1.150: RPC-Verschlsselung aktivieren**

 
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
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1082</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung sollte keine wesentlichen Auswirkungen fr Benutzer haben. Allerdings ist immer ein Kompromiss zwischen sicherer Kommunikation und Leistung erforderlich, deshalb sollten Sie die Leistungsauswirkungen einer Verschlsselung jeder Verbindung vom Outlook 2007-Clientcomputer zum Exchange-Server beurteilen.
  
### Alle E-Mail-Nachrichten verschlsseln
  
Betrifft: **Outlook**
  
Mit dieser Einstellung knnen Administratoren die Verschlsselung aller von Outlook 2007 versendeter E-Mail-Nachrichten erfordern.
  
#### Sicherheitsrisiko
  
Die meisten E-Mail-Nachrichten werden in Klartext versendet, sodass sie gefhrdet sind, wenn sie abgefangen werden. Wenn eine strkere Sicherheit erforderlich ist, knnen Benutzer Nachrichten mit digitalen Zertifikaten verschlsseln, sodass sie nur von den vorgesehenen Empfngern gelesen werden knnen. Unternehmen mit sehr hohen Sicherheitsanforderungen sollten eventuell festlegen, dass Benutzer alle versendeten E-Mail-Nachrichten verschlsseln mssen.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, wird die Schaltflche **Verschlsseln** bei allen ausgehenden E-Mail-Nachrichten, Besprechungsanfragen und anderen Outlook 2007-Elementen automatisch aktiviert. Benutzer mssen ein passendes Zertifikat auswhlen, um die Nachricht fr den vorgesehenen Empfnger zu verschlsseln.
  
**Tabelle 1.149: Alle E-Mail-Nachrichten verschlsseln**

 
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
<td style="border:1px solid black;">CCE-1181</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung fr EC- und SSLF-Konfigurationen ist **Nicht konfiguriert**. Obwohl die Verschlsselung von E-Mail-Nachrichten einen effektiven Schutz bietet, kann die Aktivierung dieser Einstellung auch fr sehr sicherheitsbewusste Unternehmen unpraktisch sein, weil sie verhindert, dass Benutzer E-Mail-Nachrichten an Empfnger senden knnen, fr die sie keine gltigen Zertifikate haben. Wenn Ihr Unternehmen die Verwendung der E-Mail-Verschlsselung standardisieren, Benutzern aber gleichzeitig ermglichen mchte, unverschlsselte Nachrichten zu versenden, wenn keine Verschlsselung verfgbar ist, empfiehlt Microsoft die Verwendung des Office-Anpassungstools (OAT), um eine standardmige Verschlsselung in neuen 2007 Office-Installationen zu ermglichen. Bei dieser Konfiguration knnen Benutzer bei Bedarf die Verschlsselung fr einzelne Nachrichten deaktivieren, aber gleichzeitig sicherstellen, dass andere Nachrichten verschlsselt werden. Weitere Informationen ber das OAT finden Sie im Artikel zum [Office-Anpassungstool in 2007 Office System](http://technet2.microsoft.com/office/en-us/library/8faae8a0-a12c-4f7b-839c-24a66a531bb51033.mspx?mfr=true) (mglicherweise in englischer Sprache).
  
### Verschlsselungstyp fr kennwortgeschtzte Office 97-2003-Dateien
  
Betrifft: **2007 Office System**
  
Mit dieser Einstellung knnen Administratoren einen Verschlsselungstypen fr kennwortgeschtzte Office 97-2003-Dateien festlegen.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Krzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103501).
  
#### Sicherheitsrisiko
  
Wenn unverschlsselte Dateien abgefangen werden, sind vertrauliche Daten in den Dateien gefhrdet. Um die Vertraulichkeit von Informationen zu schtzen, knnen Dateien aus Microsoft Office-Anwendungen verschlsselt und durch ein Kennwort geschtzt werden. Nur Benutzer, die das korrekte Kennwort kennen, knnen diese Dateien entschlsseln.
  
Standardmig verwenden Excel 2007, PowerPoint 2007 und Word 2007 die Office 97/2000-kompatible Verschlsselung, eine proprietre Verschlsselungsmethode zur Verschlsselung kennwortgeschtzter Office 97-2003-Dateien.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, knnen Administratoren den Verschlsseltypen festlegen, den Office-Anwendungen fr die Verschlsselung von kennwortgeschtzten Dateien in lteren Office 97-2003-Dateiformaten verwenden sollen. Fr den ausgewhlten Verschlsselungstypen muss ein entsprechender Kryptografiedienstanbieter (CSP) auf dem Computer installiert sein, der die Datei verschlsselt. Eine Liste der auf dem lokalen Computer installierten Kryptografiedienstanbieter finden Sie im Registrierungsschlssel **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Cryptography\\Defaults\\Provider\\**.
  
Geben Sie den zu verwendenden Verschlsselungstypen an, indem Sie ihn in der folgenden Form in das bereitgestellte Textfeld eingeben:
  
*&lt;Verschlsselungsanbieter&gt;,&lt;Verschlsselungsalgorithmus&gt;,&lt;Lnge des Verschlsselungsschlssels&gt;*
  
Zum Beispiel, Microsoft Enhanced Cryptographic Provider v1.0,RC4,128.
  
**Tabelle 1.152: Verschlsselungstyp fr kennwortgeschtzte Office 97-2003-Dateien**

 
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
<td style="border:1px solid black;">Aktiviert (Microsoft Enhanced RSA und AES Cryptographic Provider,AES 256,256)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1561</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Bercksichtigen Sie bei der Auswahl einer zu erzwingenden Verschlsselungsmethode die Anforderungen Ihres Unternehmens und Ihrer Benutzer. Wenn Sie fr eine Regierungsbehrde, als Vertragsnehmer einer Regierungsbehrde oder auf sonstige Weise mit hoch vertraulichen Daten arbeiten, mssen Sie mglicherweise eine Methode auswhlen, die den Richtlinien fr die Verarbeitung solcher Daten entspricht. Denken Sie daran, dass Sie sich sicherstellen mssen, dass der ausgewhlte Kryptografiedienstanbieter auf den Computern aller Benutzer installiert ist, die mit kennwortgeschtzten Office 97-2003-Dateien arbeiten mssen.
  
### Verschlsselungstyp fr kennwortgeschtzte Office Open XML-Dateien
  
Betrifft: **2007 Office System**
  
Mit dieser Einstellung knnen Administratoren einen Verschlsselungstypen fr Office Open XML-Dateien angeben.
  
#### Sicherheitsrisiko
  
Wenn unverschlsselte Dateien abgefangen werden, sind vertrauliche Daten in den Dateien gefhrdet. Um die Vertraulichkeit von Informationen zu schtzen, knnen Dateien aus 2007 Office-Anwendungen verschlsselt und durch ein Kennwort geschtzt werden. Nur Benutzer, die das korrekte Kennwort kennen, knnen diese Dateien entschlsseln.
  
Fr Computer unter Windows Vista ist der Standard-Kryptografiedienstanbieter (CSP) Microsoft Enhanced RSA und AES Cryptographic Provider, AES-128, 128-Bit. Fr Computer unter Windows XP ist der Standard-CSP Microsoft Enhanced RSA und AES Cryptographic Provider (Prototype), AES-128, 128-Bit.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, knnen Administratoren den Verschlsselungstypen festlegen, den Office-Anwendungen zur Verschlsselung von kennwortgeschtzten Dateien in den Office Open XML-Dateiformaten einsetzen, die von Excel 2007, PowerPoint 2007 und Word 2007 verwendet werden. Fr den ausgewhlten Verschlsselungstypen muss ein entsprechender Kryptografiedienstanbieter (CSP) auf dem Computer installiert sein, der die Datei verschlsselt. Eine Liste der auf dem lokalen Computer installierten Kryptografiedienstanbieter finden Sie im Registrierungsschlssel **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Cryptography\\Defaults\\Provider\\**.
  
Geben Sie den zu verwendenden Verschlsselungstypen an, indem Sie ihn in der folgenden Form in das bereitgestellte Textfeld eingeben:
  
*&lt;Verschlsselungsanbieter&gt;,&lt;Verschlsselungsalgorithmus&gt;,&lt;Lnge des Verschlsselungsschlssels&gt;*
  
Zum Beispiel, Microsoft Enhanced Cryptographic Provider v1.0,RC4,128.
  
**Tabelle 1.152: Verschlsselungstyp fr kennwortgeschtzte Office Open XML-Dateien**

 
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
<td style="border:1px solid black;">Aktiviert (Microsoft Enhanced RSA und AES Cryptographic Provider,AES 256,256)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1539</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Bercksichtigen Sie bei der Auswahl einer zu erzwingenden Verschlsselungsmethode die Anforderungen Ihres Unternehmens und Ihrer Benutzer. Wenn Sie fr eine Regierungsbehrde, als Vertragsnehmer einer Regierungsbehrde oder auf sonstige Weise mit hoch vertraulichen Daten arbeiten, mssen Sie mglicherweise eine Methode auswhlen, die den Richtlinien fr die Verarbeitung solcher Daten entspricht. Denken Sie daran, dass Sie sich sicherstellen mssen, dass der ausgewhlte Kryptografiedienstanbieter auf den Computern aller Benutzer installiert ist, die mit kennwortgeschtzten Office Open XML-Dateien arbeiten mssen.
  
### Beschriftung aller mit S/MIME signierter Nachrichten sicherstellen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 Sicherheitskennzeichen fr mit S/MIME signierte Nachrichten erfordert.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Krzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103516).
  
#### Sicherheitsrisiko
  
Die Dateierweiterungen der S/MIME V3 Enhanced Security Services (ESS) fr Sicherheitskennzeichen und signierte Besttigungen knnen fr eine sichere E-Mail-Kommunikation innerhalb des Unternehmens sorgen. Sie knnen die Sicherheit mithilfe dieser Erweiterungen auerdem an Ihre Anforderungen anpassen. Wenn Ihr Unternehmen S/MIME V3-Sicherheitsrichtlinien entwickelt und bereitstellt, um benutzerdefinierte Sicherheitskennzeichen hinzuzufgen, knnen Sie diese Richtlinien mithilfe dieser Einstellung erzwingen, indem Sie festlegen, dass Benutzer vor dem Versenden jeder E-Mail-Nachricht in Outlook 2007 ein Sicherheitskennzeichen anhngen mssen. Zum Beispiel:
  
-   Eine Beschriftung, die eine E-Mail nur zur internen Verwendung kennzeichnet, kann als Sicherheitskennzeichen fr E-Mail-Nachrichten implementiert werden, die nicht auerhalb Ihres Unternehmens versendet oder weitergeleitet werden drfen.  
-   Ein Sicherheitskennzeichen kann auch angeben, dass bestimmte Empfnger die Nachricht nicht weiterleiten oder drucken knnen, wenn die Sicherheitsrichtlinie bei diesen Empfngern ebenfalls installiert ist.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, mssen allen Outlook 2007 S/MIME-Nachrichten vor dem Versenden Beschriftungen angehngt werden. Benutzer knnen Nachrichten Sicherheitskennzeichen im Dialogfeld **Nachrichtenoptionen** anhngen, indem sie auf **Sicherheitseinstellungen** klicken, sich vergewissern, dass das Kontrollkstchen **Diese Nachricht digital signieren** aktiviert ist, und dann unter **Sicherheitskennzeichen** eine Beschriftung auswhlen.
  
**Tabelle 1.154: Beschriftung aller mit S/MIME signierter Nachrichten sicherstellen**

 
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
<td style="border:1px solid black;">CCE-687</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann einen zustzlichen Aufwand fr Benutzer bedeuten, die viele mit S/MIME signierte Nachrichten mit Outlook 2007 versenden, weil sie fr jede Nachricht eine entsprechende Beschriftung auswhlen mssen. Benutzer, die keine mit S/MIME signierten Nachrichten versenden, sind von dieser Einstellung nicht betroffen.
  
### bereinstimmung der Dateierweiterung mit dem Dateityp erzwingen
  
Betrifft: **Excel**
  
Diese Einstellung steuert, wie Excel 2007 Dateitypen ldt, die nicht mit ihrer Erweiterung bereinstimmen.
  
#### Sicherheitsrisiko
  
Excel 2007 kann Dateien mit Erweiterungen laden, die nicht ihrem jeweiligen Dateitypen entsprechen. Wenn beispielsweise eine Datei mit kommagetrennten Werten (CSV) namens **Beispiel.csv** in **Beispiel.xls** umbenannt wird, kann Excel diese korrekt als CSV-Datei laden.
  
Einige Angriffe zielen auf bestimmte Dateiformate ab. Wenn Excel Dateien mit Erweiterungen laden kann, die nicht ihrem Dateitypen entsprechen, kann eine bswillige Person Benutzer irrefhren, sodass diese gefhrliche Dateien mit falschen Erweiterungen laden.
  
Wenn Benutzer versuchen, Dateien mit der falschen Erweiterung zu ffnen, ffnet Excel standardmig die Datei und zeigt eine Warnung an, dass der Dateityp nicht den Erwartungen von Excel entspricht.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen fr die Arbeit mit Dateien zur Verfgung, die nicht die entsprechenden Erweiterungen aufweisen:
  
-   **Andere zulassen**. Excel 2007 ffnet die Dateien im eigentlichen Format, ohne Benutzer davor zu warnen, dass die Dateien nicht bereinstimmende Erweiterungen haben. Wenn Benutzer die Dateien dann bearbeiten und speichern, erhlt Excel sowohl das wirkliche, zugrunde liegende Dateiformat als auch die falsche Dateierweiterung.  
-   **Andere zulassen, aber warnen**. Excel ffnet die Datei im eigentlichen Format, warnt den Benutzer aber, dass der Dateityp diesem nicht entspricht. Diese Option ist die Standardkonfiguration in Excel.  
-   **Immer bereinstimmung mit Dateityp**. Excel ffnet keine Dateien mit nicht bereinstimmenden Erweiterungen.
  
**Tabelle 1.155: bereinstimmung der Dateierweiterung mit dem Dateityp erzwingen**

 
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
<td style="border:1px solid black;">Aktiviert Andere zulassen, aber warnen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert Immer bereinstimmung mit Dateityp</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-616</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Frhere Versionen von Excel haben keine bereinstimmung zwischen Dateityp und Erweiterung erzwungen. Die Aktivierung dieser Einstellung mit der Option **Immer bereinstimmung mit Dateityp** kann zu Beeintrchtigungen fr Benutzer fhren, die sich auf die Funktionalitt frherer Versionen von Excel verlassen. Sie knnte auerdem den Betrieb von Tools und Skripts beeintrchtigen, die sich ebenfalls auf die Funktionalitt verlassen.
  
### Fortezza-Zertifikatrichtlinien
  
Betrifft: **Outlook**
  
Diese Einstellung gibt eine Liste von Richtlinien an, die in der Richtlinienerweiterung eines Zertifikats zugelassen sind und anzeigen, ob das Zertifikat ein Fortezza-Zertifikat ist.
  
#### Sicherheitsrisiko
  
Fortezza ist ein hardwarebasierter Verschlsselungsstandard, der von der National Security Agency (NSA), einer Behrde des amerikanischen Verteidigungsministeriums, entwickelt wurde. Um fr die Verwendung mit Fortezza gltig zu sein, muss ein Zertifikat eine entsprechende Richtlinie in der Richtlinienerweiterung des Zertifikats beinhalten.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, knnen Administratoren eine Liste von Richtlinien in das bereitgestellte Textfeld eingeben, anhand derer angegeben werden kann, dass es sich bei einem Zertifikat um ein Fortezza-Zertifikat handelt. Die Liste sollte durch Semikolons getrennt werden. Zum Beispiel: Richtlinie1;Richtlinie2;Richtlinie3.
  
**Tabelle 1.156: Fortezza-Zertifikatrichtlinien**

 
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
<td style="border:1px solid black;">CCE-1402</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn Ihr Unternehmen Fortezza verwendet, mssen Sie mithilfe dieser Einstellung die Untersttzung fr Fortezza-Zertifikate aktivieren. Bei ordnungsgemer Konfiguration sollte die Einstellung keine Nutzbarkeitsprobleme fr Endbenutzer verursachen.
  
### Ausgeblendeten Text
  
Betrifft: **Word**
  
Diese Richtlinie steuert, ob als ausgeblendet formatierter Text auf den Bildschirmen von Word 2007-Benutzern angezeigt wird.
  
#### Sicherheitsrisiko
  
Standardmig zeigt Word 2007 als ausgeblendet formatierten Text nur dann an, wenn **Einblenden/Ausblenden** aktiviert oder Word im Bereich **Anzeige** des Dialogfelds **Word-Optionen** fr das Anzeigen von ausgeblendetem Text konfiguriert ist. Wenn ein Dokument verteilt wird, das ausgeblendeten Text enthlt, sind eventuell im Dokument vorhandene vertrauliche Daten mglicherweise gefhrdet.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, zeigt Word 2007 ausgeblendeten Text immer an. Ausgeblendeter Text wird auf Bildschirmen mit einer gepunkteten Linie unterstrichen angezeigt.
  
**Tabelle 1.157: Ausgeblendeter Text**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Word 2007\Word-Optionen\Anzeige</td>
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
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-885</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verursacht mglicherweise Probleme fr Word 2007-Benutzer, wenn diese Dokumente mit ausgeblendetem Text zum Drucken oder Verteilen formatieren. Die Anzeige von ausgeblendetem Text kann den Dokumentfluss verndern und die Abschtzung der Seitenanzahl und automatischen Seitenumbrche eines Dokuments erschweren.
  
### Benutzeroberflche fr Junk-E-Mail ausblenden
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob der Junk-E-Mail-Filter in Outlook 2007 aktiviert ist.
  
#### Sicherheitsrisiko
  
Der Junk-E-Mail-Filter in Outlook 2007 ist darauf ausgelegt, die offensichtlichsten Junk- oder Spam-E-Mails abzufangen und an den Junk-E-Mail-Ordner von Benutzern zu bermitteln. Der Filter bewertet jede eingehende Nachricht auf der Basis verschiedener Faktoren, darunter die Zeit, zu der die Nachricht gesendet wurde, und die Inhalte der Nachricht. Der Filter sondert keinen bestimmten Absender oder E-Mail-Typen aus, sondern analysiert stattdessen jede Nachricht auf der Basis ihrer Inhalte und Struktur, um zu erkennen, ob es sich wahrscheinlich um Spam handelt oder nicht.
  
Standardmig ist der Junk-E-Mail-Filter in Outlook 2007 aktiviert. Wenn diese Konfiguration verndert wird, erhalten Benutzer mglicherweise groe Mengen Junk-E-Mail-Nachrichten in ihrem Posteingang, sodass die Arbeit mit geschftlichen E-Mail-Nachrichten erschwert wird.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, ist der Junk-E-Mail-Filter in Outlook 2007 aktiv.
  
**Tabelle 1.158: Benutzeroberflche fr Junk-E-Mail ausblenden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen\Einstellungen\Junk-E-Mail</td>
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
<td style="border:1px solid black;">CCE-1187</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Der Name dieser Einstellung ist etwas irrefhrend, da bei ihrer Aktivierung die Junk-E-Mail-Filterung in Outlook 2007 vollstndig deaktiviert und die Filtersteuerelemente vor Benutzern ausblendet werden. Sie knnen mit der in diesem Handbuch dokumentierten Einstellung Junk-E-Mail-Schutzstufe vorab eine Filterstufe einrichten und verhindern, dass Benutzer diese ndern knnen.
  
Diese Einstellung wirkt sich nicht auf die Konfiguration des Microsoft Exchange Server Intelligent Message Filter (IMF) aus, der E-Mail-Filterung auf Serverebene bereitstellt.
  
### Andere Anwendungen ignorieren
  
Betrifft: **Excel**
  
Diese Einstellung steuert, ob Excel 2007 Daten mit anderen Anwendungen austauschen kann, die den dynamischen Datenaustausch (Dynamic Data Exchange, DDE) verwenden.
  
#### Sicherheitsrisiko
  
Standardmig kann Excel 2007 das DDE-Protokoll verwenden, um Nachrichten und Daten mit anderen Anwendungen auszutauschen. Eine Zelle in einer Excel-Arbeitsmappe kann beispielsweise dynamisch mit einem Wert verknpft sein, der von einer anderen Anwendung bereitgestellt wird, zum Beispiel Wetter- oder Aktienpreisinformationen. Wenn sich der von der anderen Anwendung bereitgestellte Wert ndert, kann Excel den Wert in der Arbeitsmappe automatisch aktualisieren. Obwohl Benutzer mit dieser Funktion sicherstellen knnen, dass Excel immer ber die neuesten Daten verfgt, bedingt die Funktion auch, dass Daten in Arbeitsmappen nderungen ohne Benutzerintervention unterliegen, was in einigen Situationen die Integritt der Daten gefhrden kann.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, ist das Kontrollkstchen **Andere Anwendungen ignorieren, die Dynamischen Datenaustausch (Dynamic Data Exchange, DDE) verwenden** im Bereich **Erweitert** des Dialogfelds **Excel-Optionen** aktiviert, und Benutzer knnen die Einstellung nicht ndern.
  
**Tabelle 1.159: Andere Anwendungen ignorieren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Erweitert</td>
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
<td style="border:1px solid black;">CCE-1471</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeintrchtigungen fr Benutzer fhren, die sich fr die Aktualisierung von Daten in Arbeitsmappen auf die DDE-Funktionalitt in Excel 2007 verlassen. Diese Benutzer mssen eine andere Methode zur Aktualisierung der von anderen Anwendungen bereitgestellten Daten verwenden.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung aktiviert ist, sehen Benutzer mglicherweise eine Fehlermeldung, wenn sie in Windows Explorer auf Excel-Arbeitsmappen doppelklicken, um diese zu ffnen. Weitere Informationen finden Sie im Knowledge Base-Artikel 211494 [Beim ffnen von Excel wird keine Arbeitsmappe angezeigt](http://support.microsoft.com/kb/211494).
  
### Korrekturhilfen verbessern
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob die Funktion zur Verbesserung der Korrekturhilfen Nutzungsdaten an Microsoft sendet.
  
#### Sicherheitsrisiko
  
Die Funktion Helfen Sie die Korrekturhilfen zu verbessern sammelt Daten ber die Nutzung der Korrekturhilfen, beispielsweise das Hinzufgen von Eintrgen in das benutzerdefinierte Wrterbuch, und sendet diese an Microsoft. Nach etwa sechs Monaten beendet die Funktion die Datenbertragung an Microsoft und lscht die Datensammlungsdatei vom Computer des Benutzers. Obwohl die Funktion nicht vorstzlich persnliche Daten sammelt, knnen einige der bertragenen Inhalte Elemente enthalten, die als Rechtschreib- oder Grammatikfehler gekennzeichnet wurden und Namen oder Kontonummern darstellen. Allerdings werden beim Sammeln der Daten alle Zahlen wie Kontonummern, Hausnummern und Telefonnummern in Nullen konvertiert. Microsoft verwendet diese Informationen zu dem alleinigen Zweck, die Effektivitt der Office-Korrekturhilfen zu verbessern. Das Unternehmen ist nicht daran interessiert, Benutzer zu identifizieren.
  
Standardmig wird diese Funktion aktiviert, wenn sich Benutzer fr die Teilnahme am Programm zur Verbesserung der Benutzerfreundlichkeit entscheiden. Wenn Ihr Unternehmen Richtlinien fr die Regelung der Verwendung externer Ressourcen wie das Programm zur Verbesserung der Benutzerfreundlichkeit einsetzt, fhrt die Verwendung der Funktion zur Verbesserung der Korrekturhilfen mglicherweise dazu, dass Benutzer gegen diese Richtlinien verstoen.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, sammelt die Funktion Helfen Sie die Korrekturhilfen zu verbessern keine Informationen zur Nutzung der Korrekturhilfen und bertrgt keine Daten an Microsoft.
  
**Tabelle 1.160: Korrekturhilfen verbessern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Rechtschreibung\Rechtschreibprfung fr Datensammlung</td>
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
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1292</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Das Programm zur Verbesserung der Benutzerfreundlichkeit sendet Korrekturhilfedaten automatisch und ohne Beeintrchtigung der Anwendungsnutzung an Microsoft, sodass die Deaktivierung der Sammlung und bertragung von Korrekturhilfedaten fr die meisten Benutzer keine Nutzbarkeitsprobleme verursachen sollte.
  
### Internet in sichere Zonen fr den automatischen Download von Bildern einschlieen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Bilder und externe Inhalte in HTML-E-Mail-Nachrichten von nicht vertrauenswrdigen Absendern im Internet heruntergeladen werden, ohne dass sich Outlook 2007-Benutzer ausdrcklich dafr entscheiden.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Krzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103511).
  
#### Sicherheitsrisiko
  
Bswillige E-Mail-Absender knnen HTML-Nachrichten mit eingebetteten Webbeacons versenden. Dabei handelt es sich um Bilder und andere Inhalte aus externen Servern, die verfolgen knnen, ob Empfnger die Nachrichten ffnen. Durch das Anzeigen von E-Mail-Nachrichten mit Webbeacons wird besttigt, dass die E-Mail-Adresse des Empfngers gltig ist, wodurch der Empfnger anfllig fr zustzliche Spam- und schdliche E-Mail-Nachrichten wird.
  
Standardmig ldt Outlook 2007 keine externen Inhalte in HTML-E-Mail-Nachrichten von nicht vertrauenswrdigen Absendern ber das Internet herunter. Wenn diese Konfiguration verndert wird, zeigt Outlook externe Inhalte in allen HTML-Nachrichten aus dem Internet an, auch wenn diese mglicherweise Webbeacons beinhalten.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, betrachtet Outlook 2007 das Internet als unsichere Zone, was bedeutet, dass Outlook Inhalte von externen Servern nur dann automatisch herunterldt, wenn der Absender in der Liste der sicheren Absender enthalten ist. Empfnger knnen sich auf der Basis einzelner Nachrichten entscheiden, ob externe Inhalte von nicht vertrauenswrdigen Absendern heruntergeladen werden.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, ldt Outlook automatisch externe Inhalte in allen ber das Internet versendeten E-Mail-Nachrichten herunter, und der Benutzer kann die Einstellung nicht ndern.
  
**Tabelle 1.161: Internet in sichere Zonen fr den automatischen Download von Bildern einschlieen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen fr den automatischen Download von Bildern</td>
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
<td style="border:1px solid black;">CCE-1497</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration durch und drfte daher fr die meisten Outlook 2007-Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Intranet in sichere Zonen fr den automatischen Download von Bildern einschlieen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Bilder und externe Inhalte in HTML-E-Mail-Nachrichten von nicht vertrauenswrdigen Absendern im lokalen Intranet heruntergeladen werden, ohne dass sich Outlook 2007-Benutzer ausdrcklich dafr entscheiden.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Krzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103512).
  
#### Sicherheitsrisiko
  
Bswillige E-Mail-Absender knnen HTML-Nachrichten mit eingebetteten Webbeacons versenden. Dabei handelt es sich um Bilder und andere Inhalte aus externen Servern, die verfolgen knnen, ob Empfnger die Nachrichten ffnen. Durch das Anzeigen von E-Mail-Nachrichten mit Webbeacons wird besttigt, dass die E-Mail-Adresse des Empfngers gltig ist, wodurch der Empfnger anfllig fr zustzliche Spam- und schdliche E-Mail-Nachrichten wird.
  
Standardmig ldt Outlook 2007 keine externen Inhalte in HTML-E-Mail-Nachrichten von nicht vertrauenswrdigen Absendern ber das lokale Intranet herunter. Wenn diese Konfiguration verndert wird, zeigt Outlook externe Inhalte in allen HTML-Nachrichten aus dem lokalen Intranet an, auch wenn diese mglicherweise Webbeacons beinhalten.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, betrachtet Outlook 2007 das Intranet nicht als sichere Zone, was bedeutet, dass Outlook Inhalte von anderen Servern in der lokalen Intranetzone nur dann automatisch herunterldt, wenn der Absender in der Liste der sicheren Absender enthalten ist. Empfnger knnen sich auf der Basis einzelner Nachrichten entscheiden, ob externe Inhalte von nicht vertrauenswrdigen Absendern heruntergeladen werden.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Wenn diese Einstellung **aktiviert** ist, ldt Outlook automatisch externe Inhalte in allen ber das lokale Intranet versendeten E-Mail-Nachrichten herunter, und der Benutzer kann die Einstellung nicht ndern.
  
**Tabelle 1.161: Intranet in sichere Zonen fr den automatischen Download von Bildern einschlieen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Einstellungen fr den automatischen Download von Bildern</td>
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
<td style="border:1px solid black;">CCE-1501</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration durch und drfte daher fr die meisten Outlook 2007-Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Verwaltung von Informationsrechten (IRM)
  
Betrifft: **InfoPath**
  
Diese Einstellung bestimmt, ob InfoPath 2007-Benutzer Formulare entwerfen knnen, die durch die Verwaltung von Informationsrechten (IRM) geschtzt sind.
  
#### Sicherheitsrisiko
  
Standardmig knnen Benutzer IRM in InfoPath 2007 verwenden, um Formulare mit eingeschrnkten Berechtigungen fr bestimmte Personen, die auf das Formular zugreifen werden, zu erstellen. Mithilfe von IRM knnen Benutzer verhindern, dass vertrauliche Daten von nicht autorisierten Personen gedruckt, weitergeleitet oder kopiert werden.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, knnen InfoPath 2007-Benutzer Formulare mit IRM-Schutzmanahmen entwerfen.
  
![](images/Dd443675.note(de-de,TechNet.10).gif) **Hinweis:**
  
Wie bei anderen Einstellungen fr **Eingeschrnkte Features** ist die Funktion bei Aktivierung dieser Einstellung nicht verfgbar und bei Deaktivierung verfgbar.
  
**Tabelle 1.163: Verwaltung von Informationsrechten (IRM)**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Eingeschrnkte Features</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">inf12.adm</td>
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
<td style="border:1px solid black;">CCE-1538</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration in InfoPath 2007 durch und drfte daher fr die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Internet- und Netzwerkpfade als Hyperlinks
  
Betrifft: **Excel**
  
Diese Einstellung bestimmt, ob Excel 2007 automatisch Hyperlinks erzeugt, wenn Benutzer URL- oder UNC-Pfadinformationen eingeben.
  
![](images/Dd443675.important(de-de,TechNet.10).gif) **Wichtig:**
  
Krzlich durchgefhrte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgem funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103522).
  
#### Sicherheitsrisiko
  
Wenn Benutzer eine Zeichenkette eingeben, die Excel 2007 als URL (Uniform Resource Locator)- oder UNC (Uniform Naming Convention)-Pfad zu einer Informationsquelle im Internet oder im lokalen Netzwerk erkennt, verwandelt Excel diese Angaben standardmig in einen Hyperlink. Ein Klick auf den Hyperlink ffnet diesen im konfigurierten Standardwebbrowser oder der entsprechenden Anwendung. Durch diese Funktionalitt knnen Benutzer versehentlich Links zu gefhrlichen oder beschrnkten Ressourcen erstellen und mglicherweise das Sicherheitsrisiko steigern.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, wird das Kontrollkstchen **Internet- und Netzwerkpfade als Hyperlinks** unter **Whrend der Eingabe ersetzen** im Dialogfeld **AutoKorrektur** deaktiviert, und Benutzer knnen die Einstellung nicht ndern.
  
![](images/Dd443675.note(de-de,TechNet.10).gif) **Hinweis:**
  
Wenn die Einstellung **aktiviert** ist, verwandelt Excel 2007 URLs und UNC-Pfade automatisch in Hyperlinks, und Benutzer knnen diese Funktion nicht deaktivieren.
  
**Tabelle 1.164: Internet- und Netzwerkpfade als Hyperlinks**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Dokumentprfung\AutoKorrektur-Optionen</td>
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
<td style="border:1px solid black;">CCE-1532</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung deaktiviert ist, knnen Excel 2007-Benutzer neue Hyperlinks weiterhin manuell erstellen, deshalb werden fr die meisten Benutzer kaum wesentliche Beeintrchtigungen verursacht.
  
### Junk-E-Mail-Schutzstufe
  
Betrifft: **Outlook**
  
Diese Einstellung steuert die Stufe der Junk-E-Mail-Filterung, die Outlook 2007 durchfhrt.
  
#### Sicherheitsrisiko
  
Der Junk-E-Mail-Filter in Outlook 2007 ist darauf ausgelegt, die offensichtlichsten Junk- oder Spam-E-Mails abzufangen und an den Junk-E-Mail-Ordner von Benutzern zu bermitteln. Der Filter bewertet jede eingehende Nachricht auf der Basis verschiedener Faktoren, darunter die Zeit, zu der die Nachricht gesendet wurde, und die Inhalte der Nachricht. Der Filter sondert keinen bestimmten Absender oder E-Mail-Typen aus, sondern analysiert stattdessen jede Nachricht auf der Basis ihrer Inhalte und Struktur, um zu erkennen, ob es sich wahrscheinlich um Spam handelt oder nicht.
  
Standardmig stehen Benutzern vier Stufen der Junk-E-Mail-Filterung zur Auswahl:
  
-   **Keine automatische Filterung**. Outlook fhrt keine Beurteilung eingehender Nachrichten nach Inhalten durch. Outlook bewertet Nachrichten weiterhin anhand der Domnennamen und E-Mail-Adressen in den Listen der Benutzer fr blockierte Absender und verschiebt Nachrichten von blockierten Absendern in die Junk-E-Mail-Ordner der Benutzer.  
-   **Niedrig**. Outlook verschiebt nur die offensichtlichsten Spamnachrichten in die Junk-E-Mail-Ordner der Benutzer. Diese Stufe ist die Standardeinstellung.  
-   **Hoch**. Outlook fngt die meisten Junk-E-Mails ab, kann aber flschlicherweise einige legitime Nachrichten als Junk-E-Mail klassifizieren. Benutzern wird empfohlen, ihren Junk-E-Mail-Ordner oft zu berprfen.  
-   **Nur sichere Absender und Empfnger**. Outlook verschiebt alle eingehenden Nachrichten in die Junk-E-Mail-Ordner der Benutzer, aufgenommen von Nachrichten, die von Absendern in der Liste der sicheren Absender stammen und die an Mailinglisten in der Liste der sicheren Empfnger gesendet werden.
  
Wenn Benutzer eine unangemessene Einstellung auswhlen, verpassen sie mglicherweise wichtige Nachrichten oder sammeln groe Mengen Junk-E-Mail in ihrem Posteingang an.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, knnen Administratoren eine der vier aufgelisteten Optionen auswhlen und allen betroffenen Benutzern zuweisen. Die Benutzer knnen die Einstellung nicht ndern.
  
**Tabelle 1.165: Junk-E-Mail-Schutzstufe**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen\Einstellungen\Junk-E-Mail</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>ADM-Datei</strong></td>
<td style="border:1px solid black;">outlk12.adm</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (EC)</strong></td>
<td style="border:1px solid black;">Aktiviert (Niedrig)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert (Hoch)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1588</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Unterschiedliche Benutzer erhalten mglicherweise unterschiedlich viele Junk-E-Mail-Nachrichten. Die Aktivierung dieser Einstellung kann dazu fhren, dass die Junk-E-Mail-Schutzstufe fr einige Benutzer zu hoch und fr andere zu niedrig eingerichtet wird.
  
### Schlsselverwendungsfilterung
  
Betrifft: **2007 Office System**
  
Mit dieser Einstellung knnen Administratoren eine Liste digitaler Zertifikate fr das Signieren von Excel 2007-, PowerPoint 2007- und Word 2007-Dokumenten auf der Basis des Schlsselverwendungsfelds filtern.
  
#### Sicherheitsrisiko
  
Das Feld Schlsselverwendung in einem Zertifikat dient dazu, eine Reihe von grundlegenden Einschrnkungen fr die allgemeinen Arten von Vorgngen darzustellen, die mit dem Zertifikat durchgefhrt werden knnen. Mithilfe der Schlsselverwendungsfilterung knnen Sie die Liste installierter Zertifikate filtern, die fr das digitale Signieren von Dokumenten verwendet werden knnen. Die gefilterte Liste wird angezeigt, wenn Benutzer versuchen, ein Zertifikat fr die digitale Signatur eines Dokuments auszuwhlen.
  
Standardmig werden digitale Zertifikate mit dem Wert digitale Signatur im Schlsselverwendungsfeld als verfgbare Zertifikate aufgelistet. Wenn die Schlsselfilterung nicht verwendet wird, knnen Benutzer versehentlich oder mit bswilliger Absicht die falsche Art von Zertifikat fr das digitale Signieren eines Dokuments oder das berprfen einer Signatur verwenden. Das fhrt mglicherweise zu einer Gefhrdung der Datensicherheit oder macht eine berprfung der Signaturinformationen eines Dokuments unmglich.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, werden digitale Zertifikate mit dem Wert digitale Signatur im Schlsselverwendungsfeld als verfgbare Zertifikate aufgelistet.
  
**Tabelle 1.166: Schlsselverwendungsfilterung**

 
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
<td style="border:1px solid black;">CCE-1396</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, mssen Sie sich vergewissern, dass die verwendeten Zertifikate die korrekten Informationen im Schlsselverwendungsfeld enthalten, damit sie zum Signieren und berprfen digitaler Signaturen verwendet werden knnen.
  
### Legacyformatsignaturen
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer Office 97-2003-Dokumenten digitale Signaturen im Binrformat zuweisen knnen.
  
#### Sicherheitsrisiko
  
Standardmig verwenden 2007 Office-Anwendungen das XML-basierte XMLDSIG-Format, um Dokumenten, einschlielich binren Office 97-2003-Dokumenten, digitale Signaturen anzufgen. XMLDSIG-Signaturen werden von Office 2003- oder frheren Anwendungen nicht erkannt. Wenn ein Office 2003-Benutzer ein binres Excel-, PowerPoint- oder Word-Dokument mit einer angehngten XMLDSIG-Signatur ffnet, geht die Signatur verloren.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, verwenden 2007 Office-Anwendungen das Office 2003-Binrformat, um binren Office 97-2003-Dokumenten digitale Signaturen zuzuweisen, damit diese von Anwendungen der Office 2003-Version und frheren Versionen erkannt werden.
  
**Tabelle 1.167: Legacyformatsignaturen**

 
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
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1585</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung sollte fr die meisten 2007 Office-Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Steuerelemente in Forms3 laden
  
Betrifft: **2007 Office System**
  
Diese Einstellung bestimmt, wie 2007 Office-Anwendungen ActiveX-Steuerelemente in Benutzerformularen laden.
  
#### Sicherheitsrisiko
  
ActiveX-Steuerelemente sind COM-Objekte (Component Object Model), die uneingeschrnkten Zugriff auf die Computer von Benutzern haben. ActiveX-Steuerelemente knnen auf das lokale Dateisystem zugreifen und die Registrierungseinstellungen des Betriebssystems ndern. Wenn ein bswilliger Benutzer ein ActiveX-Steuerelement umfunktioniert, um den Computer eines Benutzers zu bernehmen, knnen die Auswirkungen gravierend sein.
  
Fr eine hhere Sicherheit knnen ActiveX-Entwickler Steuerelemente als Safe for Initialization (SFI) kennzeichnen, was bedeutet, dass der Entwickler das sichere ffnen und Ausfhren der Steuerelemente garantiert und besttigt, dass die Steuerelemente den Computer nicht beschdigen werden. Wenn ein Steuerelement nicht als SFI gekennzeichnet ist, kann das Steuerelement einen Computer mglicherweise beeintrchtigen. Vielleicht hat der Entwickler das Steuerelement aber auch nicht in allen Situationen testen knnen und kann daher nicht garantieren, dass sein Steuerelement nicht zu einem spteren Zeitpunkt gefhrdet sein knnte.
  
SFI-Steuerelemente werden im sicheren Modus ausgefhrt, sodass ihr Zugriff auf den Computer beschrnkt ist. Ein Arbeitsblattsteuerelement kann beispielsweise im unsicheren Modus Dateien sowohl lesen als auch schreiben, im sicheren Modus dagegen mglicherweise nur aus Dateien lesen. Durch diese Funktionalitt kann das Steuerelement auf sehr leistungsfhige Weise verwendet werden, wenn die Sicherheit keine Rolle spielt, aber auch sicher auf einer Webseite eingesetzt werden.
  
Wenn ein Steuerelement nicht als SFI gekennzeichnet ist, wird es als Unsafe For Initialization (UFI) gekennzeichnet, was bedeutet, dass es den Computer eines Benutzers beeintrchtigen kann. Als UFI gekennzeichnete ActiveX-Steuerelemente werden nur im unsicheren Modus geladen.
  
Mit dieser Einstellung knnen Administratoren steuern, wie ActiveX-Steuerelemente in Benutzerformularen initialisiert werden, abhngig davon, ob sie als SFI oder UFI gekennzeichnet sind.
  
#### Gegenmanahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen fr das Laden von Steuerelementen in Benutzerformularen zur Verfgung:
  
-   **1**. Ein mit UFI oder SFI signiertes Steuerelement, das den sicheren und den unsicheren Modus untersttzt, wird im unsicheren Modus geladen. Ein mit SFI signiertes Steuerelement, das nur eine Konfiguration im sicheren Modus untersttzt, wird im sicheren Modus geladen. Diese Option setzt die Standardkonfiguration durch.  
-   **2**. Benutzer knnen per Eingabeaufforderung bestimmen, wie Benutzerformulare geladen werden. Die Eingabeaufforderung wird nur einmal pro Sitzung in einer Anwendung angezeigt. Wenn Benutzer auf die Eingabeaufforderung reagieren, wird das Laden fortgesetzt, abhngig davon, ob das Steuerelement als UFI oder SFI gekennzeichnet ist:
  
    -   Ein als UFI signiertes Steuerelement wird im unsicheren Modus geladen, wenn Benutzer auf die Eingabeaufforderung mit **Ja** reagieren. Wenn Benutzer mit **Nein** reagieren, wird das Steuerelement mit den Standardeigenschaften geladen.  
    -   Ein als SFI signiertes Steuerelement, das sowohl den sicheren als auch den unsicheren Modus untersttzt, wird im unsicheren Modus geladen, wenn Benutzer auf die Eingabeaufforderung mit **Ja** reagieren. Wenn Benutzer mit **Nein** reagieren, wird das Steuerelement im sicheren Modus geladen. Wenn das SFI-Steuerelement nur den sicheren Modus untersttzt, wird das Steuerelement im sicheren Modus geladen.
  
    Diese Option ist die Standardkonfiguration in der 2007 Office-Version.
  
-   **3**. Benutzer knnen per Eingabeaufforderung bestimmen, wie Benutzerformulare geladen werden. Die Eingabeaufforderung wird nur einmal pro Sitzung in einer Anwendung angezeigt. Wenn Benutzer auf die Eingabeaufforderung reagieren, wird das Laden fortgesetzt, abhngig davon, ob das Steuerelement als UFI oder SFI gekennzeichnet ist:  
    -   Ein als UFI signiertes Steuerelement wird im unsicheren Modus geladen, wenn Benutzer auf die Eingabeaufforderung mit **Ja** reagieren. Wenn Benutzer mit **Nein** reagieren, wird das Steuerelement mit den Standardeigenschaften geladen.  
    -   Ein mit SFI signiertes Steuerelement wird im sicheren Modus geladen.  
-   **4**. Ein als UFI signiertes Steuerelement wird mit den Standardeigenschaften des Steuerelements geladen. Ein mit SFI signiertes Steuerelement wird im sicheren Modus geladen (was als sicherster Modus betrachtet wird).
  
**Tabelle 1.168: Steuerelemente in Forms3 laden**

 
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
<td style="border:1px solid black;">Aktiviert (1)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Empfohlene Einstellung (SSLF)</strong></td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>CCE-ID</strong></td>
<td style="border:1px solid black;">CCE-1068</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Konfiguration fr die EC-Umgebung ist 1. Sie setzt die Standardkonfiguration durch und sollte daher fr die meisten Benutzer keine Nutzbarkeitsprobleme verursachen.
  
### Bilder von Webseiten laden, die nicht mit Excel erstellt wurden
  
Betrifft: **Excel**
  
Diese Einstellung steuert, ob Excel 2007 beim ffnen von nicht in Excel erstellten Webseiten Grafiken ldt.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Webseiten in Excel 2007 ffnen, ldt Excel standardmig alle Grafiken, die in den Seiten enthalten sind, unabhngig davon, ob diese ursprnglich in Excel erstellt wurden. Benutzer knnen diese Option im Dialogfeld **Weboptionen** ndern, das ber den Bereich **Erweitert** des Dialogfelds **Excel-Optionen** verfgbar ist.
  
Wenn Sie zulassen, dass Excel in anderen Programmen erstellte Grafiken ldt, wird Excel mglicherweise anfllig fr zuknftige Zero-Day-Angriffe, die Grafikdateien als Angriffsmittel verwenden. Falls es zu einem solchen Ereignis kommt, kann das Sicherheitsrisiko mit dieser Einstellung gemindert werden.
  
#### Gegenmanahme
  
Wenn diese Einstellung **deaktiviert** ist, ldt Excel 2007 keine Bilder aus Webseiten, die nicht in Excel erstellt wurden.
  
![](images/Dd443675.note(de-de,TechNet.10).gif) **Hinweis:**
  
Wenn die Einstellung **aktiviert** ist, ldt Excel Bilder aus Webseiten, die nicht in Excel erstellt wurden, und Benutzer knnen diese Konfiguration nicht ndern.
  
**Tabelle 1.169: Bilder von Webseiten laden, die nicht mit Excel erstellt wurden**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Speicherort in Gruppenrichtlinie</strong></td>
<td style="border:1px solid black;">Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Excel 2007\Excel-Optionen\Erweitert\Weboptionen\Allgemein</td>
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
<td style="border:1px solid black;">CCE-1464</td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung fr die SSLF-Umgebung ist **Deaktiviert**, was bedeutet, dass Excel 2007 keine Bilder aus Webseiten ldt, die nicht in Excel erstellt wurden. Diese Konfiguration kann zu einigen Beeintrchtigungen fr Benutzer fhren, die Webseiten in Excel laden, die von anderen Anwendungen erstellt wurden. Benutzer, die keine Webseiten in Excel laden, sind von dieser Einstellung nicht betroffen.
  
##### In diesem Beitrag
  
-   [berblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))  
-   -   Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 4  
-   [Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen fr Benutzerrichtlinien Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))  
-   [Sicherheitseinstellungen fr Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um ber Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%c2%a0microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenma%c3%9fnahmen:%20sicherheitseinstellungen%20in%202007%c2%a0office%20system)
  
|                                                  |                                                                                                                                                                                                                                                                                                                                                                              |  
|--------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443675.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))5 von 8[![](images/Dd443675.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10)) |
