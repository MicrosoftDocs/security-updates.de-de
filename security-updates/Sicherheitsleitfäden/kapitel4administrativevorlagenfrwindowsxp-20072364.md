---
TOCTitle: 'Kapitel 4: Administrative Vorlagen für Windows XP'
Title: 'Kapitel 4: Administrative Vorlagen für Windows XP'
ms:assetid: 'adb79ec2-691f-4a9f-b940-36d2d9807fd7'
ms:contentKeyID: 20072364
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc163076(v=TechNet.10)'
---

Windows XP-Sicherheitshandbuch
==============================

### Kapitel 4: Administrative Vorlagen für Windows XP

Aktualisiert: 20.10.2005

##### Auf dieser Seite

[](#edaa)[Überblick](#edaa)
[](#ecaa)[Computerkonfigurationseinstellungen](#ecaa)
[](#ebaa)[Benutzerkonfigurationseinstellungen](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

In diesem Kapitel wird ausführlich beschrieben, wie mithilfe administrativer Vorlagen zusätzliche Sicherheitseinstellungen auf Computern mit Microsoft® Windows® XP Professional mit Service Pack 2 (SP2) konfiguriert und angewendet werden. Administrative Vorlagedateien (.adm) werden verwendet, um die Einstellungen in der Windows XP-Registrierung zu konfigurieren, mit denen das Verhalten vieler Dienste, Anwendungen und Betriebssystemkomponenten gesteuert wird.

Fünf der administrativen Vorlagen, die mit Windows XP SP2 geliefert werden, umfassen hunderte zusätzliche Einstellungen, mit denen Sie die Sicherheit von Windows XP Professional verbessern können. Einige der Einstellungen in den administrativen Vorlagen für Windows Server™ 2003 können unter Windows XP nicht angewendet werden. Eine vollständige Liste aller für Windows XP verfügbaren Einstellungen in den administrativen Vorlagen finden Sie in der Excel-Arbeitsmappe „Richtlinieneinstellungen“, auf die im Abschnitt „Weitere Informationen“ am Ende dieses Kapitels verwiesen wird.

In der folgenden Tabelle werden die .adm-Dateien und die jeweils betroffenen Anwendungen und Dienste aufgelistet.

**Tabelle 4.1: Administrative Vorlagedateien**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Dateiname</th>
<th>Betriebssystem</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">System.adm</td>
<td style="border:1px solid black;">Windows XP Professional</td>
<td style="border:1px solid black;">Enthält zahlreiche Einstellungen für die Anpassung der jeweiligen Betriebssystemumgebung von Benutzern.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Inetres.adm</td>
<td style="border:1px solid black;">Windows XP Professional</td>
<td style="border:1px solid black;">Enthält Einstellungen für Internet Explorer 6.0.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Conf.adm</td>
<td style="border:1px solid black;">Windows XP Professional</td>
<td style="border:1px solid black;">Enthält Einstellungen für die Konfiguration von Microsoft NetMeeting®.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wmplayer.adm</td>
<td style="border:1px solid black;">Windows XP Professional</td>
<td style="border:1px solid black;">Enthält Einstellungen für die Konfiguration von Windows Media Player.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Wuau.adm</td>
<td style="border:1px solid black;">Windows XP Professional</td>
<td style="border:1px solid black;">Enthält Einstellungen für die Konfiguration von Windows Update.</td>
</tr>
</tbody>
</table>
  
**Hinweis**: Die Einstellungen der administrativen Vorlagen müssen manuell im Gruppenrichtlinienobjekt konfiguriert werden, damit sie für die Computer und Benutzer in Ihrer Umgebung gelten.
  
Es gibt zwei Hauptgruppen von Einstellungen in den administrativen Vorlagen:
  
-   Die in der Registrierungsstruktur **HKEY\_Local\_Machine** gespeicherten Computerkonfigurationseinstellungen
  
-   Die in der Registrierungsstruktur **HKEY\_Current\_User** gespeicherten Benutzerkonfigurationseinstellungen
  
Ebenso wie in Kapitel 3, „Sicherheitseinstellungen für Windows XP-Clients“, sind in diesem Kapitel empfohlene Einstellungen für die Unternehmensclient-Umgebung (EC, Enterprise Client) und die Hochsicherheitsumgebung (SSLF, Specialized Security – Limited Functionality) enthalten, die beide in diesem Handbuch behandelt werden.
  
**Hinweis**: Die Benutzereinstellungen werden auf eine Organisationseinheit angewendet, die über ein Gruppenrichtlinienobjekt verknüpfte Benutzer enthält. Weitere Informationen zu dieser Organisationseinheit finden Sie in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“.
  
Einige Einstellungen sind jeweils in der Computer- und in der Benutzerkonfiguration im Gruppenrichtlinienobjekt-Editor verfügbar. Wenn für einen Benutzer eine Einstellung konfiguriert wurde und sich der Benutzer auf einem Computer anmeldet, für den über die Gruppenrichtlinie dieselbe Computerkonfigurationseinstellung festgelegt wurde, hat die Computerkonfiguration Vorrang vor der Benutzerkonfiguration.
  
Frühere Versionen dieses Handbuchs enthalten Informationen zu Einstellungen für Office XP. Diese Einstellungen wurden jedoch für Office 2003 aktualisiert und sind auf der Microsoft-Website verfügbar. Im Abschnitt „Weitere Informationen“ am Ende dieses Kapitels finden Sie Links, die zu diesen Informationen führen.
  
In diesem Kapitel werden nicht alle möglichen Einstellungen der administrativen Vorlagen von Microsoft erläutert. Bei einigen dieser Einstellungen handelt es sich um Einstellungen für die Benutzeroberfläche, die keine Auswirkungen auf die Sicherheit haben. Entscheiden Sie anhand der Sicherheitsziele Ihrer Organisation, welche der in dieser Anleitung empfohlenen Einstellungskonfigurationen verwendet werden sollen.
  
Wenn Sie über die Gruppenrichtlinie weitere Einstellungen für Windows XP Professional anwenden möchten, können Sie benutzerdefinierte Vorlagen erstellen. Ausführliche Informationen zum Erstellen benutzerdefinierter administrativer Vorlagen finden Sie in den Whitepapers, die im Abschnitt „Weitere Informationen“ am Ende dieses Kapitels aufgeführt werden.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Computerkonfigurationseinstellungen
  
In den folgenden Abschnitten werden die im Gruppenrichtlinienobjekt-Editor unter „Computerkonfiguration“ empfohlenen Einstellungen erläutert. Konfigurieren Sie diese Einstellungen in folgendem Verzeichnis:
  
**Computerkonfiguration\\Administrative Vorlagen**
  
Dieser Speicherort ist in der folgenden Abbildung im Zusammenhang dargestellt:
  
![](images/Cc163076.SGFG0401(de-de,TechNet.10).gif)
  
**Abbildung 4.1: Gruppenrichtlinienstruktur für die Computerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0401_big(de-de,technet.10).gif)
  
Die Struktur dieses Kapitels basiert auf der Containerstruktur in der Gruppenrichtlinie. In den Tabellen in den folgenden Abschnitten sind Einstellungsempfehlungen für verschiedene Computerkonfigurationsoptionen zusammengefasst. Empfehlungen werden sowohl für Desktop- als auch für Laptopclientcomputer in den beiden Sicherheitsumgebungen gegeben, die in diesem Kapitel erörtert werden: die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung. Weitere Informationen zu den Einstellungen finden Sie in den Unterabschnitten im Anschluss an jede Tabelle.
  
Wenden Sie diese Einstellungen mithilfe eines Gruppenrichtlinienobjekts an, das mit einer Organisationseinheit verknüpft ist, die die Computerkonten Ihrer Umgebung enthält. Fügen Sie dabei die Laptopeinstellungen im mit der Laptoporganisationseinheit verknüpften Gruppenrichtlinienobjekt und die Desktopeinstellungen im mit der Desktoporganisationseinheit verknüpften Gruppenrichtlinienobjekt ein.
  
#### Windows-Komponenten
  
Die folgende Abbildung illustriert die Abschnitte in der Gruppenrichtlinie, die von den Einstellungsänderungen in diesem Abschnitt betroffen sein werden:
  
![](images/Cc163076.SGFG0402(de-de,TechNet.10).gif)
  
**Abbildung 4.2: Gruppenrichtlinienstruktur für Windows-Komponenten in der Computerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0402_big(de-de,technet.10).gif)
  
##### NetMeeting
  
Mit Microsoft NetMeeting können über das Netzwerk Ihrer Organisation virtuelle Besprechungen durchgeführt werden. Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**NetMeeting**
  
**Tabelle 4.2: Empfohlene Einstellungen für NetMeeting**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Remotedesktop-Freigabe deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Remotedesktop-Freigabe deaktivieren
  
Durch diese Richtlinieneinstellung wird die Remotedesktop-Freigabe von NetMeeting deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer NetMeeting nicht konfigurieren, um eine Remotesteuerung des lokalen Desktops zuzulassen.
  
Die Einstellung **Remotedesktop-Freigabe deaktivieren** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert**. Für die Hochsicherheitsumgebung ist sie jedoch auf **Aktiviert** gesetzt, um Benutzer von der Remotedesktop-Freigabe über NetMeeting abzuhalten.
  
##### Internet Explorer
  
Mithilfe der Gruppenrichtlinien für Microsoft Internet Explorer können Sie die Sicherheitsanforderungen für Windows XP-Arbeitsstationen umsetzen. Darüber hinaus wird dadurch der Austausch unerwünschter Inhalte über Internet Explorer verhindert. Richten Sie sich nach den folgenden Kriterien, um Internet Explorer auf den Arbeitsstationen in Ihrer Umgebung zu schützen:
  
-   Stellen Sie sicher, dass Anfragen im Internet lediglich als direkte Reaktion auf Benutzeraktionen erfolgen.
  
-   Stellen Sie sicher, dass an bestimmte Websites gesendete Informationen nur auf diese Websites übertragen werden, sofern keine spezifischen Benutzeraktionen zum Übertragen von Informationen an andere Ziele definiert wurden.
  
-   Stellen Sie sicher, dass vertrauenswürdige Kanäle zu Servern/Websites sowie die Besitzer der einzelnen Servern/Websites eindeutig identifiziert werden.
  
-   Stellen Sie sicher, dass alle mit Internet Explorer gestarteten Skripts oder Programme in einer eingeschränkten Umgebung ausgeführt werden. Die über vertrauenswürdige Kanäle übermittelten Programme können so konfiguriert werden, dass sie außerhalb der eingeschränkten Umgebung ausgeführt werden.
  
Die folgenden empfohlenen Computereinstellungen für Internet Explorer können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer**
  
In der folgenden Tabelle sind viele der empfohlenen Einstellungen für Internet Explorer zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.3: Empfohlene Einstellungen für Internet Explorer**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Automatische Installation von Internet Explorer-Komponenten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Periodische Überprüfungen auf Softwareaktualisierungen von Internet Explorer deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Softwareupdatebenachrichtigungen beim Programmstart deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Benutzern nicht erlauben, Add-Ons zu aktivieren oder zu deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Proxyeinstellungen pro Computer vornehmen (anstelle von pro Benutzer)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sicherheitszonen: Benutzer können keine Sites hinzufügen oder entfernen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Sicherheitszonen: Benutzer können keine Einstellungen ändern</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sicherheitszonen: Die Einstellungen für Sicherheitszonen statisch festlegen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Absturzerkennung deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Automatische Installation von Internet Explorer-Komponenten deaktivieren
  
Wenn Sie diese Richtlinieneinstellung aktivieren, kann Internet Explorer keine Komponenten herunterladen, wenn die Benutzer Websites ansteuern, die für ein vollständiges Funktionieren diese Komponenten erfordern. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, werden die Benutzer bei jedem Besuch der entsprechenden Websites aufgefordert, die Komponenten herunterzuladen oder zu installieren.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung ist die Einstellung **Automatische Installation von Internet Explorer-Komponenten deaktivieren** auf **Aktiviert** gesetzt.
  
**Hinweis**: Microsoft empfiehlt, vor dem Aktivieren dieser Richtlinieneinstellung mit Microsoft Update oder einem ähnlichen Dienst eine alternative Möglichkeit zum Aktualisieren von Internet Explorer einzurichten.
  
###### Periodische Überprüfungen auf Softwareaktualisierungen von Internet Explorer deaktivieren
  
Wenn Sie diese Richtlinieneinstellung aktivieren, kann durch Internet Explorer nicht mehr festgestellt werden, ob eine neuere Browserversion verfügbar ist, und die Benutzer erhalten keine entsprechende Benachrichtigung mehr. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, wird von Internet Explorer standardmäßig alle 30 Tage geprüft, ob Aktualisierungen vorhanden sind. Ist eine neue Version verfügbar, werden die Benutzer benachrichtigt.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung ist die Einstellung **Periodische Überprüfungen auf Softwareaktualisierungen von Internet Explorer deaktivieren** auf **Aktiviert** gesetzt.
  
**Hinweis**: Microsoft empfiehlt, vor dem Aktivieren dieser Richtlinieneinstellung eine alternative Strategie für die Administratoren Ihrer Organisation einzurichten, um sicherzustellen, dass auf den Clients Ihrer Umgebung regelmäßig neue Updates für Internet Explorer ausgeführt werden.
  
###### Softwareupdatebenachrichtigungen beim Programmstart deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, dass Programme, die Microsoft Software Distribution Channels verwenden, Benutzer nicht informieren, wenn neue Komponenten installiert werden. Software Distribution Channels werden für die dynamische Aktualisierung von Software auf Benutzercomputern verwendet und basieren auf Open Software Distribution-Technologie (.osd).
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Deaktivieren von Software-Update Shell-Benachrichtigungen beim Programmstart** auf **Aktiviert** gesetzt.
  
###### Benutzern nicht erlauben, Add-Ons zu aktivieren oder zu deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Möglichkeit haben, Add-Ons mithilfe des Befehls „Add-Ons verwalten“ zuzulassen oder zu verweigern. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** einstellen, können Benutzer Add-Ons nicht über den Befehl „Add-Ons verwalten“ aktivieren oder deaktivieren. Einzige Ausnahme: ein Add-On wurde in einer Art und Weise der Richtlinieneinstellung für die **Add-On-Liste** hinzugefügt, dass Benutzer das Add-On weiterhin verwalten können. In einem solchen Fall kann der Benutzer das Add-On immer noch über „Add-Ons verwalten“ verwalten. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, kann der Benutzer Add-Ons aktivieren bzw. deaktivieren.
  
**Hinweis**: Weitere Informationen zum Verwalten von Internet Explorer-Add-Ons in Windows XP SP2 finden Sie im Knowledge Base-Artikel 883256 „Verwalten von Internet Explorer-Add-Ons in Windows XP Service Pack 2“ unter <http://support.microsoft.com/?kbid=883256>.
  
Benutzer installieren häufig Add-Ons, die von der Sicherheitsrichtlinie einer Organisation nicht zugelassen sind. Solche Add-Ons können ein Sicherheits- und Vertraulichkeitsrisiko für Ihr Netzwerk darstellen. Für die beiden in diesem Kapitel behandelten Umgebungen ist diese Richtlinieneinstellung deshalb auf **Aktiviert** gesetzt.
  
**Hinweis**: Sie sollten die Gruppenrichtlinienobjekteinstellungen in Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung überprüfen, um sicherzustellen, dass entsprechend autorisierte Add-Ons weiterhin in Ihrer Umgebung ausgeführt werden können. Lesen Sie gegebenenfalls den Microsoft Knowledge Base-Artikel „[Outlook Web Access und Small Business Server Remote Web Workplace funktionieren nicht, wenn unter XP Service Pack 2 über Gruppenrichtlinien die Add-On-Blockierung aktiviert ist](http://support.microsoft.com/kb/555235/en-us)“ (in englischer Sprache) unter http://support.microsoft.com/kb/555235/en-us.
  
###### Proxyeinstellungen pro Computer vornehmen (anstelle von pro Benutzer)
  
Wenn Sie diese Richtlinieneinstellung aktivieren, ist es Benutzern nicht erlaubt, benutzerspezifische Proxyeinstellungen zu ändern. Die Benutzer müssen die Zonen verwenden, die für alle Benutzer eines Computers erstellt wurden.
  
Für Desktopclientcomputer in den beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Proxyeinstellungen pro Computer vornehmen (anstelle von pro Benutzer)** auf **Aktiviert** gesetzt. Für Laptopclientcomputer ist die Richtlinieneinstellung jedoch auf **Deaktiviert** gesetzt, da mobile Benutzer auf Reisen die Proxyeinstellungen u. U. ändern müssen.
  
###### Sicherheitszonen: Benutzer können keine Sites hinzufügen oder entfernen
  
Aktivieren Sie diese Richtlinieneinstellung, um die Einstellungen für die Siteverwaltung von Sicherheitszonen zu deaktivieren. (Um die Einstellungen für die Siteverwaltung von Sicherheitszonen anzuzeigen, öffnen Sie Internet Explorer, wählen Sie **Extras** und anschließend **Internetoptionen**. Klicken Sie auf die Registerkarte **Sicherheit** und dann auf **Sites**.) Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können Benutzer den Zonen **Vertrauenswürdige Sites** und **Eingeschränkte Sites** keine Websites hinzufügen oder Websites aus ihnen entfernen und auch die Einstellungen der Zone **Lokales Intranet** nicht verändern.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Sicherheitszonen: Benutzer können Sites nicht hinzufügen oder entfernen** auf **Aktiviert** gesetzt.
  
**Hinweis**: Wenn Sie die Einstellung **Sicherheitsseite deaktivieren** aktivieren (unter \\Benutzerkonfiguration\\  
Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung), wird die Registerkarte **Sicherheit** aus der Benutzeroberfläche entfernt, und die Einstellung **Sicherheitsseite deaktivieren** erhält Vorrang vor der Einstellung **Sicherheitszonen: Benutzer können keine Sites hinzufügen oder entfernen**.
  
###### Sicherheitszonen: Benutzer können keine Einstellungen ändern
  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Schaltfläche **Stufe anpasse**n und der Schieberegler **Sicherheitsstufe dieser Zone** auf der Registerkarte **Sicherheit** im Dialogfeld **Internetoptionen** deaktiviert. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können Benutzer die Einstellungen für Sicherheitszonen ändern. Dadurch wird verhindert, dass die Benutzer die vom Administrator vorgegebenen Einstellungen der Sicherheitszonenrichtlinie ändern.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Sicherheitszonen: Benutzer können Einstellungen nicht ändern** auf **Aktiviert** gesetzt.
  
**Hinweis**: Wenn Sie die Einstellung **Sicherheitsseite deaktivieren** (unter \\Benutzerkonfiguration\\  
Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung) aktivieren, wird die Registerkarte **Sicherheit** aus Internet Explorer in der Systemsteuerung entfernt, und die Einstellung **Sicherheitsseite deaktivieren** erhält Vorrang vor der Einstellung **Sicherheitszonen: Benutzer können keine Einstellungen ändern**.
  
###### Sicherheitszonen: Die Einstellungen für Sicherheitszonen statisch festlegen
  
Durch diese Richtlinieneinstellung wird festgelegt, wie sich Änderungen der Sicherheitszonen auf verschiedene Benutzer auswirken. Dadurch soll sichergestellt werden, dass die Sicherheitszoneneinstellungen auf dem gleichen Computer einheitlich bleiben und sich nicht von Benutzer zu Benutzer ändern. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Änderungen, die der Benutzer an einer Sicherheitszone vornimmt, auf alle Benutzer des betreffenden Computers angewendet. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können die Benutzer eines Computers ihre eigenen Sicherheitszoneneinstellungen festlegen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Sicherheitszonen: Die Einstellungen für Sicherheitszonen statisch festlegen** auf **Aktiviert** gesetzt.
  
###### Absturzerkennung deaktivieren
  
Mit dieser Richtlinieneinstellung können Sie die Absturzerkennung in der Add-On-Verwaltung in Internet Explorer verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, hat ein Absturz in Internet Explorer ähnliche Auswirkungen wie ein Absturz auf einem Computer, auf dem Windows XP Professional Service Pack 1 oder eine frühere Version ausgeführt wird: Die Windows-Fehlerberichterstattung wird aufgerufen. Wenn Sie diese Richtlinieneinstellung deaktivieren, ist die Absturzerkennung in der Add-On-Verwaltung aktiviert.
  
Da der Absturzbericht von Internet Explorer vertrauliche Informationen aus dem Speicher des Computers enthalten kann, ist die Einstellung **Absturzerkennung deaktivieren** für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt. Wenn es häufig zu wiederholten Abstürzen kommt, über die Sie für die nachfolgende Problembehandlung Bericht erstatten müssen, können Sie die Richtlinieneinstellung vorübergehend auf **Deaktiviert** setzen.
  
##### Internet Explorer\\Internetsystemsteuerung\\Sicherheitsseite
  
Diese Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung\\Sicherheitsseite**
  
Mit SP2 werden mehrere neue Richtlinieneinstellungen eingeführt, mit denen Sie die Konfiguration der Internet Explorer-Zone in Ihrer gesamten Umgebung absichern können. Die Standardwerte für diese Einstellungen bieten im Vergleich zu früheren Windows-Versionen eine höhere Sicherheit. Sie haben die Möglichkeit, diese Einstellungen zu überprüfen und zu entscheiden, ob Sie sie in Ihrer Umgebung benötigen oder aus Gründen der Benutzerfreundlichkeit oder Anwendungskompatibilität lockern möchten.
  
Durch SP2 wird z. B. Internet Explorer so konfiguriert, dass Popups standardmäßig für alle Internetzonen blockiert werden. Möglicherweise möchten Sie sicherstellen, dass diese Einstellung auf allen Computern in Ihrer Umgebung durchgesetzt wird, um störende Popupfenster zu blockieren und die Möglichkeit der Installation schädlicher Software und Spyware durch Websites zu verringern. Umgekehrt könnte Ihre Umgebung Anwendungen enthalten, die erfordern, dass Popups funktionieren. In diesem Fall können Sie diese Richtlinie so konfigurieren, dass Popups für Websites innerhalb Ihres Intranets zugelassen werden.
  
##### Internet Explorer\\Internetsystemsteuerung\\Seite "Erweitert"
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung\\Seite "Erweitert"**
  
**Tabelle 4.4: Empfohlene Einstellungen für das Zulassen der Ausführung von Software**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Ausführen oder Installieren von Software zulassen, selbst wenn die Signatur ungültig ist</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
###### Ausführen oder Installieren von Software zulassen, selbst wenn die Signatur ungültig ist
  
Microsoft ActiveX®-Steuerelemente und Dateidownloads verfügen häufig über digitale Signaturen, die sowohl für die Integrität der Datei als auch die Identität des Signaturgebers (Erstellers) der Software bürgen. Mit solchen Signaturen wird sichergestellt, dass Software unverändert heruntergeladen wird und dass Sie den Signaturgeber eindeutig identifizieren können. So können Sie entscheiden, ob Sie genügend Vertrauen in die Software haben, um sie auszuführen.
  
Durch die Einstellung **Ausführen oder Installieren von Software zulassen, selbst wenn die Signatur ungültig ist** wird festgelegt, ob heruntergeladene Software durch Benutzer installiert oder ausgeführt werden kann, selbst wenn die Signatur ungültig ist. Eine ungültige Signatur könnte bedeuten, dass die Datei verfälscht wurde. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer aufgefordert, Dateien mit einer ungültigen Signatur zu installieren oder auszuführen. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer Dateien mit einer ungültigen Signatur nicht ausführen oder installieren.
  
Da nicht signierte Software eine Sicherheitsanfälligkeit verursachen kann, ist diese Richtlinieneinstellung für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Hinweis**: Einige zugelassene Softwareprogramme und Steuerelemente können eine ungültige Signatur haben und dennoch in Ordnung sein. Solche Software sollte sorgfältig in einer isolierten Umgebung geprüft werden, bevor Sie deren Verwendung im Netzwerk Ihrer Organisation zulassen.
  
##### Internet Explorer\\Sicherheitsfunktionen\\MK-Protokoll-Sicherheitsbeschränkung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Sicherheitsfunktionen\\MK-Protokoll-Sicherheitsbeschränkung**
  
**Tabelle 4.5: Empfohlene Einstellungen für das MK-Protokoll**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (MK-Protokoll)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (MK-Protokoll)
  
Durch diese Richtlinieneinstellung wird die Angriffsfläche verringert, weil das selten verwendete MK-Protokoll blockiert wird. Einige ältere Webanwendungen rufen mithilfe des MK-Protokolls Informationen aus komprimierten Dateien ab. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, wird das MK-Protokoll für Windows Explorer und Internet Explorer blockiert. Ressourcen, die das MK-Protokoll verwenden, können dann nicht ausgeführt werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Anwendungen die MK-Protokoll-API verwenden.
  
Da das MK-Protokoll selten verwendet wird, sollte es blockiert werden, sofern es nicht erforderlich ist. Für die beiden in diesem Kapitel behandelten Umgebungen ist diese Richtlinieneinstellung auf **Aktiviert** gesetzt. Microsoft empfiehlt, das MK-Protokoll zu blockieren, sofern es nicht wirklich in Ihrer Umgebung benötigt wird.
  
**Hinweis**: Wenn Sie diese Einstellung vornehmen, können Ressourcen, die das MK-Protokoll verwenden, nicht ausgeführt werden. Daher sollten Sie sicherstellen, dass keine Ihrer Anwendungen das MK-Protokoll verwendet.
  
##### Internet Explorer\\Sicherheitsfunktionen\\Konsistente MIME-Verarbeitung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Sicherheitsfunktionen\\Konsistente MIME-Verarbeitung**
  
**Tabelle 4.6: Empfohlene Einstellungen für die konsistente MIME-Verarbeitung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Konsistente MIME-Verarbeitung)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (Konsistente MIME-Verarbeitung)
  
Internet Explorer verwendet MIME-Daten (Multipurpose Internet Mail Extensions), um Vorgehensweisen für die Verarbeitung von Dateien zu ermitteln, die über einen Webserver empfangen werden. Durch die Einstellung **Konsistente Mime-Verarbeitung** wird festgelegt, ob Internet Explorer erfordert, dass alle von Webservern bereitgestellten Dateitypinformationen konsistent sind. Der MIME-Typ einer Datei ist z. B. Text/Klartext. Die MIME-Daten zeigen jedoch an, dass es sich um eine ausführbare Datei handelt. Daraufhin ändert Internet Explorer seine Erweiterung, um die Ausführbarkeit widerzuspiegeln. Durch diese Möglichkeit wird sichergestellt, dass sich ausführbarer Code nicht als anderer, vertrauenswürdiger Datentyp ausgeben kann.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, untersucht Internet Explorer alle empfangenen Dateien und setzt eine konsistente MIME-Verarbeitung durch. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, erfordert Internet Explorer für keine der empfangenen Dateien konsistente MIME-Daten und verwendet die von der Datei bereitgestellten MIME-Daten.
  
Die Nachahmung von MIME-Dateitypen stellt eine potenzielle Bedrohung für Ihre Organisation dar. Sie sollten sicherstellen, dass diese Dateien konsistent und korrekt bezeichnet sind, um zu verhindern, dass schädliche Dateidownloads Ihr Netzwerk infizieren. Für die beiden in diesem Kapitel behandelten Umgebungen ist diese Richtlinieneinstellung auf **Aktiviert** gesetzt.
  
**Hinweis**: Diese Richtlinieneinstellung steht mit den Einstellungen für **Sicherheitsfunktion für MIME-Sniffing** in Verbindung, ohne diese jedoch zu ersetzen.
  
##### Internet Explorer\\Sicherheitsfunktionen\\Sicherheitsfunktion für MIME-Sniffing
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Sicherheitsfunktionen\\Sicherheitsfunktion für MIME-Sniffing**
  
**Tabelle 4.7: Empfohlene Einstellungen für MIME-Sniffing**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (MIME-Sniffing)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (MIME-Sniffing)
  
Beim MIME-Sniffing wird der Inhalt einer MIME-Datei untersucht, um deren Kontext zu ermitteln, also ob es sich um eine Datendatei, eine ausführbare Datei oder eine andere Art von Datei handelt. Durch diese Richtlinieneinstellung wird festgelegt, ob MIME-Sniffing in Internet Explorer verhindert, dass eine Datei eines Typs zu einem gefährlicheren Dateityp heraufgestuft wird. Wenn MIME-Sniffing auf **Aktiviert** gesetzt ist, wird eine Datei eines Typs nie zu einem gefährlicheren Dateityp heraufgestuft. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Internet Explorer-Prozesse so konfiguriert, dass sie MIME-Sniffing zulassen, durch das eine Datei eines bestimmten Typs zu einem gefährlicheren Dateityp heraufgestuft wird. Eine Textdatei kann z. B. zu einer ausführbaren Datei heraufgestuft werden. Dies ist gefährlich, da sämtlicher Code in der vermeintlichen Textdatei ausgeführt werden würde.
  
Die Nachahmung von MIME-Dateitypen ist eine potenzielle Bedrohung für Ihre Organisation. Microsoft empfiehlt, diese Dateien konsistent zu behandeln. Dadurch wird verhindert, dass schädliche Dateidownloads Ihr Netzwerk infizieren.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (MIME-Sniffing)** auf **Aktiviert** gesetzt.
  
**Hinweis**: Diese Richtlinieneinstellung steht mit den Einstellungen für **Konsistente MIME-Verarbeitung** in Verbindung, ohne diese jedoch zu ersetzen.
  
##### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Skriptgestützte Sicherheitsbeschränkungen in Windows
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Skriptgestützte Sicherheitsbeschränkungen in Windows**
  
**Tabelle 4.8: Empfohlene skriptgestützte Sicherheitsbeschränkungen in Windows**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Skriptgestützte Sicherheitsbeschränkungen in Windows)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (Skriptgestützte Sicherheitsbeschränkungen in Windows)
  
Internet Explorer ermöglicht Skripts, verschiedene Arten von Fenstern per Programm zu öffnen, in der Größe anzupassen und neu zu positionieren. Anrüchige Websites passen häufig die Größe von Fenstern an, um andere Fenster zu verstecken oder um Sie dazu zu veranlassen, mit einem Fenster zu interagieren, das schädlichen Code enthält.
  
Durch die Einstellung **Internet Explorer-Prozesse** **(Skriptgestützte Sicherheitsbeschränkungen in Windows)** werden Popupfenster eingeschränkt, und es wird verhindert, dass Skripts Fenster anzeigen, deren Titel- und Statusleisten für den Benutzer nicht sichtbar sind oder die die Titel- und Statusleisten anderer Fenster ausblenden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden in Windows  Explorer- und Internet Explorer-Prozessen keine Popupfenster angezeigt. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, können Skripts weiterhin Popupfenster sowie Fenster, die andere Fenster verbergen, erstellen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse** **(Skriptgestützte Sicherheitsbeschränkungen in Windows)** auf **Aktiviert** gesetzt. Wenn diese Richtlinieneinstellung aktiviert ist, wird es schädlichen Websites erschwert, Ihre Internet Explorer-Fenster zu steuern oder Benutzer dazu zu verleiten, in das falsche Fenster zu klicken.
  
##### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Schutz vor Zonenerhöhung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Schutz vor Zonenerhöhung**
  
**Tabelle 4.9: Empfohlene Einstellungen für den Schutz vor Zonenerhöhungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Zonenerhöhungsschutz)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (Zonenerhöhungsschutz)
  
Internet Explorer versieht jede Webseite, die geöffnet wird, mit Einschränkungen. Diese Einschränkungen hängen vom Standort der Webseite ab, z. B. Internetzone, Intranetzone oder Lokale Zone. Webseiten auf einem lokalen Computer haben die wenigsten Sicherheitsbeschränkungen und befinden sich in der Zone des lokalen Computers. Dadurch wird die Sicherheitszone des lokalen Computers zum vorrangigen Ziel für Angreifer.
  
Wenn Sie die Einstellung **Internet Explorer-Prozesse (Zonenerhöhungsschutz)** aktivieren, kann jede Zone vor einer Zonenanhebung durch Internet Explorer-Prozesse geschützt werden. Durch diese Vorgehensweise wird verhindert, dass in einer Zone ausgeführter Inhalt die erhöhten Berechtigungen einer anderen Zone erlangt. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird keine Zone gegenüber Internet Explorer-Prozessen geschützt.
  
Aufgrund des Schweregrads und der relativen Häufigkeit von Zonenerhöhungsangriffen ist die Einstellung **Internet Explorer-Prozesse (Zonenerhöhungsschutz)** für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Installation von ActiveX beschränken
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Installation von ActiveX beschränken**
  
**Tabelle 4.10: Einstellungen für das Beschränken der Installation von ActiveX**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Installation von ActiveX beschränken)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (Installation von ActiveX beschränken)
  
Diese Richtlinieneinstellung bietet die Möglichkeit, Installationsaufforderungen von ActiveX-Steuerelementen für Internet Explorer-Prozesse zu blockieren. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Aufforderungen zum Installieren von ActiveX-Steuerelementen für Internet Explorer-Prozesse blockiert. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Aufforderungen zum Installieren von ActiveX-Steuerelementen für Internet Explorer-Prozesse nicht blockiert, sondern den Benutzern angezeigt.
  
Benutzer installieren häufig Software wie z. B. ActiveX-Steuerelemente, die von den Sicherheitsrichtlinien ihrer Organisation nicht zugelassen sind. Solche Software kann für Netzwerke ein beträchtliches Sicherheits- und Datenschutzrisiko darstellen. Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (Installation von ActiveX beschränken)** deshalb auf **Aktiviert** gesetzt.
  
**Hinweis**: Durch diese Einstellung werden Benutzer außerdem daran gehindert, autorisierte, legitime ActiveX-Steuerelemente zu installieren, die wichtige Systemkomponenten wie Windows Update stören. Wenn Sie diese Richtlinieneinstellung aktivieren, sollten Sie eine alternative Methode zum Bereitstellen von Sicherheitsupdates wie z. B. Windows Server Update Services (WSUS) implementieren.  
Weitere Informationen zu WSUS finden Sie auf der Seite [Windows Server Update Services – Produktüberblick](http://www.microsoft.com/windowsserversystem/updateservices/evaluation/overview.mspx) (in englischer Sprache) unter www.microsoft.com/windowsserversystem/updateservices/evaluation/overview.mspx.  
Weitere Informationen zu Windows Update finden Sie auf der Seite [Windows Update](http://windowsupdate.microsoft.com/) unter http://windowsupdate.microsoft.com.
  
##### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Dateidownload beschränken
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Dateidownload beschränken**
  
**Tabelle 4.11: Empfohlene Einstellungen für das Beschränken von Dateidownloads**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Dateidownload beschränken)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Internet Explorer-Prozesse (Dateidownload beschränken)
  
Unter bestimmten Umständen können Websites ohne Benutzereingriff Aufforderungen zum Herunterladen von Dateien einleiten. Dieses Verfahren kann Websites ermöglichen, nicht autorisierte Dateien auf den Festplatten von Benutzern zu speichern, wenn sie auf die falsche Schaltfläche klicken und den Download akzeptieren.
  
Wenn Sie die Richtlinieneinstellung **Internet Explorer-Prozesse (Dateidownload beschränken)** auf **Aktiviert** setzen, werden nicht vom Benutzer initiierte Aufforderungen zum Herunterladen von Dateien für Internet Explorer-Prozesse blockiert. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, können ohne Zustimmung des Benutzers Dateidownloads für Internet Explorer-Prozesse initiiert werden.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (Dateidownload beschränken)** auf **Aktiviert** gesetzt, um Angreifer davon abzuhalten, beliebigen Code auf den Computern von Benutzern abzulegen.
  
##### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung**
  
**Tabelle 4.12: Einstellungen für die Add-On-Verwaltung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Add-On-Liste</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
</tbody>
</table>
  
###### Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind
  
Diese Richtlinieneinstellung ermöglicht Ihnen zusammen mit der Richtlinie **Add-On-Liste**, Internet Explorer-Add-Ons zu steuern. Standardmäßig ist in der Einstellung für die **Add-On-Liste** eine Liste von Add-Ons festgelegt, die durch eine Gruppenrichtlinie zugelassen oder verweigert werden können. Durch die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** wird sichergestellt, dass alle Add-Ons verweigert werden, es sei denn, sie sind ausdrücklich in der Einstellung **Add-On-Liste** aufgeführt.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, lässt Internet Explorer nur Add-Ons zu, die explizit in der Richtlinieneinstellung **Add-On-Liste** aufgeführt und zugelassen sind. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer über die Add-On-Verwaltung beliebige Add-Ons zulassen oder verweigern.
  
Sie sollten erwägen, sowohl die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** als auch die **Add-On-Liste** zu verwenden, um zu steuern, welche Add-Ons in Ihrer Umgebung verwendet werden können. Durch diese Vorgehensweise wird sichergestellt, dass nur autorisierte Add-Ons verwendet werden.
  
###### Add-On-Liste
  
Mit dieser Richtlinieneinstellung und der Richtlinie **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** können Sie Internet Explorer-Add-Ons steuern. Standardmäßig ist in der Einstellung für die **Add-On-Liste** eine Liste von Add-Ons festgelegt, die durch eine Gruppenrichtlinie zugelassen oder verweigert werden können. Durch die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** wird sichergestellt, dass alle Add-Ons verweigert werden, es sei denn, sie sind ausdrücklich in der Einstellung **Add-On-Liste** aufgeführt.
  
Wenn Sie die Einstellung **Add-On-Liste** aktivieren, müssen Sie eine Liste von Add-Ons eingeben, die von Internet Explorer zugelassen oder verweigert werden sollen. Die spezifische Liste der Add-Ons, die in dieser Liste enthalten sein sollten, sind je nach Organisation unterschiedlich. Aus diesem Grund wird in diesem Handbuch keine ausführliche Liste bereitgestellt. Für jeden Eintrag, den Sie der Liste hinzufügen, müssen Sie folgende Informationen bereitstellen:
  
-   **Name des Wertes**. Die CLSID (Klassen-ID) für das Add-On, das der Liste hinzugefügt werden soll. Die CLSID sollte in Klammern stehen, z. B. {000000000-0000-0000-0000-0000000000000}. Sie erhalten die CLSID für ein Add-On, indem Sie den OBJECT-Tag einer Webseite lesen, die das Add-On enthält.
  
-   **Wert**. Eine Zahl, die anzeigt, ob Internet Explorer das Laden des Add-Ons verweigern oder zulassen soll. Folgende Werte sind gültig:
  
    -   **0**    Dieses Add-On verweigern
  
    -   **1**    Dieses Add-On zulassen
  
    -   **2**    Dieses Add-On zulassen und dem Benutzer erlauben, es mithilfe des Befehls „Add-Ons verwalten“ zu verwalten
  
Wenn Sie die Einstellung **Add-On-Liste** deaktivieren, wird die Liste gelöscht. Sie sollten erwägen, sowohl die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** als auch die **Add-On-Liste** zu verwenden, um zu steuern, welche Add-Ons in Ihrer Umgebung verwendet werden können. Durch diese Vorgehensweise wird sichergestellt, dass nur autorisierte Add-Ons verwendet werden.
  
##### Terminaldienste\\Client/Server-Datenumleitung
  
Durch die Terminaldienste werden Optionen für die Umleitung von Clientressourcen auf Servern bereitgestellt, auf die über die Terminaldienste zugegriffen wird. Die folgende Einstellung gilt speziell für die Terminaldienste.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Terminaldienste\\Client/Server-Datenumleitung**
  
**Tabelle 4.13: Empfohlene Einstellungen für das Verhindern der Laufwerkumleitung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Laufwerkumleitung nicht zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Laufwerkumleitung nicht zulassen
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die lokalen Laufwerke auf ihren Clientcomputern für Terminalserver freigeben, auf die sie Zugriff haben. Zugeordnete Laufwerke werden im folgenden Format in der Ordnerstruktur der Sitzung in Windows Explorer oder unter Arbeitsplatz angezeigt:
  
\\\\TSClient\\*&lt;Laufwerkbuchstabe&gt;$*
  
Wenn lokale Laufwerke freigegeben werden, besteht die Möglichkeit, dass sich Eindringlinge unerlaubt Zugang zu den Daten auf diesen Laufwerken verschaffen.
  
Aus diesem Grund ist die Einstellung **Laufwerkumleitung nicht zulassen** in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung jedoch auf **Nicht konfiguriert** gesetzt.
  
##### Terminaldienste\\Verschlüsselung und Sicherheit
  
Die folgenden empfohlenen Einstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Terminaldienste\\Verschlüsselung und Sicherheit**
  
**Tabelle 4.14: Empfohlene Einstellungen für die Verschlüsselung und Sicherheit von Terminaldiensten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Immer Kennworteingabeaufforderung für Clients beim Herstellen von Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verschlüsselungsstufe der Clientverbindung festlegen</td>
<td style="border:1px solid black;">Höchste Stufe</td>
<td style="border:1px solid black;">Höchste Stufe</td>
<td style="border:1px solid black;">Höchste Stufe</td>
<td style="border:1px solid black;">Höchste Stufe</td>
</tr>
</tbody>
</table>
  
###### Immer Kennworteingabeaufforderung für Clients beim Herstellen von Verbindungen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Clientcomputer von Terminaldiensten beim Herstellen der Verbindung stets zur Eingabe eines Kennworts aufgefordert wird. Mithilfe dieser Richtlinieneinstellung können sie für Benutzer, die sich bei Terminaldiensten anmelden, eine Aufforderung zur Kennworteingabe erzwingen, auch wenn die Benutzer das Kennwort bereits im Remotedesktopverbindungsclient eingegeben haben. Die Terminaldienste gestatten den Benutzern standardmäßig die automatische Anmeldung, wenn diese ihr Kennwort im Remotedesktopverbindungsclient eingeben.
  
Für die Hochsicherheitsumgebung ist die Einstellung **Immer Kennworteingabeaufforderung für Clients beim Herstellen von Verbindungen** auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung jedoch auf **Nicht konfiguriert** gesetzt.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, kann der lokale Computeradministrator mit dem Terminaldienste-Konfigurationsprogramm festlegen, ob Kennwörter automatisch gesendet werden dürfen oder nicht.
  
###### Verschlüsselungsstufe der Clientverbindung festlegen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Computer, der die Remoteverbindung soll, für alle zwischen dem Client und dem Remotecomputer gesendeten Daten eine Verschlüsselungsstufe erzwingt.
  
Die Verschlüsselungsstufe ist auf **Höchste Stufe** gesetzt, um für die beiden in diesem Kapitel behandelten Umgebungen eine 128-Bit-Verschlüsselung zu erzwingen.
  
##### Terminaldienste\\Client
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Windows-Komponenten\\Terminaldienste\\Client**
  
**Tabelle 4.15: Empfohlene Einstellungen für das Verhindern der Speicherung von Kennwörtern**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Speichern von Kennwörtern nicht zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Speichern von Kennwörtern nicht zulassen
  
Durch diese Richtlinieneinstellung wird verhindert, dass Kennwörter von Terminaldienstclients auf einem Computer gespeichert werden. Wenn Sie diese Richtlinieneinstellung aktivieren, wird das Kontrollkästchen zum Speichern von Kennwörtern in Terminaldienstclients deaktiviert. Benutzer sind dann nicht mehr in der Lage, Kennwörter zu speichern.
  
Da gespeicherte Kennwörter zusätzliche Gefährdungen verursachen können, ist die Einstellung **Speichern von Kennwörtern nicht zulassen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis**: Wenn diese Einstellung zuvor auf **Deaktiviert** bzw. **Nicht konfiguriert** gesetzt war, werden alle zuvor gespeicherten Kennwörter gelöscht, wenn ein Terminaldienstclient zum ersten Mal die Verbindung mit einem beliebigen Server beendet.
  
##### Windows Messenger
  
Mit Windows Messenger können Sofortnachrichten an andere Benutzer in einem Computernetzwerk gesendet werden. Den Nachrichten können Dateien und andere Anlagen hinzugefügt werden.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Windows Messenger**
  
**Tabelle 4.16: Empfohlene Einstellungen für Windows Messenger**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Ausführung von Windows Messenger nicht zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Ausführung von Windows Messenger nicht zulassen
  
Sie können die Einstellung **Ausführung von Windows Messenger nicht zulassen** aktivieren, um Windows Messenger zu deaktivieren und zu verhindern, dass das Programm ausgeführt wird. Da diese Anwendung für böswillige Absichten wie z. B. das Versenden von Spam, die Verbreitung schädlicher Software und die Offenlegung vertraulicher Daten verwendet werden kann, empfiehlt Microsoft, die Einstellung **Ausführung von Windows Messenger nicht zulassen** sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** zu setzen.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, werden auch die Verwendung von Windows Messenger durch die Remoteunterstützung und das Aufrufen von MSN® Messenger durch Benutzer verhindert.
  
##### Windows Update
  
Administratoren können über die Einstellungen von Windows Update festlegen, wie Patches und Hotfixes auf Windows XP-Arbeitsstationen angewendet werden. Updates sind auf der Website von Microsoft Windows Update verfügbar. Wahlweise kann eine Intranetwebsite eingerichtet werden, die eine bessere administrative Kontrolle bei der Bereitstellung von Patches und Hotfixes ermöglicht. Die Vorlage WUAU.adm (Windows Update Administrative Template, Administrative Vorlage für Windows Update) wurde mit Windows XP Service Pack 1 (SP1) eingeführt.
  
Windows Server Update Services (WSUS) ist ein Dienst der Infrastruktur, der auf den erfolgreichen Technologien von Microsoft Windows Update und Software Update Services (SUS) aufbaut. WSUS verwaltet und verteilt wichtige Windows-Patches zur Behebung bekannter Sicherheitsanfälligkeiten und anderer Stabilitätsprobleme in Betriebsystemen von Microsoft Windows.
  
WSUS macht manuelle Aktualisierungsschritte unnötig. Ein dynamisches Benachrichtigungssystem informiert alle Windows-Clientcomputer über wichtige Updates und stellt diese auf dem Intranetserver bereit. Die Clients müssen keine Internetverbindung aufbauen, um diesen Dienst nutzen zu können. Außerdem wird mit dieser Technologie eine einfache Lösung für die automatische Verteilung von Updates auf Ihren Windows-Arbeitsstationen und -Servern bereitgestellt.
  
Darüber hinaus bietet WSUS folgende Funktionen:
  
-   **Verwaltung und Steuerung der Inhaltssynchronisierung innerhalb des Intranets durch den Administrator**. Bei diesem Synchronisierungsdienst handelt es sich um eine Komponente auf dem Server, die die neuesten und wichtigsten Updates von Windows Update abruft. Wenn neue Updates auf Windows Update gefunden werden, lädt der Server, der WSUS ausführt, diese nach einem vom Administrator definierten Zeitplan automatisch herunter und speichert sie.
  
-   **Verwaltung eines Windows Update-Servers innerhalb des Intranets**. Dieser einfach zu verwaltende Server dient als virtueller Windows Update-Server für Clientcomputer. Er verfügt über einen Synchronisierungsdienst und über Programme für die Verwaltung der Updates. Er verarbeitet Anfragen auf genehmigte Updates, die von den Clientcomputern ausgegeben werden, die über das HTTP-Protokoll mit dem Server verbunden sind. Dieser Server kann auch wichtige Updates hosten, die vom Synchronisierungsdienst heruntergeladen wurden, und kann die Clientcomputer über diese Updates informieren.
  
-   **Kontrolle der Updates durch den Administrator**. Der Administrator kann die über die öffentliche Website von Windows Update bereitgestellten Updates vor der Verteilung im Intranet der Organisation prüfen und genehmigen. Die Verteilung erfolgt nach einem vom Administrator erstellten Zeitplan. Wenn WSUS auf mehreren Servern ausgeführt wird, legt der Administrator fest, welche Computer auf bestimmte Server zugreifen, auf denen der Dienst ausgeführt wird. Administratoren können die genannten Verwaltungsmöglichkeiten über Gruppenrichtlinien in einem Active Directory®-Verzeichnisdienst oder über Registrierungsschlüssel konfigurieren.
  
-   **Automatische Updates auf den Computern (Arbeitsstationen oder Server)**. Die Windows-Funktion „Automatische Updates“ ermöglicht es, automatisch prüfen zu lassen, ob bei Windows Update neu veröffentlichte Updates verfügbar sind. WSUS verwendet diese Windows-Funktion für die Veröffentlichung aller vom Administrator genehmigten Updates in einem Intranet.
  
    **Hinweis**: Wenn Patches durch eine andere Methode verteilt werden sollen, wie z. B. Microsoft Systems Management Server, wird empfohlen, die Einstellung **Automatische Updates konfigurieren** zu deaktivieren.
  
Es gibt mehrere Einstellungen für Windows Update. Es sind mindestens drei Einstellungen erforderlich, damit Windows Update funktioniert: **Automatische Updates konfigurieren**, **Kein automatischer Neustart für geplante Installationen automatischer Updates** und **Geplante Installationen automatischer Updates erneut planen**. Eine vierte Einstellung ist optional und hängt von den Anforderungen Ihrer Organisation ab: **Internen Pfad für den Microsoft Updatedienst angeben**.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Windows Messenger**
  
Die in diesem Abschnitt beschriebenen Einstellungen stehen nicht explizit in Zusammenhang mit bestimmten Sicherheitsrisiken. Sie dienen hauptsächlich einer Anpassung der Umgebung an die vom Administrator festgelegten Konfigurationsvorgaben. Ungeachtet dessen ist die Konfiguration von Windows Update unerlässlich, da die Sicherheit der Umgebung nur gewährleistet ist, wenn die Clientcomputer möglichst bald nach der Bereitstellung neuer Sicherheitspatches durch Microsoft entsprechend aktualisiert werden.
  
**Hinweis**: Windows Update ist abhängig von mehreren Diensten, zu denen auch der Remoteregistrierungsdienst und der Intelligente Hintergrundübertragungsdienst gehören. In Kapitel 3, „Sicherheitseinstellungen für Windows XP-Clients“, werden diese Dienste in der Hochsicherheitsumgebung deaktiviert. Windows Update kann daher bei einer Deaktivierung dieser Dienste nicht in der Hochsicherheitsumgebung ausgeführt werden, und die vier folgenden Einstellungen können für diese spezielle Umgebung ignoriert werden.
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für Windows Update zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.17: Empfohlene Einstellungen für Windows Update**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Option 'Updates installieren und herunterfahren' im Dialogfeld &quot;Windows herunterfahren&quot; nicht anzeigen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Standardoption 'Updates installieren und herunterfahren' im Dialogfeld &quot;Windows herunterfahren&quot; nicht anpassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Automatische Updates konfigurieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kein automatischer Neustart für geplante Installationen automatischer Updates</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Geplante Installationen automatischer Updates erneut planen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internen Pfad für den Microsoft Updatedienst angeben</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Option 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anzeigen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob im Dialogfeld **Windows herunterfahren** die Option **Updates installieren und herunterfahren** angezeigt wird. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird die Option **Updates installieren und herunterfahren** im Dialogfeld **Windows herunterfahren** verfügbar. Dies gilt für den Fall, dass Updates zur Verfügung stehen, wenn der Benutzer im Menü **Start** die Option **Herunterfahren** auswählt oder in dem Fenster, das nach Betätigen der Tasten STRG+ALT+ENTF angezeigt wird, auf die Schaltfläche **Herunterfahren** klickt.
  
Da Updates für die Gesamtsicherheit aller Computer wichtig sind, ist die Einstellung **Option 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anzeigen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt. Diese Einstellung steht mit der Einstellung **Standardoption 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anpassen** in Verbindung.
  
###### Standardoption 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anpassen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Option **Updates installieren und herunterfahren** als Standardwahl im Dialogfeld **Windows herunterfahren** zugelassen wird. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird die Option **Updates installieren und herunterfahren** zur Standardoption im Dialogfeld **Windows herunterfahren**, wenn zu dem Zeitpunkt, zu dem der Benutzer im Menü **Start** die Option **Herunterfahren** auswählt, Updates zur Installation zur Verfügung stehen.
  
Da Updates für die Gesamtsicherheit aller Computer wichtig sind, ist die Einstellung **Standardoption 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anpassen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Hinweis**: Diese Richtlinieneinstellung hat keine Auswirkungen, wenn die Option **Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Windows Update\\Option 'Updates installieren und herunterfahren' im Dialogfeld "Windows herunterfahren" nicht anzeigen** auf **Aktiviert** gesetzt ist.
  
###### Automatische Updates konfigurieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Computer in Ihrer Umgebung Sicherheitsupdates von Windows Update oder WSUS empfangen sollen. Bei Auswahl der Option **Aktiviert** für diese Richtlinieneinstellung kann das Betriebssystem feststellen, wann eine Netzwerkverbindung verfügbar ist, und anschließend über diese Verbindung die Website von Windows Update oder die ausgewiesene Intranetsite auf relevante Updates überprüfen.
  
Wählen Sie, nachdem Sie diese Richtlinieneinstellung auf **Aktiviert** gesetzt haben, im Dialogfeld **Eigenschaften von Automatische Updates konfigurieren** eine der drei folgenden Optionen für die Funktionsweise des Dienstes aus:
  
1.  **Vor dem Download von Updates benachrichtigen und vor deren Installation erneut benachrichtigen**
  
2.  **Updates automatisch downloaden und über installierbare Updates benachrichtigen. (Standardeinstellung)**
  
3.  **Updates automatisch downloaden und laut angegebenem Zeitplan installieren.**
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, müssen alle verfügbaren Updates von der Website [Windows Update](http://windowsupdate.microsoft.com/) (http://windowsupdate.microsoft.com) manuell heruntergeladen und installiert werden.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Automatische Updates konfigurieren** auf **Aktiviert** gesetzt.
  
###### Kein automatischer Neustart für geplante Installationen automatischer Updates
  
Wenn diese Richtlinieneinstellung aktiviert ist, muss der Computer von einem angemeldeten Benutzer neu gestartet werden, um eine geplante Installation abzuschließen. Durch Aktivierung dieser Richtlinieneinstellung wird auch verhindert, dass Automatische Updates den Computer während einer geplanten Installation automatisch neu startet. Wenn ein Benutzer zu der Zeit an einem Computer angemeldet ist, zu der Automatische Updates einen Neustart erfordert, um die Installation eines Updates abzuschließen, wird der Benutzer darauf hingewiesen. Der Benutzer kann den Neustart dann verschieben. Beachten Sie, dass Automatische Updates bis zum erforderlichen Neustart keine weiteren Updates erkennt.
  
Wenn die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Deaktiviert** oder **Nicht konfiguriert** gesetzt ist, benachrichtigt Automatische Updates den Benutzer, dass der Computer für den Abschluss einer Installation in 5 Minuten automatisch neu gestartet wird. Wenn automatische Neustarts ein Problem darstellen, können Sie die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Aktiviert** setzen. Um den Abschluss durchgeführter Installationen sicherzustellen, richten Sie Ihre Clientcomputer so ein, dass sie nach Ende der normalen Geschäftszeiten automatisch neu gestartet werden, wenn Sie diese Richtlinieneinstellung aktivieren.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Deaktiviert** gesetzt.
  
**Hinweis**: Diese Einstellung ist nur wirksam, wenn Automatische Updates für die Durchführung automatischer Updateinstallationen konfiguriert ist. Wenn die Einstellung **Automatische Updates konfigurieren** auf **Deaktiviert** gesetzt ist, hat sie keine Auswirkungen. Die meisten Updates erfordern nach der Installation einen Neustart.
  
###### Geplante Installationen automatischer Updates erneut planen
  
Durch diese Richtlinieneinstellung wird festgelegt, wie lange nach dem Systemstart gewartet wird, bevor geplante automatische Updateinstallationen fortgesetzt werden. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, wird eine zuvor geplante Installation nach Ablauf einer gewissen Zeit (in Minuten) nach dem Start des Computers durchgeführt. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** oder **Nicht konfiguriert** setzen, werden zuvor geplante Installationen erst zum nächsten regulär geplanten Installationszeitpunkt durchgeführt.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Geplante Installationen automatischer Updates erneut planen** auf **Aktiviert** gesetzt. Nach dem Aktivieren der Richtlinieneinstellung können Sie die standardmäßige Wartezeit entsprechend den Anforderungen in der Umgebung ändern.
  
**Hinweis**: Diese Einstellung ist nur wirksam, wenn Automatische Updates für die Durchführung automatischer Updateinstallationen konfiguriert ist. Wenn die Einstellung **Automatische Updates konfigurieren** auf **Deaktiviert** gesetzt ist, hat die Einstellung **Geplante Installationen automatischer Updates erneut planen** keine Auswirkungen. Sie können die beiden letztgenannten Einstellungen aktivieren, um sicherzustellen, dass zuvor übergangene Installationen bei jedem Neustart des Computers neu angesetzt werden.
  
###### Internen Pfad für den Microsoft Updatedienst angeben
  
Durch diese Richtlinieneinstellung wird ein Intranetserver bestimmt, auf dem Updates von der Microsoft Update-Website gehostet werden. Anschließend kann dieser Updatedienst verwendet werden, um die Computer in Ihrem Netzwerk automatisch zu aktualisieren. Diese Richtlinieneinstellung ermöglicht die Angabe eines WSUS-Servers, der in Ihrem Netzwerk als interner Updatedienst fungieren soll. Der Client für Automatische Updates verwendet den WSUS-Server, um den Dienst auf gültige Updates für die Computer im Netzwerk zu überprüfen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Internen Pfad für den Microsoft Updatedienst angeben** auf **Aktiviert** gesetzt.
  
**Hinweis**: Das Aktivieren der Einstellung **Internen Pfad für den Microsoft Updatedienst angeben** hat keine Auswirkungen, wenn die Einstellung **Automatische Updates konfigurieren** deaktiviert ist.
  
#### System
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System**
  
Die folgende Abbildung illustriert die Abschnitte in der Gruppenrichtlinie, die von den Einstellungsänderungen in diesem Abschnitt betroffen sein werden:
  
![](images/Cc163076.SGFG0403(de-de,TechNet.10).gif)
  
**Abbildung 4.3: Gruppenrichtlinienstruktur für das System in der Computerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0403_big(de-de,technet.10).gif)
  
In der folgenden Tabelle sind die empfohlenen Systemeinstellungen zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.18: Empfohlene Systemeinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Autoplay deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert –<br />
Alle Laufwerke</td>
<td style="border:1px solid black;">Aktiviert –<br />
Alle Laufwerke</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Suchbefehl für Gerätetreiber in Windows Update deaktivieren</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
##### Autoplay deaktivieren
  
Autoplay sorgt dafür, dass der Lesevorgang von einem Laufwerk unmittelbar nach dem Einlegen eines Mediums gestartet wird. Auf dem Medium gespeicherte Setupdateien oder Audiodaten werden dann automatisch ausgeführt bzw. abgespielt. Ein Angreifer kann diese Funktion ausnutzen, um ein Programm zu starten, das einen Computer oder die Daten auf dem Computer beschädigen könnte. Sie können die Einstellung **Autoplay deaktivieren** aktivieren, um die Autoplay-Funktion zu deaktivieren. Autoplay ist bei austauschbaren Datenträgern, wie z. B. Disketten- oder Netzlaufwerken, bereits in der Standardeinstellung deaktiviert, aber nicht bei CD-ROM-Laufwerken.
  
Für die Hochsicherheitsumgebung ist die Einstellung **Autoplay deaktivieren** auf **Aktiviert – Alle Laufwerke** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung jedoch auf **Nicht konfiguriert** gesetzt.
  
**Hinweis**: Sie können diese Einstellung nicht verwenden, um Autoplay für Computerlaufwerke zu aktivieren, bei denen diese Funktion in der Standardeinstellung deaktiviert ist, z. B. bei Disketten- oder Netzlaufwerken.
  
##### Suchbefehl für Gerätetreiber in Windows Update deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Administrator aufgefordert wird, über das Internet in Windows Update nach Gerätetreibern zu suchen. Wenn diese Richtlinieneinstellung **Aktiviert** ist, werden Administratoren nicht aufgefordert, Windows Update zu durchsuchen. Wenn sowohl diese Richtlinieneinstellung als auch **Gerätetreibersuche in Windows Update deaktivieren** auf **Deaktiviert** oder **Nicht konfiguriert** gesetzt ist, wird der Administrator zur Bestätigung aufgefordert, bevor Windows Update nach Gerätetreibern durchsucht wird.
  
Das Herunterladen von Gerätetreibern aus dem Internet birgt gewisse Risiken. Deshalb wird empfohlen, die Einstellung **Suchbefehl für Gerätetreiber in Windows Update deaktivieren** für Hochsicherheitsumgebungen auf **Aktiviert** und für Unternehmensclient-Umgebungen auf **Deaktiviert** zu setzen. Der Grund für diese Empfehlung ist, dass den Angriffsarten, die einen Treiberdownload ausnutzen, in der Regel durch eine korrekte Verwaltung von Unternehmensanwendungen begegnet werden kann.
  
**Hinweis**: Diese Richtlinieneinstellung ist nur dann wirksam, wenn **Gerätetreibersuche in Windows Update deaktivieren** in **Administrative Vorlagen/System/Internetkommunikationsverwaltung/Internetkommunikation** auf **Deaktiviert** oder **Nicht konfiguriert** gesetzt ist.
  
##### Anmeldung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Anmeldung**
  
In der folgenden Tabelle sind die empfohlenen Anmeldeeinstellungen zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.19: Empfohlene Anmeldeeinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Herkömmliche Ausführungsliste nicht verarbeiten</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Einmalige Ausführungsliste nicht verarbeiten</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Herkömmliche Ausführungsliste nicht verarbeiten
  
Durch diese Richtlinieneinstellung wird festgelegt, dass die Ausführungsliste mit allen beim Start von Windows XP automatisch auszuführenden Programmen ignoriert werden soll. Die benutzerdefinierten Ausführungslisten für Windows XP werden in der Registrierung in folgenden Verzeichnissen gespeichert:
  
-   **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\Run**
  
-   **HKEY\_CURRENT\_USER\\Software\\Microsoft\\Windows\\CurrentVersion\\Run**
  
Durch Aktivieren der Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten** wird verhindert, dass ein böswilliger Benutzer bei jedem Start von Windows XP ein Programm ausführen lässt, durch das Daten beeinträchtigt oder in anderer Weise Schaden angerichtet wird. Wenn diese Richtlinieneinstellung aktiviert ist, wird die Ausführung bestimmter Systemprogramme verhindert, z. B. die Ausführung von Antivirensoftware oder von Programmen für Softwareverteilung und -überwachung. Microsoft empfiehlt, das Bedrohungsniveau Ihrer Umgebung abzuschätzen, bevor Sie entscheiden, diese Richtlinieneinstellung für Ihre Organisation zu verwenden.
  
Die Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert** und für die Hochsicherheitsumgebung **Aktiviert**.
  
###### Einmalige Ausführungsliste nicht verarbeiten
  
Diese Richtlinieneinstellung sorgt dafür, dass die einmalige Ausführungsliste mit allen beim Start von Windows XP automatisch auszuführenden Programmen ignoriert wird. Diese Richtlinieneinstellung unterscheidet sich von der Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten**, da Programme in dieser Liste beim nächsten Neustart des Clientcomputers einmalig ausgeführt werden. Dieser Liste werden z. B. Setup- und Installationsprogramme hinzugefügt, um Installationen nach einem Neustart des Clientcomputers abzuschließen. Wenn Sie diese Richtlinieneinstellung aktivieren, können Angreifer die Liste mit einmalig auszuführenden Programmen nicht missbrauchen, um unzulässige Anwendungen auszuführen, was früher eine beliebte Angriffsmethode war. Ein böswilliger Benutzer kann die einmalige Ausführungsliste missbrauchen, um ein Programm zu installieren, mit dem möglicherweise die Sicherheit von Windows XP-Clientcomputern gefährdet wird.
  
**Hinweis**: Benutzerdefinierte einmalige Ausführungslisten werden in der Registrierung in folgendem Verzeichnis gespeichert: **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\RunOnce**.
  
Die Einstellung **Einmalige Ausführungsliste nicht verarbeiten** sollte für die Benutzer in Ihrer Umgebung lediglich einen minimalen Funktionalitätsverlust verursachen, insbesondere wenn die Clientcomputer mit der gesamten Standardsoftware Ihrer Organisation konfiguriert wurden, bevor diese Richtlinieneinstellung durch Gruppenrichtlinien angewendet wird.
  
Die Einstellung **Einmalige Ausführungsliste nicht verarbeiten** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert** und für die Hochsicherheitsumgebung **Aktiviert**.
  
##### Gruppenrichtlinien
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Gruppenrichtlinie**
  
**Tabelle 4.20: Empfohlene Gruppenrichtlinieneinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Registrierungsrichtlinienverarbeitung</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Registrierungsrichtlinienverarbeitung
  
Durch diese Richtlinieneinstellung wird festgelegt, wann Registrierungsrichtlinien aktualisiert werden. Sie betrifft alle Richtlinien im Ordner „Administrative Vorlagen“ sowie alle Richtlinien, mit denen Werte in der Registrierung gespeichert werden. Wenn diese Richtlinieneinstellung aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Während regelmäßiger Hintergrundverarbeitung nicht übernehmen**
  
-   **Gruppenrichtlinienobjekte auch ohne Änderungen bearbeiten**
  
Einige der in den administrativen Vorlagen konfigurierten Einstellungen werden in der Registrierung in Bereichen gespeichert, auf die Benutzer Zugriff haben. Änderungen von Benutzern an diesen Einstellungen werden überschrieben, wenn diese Richtlinieneinstellung aktiviert wird.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Registrierungsrichtlinienverarbeitung** auf **Aktiviert** gesetzt.
  
##### Remoteunterstützung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Remoteunterstützung**
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für die Remoteunterstützung zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.21: Empfohlene Einstellungen für die Remoteunterstützung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Remoteunterstützung anbieten</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Angeforderte Remoteunterstützung</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
###### Remoteunterstützung anbieten
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Supportmitarbeiter oder ein versierter IT-Administrator Remoteunterstützung für Computer in Ihrer Umgebung anbieten kann, ohne dass ein Benutzer zuvor explizit Unterstützung über Kanäle, E-Mail oder Instant Messenger angefordert hat.
  
**Hinweis**: Spezialisten können nicht unangekündigt eine Verbindung zum Computer herstellen oder diesen ohne Erlaubnis des Benutzers steuern. Wenn ein Verbindungsversuch erfolgt, kann der Benutzer die Verbindung immer noch verweigern (und damit dem Spezialisten nur Anzeigeberechtigungen gewähren). Der Benutzer muss auf die Schaltfläche **Ja** klicken, um die Remotesteuerung der Arbeitsstation zuzulassen, wenn für die Einstellung **Remoteunterstützung anbieten** die Option **Aktiviert** angegeben wurde.
  
Wenn diese Richtlinieneinstellung aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Helfer dürfen den Computer nur ansehen**
  
-   **Helfer dürfen den Computer remote steuern**
  
Beim Konfigurieren dieser Richtlinieneinstellung können Sie eine Liste mit Benutzern oder Benutzergruppen angeben, die als „Helfer“ Remoteunterstützung anbieten können.
  
**So konfigurieren Sie die Liste der Helfer**
  
1.  Klicken Sie im Einstellungsfenster **Remoteunterstützung anbieten** auf **Anzeigen**. Im daraufhin geöffneten neuen Fenster können Sie die Namen der Helfer eingeben.
  
2.  Verwenden Sie beim Hinzufügen von Benutzern oder Gruppen zur Liste **Helfer** eines der folgenden Formate:
  
    -   *&lt;Domänenname&gt;*\\*&lt;Benutzername&gt;*
  
    -   *&lt;Domänenname&gt;*\\*&lt;Gruppenname&gt;*
  
Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können Benutzer oder Gruppen Computerbenutzern in Ihrer Umgebung keine unerwünschte Remoteunterstützung anbieten.
  
Die Einstellung **Remoteunterstützung anbieten** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Deaktiviert** gesetzt, um den Zugriff auf Windows XP-Clientcomputer über das Netzwerk zu verhindern.
  
###### Angeforderte Remoteunterstützung
  
Durch diese Richtlinieneinstellung wird festgelegt, ob von den Windows XP-Computern in Ihrer Umgebung Remoteunterstützung angefordert werden kann. Sie können diese Richtlinieneinstellung aktivieren, damit Benutzer Remoteunterstützung von versierten IT-Administratoren anfordern können.
  
**Hinweis**: Spezialisten können nicht unangekündigt eine Verbindung zum Computer herstellen oder diesen ohne Erlaubnis des Benutzers steuern. Wenn ein Verbindungsversuch erfolgt, kann der Benutzer die Verbindung immer noch verweigern (und damit dem Spezialisten nur Anzeigeberechtigungen gewähren). Der Benutzer muss ausdrücklich auf die Schaltfläche **Ja** klicken, um die Remotesteuerung der Arbeitsstation zuzulassen.
  
Wenn die Einstellung **Angeforderte Remoteunterstützung** aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Helfer dürfen den Computer remote steuern**
  
-   **Helfer dürfen den Computer nur ansehen**
  
Zusätzlich sind folgende Optionen verfügbar, um die Zeitdauer zu konfigurieren, für die die Hilfeanforderung eines Benutzers Gültigkeit behält:
  
-   **Maximale Gültigkeitsdauer der Einladung (Wert):**
  
-   **Maximale Gültigkeitsdauer (Einheiten): Stunden, Minuten oder Tage**
  
Wenn ein Ticket (Hilfeanforderung) abgelaufen ist, muss der Benutzer eine neue Anforderung senden, damit der Spezialist eine Verbindung mit dem Computer herstellen kann. Wenn Sie die Einstellung **Angeforderte Remoteunterstützung** deaktivieren, können Benutzer keine Hilfeanforderungen senden, und ein Spezialist kann keine Verbindung zum Computer des Benutzers herstellen.
  
Wenn die Einstellung **Angeforderte Remoteunterstützung** nicht konfiguriert ist, können Benutzer angeforderte Remoteunterstützung über die Systemsteuerung konfigurieren. Die folgenden Einstellungen sind standardmäßig in der Systemsteuerung aktiviert: **Angeforderte Remoteunterstützung**, **Benutzerunterstützung** und **Remotesteuerung**. Als Wert für die **Maximale Gültigkeitsdauer der Einladung** sind **30 Tage** festgelegt. Wenn diese Richtlinieneinstellung deaktiviert ist, kann niemand über das Netzwerk auf Windows XP-Clientcomputer zugreifen.
  
Die Einstellung **Angeforderte Remoteunterstützung** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Fehlerberichterstattung
  
Mit diesen Einstellungen wird die Berichterstattung bei Betriebssystem- und Anwendungsfehlern gesteuert. Wenn in der Standardkonfiguration ein Fehler auftritt, wird ein Dialogfeld mit der Frage angezeigt, ob der Benutzer einen Fehlerbericht an Microsoft senden möchte. Bei Microsoft gelten strenge Richtlinien für den Umgang mit den Daten aus diesen Berichten. Da diese Informationen jedoch unverschlüsselt übertragen werden, stellen sie dennoch ein potenzielles Sicherheitsrisiko dar.
  
Für Organisationen stellt Microsoft das Programm Firmen-Fehlerberichterstattung zur Verfügung, damit diese die Berichte lokal sammeln können, anstatt sie über das Internet an Microsoft zu übertragen. Microsoft empfiehlt die Verwendung der Firmen-Fehlerberichterstattung in der Hochsicherheitsumgebung, um die Offenlegung vertraulicher Informationen im Internet zu verhindern. Zusätzliche Informationen zu diesem Tool finden Sie im Abschnitt „Weitere Informationen“ am Ende dieses Kapitels.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Fehlerberichterstattung**
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für die Fehlerberichterstattung zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.22: Empfohlene Einstellungen für die Fehlerberichterstattung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Fehlerbenachrichtigung anzeigen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Fehlerberichterstattung konfigurieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Fehlerbenachrichtigung anzeigen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob den Benutzern Fehlermeldungen auf dem Computerbildschirm angezeigt werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden beim Auftreten von Fehlern entsprechende Benachrichtigungen gesendet, und Benutzern wird Zugriff auf detaillierte Fehlerinformationen gewährt. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden Benutzern keine Fehlerbenachrichtigungen angezeigt.
  
Beim Auftreten eines Fehlers ist es wichtig, dass dem Benutzer das Vorhandensein eines Problems bekannt ist. Benutzer werden nicht auf Probleme aufmerksam gemacht, wenn Sie die Einstellung **Fehlerbenachrichtigung anzeigen** deaktivieren. Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Fehlerbenachrichtigung anzeigen** deshalb auf **Aktiviert** gesetzt.
  
###### Fehlerberichterstattung konfigurieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Fehler gemeldet werden. Wenn diese Richtlinieneinstellung aktiviert ist, können Benutzer wählen, ob beim Auftreten von Fehlern eine Berichterstellung durchgeführt wird. Fehlerbericht können an eine lokale Dateifreigabe oder über das Internet an Microsoft gesendet werden. Wenn Sie diese Richtlinieneinstellung aktivieren, sind auch folgende Optionen verfügbar:
  
-   **Keine von Microsoft angebotenen Websites bezüglich "Weiterer Informationen" anzeigen**
  
-   **Keine zusätzlichen Dateien sammeln**
  
-   **Keine zusätzlichen Computerdaten sammeln**
  
-   **Warteschlangenmodus für Anwendungsfehler erzwingen**
  
-   **Dateiuploadpfad für zentrale Fehlerberichte**
  
-   **Instanzen des Worts "Microsoft" ersetzen durch**
  
Wenn die Einstellung **Fehlerberichterstattung konfigurieren** deaktiviert ist, können Benutzer keine Fehler melden. Wenn die Einstellung **Fehlerbenachrichtigung anzeigen** aktiviert ist, werden Benutzer über Fehler benachrichtigt, sie können jedoch keine entsprechenden Fehlerberichte senden. Mit der Einstellung **Fehlerberichterstattung konfigurieren** können Sie die Fehlerberichterstattung an die Anforderungen Ihrer Organisation anpassen und Berichte für die Analyse vor Ort sammeln.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Fehlerberichterstattung konfigurieren** auf **Aktiviert** gesetzt. Außerdem wurden für die Hochsicherheitsumgebung folgende Optionen ausgewählt:
  
-   **Keine zusätzlichen Dateien sammeln**
  
-   **Keine zusätzlichen Computerdaten sammeln**
  
-   **Warteschlangenmodus für Anwendungsfehler erzwingen**
  
Sie können auch die Option **Dateiuploadpfad für zentrale Fehlerberichte** auswählen und den Pfad zum Server angeben, auf dem das Programm zur Firmen-Fehlerberichterstattung installiert ist. Sie sollten die Bedürfnisse Ihrer Organisation bewerten, um zu ermitteln, welche dieser Optionen zu verwenden ist.
  
##### Remoteprozeduraufruf
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\System\\Remoteprozeduraufruf**
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für den Remoteprozeduraufruf zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.23: Empfohlene Einstellungen für den Remoteprozeduraufruf**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Einschränkungen für nicht authentifizierte RPC-Clients</td>
<td style="border:1px solid black;">Aktiviert – Authentifiziert</td>
<td style="border:1px solid black;">Aktiviert – Authentifiziert</td>
<td style="border:1px solid black;">Aktiviert – Authentifiziert</td>
<td style="border:1px solid black;">Aktiviert – Authentifiziert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RPC-Endpunktzuordnung Clientauthentifizierung</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Einschränkungen für nicht authentifizierte RPC-Clients
  
Diese Richtlinieneinstellung sorgt dafür, dass die RPC-Laufzeit auf einem RPC-Server nicht authentifizierte RPC-Clients daran hindert, eine Verbindung zu RPC-Servern herzustellen Ein Client wird als authentifizierter Client betrachtet, wenn er eine Named Pipe für die Kommunikation mit dem Server oder RPC-Sicherheit verwendet. RPC-Schnittstellen, die ausdrücklich darum ersucht haben, für nicht authentifizierte Clients zugänglich zu sein, können von dieser Einschränkung ausgenommen sein. Das hängt von dem für diese Richtlinie ausgewählten Wert ab. Wenn Sie diese Richtlinieneinstellung aktivieren, sind folgende Werte verfügbar:
  
-   **Keine**. Erlaubt allen RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt.
  
-   **Authentifiziert**. Erlaubt nur authentifizierten RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt. Schnittstellen, die von dieser Einschränkung ausgenommen sind, wird eine Ausnahme gewährt.
  
-   **Authentifiziert ohne Ausnahmen**. Erlaubt nur authentifizierten RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt. Es sind keine Ausnahmen erlaubt.
  
Da nicht authentifizierte RPC-Kommunikation eine Sicherheitsanfälligkeit verursachen kann, ist für die beiden in diesem Kapitel behandelten Umgebungen die Einstellung **Einschränkungen für nicht authentifizierte RPC-Clients** auf **Aktiviert** und der Wert **RPC-Laufzeit: Einschränkungen für nicht authentifizierte Clients anwenden** auf **Authentifiziert** gesetzt.
  
**Hinweis**: RPC-basierte Anwendungen, die unerwünscht eingehende Verbindungsanforderungen nicht authentifizieren, funktionieren möglicherweise nicht richtig, wenn diese Konfiguration angewendet wird. Testen Sie die Anwendungen unbedingt, bevor Sie diese Richtlinieneinstellung für Ihre gesamte Umgebung bereitstellen. Obwohl der Wert „Authentifiziert“ für diese Richtlinieneinstellung nicht vollständig sicher ist, kann er für die Bereitstellung von Anwendungskompatibilität in Ihrer Umgebung nützlich sein.
  
###### RPC-Endpunktzuordnung Clientauthentifizierung
  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden mit diesem Computer kommunizierende Clientcomputer zur Authentifizierung gezwungen, bevor eine RPC-Kommunikation eingerichtet wird. Standardmäßig verwenden RPC-Clients keine Authentifizierung, um mit der RPC-Endpunktzuordnung zu kommunizieren, wenn sie den Endpunkt von einem Server anfordern. Dieser Standard wurde jedoch für die Hochsicherheitsumgebung geändert, um von Clientcomputern eine Authentifizierung zu fordern, bevor eine RPC-Kommunikation zugelassen wird.
  
##### Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen
  
In der Gruppe „Internetkommunikationseinstellungen“ sind mehrere Konfigurationseinstellungen verfügbar. Es wird empfohlen, viele dieser Einstellungen einzuschränken, v. a. um die Sicherheit der Daten auf Ihren Computersystemen zu erhöhen. Wenn diese Einstellungen nicht eingeschränkt werden, könnten Informationen abgefangen und von Angreifern verwendet werden. Obwohl diese Art von Angriff heutzutage selten ist, können Sie Ihre Umgebung durch die richtige Konfiguration dieser Einstellungen vor zukünftigen Angriffen schützen.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\System\\Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen**
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für die Internetkommunikationseinstellungen zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.24: Empfohlene Einstellungen für die Internetkommunikation**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Aufgabe &quot;Im Web veröffentlichen&quot; für Dateien und Ordner deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetdownload für Webpublishing und Assistenten für Onlinebestellungen deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Programm zur Verbesserung der Benutzerfreundlichkeit von Windows Messenger deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Such-Assistent für Updates von Inhaltsdateien deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Druckausgabe über HTTP deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herunterladen von Druckertreibern über HTTP deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Gerätetreibersuche in Windows Update deaktivieren</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Aufgabe "Im Web veröffentlichen" für Dateien und Ordner deaktivieren
  
Durch diese Einstellung wird festgelegt, ob die Aufgaben **Datei im Web veröffentlichen**, **Ordner im Web veröffentlichen** und **Ausgewählte Elemente im Web veröffentlichen** in den Datei- und Ordneraufgaben in Windows-Ordnern zur Verfügung stehen. Mit dem Webpublishing-Assistenten wird eine Liste von Anbietern heruntergeladen, und Benutzer können Inhalte im Internet veröffentlichen.
  
Wenn Sie die Einstellung **Aufgabe "Im Web veröffentlichen" für Dateien und Ordner deaktivieren** auf **Aktiviert** setzen, werden diese Optionen aus den Datei- und Ordneraufgaben in Windows-Ordnern entfernt. Die Option zur Veröffentlichung im Internet ist standardmäßig verfügbar. Da diese Funktion dazu genutzt werden könnte, gesicherten Inhalt gegenüber einem nicht authentifizierten Webclientcomputer offen zu legen, ist diese Richtlinieneinstellung sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
###### Internetdownload für Webpublishing und Assistenten für Onlinebestellungen deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows eine Liste von Anbietern für das Webpublishing und Assistenten für Onlinebestellungen herunterlädt. Wenn diese Richtlinieneinstellung aktiviert ist, wird Windows daran gehindert, Anbieter herunterzuladen. Es werden nur die Dienstanbieter angezeigt, die in der lokalen Registrierung zwischengespeichert sind.
  
Da die Einstellung **Aufgabe** **"Im Web veröffentlichen" für Dateien und Ordner deaktivieren** sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung aktiviert wurde (siehe vorherige Einstellung), ist diese Option nicht erforderlich. Die Einstellung **Internetdownload für Webpublishing und Assistenten für Onlinebestellungen deaktivieren** ist auf **Aktiviert** gesetzt, um die Angriffsfläche von Clientcomputern zu minimieren und sicherzustellen, dass diese Funktion nicht auf andere Weise ausgenutzt werden kann.
  
###### Programm zur Verbesserung der Benutzerfreundlichkeit von Windows Messenger deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows Messenger anonyme Informationen darüber sammelt, wie Software und Dienste von Windows Messenger verwendet werden. Sie können diese Richtlinieneinstellung aktivieren, um sicherzustellen, dass Windows Messenger keine Verwendungsdaten sammelt. Außerdem wird die Benutzereinstellung, mit der das Sammeln von Verwendungsdaten aktiviert werden kann, nicht angezeigt.
  
In großen Unternehmensumgebungen ist es möglicherweise unerwünscht, dass Informationen von verwalteten Clientcomputern gesammelt werden. Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Programm zur Verbesserung der Benutzerfreundlichkeit von Windows Messenger deaktivieren** auf **Aktiviert** gesetzt, um das Sammeln von Informationen zu verhindern.
  
###### Such-Assistent für Updates von Inhaltsdateien deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Such-Assistent bei lokalen Suchen und Internetsuchen automatisch Inhaltsaktualisierungen herunterladen soll. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, hindern Sie den Such-Assistenten daran, im Verlauf von Suchen Inhaltsaktualisierungen herunterzuladen.
  
Die Einstellung **Such-Assistent für Updates von Inhaltsdateien** ist sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt, um unnötige Netzwerkkommunikation von jedem verwalteten Clientcomputer zu kontrollieren.
  
**Hinweis**: Internetsuchen senden den Suchtext und Informationen zur Suche weiterhin an Microsoft und den ausgewählten Suchprovider. Wenn Sie Klassische Suche auswählen, ist die Funktion Such-Assistent nicht verfügbar. Sie können „Klassische Suche“ auswählen, indem Sie auf **Start**, **Suchen**, **Bevorzugte Einstellungen ändern** und schließlich auf **Internetsuchverhalten ändern** klicken.
  
###### Druckausgabe über HTTP deaktivieren
  
Mit dieser Richtlinieneinstellung können Sie verhindern, dass der Clientcomputer über HTTP und damit auf Druckern im Intranet sowie im Internet drucken kann. Wenn Sie diese Richtlinieneinstellung aktivieren, kann der Clientcomputer nicht über HTTP auf Internetdruckern drucken.
  
Informationen, die mithilfe dieser Funktion über HTTP übertragen werden, sind nicht geschützt und können von unbefugten Benutzern abgefangen werden. Aus diesem Grund wird sie nicht oft in Unternehmensumgebungen verwendet. Die Einstellung **Druckausgabe über HTTP deaktivieren** ist sowohl für die Unternehmensclient-Umgebung als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt, um eine potenzielle Sicherheitsverletzung durch einen unsicheren Druckauftrag zu verhindern.
  
**Hinweis**: Diese Richtlinieneinstellung beim Internetdrucken wirkt sich nur auf den Client aus. Ungeachtet der Konfiguration könnte ein Computer als Internetdruckserver agieren und seine freigegebenen Drucker über HTTP zur Verfügung stellen.
  
###### Herunterladen von Druckertreibern über HTTP deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Computer Drucktreiberpakete über HTTP herunterladen kann. Für das Einrichten der Druckausgabe über HTTP müssen möglicherweise Druckertreiber über HTTP heruntergeladen werden, die nicht in der Standard-Betriebssysteminstallation enthalten sind.
  
Die Einstellung **Herunterladen von Drucktreibern über HTTP deaktivieren** ist auf **Aktiviert** gesetzt, damit keine Druckertreiber über HTTP heruntergeladen werden können.
  
**Hinweis**: Diese Richtlinieneinstellung hindert den Clientcomputer nicht daran, über HTTP auf Druckern im Intranet oder Internet zu drucken. Sie unterbindet lediglich das Herunterladen von Treibern, die nicht bereits lokal installiert sind.
  
###### Gerätetreibersuche in Windows Update deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows in Windows Update nach Gerätetreibern sucht, wenn lokal keine Treiber für ein Gerät vorhanden sind.
  
Das Herunterladen von Gerätetreibern aus dem Internet birgt gewisse Risiken. Deshalb wird empfohlen, die Einstellung **Gerätetreibersuche in Windows Update deaktivieren** für Hochsicherheitsumgebungen auf **Aktiviert** und für Unternehmensclient-Umgebungen auf **Deaktiviert** zu setzen. Der Grund für diese Konfiguration ist, dass den Angriffsarten, die einen Treiberdownload ausnutzen, in der Regel durch eine korrekte Verwaltung von Unternehmensanwendungen und Konfigurationen begegnet werden kann.
  
**Hinweis**: Befassen Sie sich außerdem mit **Suchbefehl für Gerätetreiber in Windows Update deaktivieren** in **Administrative Vorlagen/System**. Durch diese Einstellung wird festgelegt, ob ein Administrator um Zustimmung gebeten wird, bevor Windows Update nach einem Gerätetreiber durchsucht wird, der lokal nicht vorhanden ist.
  
#### Netzwerk
  
Es gibt keine bestimmten sicherheitsrelevanten Konfigurationen im Netzwerkcontainer der Gruppenrichtlinie. Es gibt jedoch eine Reihe sehr wichtiger Einstellungen im Container **Netzwerkverbindungen\\Windows Firewall**. Diese werden in den folgenden Abschnitten erklärt.
  
Die folgende Abbildung illustriert die Abschnitte in der Gruppenrichtlinie, die von den Einstellungsänderungen in diesem Abschnitt betroffen sein werden:
  
![](images/Cc163076.SGFG0404(de-de,TechNet.10).gif)
  
**Abbildung 4.2: Gruppenrichtlinienstruktur für Netzwerkverbindungen in der Computerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0404_big(de-de,technet.10).gif)
  
#### Netzwerkverbindungen\\Windows Firewall
  
Einstellungen der Windows-Firewall werden in zwei Profilen vorgenommen: im Domänenprofil und im Standardprofil. Immer wenn eine Domänenumgebung erkannt wird, wird das Domänenprofil verwendet. Wenn keine Domänenumgebung verfügbar ist, wird das Standardprofil genutzt.
  
Wenn eine Einstellung der Windows-Firewall in einer der beiden folgenden Tabellen **Empfohlen** lautet, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Beispielsweise verfügt jede Organisation über eine eigene Liste von Anwendungen, die definierte Ausnahmen für die Windows-Firewall erfordern. Deshalb ist es nicht möglich, in diesem Handbuch eine Liste zu definieren, die generell verwendet werden kann.
  
Wenn Sie ermitteln müssen, welche Anwendungen oder Ports möglicherweise Ausnahmen benötigen, kann es nützlich sein, Windows-Firewall-Protokollierung, Windows Firewall-Überwachung und Ablaufverfolgung für das Netzwerk zu aktivieren. Weitere Informationen finden Sie im Artikel „[Konfigurieren eines Computers für Windows-Firewall-Problembehandlung](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/operations/bfdeda55-46fc-4b53-b4cd-c71838ef4b41.mspx)“ (in englischer Sprache), der online unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/Operations/bfdeda55-46fc-4b53-b4cd-c71838ef4b41.mspx verfügbar ist.
  
Weitere Informationen dazu, wie Windows XP mithilfe von NLA (Network Location Awareness) ermittelt, mit welcher Art von Netzwerk es verbunden ist, finden Sie im Artikel „[Netzwerkerkennungsverhalten für netzwerkbezogene Gruppenrichtlinieneinstellungen](http://www.microsoft.com/technet/community/columns/cableguy/cg0504.mspx)“ (in englischer Sprache) auf der Microsoft-Website unter http://www.microsoft.com/technet/community/columns/cableguy/cg0504.mspx.
  
In der Regel wird das Domänenprofil mit weniger Einschränkungen konfiguriert als das Standardprofil, denn eine Domänenumgebung bietet häufig zusätzliche Schutzebenen.
  
Die Namen der Richtlinieneinstellungen sind in beiden Profilen identisch. In den beiden folgenden Tabellen werden die Richtlinieneinstellungen für die verschiedenen Profile zusammengefasst. In den Unterabschnitten im Anschluss an die Tabellen werden ausführlichere Erklärungen geboten.
  
##### Netzwerkverbindungen\\Windows Firewall\\Domänenprofil
  
Mit den Einstellungen in diesem Abschnitt wird das Domänenprofil der Windows-Firewall konfiguriert.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen\\Windows Firewall\\Domänenprofil**
  
**Tabelle 4.25: Empfohlene Einstellungen für das Domänenprofil der Windows-Firewall**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alle Netzwerkverbindungen schützen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Keine Ausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Programmausnahmen definieren</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lokale Programmausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ausnahme für Remoteverwaltung zulassen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ausnahme für Datei- und Druckerfreigabe zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ICMP-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ausnahme für Remotedesktop zulassen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ausnahme für UPnP-Framework zulassen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Benachrichtigungen verbieten</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Portausnahmen definieren</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lokale Portausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Hinweis**: Wenn in dieser Tabelle eine Einstellung der Windows-Firewall **Empfohlen** ist, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Beispielsweise verfügt jede Organisation über eine eigene Liste von Anwendungen, die definierte Ausnahmen für die Windows-Firewall erfordern. Deshalb ist es nicht möglich, in diesem Handbuch eine Liste zu definieren, die generell verwendet werden kann.
  
##### Netzwerkverbindungen\\Windows Firewall\\Standardprofil
  
Mit den Einstellungen in diesem Abschnitt wird das Standardprofil der Windows-Firewall konfiguriert. Dieses Profil schränkt oft stärker ein als das Domänenprofil, welches davon ausgeht, dass eine Domänenumgebung ein grundlegendes Maß an Sicherheit bereitstellt. Das Standardprofil soll dann verwendet werden, wenn ein Computer sich in einem nicht vertrauenswürdigen Netzwerk befindet, z. B. in einem Hotelnetzwerk oder einem öffentlich zugänglichen, drahtlosen Zugriffspunkt. Solche Umgebungen stellen unbekannte Bedrohungen dar und erfordern zusätzliche Sicherheitsvorkehrungen.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen\\Windows Firewall\\Standardprofil**
  
**Tabelle 4.26: Empfohlene Einstellungen für das Standardprofil der Windows-Firewall**

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Unternehmensclient-Desktop</th>
<th>Unternehmensclient-Laptop</th>
<th>Hochsicher-Desktop</th>
<th>Hochsicher-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Alle Netzwerkverbindungen schützen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Keine Ausnahmen zulassen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Programmausnahmen definieren</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lokale Programmausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ausnahme für Remoteverwaltung zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ausnahme für Datei- und Druckerfreigabe zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ICMP-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ausnahme für Remotedesktop zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ausnahme für UPnP-Framework zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Benachrichtigungen verbieten</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Portausnahmen definieren</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
<td style="border:1px solid black;">Nicht Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lokale Portausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Hinweis**: Wenn in dieser Tabelle eine Einstellung der Windows-Firewall **Empfohlen** ist, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Beispielsweise verfügt jede Organisation über eine eigene Liste von Anwendungen, die definierte Ausnahmen für die Windows-Firewall erfordern. Deshalb ist es nicht möglich, in diesem Handbuch eine Liste zu definieren, die generell verwendet werden kann.
  
###### Windows-Firewall: Alle Netzwerkverbindungen schützen
  
Durch diese Richtlinieneinstellung wird die Windows-Firewall aktiviert. Sie ersetzt die Internetverbindungsfirewall auf allen Computern, auf denen Windows XP mit SP2 ausgeführt wird. Es wird empfohlen, diese Richtlinieneinstellung auf **Aktiviert** zu setzen. Dadurch werden für Computer in allen in diesem Handbuch behandelten Umgebungen sämtliche Netzwerkverbindungen geschützt.
  
Wenn die Einstellung **Windows-Firewall: Alle Netzwerkverbindungen schützen** auf **Deaktiviert** gesetzt ist, ist die Windows-Firewall deaktiviert, und alle anderen Einstellungen für die Windows-Firewall werden ignoriert.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung aktivieren, wird die Windows-Firewall ausgeführt, und die Richtlinieneinstellung **Computerkonfiguration\\Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen\\Verwendung der Internetverbindungsfirewall im eigenen DNS-Domänennetzwerk nicht zulassen** wird ignoriert.
  
###### Windows-Firewall: Keine Ausnahmen zulassen
  
Diese Richtlinieneinstellung sorgt dafür, dass die Windows-Firewall alle unerwünscht eingehenden Meldungen blockiert. Sie setzt alle anderen Einstellungen der Windows-Firewall außer Kraft, die solche Nachrichten zulassen. Wenn Sie diese Richtlinieneinstellung in der Systemsteuerung für die Windows-Firewall aktivieren, wird das Kontrollkästchen **Keine Ausnahmen zulassen** aktiviert. Administratoren können es nicht deaktivieren.
  
Viele Umgebungen enthalten Anwendungen und Dienste, denen im Rahmen ihres normalen Betriebs erlaubt werden muss, eingehende unerwünschte Kommunikationen zu empfangen. In solchen Umgebungen muss die Einstellung **Windows-Firewall: Keine Ausnahmen zulassen** möglicherweise auf **Deaktiviert** gesetzt werden, damit diese Anwendungen und Dienste richtig ausgeführt werden. Bevor Sie jedoch diese Richtlinieneinstellung konfigurieren, sollten Sie die Umgebung prüfen und genau ermitteln, welche Kommunikationen Sie zulassen möchten.
  
**Hinweis**: Diese Richtlinieneinstellung bietet einen sehr guten Schutz vor externen Angreifern. Sie sollte in Situationen auf **Aktiviert** gesetzt sein, in denen Sie vollständigen Schutz vor externen Angriffen benötigen, wie z. B. beim Ausbruch eines neuen Netzwerkwurms. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, kann die Windows-Firewall andere Richtlinieneinstellungen anwenden, die unerwünscht eingehende Meldungen zulassen.
  
###### Windows-Firewall: Programmausnahmen definieren
  
Einige Anwendungen müssen möglicherweise Netzwerkports öffnen und verwenden, die normalerweise nicht von der Windows-Firewall zugelassen sind. Mit der Einstellung **Windows-Firewall: Programmausnahmen definieren** können Sie die Liste der durch die Gruppenrichtlinie definierten Programmausnahmen anzeigen und ändern.
  
Wenn diese Richtlinieneinstellung **Aktiviert** ist, können Sie die Liste der Programmausnahmen anzeigen und ändern. Wenn Sie dieser Liste ein Programm hinzufügen und den entsprechenden Status auf **Aktiviert** setzen, kann dieses Programm über jeden Port, den die Windows-Firewall auf sein Ersuchen hin öffnet, unerwünscht eingehende Meldungen empfangen. Dies gilt selbst dann, wenn der Port von einer anderen Richtlinieneinstellung blockiert wird. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, wird die durch die Gruppenrichtlinie definierte Liste der Programmausnahmen gelöscht.
  
**Hinweis**: Wenn Sie eine ungültige Definitionszeichenfolge eingeben, fügt Windows-Firewall diese der Liste hinzu, ohne eine Fehlerprüfung vorzunehmen. Da der Eintrag nicht geprüft wird, können Sie Programme hinzufügen, die Sie noch nicht installiert haben. Sie können auch versehentlich mehrere Ausnahmen für dasselbe Programm mit sich widersprechenden Bereichs- oder Statuswerten erstellen.
  
###### Windows-Firewall: Lokale Programmausnahmen zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Administratoren mithilfe der Windows-Firewall in der Systemsteuerung eine Liste lokaler Programmausnahmen definieren können. Wenn Sie diese Richtlinieneinstellung deaktivieren, sind Administratoren nicht in der Lage, eine Liste lokaler Programmausnahmen zu definieren. Außerdem wird durch diese Konfiguration sichergestellt, dass sämtliche Programmausnahmen der Gruppenrichtlinie entstammen. Wenn diese Richtlinieneinstellung aktiviert ist, können lokale Administratoren die Systemsteuerung dazu verwenden, Programmausnahmen lokal zu definieren.
  
Bei Unternehmensclientcomputern kann es Bedingungen geben, die die Definition lokaler Programmausnahmen rechtfertigen. Diese Bedingungen umfassen z. B. Anwendungen, die bei Erstellung der Firewallrichtlinie der Organisation nicht analysiert wurden, sowie neue Anwendungen, die eine nicht standardmäßige Portkonfiguration erfordern. Wenn Sie sich in solchen Situationen dafür entscheiden, die Einstellung **Windows-Firewall: Lokale Programmausnahmen zulassen** zu aktivieren, müssen Sie sich dessen bewusst sein, dass dadurch die Angriffsfläche der betroffenen Computer vergrößert wird.
  
###### Windows-Firewall: Ausnahme für Remoteverwaltung zulassen
  
Viele Organisationen nutzen bei ihren täglichen Aktionen die Vorteile der Remotecomputerverwaltung. Bei einigen Angriffsmethoden wurden jedoch die Ports ausgenutzt, die normalerweise von Remoteverwaltungsprogrammen verwendet werden. Die Windows-Firewall kann diese Ports blockieren.
  
Mit der Einstellung **Windows-Firewall: Ausnahme für Remoteverwaltung zulassen** wird Flexibilität für die Remoteverwaltung bereitgestellt. Wenn diese Richtlinieneinstellung aktiviert ist, kann der Computer die unerwünscht eingehenden Meldungen, die mit der Remoteverwaltung einhergehen, über die TCP-Ports 135 und 445 empfangen. Außerdem erlaubt diese Richtlinieneinstellung SVCHOST.EXE und LSASS.EXE, unerwünscht eingehende Meldungen zu empfangen. Gehostete Dienste können zusätzlich dynamisch zugewiesene Ports öffnen, in der Regel im Bereich von 1024 bis 1034. Möglich ist jedoch der Bereich zwischen 1024 und 65535. Wenn Sie diese Richtlinieneinstellung aktivieren, müssen Sie die IP-Adressen oder die Subnetze angeben, von denen diese Meldungen eingehen dürfen.
  
Wenn Sie die Einstellung **Windows-Firewall: Ausnahmen für Remoteverwaltung zulassen** auf **Deaktiviert** setzen, macht die Windows-Firewall keine der beschriebenen Ausnahmen. Diese Richtlinieneinstellung auf **Deaktiviert** zu setzen, kann Auswirkungen haben, die für viele Organisationen nicht akzeptabel sind, da viele Remoteverwaltungstools und Programme, die nach Sicherheitsanfälligkeiten suchen, fehlschlagen werden. Deshalb empfiehlt Microsoft, dass diese Richtlinieneinstellung nur in Organisationen aktiviert wird, die extrem strenger Sichermaßnahmen bedürfen.
  
Für das Domänenprofil empfiehlt Microsoft, die Einstellung **Windows-Firewall: Ausnahmen für Remoteverwaltung zulassen** für Computer in der Unternehmensclient-Umgebung (wenn möglich) auf **Aktiviert** und für Computer in der Hochsicherheitsumgebung auf **Deaktiviert** zu setzen. Computer in Ihrer Umgebung sollten Anforderungen zur Remoteverwaltung von so wenigen Computern wie möglich annehmen. Um den von der Windows-Firewall gebotenen Schutz zu maximieren, sollten Sie nur die IP-Adressen und Subnetze der Computer angeben, die für die Remoteverwaltung verwendet werden.
  
Microsoft empfiehlt, die Einstellung **Windows Firewall: Ausnahmen für Remoteverwaltung zulassen** für alle Computer im Standardprofil auf **Deaktiviert** zu setzen, um bekannte Angriffsmethoden zu vermeiden, die insbesondere die TCP-Ports 135 und 445 ausnutzen.
  
**Hinweis**: Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, umfassen **Windows-Firewall: Ausnahme für Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Ausnahme für Remoteverwaltung zulassen** und **Windows-Firewall: Portausnahmen definieren.**
  
###### Windows-Firewall: Ausnahme für Datei- und Druckerfreigabe zulassen
  
Durch diese Richtlinieneinstellung wird eine Ausnahme geschaffen, die die Datei- und Druckerfreigabe zulässt. Dadurch wird die Windows-Firewall so konfiguriert, dass die UDP-Ports 137 und 138 sowie die TCP-Ports 139 und 445 geöffnet werden. Wenn Sie diese Richtlinieneinstellung aktivieren, öffnet die Windows-Firewall diese Ports, damit der Computer Druckaufträge und Anforderungen für den Zugriff auf freigegebene Dateien empfangen kann. Sie müssen die IP-Adressen oder Subnetze angeben, von denen diese Meldungen zulässig sind.
  
Wenn Sie die Einstellung **Windows-Firewall: Datei- und Druckerfreigabe zulassen** deaktivieren, blockiert die Windows-Firewall diese Ports und hindert den Computer an der Freigabe von Dateien und Druckern.
  
Die Computer in Ihrer Umgebung, auf denen Windows XP ausgeführt wird, geben Dateien und Drucker normalerweise nicht frei. Aus diesem Grund empfiehlt Microsoft, die Einstellung **Windows-Firewall: Datei- und Druckerfreigabe zulassen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** zu setzen.
  
**Hinweis**: Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, umfassen **Windows-Firewall: Ausnahme für Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Ausnahme für Remoteverwaltung zulassen** und **Windows-Firewall: Portausnahmen definieren.**
  
###### Windows-Firewall: ICMP-Ausnahmen zulassen
  
Durch dieser Richtlinieneinstellung wird der Satz an ICMP-Meldungstypen (Internet Control Message Protocol) definiert, den die Windows-Firewall zulässt. Mithilfe von ICMP-Meldungen können Dienstprogramme den Status anderer Computer bestimmen. Ping verwendet z. B. die Echoanforderungsmeldung.
  
Wenn Sie die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** auf **Aktiviert** setzen, müssen Sie angeben, welchen ICMP-Meldungstyp der Computer durch die Windows-Firewall senden bzw. empfangen kann. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, blockiert die Windows-Firewall alle unerwünscht eingehenden ICMP-Meldungstypen sowie die aufgeführten ausgehenden ICMP-Meldungstypen. Demzufolge können Dienstprogramme fehlschlagen, die ICMP verwenden.
  
Viele Angriffstools nutzen Computer aus, die ICMP-Meldungstypen akzeptieren. Diese Meldungen werden für verschiedenartige Angriffe verwendet. Einige Anwendungen benötigen jedoch einige ICMP-Meldungen, um ordnungsgemäß zu funktionieren. Mithilfe von ICMP-Meldungen wird außerdem die Netzwerkleistung eingeschätzt, wenn Gruppenrichtlinien heruntergeladen und verarbeitet werden. Wenn ICMP-Meldungen blockiert werden, kann die Gruppenrichtlinie nicht auf betroffene Systeme angewendet werden. Aus diesem Grund empfiehlt Microsoft, die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** nach Möglichkeit auf **Deaktiviert** zu setzen. Wenn es in Ihrer Umgebung erforderlich ist, dass einige ICMP-Meldungen durch die Windows-Firewall gelangen, legen Sie für die Einstellung die entsprechenden Meldungstypen fest.
  
Wann immer der Computer sich in einem nicht vertrauenswürdigen Netzwerk befindet, sollte die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** auf **Deaktiviert** gesetzt werden.
  
**Hinweis**: Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, umfassen **Windows-Firewall: Ausnahme für Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Ausnahme für Remoteverwaltung zulassen** und **Windows-Firewall: Portausnahmen definieren.**
  
###### Windows-Firewall: Ausnahme für Remotedesktop zulassen
  
Viele Organisationen verwenden bei ihren normalen Problembehandlungsverfahren oder Vorgängen Remotedesktopverbindungen. Bei einigen Angriffsmethoden wurden jedoch die Ports ausgenutzt, die normalerweise von Remotedesktop verwendet werden.
  
Mit der Einstellung **Windows Firewall: Ausnahme für Remotedesktop zulassen** wird Flexibilität für die Remoteverwaltung bereitgestellt. Wenn Sie diese Richtlinieneinstellung aktivieren, öffnet die Windows-Firewall den TCP-Port 3389 für eingehende Verbindungen. Sie müssen außerdem die IP-Adressen oder Subnetze angeben, von denen diese Meldungen eingehen dürfen.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, blockiert die Windows-Firewall diesen Port und hindert den Computer daran, Anforderungen vom Remotedesktop zu empfangen. Wenn ein Administrator diesen Port einer Liste mit lokalen Portausnahmen hinzufügt, um ihn damit zu öffnen, hält die Windows-Firewall diesen Port geschlossen.
  
Einige Angriffe können den offenen Port 3389 ausnutzen. Daher empfiehlt Microsoft, die Einstellung **Windows-Firewall: Ausnahme für Remotedesktop zulassen** für die Hochsicherheitsumgebung auf **Deaktiviert** zu setzen. Um die erweiterten Verwaltungsmöglichkeiten beizubehalten, die von Remotedesktop bereitgestellt werden, sollten Sie diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Aktiviert** setzen. Sie müssen die IP-Adressen und Subnetze der Computer angeben, die für die Remoteverwaltung verwendet werden. Computer in Ihrer Umgebung sollten Remotedesktopanforderungen von so wenigen Computern wie möglich annehmen.
  
###### Windows-Firewall: Ausnahme für UPnP-Framework zulassen
  
Diese Richtlinieneinstellung ermöglicht es einem Computer, unerwünschte Plug & Play-Meldungen zu empfangen, die von Netzwerkgeräten gesendet werden, wie z. B. von Routern mit integrierten Firewalls. Um diese Meldungen zu empfangen, öffnet die Windows-Firewall den TCP-Port 2869 und den UDP-Port 1900.
  
Wenn Sie die Einstellung **Windows-Firewall: Ausnahme für UPnP-Framework zulassen** aktivieren, öffnet die Windows-Firewall diese Ports, damit der Computer Plug & Play-Meldungen empfangen kann. Sie müssen die IP-Adressen oder Subnetze angeben, von denen diese Meldungen eingehen dürfen. Wenn Sie diese Richtlinieneinstellung deaktivieren, blockiert die Windows-Firewall diese Ports und hindert den Computer am Empfang von Plug & Play-Meldungen.
  
Wenn der UPnP-Netzwerkverkehr blockiert wird, wird die Angriffsfläche der Computer in Ihrer Umgebung wirksam verkleinert. Microsoft empfiehlt, die Einstellung **Windows-Firewall: Ausnahme für UPnP-Framework zulassen** in vertrauenswürdigen Netzwerken auf **Deaktiviert** zu setzen, es sei denn, Sie verwenden in Ihrem Netzwerk UPnP-Geräte. In nicht vertrauenswürdigen Netzwerken sollte diese Richtlinieneinstellung immer auf **Deaktiviert** gesetzt werden.
  
###### Windows-Firewall: Benachrichtigungen verbieten
  
Die Windows-Firewall kann Benutzern Benachrichtigungen anzeigen, wenn ein Programm die Anforderung stellt, zur Liste mit den Programmausnahmen hinzugefügt zu werden. Diese Situation tritt ein, wenn Programme versuchen, einen Port zu öffnen, den sie aufgrund der aktuellen Regeln der Windows-Firewall nicht öffnen dürfen.
  
Durch die Einstellung **Windows-Firewall: Benachrichtigungen verbieten** wird festgelegt, ob diese Einstellungen Benutzern angezeigt werden. Wenn Sie diese Richtlinie auf **Aktiviert** setzen, wird das Anzeigen dieser Benachrichtigungen von der Windows-Firewall verhindert. Wenn Sie die Richtlinie auf **Deaktiviert** setzen, lässt die Windows-Firewall das Anzeigen dieser Benachrichtigungen zu.
  
In Unternehmensclient- oder Hochsicherheitsumgebungen ist es Benutzern meist nicht erlaubt, in Reaktion auf diese Meldungen Anwendungen und Ports hinzuzufügen. In solchen Fällen würde diese Meldung den Benutzer über etwas informieren, auf das er keinen Einfluss hat, weshalb Sie die Einstellung **Windows-Firewall: Benachrichtigungen verbieten** auf **Aktiviert** setzen sollten. In anderen Umgebungen, in denen für einige Benutzer Ausnahmen zulässig sind, sollten Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen.
  
###### Windows-Firewall: Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten
  
Durch diese Richtlinieneinstellung wird ein Computer daran gehindert, Unicast-Antworten auf seine ausgehenden Multicast- oder Broadcastmeldungen zu empfangen. Wenn diese Richtlinieneinstellung aktiviert ist und der Computer Multicast- oder Broadcastmeldungen an andere Computer sendet, blockiert die Windows-Firewall die Unicast-Antworten, die von den anderen Computern gesendet werden. Wenn diese Richtlinieneinstellung deaktiviert ist und dieser Computer eine Multicast- oder Broadcastmeldung an andere Computer sendet, wartet die Windows-Firewall bis zu drei Sekunden auf Unicast-Antworten von den anderen Computern und blockiert alle späteren Antworten.
  
Normalerweise ist es nicht wünschenswert, auf Multicast- oder Broadcastmeldungen Unicast-Antworten zu erhalten. Solche Antworten können auf einen DoS-Angriff (Denial of Service) oder auf einen Angreifer hindeuten, der versucht, einen ihm bekannten Computer zu untersuchen. Microsoft empfiehlt, die Einstellung **Windows-Firewall: Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten** auf **Aktiviert** zu setzen, um diese Art von Angriff zu verhindern.
  
**Hinweis**: Diese Richtlinieneinstellung ist wirkungslos, wenn es sich bei der Unicast-Meldung um eine Antwort auf eine DHCP-Broadcastmeldung (Dynamic Host Configuration Protocol) handelt, die vom Computer gesendet wurde. Die Windows-Firewall lässt diese DHCP-Unicast-Antworten immer zu. Diese Richtlinieneinstellung kann die NetBIOS-Meldungen stören, die Namenskonflikte erkennen.
  
###### Windows-Firewall: Portausnahmen definieren
  
Die Liste der Portausnahmen für die Windows-Firewall sollte von der Gruppenrichtlinie definiert werden. Diese ermöglicht Ihnen, Ihre Portausnahmen zentral zu verwalten und bereitzustellen und stellt sicher, dass lokale Administratoren keine weniger sicheren Einstellungen erstellen.
  
Wenn Sie die Einstellung **Windows-Firewall: Portausnahmen definieren** aktivieren, können Sie die durch die Gruppenrichtlinie definierte Liste von Portausnahmen anzeigen und ändern. Wenn Sie die Liste der Portausnahmen anzeigen und ändern möchten, setzen Sie die Richtlinieneinstellung auf **Aktiviert**, und klicken Sie anschließend auf die Schaltfläche **Anzeigen**. Wenn Sie eine ungültige Definitionszeichenfolge eingeben, fügt die Windows-Firewall diese der Liste hinzu, ohne eine Fehlerprüfung vorzunehmen. Sie können also versehentlich mehrere Einträge für den gleichen Port erstellen, wobei die Bereichs- oder Statuswerte einander widersprechen.
  
Wenn Sie die Einstellung **Windows-Firewall: Portausnahmen definieren** deaktivieren, wird die von der Gruppenrichtlinie definierte Liste mit Portausnahmen zwar gelöscht, aber andere Einstellungen können weiterhin Ports öffnen oder blockieren. Außerdem wird eine möglicherweise vorhandene Liste lokaler Portausnahmen ignoriert, es sei denn, Sie aktivieren die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen**.
  
Für Umgebungen mit nicht standardisierten Anwendungen, für die bestimmte Ports geöffnet sein müssen, sollte erwogen werden, Programmausnahmen anstelle von Portausnahmen bereitzustellen. Microsoft empfiehlt, dass nur dann die Einstellung **Windows-Firewall: Portausnahmen definieren** auf **Aktiviert** gesetzt und eine Liste mit Portausnahmen festgelegt wird, wenn keine Programmausnahmen definiert werden können. Programmausnahmen erlauben der Windows-Firewall, unerwünschten Netzwerkverkehr nur dann zu akzeptieren, wenn das angegebene Programm ausgeführt wird. Portausnahmen halten die angegebenen Ports stets offen.
  
**Hinweis**: Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, umfassen **Windows-Firewall: Ausnahme für Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Ausnahme für Remoteverwaltung zulassen** und **Windows-Firewall: Portausnahmen definieren.**
  
###### Windows-Firewall: Lokale Portausnahmen zulassen
  
Diese Richtlinieneinstellung ermöglicht es Administratoren, in der Systemsteuerung mithilfe der Windows-Firewall eine Liste lokaler Portausnahmen zu definieren. Die Windows-Firewall kann zwei Portausnahmelisten verwenden. Die andere Liste wird über die Einstellung **Windows-Firewall: Portausnahmen definieren** festgelegt.
  
Wenn Sie die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen** aktivieren, können Administratoren in der Systemsteuerung mithilfe der Windows-Firewall eine Liste lokaler Portausnahmen definieren. Wenn Sie diese Richtlinieneinstellung deaktivieren, erlaubt die Windows-Firewall in der Systemsteuerung Administratoren nicht, eine solche Liste zu definieren.
  
Normalerweise sind lokale Administratoren nicht berechtigt, Unternehmensrichtlinien außer Kraft zu setzen und in Unternehmensclient- oder Hochsicherheitsumgebungen ihre eigene Liste mit Portausnahmen einzurichten. Aus diesem Grund empfiehlt Microsoft, die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen** auf **Deaktiviert** zu setzen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Benutzerkonfigurationseinstellungen
  
In den übrigen Abschnitten dieses Kapitels werden Empfehlungen für die Benutzerkonfiguration erörtert. Denken Sie daran, dass diese Einstellungen auf Benutzer angewendet werden müssen, nicht auf Computer. Sie sollten mit einer Gruppenrichtlinie implementiert werden, die mit der Organisationseinheit verknüpft ist, die die zu konfigurierenden Benutzer enthält. Sie können sich Abbildung 2.3, „Erweiterte Organisationseinheitenstruktur zur Unterbringung von Windows XP-basierten Desktop- und Laptopcomputern“, in Kapitel 2 ansehen, um sich die nötigen Informationen in Erinnerung zu rufen. Diese Einstellungen werden im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert:
  
**Benutzerkonfiguration\\Administrative Vorlagen**
  
Dieser Speicherort ist in der folgenden Abbildung im Zusammenhang dargestellt:
  
![](images/Cc163076.SGFG0405(de-de,TechNet.10).gif)
  
**Abbildung 4.5: Gruppenrichtlinienstruktur für die Benutzerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0405_big(de-de,technet.10).gif)
  
Wenden Sie diese Einstellungen mithilfe eines Gruppenrichtlinienobjekts an, das mit einer Organisationseinheit verknüpft ist, die die Benutzerkonten enthält.
  
**Hinweis**: Benutzerkonfigurationseinstellungen werden auf jeden Windows XP-basierten Computer angewendet, bei dem sich ein Benutzer in einer Active Directory-Domäne anmeldet. Computerkonfigurationseinstellungen gelten jedoch für alle Clientcomputer, die von einem Gruppenrichtlinienobjekt in Active Directory gesteuert werden, unabhängig davon, welcher Benutzer sich beim Computer anmeldet. Aus diesem Grund enthalten die Tabellen in diesem Abschnitt nur empfohlene Einstellungen für die in diesem Kapitel behandelten Unternehmensclient- und die Hochsicherheitsumgebungen. Für diese Einstellungen sind keine Laptop- oder Desktop-spezifischen Optionen vorgesehen.
  
#### Windows-Komponenten
  
Die folgende Abbildung illustriert die Abschnitte in der Gruppenrichtlinie, die von den Einstellungsänderungen im Abschnitt Windows-Komponenten betroffen sein werden:
  
![](images/Cc163076.SGFG0406(de-de,TechNet.10).gif)
  
**Abbildung 4.2: Gruppenrichtlinienstruktur für Windows-Komponenten in der Benutzerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0406_big(de-de,technet.10).gif)
  
##### Internet Explorer
  
Die folgenden empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**Internet Explorer**
  
In der folgenden Tabelle sind die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.27: Empfohlene Benutzerkonfigurationseinstellungen für Internet Explorer**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer</th>
<th>SSLF-Computer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Browser-Menüs\Option &quot;Das Programm speichern&quot; deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetsystemsteuerung\Seite &quot;Erweitert&quot; deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetsystemsteuerung\Sicherheitsseite deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Offlineseiten\Hinzufügen von Channels deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Offlineseiten\Hinzufügen von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Offlineseiten\Alle geplanten Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Offlineseiten\Channel-Benutzeroberfläche vollständig deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Offlineseiten\Download von abonnierten Siteinhalten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Offlineseiten\Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Offlineseiten\Bearbeiten von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Offlineseiten\Trefferprotokollierung für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Offlineseiten\Entfernen von Channels deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Offlineseiten\Entfernen von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurieren von Outlook Express</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Einstellungen für die Seite &quot;Erweitert&quot; deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Änderung der Einstellungen für die automatische Konfiguration deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Änderung der Zertifikatseinstellungen deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Änderung der Verbindungseinstellungen deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Änderung der Proxyeinstellungen deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Die Speicherung von Kennwörtern mit AutoVervollständigen nicht zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Browser-Menüs\\Option "Das Programm speichern" deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Programme oder Dateien speichern können, die Internet Explorer auf die Festplatte heruntergeladen hat. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer Programme nicht mit der Option **Das Programm speichern** auf der Festplatte speichern. Die Programmdatei wird nicht heruntergeladen, und der Benutzer wird darüber informiert, dass dieser Befehl nicht verfügbar ist. Diese Richtlinieneinstellung trägt zum Schutz von Hochsicherheitsumgebungen bei, da Benutzer keine möglicherweise schädlichen Programme über Internet Explorer herunterladen und auf der Festplatte speichern können.
  
Die Einstellung **Browser-Menüs\\Option "Das Programm speichern" deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
###### Internetsystemsteuerung\\Seite "Erweitert" deaktivieren
  
Diese Richtlinieneinstellung steht mit anderen Einstellungen in Verbindung, um sicherzustellen, dass Benutzer die Einstellungen auf der Registerkarte **Erweitert** in der Benutzeroberfläche von Internet Explorer nicht ändern können.
  
Die Einstellung **Internetsystemsteuerung\\Seite "Erweitert" deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
###### Internetsystemsteuerung\\Sicherheitsseite deaktivieren
  
Diese Richtlinieneinstellung steht mit anderen Einstellungen in Verbindung, um sicherzustellen, dass Benutzer keine Einstellungen ändern können, die durch Gruppenrichtlinien konfiguriert wurden. Durch diese Richtlinieneinstellung wird die Registerkarte **Sicherheit** aus dem Dialogfeld **Internetoptionen** entfernt. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer daran gehindert, die Einstellungen für Sicherheitszonen wie Skripterstellung, Downloads und Benutzerauthentifizierung anzuzeigen und zu ändern. Microsoft empfiehlt, diese Richtlinieneinstellung zu aktivieren, damit Benutzer keine Einstellungen ändern und dadurch andere Sicherheitseinstellungen in Internet Explorer beeinträchtigen können.
  
Die Einstellung **Internetsystemsteuerung\\Sicherheitsseite deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
###### Offlineseiten\\Hinzufügen von Channels deaktivieren
  
Diese Richtlinieneinstellung sorgt dafür, dass Benutzer in Internet Explorer keine Channels hinzufügen können. Channels sind Websites, die auf Computern, auf denen Internet Explorer ausgeführt wird, nach einem vom Channelanbieter vorgegebenen Zeitplan automatisch aktualisiert werden. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen. Es handelt sich um eine bewährte Methode, das Herunterladen von Seiten aus dem Internet auf einen Computer nur zu ermöglichen, wenn ein Benutzer diese Funktion direkt an diesem Computer anfordert.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Hinzufügen von Channels deaktivieren** deshalb auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Hinzufügen von Zeitplänen für Offlineseiten deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Webseiten herunterladen und offline anzeigen können. Eine solche Funktion ermöglicht es Benutzern, Webseiten anzuzeigen, wenn ihre Computer nicht mit dem Internet verbunden sind.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Hinzufügen von Zeitplänen für Offlineseiten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Alle geplanten Offlineseiten deaktivieren
  
Durch diese Richtlinieneinstellung werden alle vorhandenen Zeitpläne deaktiviert, die zum Herunterladen von Webseiten eingerichtet wurden, damit diese offline angezeigt werden können. Wenn Sie diese Richtlinie aktivieren, werden im Dialogfeld **Eigenschaften der Webseite** auf der Registerkarte **Zeitplan** die Kontrollkästchen für Zeitpläne ausgeblendet, damit die Benutzer diese nicht aktivieren können. Benutzer klicken zum Anzeigen dieser Registerkarte im Menü **Extras** auf **Synchronisieren**, wählen eine Webseite aus, klicken dann auf die Schaltfläche **Eigenschaften** und schließlich auf die Registerkarte **Zeitplan**. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Alle geplanten Offlineseiten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Channel-Benutzeroberfläche vollständig deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die Channelleiste anzeigen können. Channels sind Websites, die auf Computern nach einem vom Channelanbieter vorgegebenen Zeitplan automatisch aktualisiert werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer daran gehindert, auf die Channelleiste zuzugreifen und im Dialogfeld **Eigenschaften von Anzeige** auf der Registerkarte **Web** das Kontrollkästchen **Internet Explorer-Channelleiste** zu aktivieren. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Channel-Benutzeroberfläche vollständig deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Download von abonnierten Siteinhalten deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer abonnierte Websiteinhalte herunterladen können. Dennoch erfolgt eine Überprüfung auf Aktualisierung und entsprechende Synchronisierung des Webseiteninhalts, wenn ein Benutzer zu einer zuvor aufgerufenen Seite zurückkehrt. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Download von abonnierten Siteinhalten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Zeitpläne für die Offlineansicht von abonnierten Webseiten und Webseitengruppen hinzufügen, bearbeiten oder entfernen können. Eine Abonnementgruppe besteht aus einer Favoritenwebseite sowie den damit verknüpften Webseiten. Wenn Sie diese Richtlinie aktivieren, werden im Dialogfeld **Eigenschaften der Webseite** auf der Registerkarte **Zeitplan** die Schaltflächen **Hinzufügen**, **Entfernen** und **Bearbeiten** abgeblendet dargestellt. Um diese Registerkarte anzuzeigen, klicken Benutzer im Menü **Extras** auf **Synchronisieren**, wählen eine Webseite aus, klicken dann auf die Schaltfläche **Eigenschaften** und schließlich auf die Registerkarte **Zeitplan**. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren** deshalb auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Bearbeiten von Zeitplänen für Offlineseiten deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer vorhandene Zeitpläne bearbeiten können, die festgelegt wurden, um Webseiten herunterzuladen und offline anzuzeigen. Wenn Sie diese Richtlinie aktivieren, können Benutzer keine Zeitplaneigenschaften von Seiten anzeigen, die für die Offlineansicht eingerichtet wurden. Es werden keine Eigenschaften angezeigt, wenn Benutzer in Internet Explorer im Menü **Extras** auf **Synchronisieren** klicken, eine Webseite auswählen und dann auf die Schaltfläche **Eigenschaften** klicken. Es wird keine Meldung angezeigt, dass der Befehl nicht verfügbar ist. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Bearbeiten von Zeitplänen für Offlineseiten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Trefferprotokollierung für Offlineseiten deaktivieren
  
Diese Richtlinieneinstellung nimmt Channelanbietern die Möglichkeit, aufzuzeichnen, wie oft ihre Channelseiten von Offlinebenutzern angezeigt werden. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Trefferprotokollierung für Offlineseiten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Entfernen von Channels deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die Channelsynchronisierung in Internet Explorer deaktivieren können. Es handelt sich um eine bewährte Methode, das Herunterladen von Seiten aus dem Internet auf einen Computer nur zu ermöglichen, wenn ein Benutzer diese Funktion direkt an diesem Computer anfordert.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Entfernen von Channels deaktivieren** deshalb auf **Aktiviert** gesetzt.
  
###### Offlineseiten\\Entfernen von Zeitplänen für Offlineseiten deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer vorkonfigurierte Einstellungen löschen können, die dafür sorgen, dass Webseiten für die Offlineansicht heruntergeladen werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden vorkonfigurierte Einstellungen für Webseiten geschützt. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Möglichkeit von Internet Explorer blockieren, Inhalt automatisch herunterzuladen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Offlineseiten\\Entfernen von Zeitplänen für Offlineseiten deaktivieren** auf **Aktiviert** gesetzt.
  
###### Konfigurieren von Outlook Express
  
Diese Richtlinieneinstellung ermöglicht es Administratoren, für Benutzer von Microsoft Outlook Express® festzulegen, ob sie Anlagen speichern oder öffnen können, die einen Virus enthalten könnten. Benutzer können die Einstellung **Outlook Express konfigurieren** nicht deaktivieren und damit die Sperrung von Anlagen nicht aufheben. Um diese Richtlinieneinstellung zu erzwingen, klicken Sie auf **Aktivieren**, und wählen Sie die Option **Anhänge sperren, die einen Virus enthalten können** aus.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Outlook Express konfigurieren** auf die Werte **Aktiviert** und **Anhänge sperren, die einen Virus enthalten können** gesetzt.
  
###### Einstellungen für die Seite "Erweitert" deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die Einstellungen auf der Registerkarte **Erweitert** im Dialogfeld **Internetoptionen** von Internet Explorer ändern können. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer keine erweiterten Einstellungen des Browsers in Bezug auf Sicherheit, Multimedia und Drucken ändern. Außerdem können sie die Kontrollkästchen dieser Optionen auf der Registerkarte **Erweitert** im Dialogfeld **Internetoptionen** nicht aktivieren oder deaktivieren. Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden.
  
Die Einstellung **Einstellungen für die Seite "Erweitert" deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
**Hinweis:** Wenn Sie die Einstellung **Seite "Erweitert" deaktivieren** (unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung) verwenden, müssen Sie diese Richtlinieneinstellung nicht konfigurieren, da durch die Einstellung **Seite "Erweitert" deaktivieren** die Registerkarte **Erweitert** aus dem Dialogfeld **Internetoptionen** entfernt wird.
  
###### Änderung der Einstellungen für die automatische Konfiguration deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer automatisch konfigurierte Einstellungen ändern können. Administratoren verwenden die automatische Konfiguration zur regelmäßigen Aktualisierung von Browsereinstellungen. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Einstellungen für die automatische Konfiguration in Internet Explorer abgeblendet. (Diese Einstellungen befinden sich im Bereich **Automatische Konfiguration** des Dialogfelds **Einstellungen für lokales Netzwerk (LAN)**.) Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden.
  
**So zeigen Sie das Dialogfeld „Einstellungen für lokales Netzwerk (LAN)“ an**
  
1.  Öffnen Sie das Dialogfeld **Internetoptionen**, und klicken Sie auf die Registerkarte **Verbindungen**.
  
2.  Klicken Sie auf die Schaltfläche **Einstellungen**, um die Einstellungen anzuzeigen.
  
Die Einstellung **Änderung der Einstellungen für die automatische Konfiguration deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
**Hinweis**: Durch die Einstellung **Verbindungsseite deaktivieren** (unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung) wird die Registerkarte **Verbindungen** aus Internet Explorer in der Systemsteuerung entfernt. Diese Einstellung hat Vorrang vor der Konfigurationsoption **Änderung der Einstellungen für die automatische Konfiguration deaktivieren**. Wenn Sie erstere Einstellung aktivieren, wird die letztere Einstellung ignoriert.
  
###### Änderung der Zertifikatseinstellungen deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Zertifikatseinstellungen in Internet Explorer ändern können. Zertifikate werden verwendet, um die Identität von Softwareherausgebern zu überprüfen. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Einstellungen im Bereich **Zertifikate** auf der Registerkarte **Inhalte** des Dialogfelds **Internetoptionen** deaktiviert. Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden.
  
Die Einstellung **Änderung der Zertifikatseinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
**Hinweis**: Wenn diese Richtlinieneinstellung aktiviert ist, können Benutzer weiterhin auf die Datei für Zertifikate von Softwareherausgebern (.spc) doppelklicken, um den Assistenten zum Importieren der Zertifikatverwaltung auszuführen. Dieser Assistent bietet Benutzern die Möglichkeit, noch nicht in Internet Explorer konfigurierte Einstellungen für Zertifikate von Softwareherstellern zu importieren und zu konfigurieren.
  
**Hinweis**: Durch die Einstellung **Verbindungsseite deaktivieren** (unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung) wird die Registerkarte **Verbindungen** aus Internet Explorer in der Systemsteuerung entfernt. Diese Einstellung hat Vorrang vor der Konfigurationsoption **Änderung der Zertifikatseinstellungen deaktivieren**. Wenn Sie erstere Einstellung aktivieren, wird die letztere Einstellung ignoriert.
  
###### Änderung der Verbindungseinstellungen deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer DFÜ-Einstellungen ändern können. Wenn Sie diese Richtlinieneinstellung aktivieren, wird die Schaltfläche **Einstellungen** auf der Registerkarte **Verbindungen** des Dialogfelds **Internetoptionen** deaktiviert. Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden. Für Benutzer von Laptopcomputern bietet es sich an, diese Einstellung zu deaktivieren, wenn sie z. B. auf Reisen die Verbindungseinstellungen ändern müssen.
  
Die Einstellung **Änderung der Verbindungseinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
**Hinweis**: Wenn Sie die Einstellung **Verbindungsseite deaktivieren** konfigurieren (unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung), müssen Sie diese Richtlinieneinstellung nicht konfigurieren. Durch die Einstellung **Verbindungsseite deaktivieren** wird die Registerkarte **Verbindungen** aus der Benutzeroberfläche entfernt.
  
###### Änderung der Proxyeinstellungen deaktivieren
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Proxyeinstellungen ändern können. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Proxyeinstellungen abgeblendet. (Die Proxyeinstellungen sind im Dialogfeld **Einstellungen für lokales Netzwerk (LAN)** im Bereich **Proxyserver** zu finden. Dieses Dialogfeld wird angezeigt, wenn der Benutzer im Dialogfeld **Internetoptionen** auf die Registerkarte **Verbindungen** und anschließend auf die Schaltfläche **Einstellungen für lokales Netzwerk (LAN)** klickt.) Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden. Für Benutzer von Laptopcomputern bietet es sich an, diese Einstellung zu deaktivieren, wenn sie z. B. auf Reisen die Verbindungseinstellungen ändern müssen.
  
Die Einstellung **Änderung der Proxyeinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung nicht konfiguriert.
  
**Hinweis**: Wenn Sie die Einstellung **Verbindungsseite deaktivieren** konfigurieren (unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung), müssen Sie diese Richtlinieneinstellung nicht konfigurieren. Durch die Einstellung **Verbindungsseite deaktivieren** wird die Registerkarte **Verbindungen** aus der Benutzeroberfläche entfernt.
  
###### Die Speicherung von Kennwörtern mit AutoVervollständigen nicht zulassen
  
Durch diese Richtlinieneinstellung wird das automatische Ausfüllen von Benutzernamen und Kennwörtern in Webseitenformularen und die Abfrage zur Kennwortspeicherung deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Kontrollkästchen **Benutzernamen und Kennwörter für Formulare** und **Nachfragen, ob Kennwörter gespeichert werden sollen** abgeblendet. Außerdem werden die Benutzer daran gehindert, Kennwörter lokal zu speichern. Benutzer können sich diese Kontrollkästchen anzeigen lassen, indem sie das Dialogfeld **Internetoptionen** öffnen, zur Registerkarte **Inhalte** wechseln und dann auf die Schaltfläche **AutoVervollständigen** klicken.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Die Speicherung von Kennwörtern mit AutoVervollständigen nicht zulassen** auf **Aktiviert** gesetzt.
  
##### Anlagen-Manager
  
Die folgenden empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**Anlagen-Manager**
  
In der folgenden Tabelle sind die empfohlenen Benutzerkonfigurationseinstellungen für den Anlagen-Manager zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.28: Empfohlene Benutzerkonfigurationseinstellungen für den Anlagen-Manager**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer</th>
<th>SSLF-Computer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zoneninformationen nicht in Dateianhängen aufbewahren</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Mechanismen zum Entfernen von Zoneninformationen ausblenden</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beim Öffnen von Anhängen Antivirusprogramme benachrichtigen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### Zoneninformationen nicht in Dateianhängen aufbewahren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows-Dateianhänge von Internet Explorer oder Outlook Express mit Informationen zu deren Ursprungszone (wie z. B. eingeschränkt, Internet, Intranet oder lokal) markiert werden. Für das richtige Funktionieren dieser Einstellung ist es erforderlich, dass Dateien auf NTFS-Festplattenpartitionen heruntergeladen werden. Wenn Zoneninformationen nicht aufbewahrt werden, kann Windows keine geeigneten Risikoanalysen auf der Grundlage der Zone durchführen, welcher der Anhang entstammt.
  
Wenn die Einstellung **Zoneninformationen nicht in Dateianhängen aufbewahren** aktiviert ist, werden Dateianhänge nicht mit ihren Zoneninformationen gekennzeichnet. Wenn diese Richtlinieneinstellung deaktiviert ist, ist Windows gezwungen, Dateianhänge mit ihren Zoneninformationen zu speichern. Da gefährliche Anhänge oft von nicht vertrauenswürdigen Internet Explorer-Zonen wie z. B. der Internetzone heruntergeladen werden, empfiehlt Microsoft, diese Einstellung auf **Deaktiviert** zu setzen. Dadurch wird sichergestellt, dass zu jeder Datei so viele Sicherheitsinformationen wie möglich aufbewahrt werden.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Zoneninformationen nicht in Dateianhängen aufbewahren** auf **Deaktiviert** gesetzt.
  
###### Mechanismen zum Entfernen von Zoneninformationen ausblenden
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer manuell Zoneninformationen von gespeicherten Dateianlagen entfernen können. Normalerweise können Benutzer entweder auf der Seite **Eigenschaften** der Datei auf die Schaltfläche **Zulassen** klicken oder ein Kontrollkästchen im Dialogfeld **Sicherheitswarnung** aktivieren. Das Entfernen von Zoneninformationen ermöglicht es Benutzern, potenziell gefährliche Dateianhänge zu öffnen, obwohl Windows dies zuvor verhindert hat.
  
Wenn die Einstellung **Mechanismen zum Entfernen von Zoneninformationen ausblenden** aktiviert ist, blendet Windows das Kontrollkästchen und die Schaltfläche **Zulassen** aus. Wenn diese Richtlinieneinstellung deaktiviert ist, zeigt Windows das Kontrollkästchen und die Schaltfläche **Zulassen** an. Da gefährliche Anhänge oft von nicht vertrauenswürdigen Internet Explorer-Zonen wie z. B. der Internetzone heruntergeladen werden, empfiehlt Microsoft, diese Richtlinieneinstellung auf **Deaktiviert** zu setzen. Dadurch wird sichergestellt, dass zu jeder Datei so viele Sicherheitsinformationen wie möglich aufbewahrt werden.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Mechanismen zum Entfernen von Zoneninformationen** auf **Aktiviert** gesetzt.
  
**Hinweis**: Informationen dazu, wie Sie festlegen können, ob Dateien mit Zoneninformationen gespeichert werden, finden Sie in den vorangegangenen Ausführungen zur Einstellung **Zoneninformationen nicht in Dateianhängen aufbewahren**.
  
###### Beim Öffnen von Anhängen Antivirusprogramme benachrichtigen
  
Antivirusprogramme sind in vielen Umgebungen obligatorisch und stellen einen sehr guten Schutz gegen aktuelle Angriffsmethoden dar.
  
Die Einstellung **Beim Öffnen von Anhängen Antivirusprogramme benachrichtigen** ermöglicht es Ihnen festzulegen, wie registrierte Antivirusprogramme benachrichtigt werden. Wenn diese Richtlinieneinstellung aktiviert ist, ruft Windows das registrierte Antivirenprogramm auf und überprüft Dateianhänge, wenn sie von Benutzern geöffnet werden. Wenn der Virenscan fehlschlägt, wird das Öffnen der Anhänge verhindert. Wenn diese Richtlinieneinstellung deaktiviert ist, ruft Windows das registrierte Antivirenprogramm nicht auf, wenn Dateianhänge geöffnet werden. Um sicherzustellen, dass Antivirusprogramme jede Datei vor dem Öffnen untersuchen, empfiehlt Microsoft, diese Richtlinie in allen Umgebungen auf **Aktiviert** zu setzen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Beim Öffnen von Anhängen Antivirusprogramme benachrichtigen** auf **Aktiviert** gesetzt.
  
**Hinweis**: Für das richtige Funktionieren dieser Einstellung muss ein aktualisiertes Antivirenprogramm installiert werden. Viele aktualisierte Antivirusprogramme verwenden neue APIs, die in SP2 enthalten sind.
  
##### Windows Explorer
  
Windows Explorer wird auf Clients mit Windows XP Professional dazu verwendet, durch das Dateisystem zu navigieren.
  
Die folgenden empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**Windows Explorer**
  
In der folgenden Tabelle sind die empfohlenen Benutzerkonfigurationseinstellungen für Windows Explorer zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle 4.29: Empfohlene Benutzerkonfigurationseinstellungen für Windows Explorer**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer</th>
<th>SSLF-Computer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CD-Brennfunktionen entfernen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Registerkarte &quot;Sicherheit&quot; entfernen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
###### CD-Brennfunktionen entfernen
  
Durch diese Richtlinieneinstellung werden die integrierten Windows XP-Funktionen entfernt, die es Benutzern erlauben, CDs mithilfe von Windows Explorer zu brennen. Windows XP ermöglicht es Ihnen, wiederbeschreibbare CDs zu erstellen und zu ändern, wenn an Ihren Computer ein CD-Brenner angeschlossen ist. Mit dieser Funktion können große Datenmengen von einer Festplatte auf eine CD kopiert werden, die aus dem Computer genommen werden kann.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **CD-Brennfunktionen entfernen** auf **Nicht konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt.
  
**Hinweis**: Durch diese Richtlinieneinstellung wird nicht verhindert, dass Anwendungen von Drittanbietern CDs mit einem CD-Brenner erstellen oder ändern können. Dieses Handbuch empfiehlt die Verwendung von Richtlinien für Softwareeinschränkungen, um die Erstellung oder Änderung von CDs durch Anwendungen von Drittanbietern zu blockieren. Weitere Informationen finden Sie in Kapitel 6, „Richtlinie für Softwareeinschränkungen auf Windows XP-Clients“.
  
Eine weitere Möglichkeit, Benutzer am Brennen von CDs zu hindern, besteht darin, die CD-Brenner aus den Clientcomputern Ihrer Umgebung zu entfernen oder sie durch CD-ROM-Laufwerke zu ersetzen, die nicht für das Brennen genutzt werden können.
  
###### Registerkarte "Sicherheit" entfernen
  
Durch diese Richtlinieneinstellung wird in Windows Explorer die Registerkarte **Sicherheit** in den Eigenschaftendialogfeldern für Dateien und Verzeichnisse deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer bei allen Dateisystemobjekten (wie Ordnern, Dateien, Verknüpfungen und Laufwerken) daran gehindert, im Dialogfeld **Eigenschaften** auf die Registerkarte **Sicherheit** zuzugreifen. Da die Registerkarte **Sicherheit** nicht verfügbar ist, können Benutzer weder Einstellungen ändern noch die Liste der Benutzer anzeigen.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Registerkarte "Sicherheit" entfernen** deshalb auf **Nicht** **konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt.
  
#### System
  
Die folgende Abbildung illustriert die Abschnitte in der Gruppenrichtlinie, die von den Einstellungsänderungen im Abschnitt System betroffen sein werden:
  
![](images/Cc163076.SGFG0407(de-de,TechNet.10).gif)
  
**Abbildung 4.7: Gruppenrichtlinienstruktur für das System unter Benutzerkonfiguration**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163076.sgfg0407_big(de-de,technet.10).gif)
  
Die folgende empfohlene Einstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\System**
  
##### Zugriff auf Programme zum Bearbeiten der Registrierung verhindern
  
In der folgenden Tabelle sind die empfohlenen Benutzerkonfigurationseinstellungen für den Registrierungs-Editor zusammengefasst.
  
**Tabelle 4.30: Empfohlene Benutzerkonfigurationseinstellungen für den Registrierungs-Editor**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer</th>
<th>SSLF-Computer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zugriff auf Programme zum Bearbeiten der Registrierung verhindern</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
Durch diese Richtlinieneinstellung werden die Registrierungs-Editoren von Windows, REGEDIT.EXE und REGEDT32.EXE, deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, wird eine Meldung angezeigt, wenn Benutzer versuchen, einen Registrierungs-Editor zu verwenden. Mit dieser Meldung werden die Benutzer darüber informiert, dass sie keinen dieser Editoren verwenden können. Diese Richtlinieneinstellung sorgt dafür, dass Benutzer und Eindringlinge nicht mit diesen Tools auf die Registrierung zugreifen können, verhindert aber nicht den Zugriff auf die Registrierung selbst.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Zugriff auf Programme zum Bearbeiten der Registrierung verhindern** auf **Nicht konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt.
  
##### System\\Energieverwaltung
  
Die folgende empfohlene Einstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\System\\Energieverwaltung**
  
###### Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus
  
In der folgenden Tabelle sind die empfohlenen Konfigurationseinstellungen für **Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus** zusammengefasst.
  
**Tabelle 4.31: Empfohlene Benutzerkonfigurationseinstellungen für „System\\Energieverwaltung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer</th>
<th>SSLF-Computer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Clientcomputer in Ihrer Umgebung gesperrt werden, wenn sie aus dem Ruhezustand oder Standbymodus zurückkehren. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Clientcomputer gesperrt, wenn sie in den Betriebsmodus zurückkehren. Benutzer müssen ihr Kennwort eingeben, um die Sperre aufzuheben. Es können potenziell schwerwiegende Sicherheitsverletzungen auftreten, wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert wird, denn dadurch kann jeder auf die Clientcomputer zugreifen.
  
Für die beiden in diesem Kapitel behandelten Umgebungen ist die Einstellung **Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus** deshalb auf **Aktiviert** gesetzt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurden viele der wichtigsten Sicherheitseinstellungen beschrieben, die in den administrativen Vorlagen von Windows XP zur Verfügung stehen. Mithilfe dieser Vorlagen können Sie in Ihrer Organisation Desktops und Laptops mit Windows XP sichern. Wenn Sie für Ihre Organisation Überlegungen zu den Richtlinien für Sicherheitseinstellungen anstellen, bedenken Sie die Wechselwirkungen zwischen Sicherheit und Benutzerproduktivität. Ziel ist es, Ihre Benutzer in einer sicheren Umgebung vor schädlichen Programmen und Viren zu schützen und es ihnen zu ermöglichen, ihre Arbeit zu erledigen, ohne dass sie durch übermäßig einschränkende Sicherheitseinstellungen behindert werden.
  
#### Weitere Informationen
  
Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen hinsichtlich Windows XP Professional.
  
-   Eine vollständige Auflistung aller unter Windows XP und Windows Server 2003 verfügbaren Gruppenrichtlinieneinstellungen für administrative Vorlagen bietet die Arbeitsmappe „[Informationen zu Gruppenrichtlinieneinstellungen für Windows Server 2003 mit Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=7821c32f-da15-438d-8e48-45915cd2bc14&displaylang=en)“ (in englischer Sprache) unter www.microsoft.com/downloads/details.aspx?FamilyId=7821C32F-DA15-438D-8E48-45915CD2BC14.
  
-   Informationen zum Erstellen Ihrer eigenen administrativen Vorlagen finden Sie im Whitepaper „[Implementieren registrierungsbasierter Gruppenrichtlinien](http://www.microsoft.com/windows2000/techinfo/howitworks/management/rbppaper.asp)“ (in englischer Sprache) unter  
    www.microsoft.com/windows2000/techinfo/howitworks/management/rbppaper.asp.
  
-   Informationen zur Fehlerberichterstattung finden Sie auf der Website [Corporate Error Reporting](http://www.microsoft.com/resources/satech/cer/) (in englischer Sprache) unter www.microsoft.com/resources/satech/cer/.
  
-   Allgemeine Informationen zu den Windows Server Update Services (WSUS) finden Sie in [Windows Server Update Services Product Overview](http://www.microsoft.com/windowsserversystem/updateservices/evaluation/overview.mspx) (in englischer Sprache) unter  
    www.microsoft.com/windowsserversystem/updateservices/evaluation/overview.mspx.
  
-   Weitere Informationen zum Bereitstellen von WSUS finden Sie unter [Bereitstellen von Microsoft Windows Server Update Services](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/wsus/wsusdeploymentguidetc/) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/WSUS/WSUSDeploymentGuideTC/.
  
-   Weitere Informationen zur Gruppenrichtlinienverwaltung finden Sie in [Unternehmensmanagement mit der Managementkonsole für Gruppenrichtlinien](http://www.microsoft.com/windowsserver2003/gpmc/default.mspx) (in englischer Sprache) unter www.microsoft.com/windowsserver2003/gpmc/.
  
-   Links zu Artikeln, in denen die Verwendung der Sicherheitseinstellungen und Funktionen in Office 2003 erklärt wird, finden Sie auf Hauptseite zum Thema [Sicherheit](http://office.microsoft.com/en-us/assistance/ha011403061033.aspx) in Office 2003 (in englischer Sprache) unter  
    http://office.microsoft.com/en-us/assistance/HA011403061033.aspx.
  
-   „[Office 2003 Resource Kit toolset](http://download.microsoft.com/download/0/e/d/0eda9ae6-f5c9-44be-98c7-ccc3016a296a/ork.exe)“ umfasst „Office 2003 Policy Template Files and Deployment Planning Tools“ sowie eine Reihe anderer nützlicher Programme für die Bereitstellung und Verwaltung von Office 2003: http://download.microsoft.com/download/0/e/d/0eda9ae6-f5c9-44be-98c7-ccc3016a296a/ork.exe.
  
-   Weitere Informationen zum [*Internet Explorer Administration Kit*](http://www.microsoft.com/technet/prodtechnol/ie/ieak/) finden Sie (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/ie/ieak/.
  
##### In diesem Beitrag
  
-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/default.mspx)  
-   [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch01.mspx)  
-   [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch02.mspx)  
-   [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch03.mspx)  
-   Kapitel 4: Administrative Vorlagen für Windows XP  
-   [Kapitel 5: Schützen eigenständiger Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch05.mspx)  
-   [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch06.mspx)  
-   [Kapitel 7: Zusammenfassung](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch07.mspx)  
-   [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)  
-   [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxa.mspx)  
-   [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxb.mspx)  
-   [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgack.mspx)
  
##### Download
  
[![](images/Cc163076.icon_exe(de-de,TechNet.10).gif)Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
