---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5'
ms:assetid: '30aec6b9-6584-4724-8f8e-46357eecddd6'
ms:contentKeyID: 20075620
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443677(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen
=========================================================================

### Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5

Veröffentlicht: 11. Nov 2007

Die Einstellungen im folgenden Abschnitt sind nach Namen aufgeführt.

##### Auf dieser Seite

[Informationen zu Benutzerrichtlinieneinstellungen](#ecd)

Informationen zu Benutzerrichtlinieneinstellungen
-------------------------------------------------

Für jede Einstellung werden neben einer Beschreibung auch Informationen über die betroffenen Anwendungen, das behandelte Sicherheitsrisiko, die Art und Weise, in der das Sicherheitsrisiko behandelt wird, und eventuelle andere Erwägungen bereitgestellt. Darüber hinaus ist für jede Einstellung eine Tabelle enthalten, die den Speicherort der Einstellung in der Gruppenrichtlinie, die ADM-Datei mit der Einstellung sowie die empfohlene Konfiguration für EC- und SSLF-Umgebungen aufführt.

### Ausgeblendete Markups anzeigen

Betrifft: **PowerPoint**

Diese Einstellung steuert, ob ausgeblendetes Markup beim Öffnen von PowerPoint-Dateien im Standard- oder HTML-Format sichtbar ist.

#### Sicherheitsrisiko

PowerPoint-Präsentationen, die im Standard- oder HTML-Format gespeichert sind, können ein Kennzeichen enthalten, das festlegt, ob Markup (Kommentare oder Freihandanmerkungen) in einer geöffneten Präsentation sichtbar ist. Standardmäßig ignoriert PowerPoint 2007 dieses Kennzeichen beim Öffnen einer Datei und zeigt jegliches in der Datei vorhandenen Markup an. Darüber hinaus richtet PowerPoint beim Speichern einer Datei das Kennzeichen so ein, dass Markup beim nächsten Öffnen der Präsentation angezeigt wird.

Wenn diese Standardkonfiguration geändert wird, stellt PowerPoint beim Speichern von Präsentationen im Standard- oder HTML-Format das Kennzeichen je nach Status der Option **Markup anzeigen** auf der Registerkarte **Überprüfen** ein. Darüber hinaus aktiviert oder deaktiviert PowerPoint beim Öffnen von Dateien die Option **Markup anzeigen** je nach der Art und Weise, in der das Kennzeichen eingerichtet ist. Das bedeutet, dass eine Präsentation, die mit ausgeblendetem Markup gespeichert wurde, auch mit ausgeblendetem Markup geöffnet wird.

Wenn eine Datei mit ausgeblendetem Markup gespeichert wird, verteilen Benutzer über die Präsentationsdatei möglicherweise unabsichtlich vertrauliche Kommentare oder Informationen an andere.

#### Gegenmaßnahme

Wenn diese Einstellung **aktiviert** ist, macht PowerPoint beim Öffnen von Präsentation jegliches ausgeblendete Markup sichtbar. Diese Funktionalität stellt sicher, dass Benutzer vor dem Verteilen von Dateien wissen, dass ausgeblendetes Markup in der Präsentation vorhanden ist.

**Tabelle 1.170: Ausgeblendete Markups anzeigen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office PowerPoint 2007\PowerPoint-Optionen\Sicherheit</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>ppt12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1279</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Wenn diese Einstellung **aktiviert** ist, wird ausgeblendetes Markup beim Öffnen der Datei sichtbar. Wenn Benutzer beabsichtigen, Markup auszublenden, müssen sie dieses erneut ausblenden. (Benutzer können mithilfe der Funktion „Dokumentinspektor“ in PowerPoint 2007 nach unerwünschtem Markup suchen und dieses endgültig entfernen.) Die Aktivierung dieser Einstellung setzt die Standardkonfiguration in PowerPoint 2007 durch.
  
In den meisten Fällen sollte Markup für Benutzer sichtbar sein. Markup wird in PowerPoint nicht im Präsentationsmodus angezeigt, selbst wenn es im Entwurfsmodus sichtbar ist, deshalb dürfte diese Einstellung nur minimale Auswirkungen auf die Nutzbarkeit haben.
  
### Outlook als Standardprogramm für E-Mail, Kontakte und Kalender einrichten
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 das Standardprogramm für E-Mail, Kontakte und Kalenderdienste ist.
  
#### Sicherheitsrisiko
  
Standardmäßig wird Outlook 2007 bei der Installation als Standardprogramm für E-Mail, Kontakte und Kalenderdienste festgelegt, aber Benutzer können auch andere Programme als Standardprogramm für diese Dienste auswählen. Wenn eine andere Anwendung für die Bereitstellung dieser Dienste verwendet wird und Ihr Unternehmen die Sicherheit der Anwendung nicht sicherstellt, kann diese möglicherweise ausgenutzt werden, um auf vertrauliche Daten zuzugreifen oder andere schädliche Angriffe durchzuführen.
  
Wenn das Unternehmen über Richtlinien für die Regelung der Verwendung von Software für die Verwaltung persönlicher Daten verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn eine Änderung der Standardkonfiguration durch Benutzer zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, ist das Kontrollkästchen **Outlook als Standardprogramm für E-Mail, Kontakte und Kalender einrichten** auf der Registerkarte **Weitere** des Dialogfelds **Outlook-Optionen** aktiviert, und Benutzer können diese Einstellung nicht ändern.
  
Wenn die Einstellung deaktiviert ist, können Benutzer Outlook 2007 nicht als Standardprogramm für diese Dienste festlegen.
  
**Tabelle 1.171: Outlook als Standardprogramm für E-Mail, Kontakte und Kalender einrichten**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Weitere</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1111</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
In den meisten Umgebungen, in denen Microsoft Office System eingesetzt wird, ist Outlook für den Großteil der Benutzer häufig bereits als Standardprogramm für E-Mail, Kontakte und Kalender eingerichtet. Daher dürfte die Aktivierung dieser Einstellung keine Nutzbarkeitsprobleme verursachen.
  
### Nachrichtenformate
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, welche Nachrichtenverschlüsselungsformate Outlook 2007 verwenden kann.
  
#### Sicherheitsrisiko
  
E-Mail-Nachrichten werden in der Regel über offene Netzwerke übertragen und von Server zu Server weitergegeben. Deshalb besteht für Nachrichten das Risiko, dass sie abgefangen werden und Angreifer ihre Inhalte lesen oder ändern können. Daher sollten Sie unbedingt einen Mechanismus für das Signieren von Nachrichten und das Bereitstellen einer End-to-End-Verschlüsselung einrichten.
  
Outlook 2007 unterstützt drei Formate für das Verschlüsseln und Signieren von Nachrichten: S/MIME, Exchange und Fortezza. Standardmäßig verwendet Outlook für das Verschlüsseln und Signieren von Nachrichten nur S/MIME. Wenn das Unternehmen über Richtlinien verfügt, die das Verwenden bestimmter Verschlüsselungsformate vorschreiben, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn zugelassen wird, dass Benutzer das jeweilige Format frei auswählen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren angeben, ob Outlook 2007 S/MIME (die Standardoption), Exchange oder Fortezza bzw. eine beliebige Kombination dieser drei Optionen für die Verschlüsselung verwenden kann.
  
**Tabelle 1.172: Nachrichtenformate**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (S/MIME)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (S/MIME und Fortezza)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-IDs</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1357, CCE-1132</p></td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die empfohlene Einstellung für die EC-Umgebung ändert die Standardkonfiguration nicht und sollte sich deshalb nicht auf Endbenutzer auswirken. Das Signieren und Verschlüsseln bedeutet eine zusätzliche Leistungsbelastung, daher werden Benutzer in vielen Fällen nur E-Mail-Nachrichten mit sensiblen oder vertraulichen Inhalten auf diese Weise versenden.
  
Die empfohlene Einstellung für die SSLF-Umgebung bietet zudem Unterstützung für Fortezza, einen hardwarebasierten Verschlüsselungsstandard, der von der National Security Agency (NSA), einer Behörde des amerikanischen Verteidigungsministeriums, entwickelt wurde. Wenn Ihr Unternehmen Fortezza nutzt, müssen Sie Outlook die erforderliche Unterstützung für Fortezza mithilfe dieser Einstellung hinzuzufügen. Die empfohlene SSLF-Konfiguration unterstützt weiterhin auch S/MIME, deshalb sollte die Implementierung dieser Empfehlung keine Beeinträchtigung für Benutzer bedeuten, die Zugriff auf die S-MIME-Verschlüsselung und -Signierung in Outlook 2007 benötigen.
  
### Mindestverschlüsselungseinstellungen
  
Betrifft: **Outlook**
  
Mithilfe dieser Einstellung können Administratoren eine Mindestschlüsselgröße festlegen, die für die Verschlüsselung von E-Mail-Nachrichten in Outlook 2007 verwendet werden soll.
  
#### Sicherheitsrisiko
  
Nachrichten werden für die Übertragung über ungesicherte Kanäle mithilfe kryptografischer Schlüssel ver- und entschlüsselt. Die Schlüsselgrößen werden in Bit gemessen, wobei größere Schlüssel in der Regel weniger anfällig für Angriffe sind als kleinere. Früher waren 40-Bit- und 56-Bit-Schlüssel üblich, aber mit der Verbreitung schnellerer und leistungsstärkerer Computer wurden diese kleineren Schlüsselgrößen anfällig für Brute-Force-Angriffe, bei denen der angreifende Computer mit hoher Geschwindigkeit sämtliche möglichen Schlüsselkombinationen durchläuft, bis die Nachricht erfolgreich entschlüsselt wird. Der von der US-Regierung veröffentlichte Advanced Encryption Standard (AES) erfordert eine Mindestschlüsselgröße von 128 Bit für die symmetrische Verschlüsselung und bietet damit bedeutend mehr Schutz vor Brute-Force-Angriffen als kleinere Schlüsselgrößen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Administratoren eine Mindestschlüsselgröße (in Bit) eingeben, die Outlook 2007 für die symmetrische Verschlüsselung verwendet. Wenn Benutzer eine Schlüsselgröße auswählen, die unter dieser Mindestgröße liegt, zeigt Outlook ein Warndialogfeld an.
  
**Tabelle 1.173: Mindestverschlüsselungseinstellungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (128)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (256)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-13</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Da Benutzer, denen das Warndialogfeld zur Mindestverschlüsselung angezeigt wird, trotzdem entscheiden können, die Nachricht mit dem ausgewählten Schlüssel zu versenden, wird die Aktivierung dieser Einstellung vermutlich keine wesentlichen Beeinträchtigungen verursachen.
  
Die 128-Bit-Verschlüsselung ist seit einigen Jahren weit verbreitet. Daher dürfte die Aktivierung dieser Einstellung keine Nutzbarkeitsprobleme für Benutzer verursachen.
  
### Fehlende Zertifikatsperrlisten
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007 eine fehlende Zertifikatsperrliste als Grund für eine Warnung oder eine Fehlermeldung betrachtet.
  
#### Sicherheitsrisiko
  
Digitale Zertifikate enthalten ein Attribut, das den Speicherort der entsprechenden Zertifikatsperrliste angibt. Zertifikatsperrlisten enthalten Listen mit digitalen Zertifikaten, die von ihren Zertifizierungsstellen gesperrt wurden, normalerweise weil die Zertifikate nicht ordnungsgemäß ausgestellt oder die damit verbundenen privaten Schlüssel beschädigt wurden.
  
Wenn eine Zertifikatsperrliste fehlt oder nicht verfügbar ist, kann Outlook 2007 nicht bestimmen, ob ein Zertifikat gesperrt wurde. Daher könnte ein nicht ordnungsgemäß ausgestelltes oder beschädigtes Zertifikat verwendet werden, um Zugriff auf Daten zu erhalten.
  
Standardmäßig zeigt Outlook eine Warnmeldung an, wenn eine Zertifikatsperrliste nicht verfügbar ist.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren zwei Optionen zur Verfügung, mit denen sie die Funktionsweise von Outlook 2007 bestimmen können, wenn eine Zertifikatsperrliste fehlt:
  
-   **Warnung**. Diese Option ist die Standardkonfiguration in Outlook 2007, die sicherstellt, dass Outlook eine Warnmeldung anzeigt, wenn eine Zertifikatsperrliste fehlt.
  
-   **Fehler**. Diese Option sorgt dafür, dass Outlook eine Fehlermeldung anzeigt, wenn eine Zertifikatsperrliste fehlt.
  
**Tabelle 1.174: Fehlende Zertifikatsperrlisten**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie\Dialogfeld „Signaturstatus“</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Fehler)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Fehler)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-IDs</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1662, CCE-1080</p></td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die empfohlene Einstellung für EC- und SSLF-Umgebungen ist **aktiviert**. Gleichzeitig sollte in der Dropdownliste die Option **Fehler** ausgewählt werden. Diese Konfiguration verhindert, dass Outlook 2007-Benutzer Zertifikate verwenden, wenn die entsprechende Zertifikatsperrliste nicht zu deren Überprüfung zur Verfügung steht, was zu vermehrten Anfragen an den Desktopsupport führen könnte.
  
### Fehlende Stammzertifikate
  
Betrifft: **Outlook**
  
Diese Einstellung steuert die Funktionsweise von Outlook 2007, wenn ein Stammzertifikat fehlt.
  
#### Sicherheitsrisiko
  
Beim Zugriff auf ein Zertifikat überprüft Outlook 2007, ob das Zertifikat vertrauenswürdig ist, indem das Stammzertifikat der ausstellenden Zertifizierungsstelle überprüft wird. Wenn das Stammzertifikat vertrauenswürdig ist, sind es auch die von der Zertifizierungsstelle ausgestellten Zertifikate.
  
Wenn Outlook das Stammzertifikat nicht finden kann, ist eine Überprüfung der Vertrauenswürdigkeit der von dieser Zertifizierungsstelle ausgestellten Zertifikate nicht möglich. Ein Angreifer könnte ein Stammzertifikat beschädigen und es dann entfernen, um den Angriff möglichst zu verbergen.
  
Standardmäßig erhalten Benutzer weder eine Warnung noch eine Fehlermeldung, wenn kein Stammzertifikat gefunden wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen zur Verfügung, um die Funktionsweise von Outlook 2007 zu bestimmen, wenn ein Stammzertifikat fehlt:
  
-   **Weder Fehler noch Warnung**. Diese Option zeigt weder eine Fehlermeldung noch eine Warnung an und setzt die Standardkonfiguration in Outlook 2007 durch.
  
-   **Warnung**. Diese Option stellt sicher, dass Outlook eine Warnmeldung anzeigt, wenn ein Stammzertifikat fehlt.
  
-   **Fehler**. Diese Option stellt sicher, dass Outlook eine Fehlermeldung anzeigt, wenn ein Stammzertifikat fehlt.
  
**Tabelle 1.175: Fehlende Stammzertifikate**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie\Dialogfeld „Signaturstatus“</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Warnung)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Warnung)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-IDs</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1076, CCE-1636</p></td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Outlook 2007-Benutzer Zertifikate verwenden, wenn das entsprechende Stammzertifikat zu deren Überprüfung nicht zur Verfügung steht, was zu vermehrten Anfragen an den Desktopsupport führen könnte.
  
### Nur modale Vertrauensentscheidung
  
Betrifft: **Access**
  
Diese Einstellung steuert, wie Access 2007 Benutzer über nicht vertrauenswürdige Komponenten benachrichtigt.
  
#### Sicherheitsrisiko
  
Wenn Benutzer eine nicht vertrauenswürdige Access 2007-Datenbank öffnen, die von Benutzern programmierte ausführbare Komponenten enthält, öffnet Access die Datenbank standardmäßig mit deaktivierten Komponenten und zeigt in der Statusleiste eine Warnung an, die den Benutzer informiert, dass Datenbankinhalte deaktiviert wurden. Benutzer können die Inhalte der Datenbank überprüfen, deaktivierte Funktionen aber erst verwenden, wenn sie diese aktivieren, indem sie auf **Optionen** in der Statusleiste klicken und die entsprechende Aktion auswählen.
  
Die Standardkonfiguration kann geändert werden, sodass Benutzern beim Öffnen einer nicht vertrauenswürdigen Datenbank mit ausführbaren Komponenten ein Dialogfeld angezeigt wird. Benutzer müssen dann auswählen, ob sie die Komponenten aktivieren oder deaktivieren möchten, bevor sie mit der Datenbank arbeiten. Benutzer aktivieren die Komponenten in solchen Fällen häufig, auch wenn sie diese nicht benötigen. Ausführbare Komponenten können verwendet werden, um einen Angriff auf eine Computerumgebung zu starten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, deaktiviert Access 2007 die ausführbaren Komponenten und zeigt in einer Statusleistenwarnung an, dass Datenbankinhalte deaktiviert wurden.
  
**Tabelle 1.176: Nur modale Vertrauensentscheidung**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Access 2007\Extras | Sicherheit</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>access12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1214</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die Standardkonfiguration für Access 2007 durch und sollte daher keine Nutzbarkeitsprobleme verursachen. Allerdings hat sich diese Funktionalität gegenüber früheren Versionen von Access geändert. In Access 2003 wurde dem Benutzer bei der Standardkonfiguration ein Dialogfeld bereitgestellt (entsprechend der Funktionsweise von Access 2007, wenn die Einstellung aktiviert ist).
  
### Benutzer können nie Gruppen angeben, wenn die Berechtigung für Dokumente eingeschränkt wird
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer Berechtigungen für Verteilerlisten zuweisen können, wenn die Verwaltung von Informationsrechten (IRM) verwendet wird.
  
#### Sicherheitsrisiko
  
Standardmäßig können 2007 Office-Benutzer bei Anwendung der Verwaltung von Informationsrechten Verteilerlisten angeben, um den Zugriff auf Excel 2007-Arbeitsmappen, InfoPath 2007-Vorlagen, Outlook 2007-E-Mail-Nachrichten, PowerPoint 2007-Präsentationen oder Word 2007-Dokumente einzuschränken. Wenn Benutzer die Mitgliedschaft der Verteilerliste nicht vollständig kennen, bevor sie diese Berechtigungen für das Öffnen oder Ändern eines Dokuments zuweisen, besteht ein Sicherheitsrisiko für vertrauliche Daten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Benutzer im Dialogfeld **Berechtigungen** eine Verteilerliste nicht als autorisierte Partei angeben.
  
**Tabelle 1.177: Benutzer können nie Gruppen angeben, wenn die Berechtigung für Dokumente eingeschränkt wird**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1589</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung kann zu Beeinträchtigungen für 2007 Office-Benutzer führen, die daran gewöhnt sind, bei der Festlegung von Berechtigungen für ein Dokument Verteilergruppen anzugeben. Diese Benutzer müssen Benutzer im Dialogfeld **Berechtigungen** einzeln auflisten, um ihnen die Berechtigung zum Lesen oder Ändern des Dokuments zuzuweisen. Benutzer, die die Verwaltung von Informationsrechten nicht verwenden, sind von dieser Einstellung nicht betroffen.
  
### Offlinemodusstatus
  
Betrifft: **InfoPath**
  
Diese Einstellung bestimmt die Konfiguration des Offlinemodus in InfoPath 2007.
  
#### Sicherheitsrisiko
  
InfoPath 2007 kann im Online- oder Offlinemodus arbeiten. Das Programm kann außerdem Abfragen für eine Nutzung im Offlinemodus zwischenspeichern. Wenn der Offlinemodus verwendet wird und zwischengespeicherte Abfragen aktiviert werden, besteht ein Sicherheitsrisiko für vertrauliche Daten im Zwischenspeicher.
  
Standardmäßig arbeitet InfoPath im Onlinemodus, aber der Offlinemodus steht Benutzern ebenfalls zur Verfügung. Benutzer können außerdem Abfragen für die Verwendung im Offlinemodus zwischenspeichern.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, müssen Administratoren einen Offlinemodusstatus auswählen. Die folgenden Optionen sind verfügbar:
  
-   **Deaktiviert**. Wenn diese Option aktiviert ist, startet InfoPath 2007 im Onlinemodus, und der Offlinemodus kann nicht ausgewählt werden.
  
-   **InfoPath im Offlinemodus**. Wenn diese Option aktiviert ist, startet InfoPath 2007 im Offlinemodus und speichert Abfragen für die Verwendung im Offlinemodus zwischen. Der Benutzer kann bei Bedarf den Onlinemodus auswählen.
  
-   **InfoPath nicht im Offlinemodus**. Wenn diese Option aktiviert ist, startet InfoPath 2007 im Onlinemodus, aber der Benutzer kann bei Bedarf den Offlinemodus auswählen. InfoPath speichert Abfragen für die Verwendung im Offlinemodus zwischen.
  
**Tabelle 1.178: Offlinemodusstatus**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Extras | Optionen\Erweitert\Offline</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>inf12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Aktiviert, InfoPath nicht im Offlinemodus)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Deaktiviert)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-569</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die EC-Umgebung ist **aktiviert**, wobei in der Dropdownliste die Option **Aktiviert, InfoPath nicht im Offlinemodus** ausgewählt sein sollte. Diese Konfiguration verhindert, dass InfoPath 2007-Benutzer die Option **Abfragen zur Verwendung im Offlinemodus zwischenspeichern** ändern.
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **aktiviert**, wobei in der Dropdownliste die Option **Deaktiviert** ausgewählt sein sollte. Diese Konfiguration bedeutet, dass Benutzer InfoPath überhaupt nicht im Offlinemodus verwenden können.
  
### Onlineinhaltoptionen
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob das 2007 Office-Hilfesystem Hilfeinhalte von Microsoft Office Online herunterladen kann.
  
#### Sicherheitsrisiko
  
Standardmäßig durchsucht das 2007 Office-Hilfesystem Microsoft Office Online automatisch nach Inhalten, wenn ein Computer mit dem Internet verbunden ist. Benutzer können diese Standardeinstellung ändern, indem sie das Kontrollkästchen **Microsoft Office Online nach Hilfeinhalt durchsuchen, wenn eine Verbindung mit dem Internet besteht** im Bereich **Datenschutzoptionen** des Vertrauensstellungscenters deaktivieren. Wenn Ihr Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Office Online verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn das Herunterladen von Inhalten über das Hilfesystem zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen für den Zugriff auf Onlinehilfeinhalte zur Verfügung:
  
-   **Onlineinhalt oder Einstiegspunkte nie anzeigen**. Das 2007 Office-Hilfesystem stellt keine Verbindung zu Microsoft Office Online her, um Inhalte herunterzuladen.
  
-   **Nur Offlineinhalt soweit verfügbar durchsuchen**. Das Hilfesystem stellt keine Verbindung zu Microsoft Office Online her, um Inhalte herunterzuladen.
  
-   **Onlineinhalt soweit verfügbar durchsuchen**. Das Hilfesystem stellt eine Verbindung zu Microsoft Office Online her, um Inhalte herunterzuladen, wenn der Computer mit dem Internet verbunden ist. Diese Option setzt die Standardkonfiguration durch.
  
**Tabelle 1.179: Onlineinhaltoptionen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Dienstoptionen…\Onlineinhalte</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Onlineinhalt oder Einstiegspunkte nie anzeigen)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-967</p></td>
</tr>
</tbody>
</table>
  
![](images/Dd443677.note(de-de,TechNet.10).gif)**Hinweis:**
  
Die drei Optionen, die bei Aktivierung dieser Einstellung zur Verfügung gestellt werden, entsprechen den Benutzeroberflächenoptionen in Microsoft Office 2003, die den Zugriff auf die Onlinehilfe auf andere Weise steuerten. Wie bereits beschrieben, verhindert die Aktivierung der Option **Onlineinhalt oder Einstiegspunkte nie anzeigen** oder der Option **Nur Offlineinhalt soweit verfügbar durchsuchen**, dass das Hilfesystem auf Inhalte von Microsoft Office Online zugreift.
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **Onlineinhalt oder Einstiegspunkte nie anzeigen**. Sie führt zu Beeinträchtigungen für Benutzer, die daran gewöhnt sind, Inhalte von Microsoft Office Online in 2007 Office-Anwendungen zu erhalten. Diese Benutzer müssen über ihren Webbrowser auf Microsoft Office Online zugreifen, um diese Inhalte zu erhalten, falls das zugelassen ist.
  
### Office-Dokumente beim Browsen mit Lese-/Schreibzugriff senden
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob Benutzer 2007 Office-Dokumente auf Webservern bearbeiten und speichern können, die in Internet Explorer geöffnet wurden.
  
#### Sicherheitsrisiko
  
Wenn Benutzer in Internet Explorer zu einem 2007 Office-Dokument auf einem Webserver navigieren, öffnet die entsprechende Anwendung die Datei standardmäßig im schreibgeschützten Modus. Bei einer Änderung der Standardkonfiguration wird das Dokument dagegen mit Lese-/Schreibzugriff geöffnet. Benutzer könnten potenziell Änderungen an Dokumenten vornehmen und diese erneut speichern, wenn die Konfiguration der Webserversicherheit derartige Änderungen nicht verhindert.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, werden 2007 Office-Dokumente, die in Internet Explorer aus Websites geöffnet werden, im Lese-/Schreibmodus geöffnet.
  
**Tabelle 1.180: Office-Dokumente beim Browsen mit Lese-/Schreibzugriff öffnen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…\Dateien</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-646</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Diese Einstellung setzt die 2007 Office-Standardkonfiguration durch und sollte deshalb nur minimale Auswirkungen für Benutzer haben.
  
### Outlook Rich-Text-Optionen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, wie Outlook 2007 Nachrichten im Rich-Text-Format an Internetempfänger sendet.
  
#### Sicherheitsrisiko
  
Outlook 2007-Benutzer können Nachrichten wahlweise im HTML-, Rich-Text- oder Nur-Text-Format erstellen. Für das Verfassen formatierter Nachrichten empfiehlt Microsoft das weit verbreitete HTML-Format. Zum Senden von Nachrichten innerhalb eines Unternehmens, das Microsoft Exchange verwendet, kann auch das Rich-Text-Format (RTF) benutzt werden.
  
Standardmäßig konvertiert Outlook über das Internet gesendete Nachrichten im Rich-Text-Format automatisch in das HTML-Format, damit die Nachrichtenformatierung erhalten bleibt und Anlagen empfangen werden können. Bei einer Änderung dieser Konfiguration können Empfänger Nachrichten möglicherweise nicht lesen oder erhalten diese nicht mit den entsprechenden Formatierungen und Anlagen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren drei Optionen für die Verarbeitung von RTF-Nachrichten zur Verfügung, die an Empfänger im Internet adressiert sind:
  
-   **In HTML-Format konvertieren**. Outlook 2007 konvertiert die Nachricht in das HTML-Format und erhält die Formatierung der Nachricht so weit wie möglich.
  
-   **In Nur-Text-Format konvertieren**. Outlook konvertiert die Nachricht in das Nur-Text-Format im Standardzeichensatz. Die gesamte Nachrichtenformatierung geht dabei verloren.
  
-   **Im Outlook-Rich-Text-Format senden**. Outlook sendet die Nachricht im Rich-Text-Format, ohne sie zu konvertieren.
  
**Tabelle 1.181: Outlook Rich-Text-Optionen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\E-Mail-Format\Internetformatierung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (In Nur-Text-Format konvertieren)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-655</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die empfohlene Einstellung für die SSLF-Umgebung ist **In Nur-Text-Format konvertieren**. Sie führt dazu, dass RTF-Nachrichten jegliche ihnen zugewiesene Formatierung verlieren, wenn sie über das Internet an Empfänger gesendet werden. Benutzer, die Nachrichten im HTML- oder Nur-Text-Format erstellen, sind von dieser Einstellung nicht betroffen.
  
### Outlook-Sicherheitsmodus
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, welche Gruppe von Sicherheitseinstellungen in Outlook 2007 durchgesetzt wird.
  
#### Sicherheitsrisiko
  
Wenn Benutzer Sicherheitseinstellungen selbst konfigurieren können, wählen sie möglicherweise Sicherheitsstufen aus, die Computer anfällig für Angriffe machen.
  
Standardmäßig können Outlook 2007-Benutzer Sicherheitseinstellungen selbst konfigurieren, und Outlook ignoriert alle sicherheitsrelevanten Einstellungen, die in der Gruppenrichtlinie konfiguriert sind.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, stehen Administratoren vier Optionen zur Verfügung, um Outlook 2007-Sicherheitseinstellungen zu durchzusetzen:
  
-   **Outlook-Standardsicherheit**. Diese Option ist die Standardkonfiguration in Outlook 2007. Benutzer können Sicherheitseinstellungen selbst konfigurieren, und Outlook ignoriert alle sicherheitsrelevanten Einstellungen, die in der Gruppenrichtlinie konfiguriert sind.
  
-   **Sicherheitsformular aus öffentlichem Ordner „Outlook-Sicherheitseinstellungen“ verwenden**. Outlook verwendet die Einstellungen aus dem Sicherheitsformular, das im festgelegten öffentlichen Ordner veröffentlicht ist.
  
-   **Sicherheitsformular aus öffentlichem Ordner „Outlook 10-Sicherheitseinstellungen“ verwenden**. Outlook verwendet die Einstellungen aus dem Sicherheitsformular, das im festgelegten öffentlichen Ordner veröffentlicht ist.
  
-   **Outlook-Sicherheitsgruppenrichtlinie verwenden**. Outlook verwendet Sicherheitseinstellungen aus der Gruppenrichtlinie.
  
**Tabelle 1.182: Outlook-Sicherheitsmodus**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Sicherheitsformulareinstellungen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Outlook-Sicherheitsgruppenrichtlinie verwenden)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert (Outlook-Sicherheitsgruppenrichtlinie verwenden)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1516</p></td>
</tr>
</tbody>
</table>
  
![](images/Dd443677.important(de-de,TechNet.10).gif)**Wichtig:**
  
Sie müssen diese Einstellung aktivieren, wenn Sie die anderen in diesem Handbuch erwähnten Outlook-Sicherheitseinstellungen anwenden möchten.
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass Benutzer ihre eigenen Sicherheitseinstellungen ändern können, und kann daher möglicherweise zu mehr Supportanfragen führen. Dennoch ist diese Einstellung unerlässlich, wenn Sie sicherstellen möchten, dass die anderen in diesem Handbuch erwähnten Outlook 2007-Sicherheitseinstellungen wie vorgeschlagen angewendet werden.
  
![](images/Dd443677.note(de-de,TechNet.10).gif)**Hinweis:**
  
Wenn in früheren Versionen von Outlook Sicherheitseinstellungen in einem Formular in öffentlichen Ordnern von Exchange Server veröffentlicht wurden, mussten Benutzer auf den entsprechenden Computern den Registrierungsschlüssel „HKEY\_CURRENT\_USER\\Software\\Policies\\Microsoft\\Security\\CheckAdminSettings“ einrichten, damit die Einstellungen angewendet wurden. In Outlook 2007 wird der Registrierungsschlüssel „CheckAdminSettings“ nicht mehr verwendet, um die Sicherheitseinstellungen von Benutzern zu bestimmen. Stattdessen kann über die Einstellung „Outlook-Sicherheitsmodus“ festgelegt werden, ob die Outlook-Sicherheit direkt über die Gruppenrichtlinie, über das Sicherheitsformular aus dem öffentlichen Ordner „Outlook-Sicherheitseinstellungen“ oder über die Einstellungen auf den Computern der Benutzer gesteuert werden.
  
### Nur-Text-Optionen
  
Mit dieser Einstellung kann ein Administrator steuern, wie Nur-Text-Nachrichten beim Versenden in Outlook 2007 formatiert werden.
  
Betrifft: **Outlook**
  
#### Sicherheitsrisiko
  
Wenn ausgehende E-Mail-Nachrichten auf eine bestimmte Weise formatiert sind, beispielsweise mit Anlagen im UUENCODE-Format, können Angreifer die Nachrichten für ihre eigenen Zwecke manipulieren. Bei Verwendung der UUENCODE-Formatierung könnte ein Angreifer die codierte Anlange so manipulieren, dass sie Inhaltsfilterungssoftware umgeht.
  
Standardmäßig bricht Outlook 2007 Nur-Text-Nachrichten bei 76 Zeichen um und verwendet das Standard-MIME-Format, um Anlagen in Nur-Text-Nachrichten zu codieren. Diese Einstellungen können aber geändert werden, damit E-Mail-Nachrichten in Nur-Text-E-Mail-Programmen gelesen werden können, die eine nicht dem Standard entsprechende Zeilenlänge verwenden oder keine MIME-Anlagen verarbeiten können.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, können Administratoren gewährleisten, dass für die Codierung von Anlagen in Outlook 2007-Nachrichten im Nur-Text-Format das MIME-Format verwendet wird.
  
**Tabelle 1.183: Nur-Text-Optionen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\E-Mail-Format\Internetformatierung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-IDs</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1592, CCE-1614</p></td>
</tr>
</tbody>
</table>
  
Weitere Informationen über die bestimmten Konfigurationen, die diese CCE-IDs betreffen, finden Sie in der Arbeitsmappe „Sicherheitseinstellungen“ in diesem Solution Accelerator.
  
#### Auswirkung
  
Wenn diese Einstellung nicht konfiguriert ist, können Benutzer bei Bedarf Nur-Text-Optionen in Outlook 2007 ändern, indem sie nacheinander auf **Extras**, **Optionen**, die Registerkarte **E-Mail-Format** und **Internetformat** klicken und dann die Werte unter **Nur-Text-Optionen** ändern. Die SSLF-Einstellung verhindert, dass Benutzer diese Änderungen vornehmen können, weshalb einige E-Mail-Empfänger eventuell keine Anlagen empfangen können.
  
### Veröffentlichen auf einem DAV-Server verhindern
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer ihre Kalender auf einem DAV-Server veröffentlichen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer ihre Kalender für andere freigeben, indem sie diese auf einem Server veröffentlichen, der das WebDAV-Protokoll (World Wide Web Distributed Authoring and Versioning) unterstützt. Im Gegensatz zum Microsoft Office Online-Freigabedienst für Kalender, bei dem Benutzer den Zugriff auf ihre Kalender durch andere Benutzer verwalten können, werden DAV-Zugriffsbeschränkungen nur über Server- und Ordnerberechtigungen erreicht. Für das Einrichten und Verwalten dieser Berechtigungen ist möglicherweise die Unterstützung des Serveradministrators erforderlich. Wenn diese Berechtigungen nicht ordnungsgemäß verwaltet werden, können nicht autorisierte Personen Zugriff auf vertrauliche Daten erlangen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer ihre Kalender nicht auf einem DAV-Server veröffentlichen.
  
**Tabelle 1.184: Veröffentlichen auf einem DAV-Server verhindern**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Kalenderoptionen\Microsoft Office Online-Freigabedienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1368</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt zu Beeinträchtigungen für Outlook 2007-Benutzer, die ihre Kalender auf einem DAV-Server veröffentlichen. Diese Benutzer müssen ihre Kalender bei einer anderen Ressource, wie dem Microsoft Office Online-Freigabedienst für Kalender, veröffentlichen oder die Veröffentlichung ihrer Kalenderdaten einstellen. Benutzer, die Kalenderdaten nicht veröffentlichen, sind von dieser Einstellung nicht betroffen.
  
### Veröffentlichen auf Office Online verhindern
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, ob Outlook 2007-Benutzer ihre Kalender bei dem Microsoft Office Online-Freigabedienst für Kalender veröffentlichen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können Outlook 2007-Benutzer ihre Kalender für andere Benutzer freigeben, indem sie diese bei dem Microsoft Office Online-Freigabedienst für Kalender veröffentlichen. Benutzer können steuern, wer ihren Kalender mit welchen Details anzeigen kann. Wenn Ihr Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Office Online verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn die Veröffentlichung von Kalendern zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können Outlook 2007-Benutzer ihre Kalender nicht auf Office Online veröffentlichen.
  
**Tabelle 1.184: Veröffentlichen auf Office Online verhindern**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Extras | Optionen…\Einstellungen\Kalenderoptionen\Microsoft Office Online-Freigabedienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1478</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung führt zu Beeinträchtigungen für Outlook 2007-Benutzer, die ihre Kalenderdaten auf Microsoft Office Online veröffentlichen. Diese Benutzer müssen ihre Kalender bei einer anderen Ressource veröffentlichen oder die Veröffentlichung ihrer Kalenderdaten einstellen. Benutzer, die Kalenderdaten nicht veröffentlichen, sind von dieser Einstellung nicht betroffen.
  
### Benutzer können Formularen keine unsicheren Dateitypen anfügen
  
Betrifft: **InfoPath**
  
Diese Einstellung bestimmt, ob InfoPath 2007 das Anfügen von unsicheren Dateitypen an Formulare zulässt.
  
#### Sicherheitsrisiko
  
Standardmäßig kann ein Benutzer Formularen alle Dateitypen anfügen, mit Ausnahme von potenziell unsicheren Dateien, die Viren enthalten können, z. B. BAT- oder EXE-Dateien. Eine vollständige Liste der von InfoPath® 2007 standardmäßig nicht zugelassenen Dateitypen finden Sie im Abschnitt über Sicherheitsdetails unter dem Thema zum [Einfügen eines Dateianlagesteuerelements](http://office.microsoft.com/en-us/infopath/hp100809081033.aspx) (möglicherweise in englischer Sprache) auf der Microsoft Office Online-Website.
  
Wenn InfoPath-Formularen unsichere Dateitypen hinzugefügt werden, können die Formulare als Mittel für einen Angriff auf den Computer verwendet werden, auf dem das Formular geöffnet wird. Diese unsicheren Dateitypen können beispielsweise aktiven Inhalt enthalten oder andere Sicherheitsrisiken einschleusen, die ein Angreifer ausnutzen kann.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können InfoPath 2007-Benutzer Formularen keine unsicheren Dateitypen anfügen.
  
**Tabelle 1.186: Benutzer können Formularen keine unsicheren Dateitypen anfügen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office InfoPath 2007\Sicherheit</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>inf12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1060</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung allein bewirkt nicht, dass InfoPath 2007-Benutzer Formularen unsichere Dateitypen anfügen können. Sie müssen außerdem die Einstellung „Dateitypen als Anlagen für Formulare zulassen“ aktivieren und angeben, welche Dateitypen Sie zulassen möchten. (Weitere Informationen finden Sie im Eintrag für die Einstellung „Dateitypen als Anlagen für Formulare zulassen“ in diesem Handbuch.)
  
Wenn kein legitimer unternehmenswichtiger Grund für das Anfügen von unsicheren Dateitypen an Formulare vorliegt, sollte diese Einstellung aktiviert werden, um einen maximalen Schutz vor unsicheren Dateianlagen zu gewährleisten. Die Aktivierung dieser Einstellung ändert die Standardkonfiguration nicht und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Benutzer können Berechtigungen für Inhalte, deren Rechte verwaltet werden, nicht ändern
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer Berechtigungen für Inhalte ändern können, die durch die Verwaltung von Informationsrechten (IRM) geschützt sind.
  
#### Sicherheitsrisiko
  
Die Funktion zur Verwaltung von Informationsrechten (IRM) der 2007 Office-Version ermöglicht Einzelpersonen und Administratoren die Angabe von Zugriffsberechtigungen für Word 2007-Dokumente, Excel 2007-Arbeitsmappen, PowerPoint 2007-Präsentationen, InfoPath 2007-Vorlagen und -Formulare sowie Outlook 2007-E-Mail-Nachrichten. Diese Funktion trägt dazu bei, das Drucken, Weiterleiten oder Kopieren vertraulicher Daten durch nicht autorisierte Personen zu verhindern.
  
Mit dieser Einstellung können Sie verhindern, dass 2007 Office-Benutzer die IRM-Berechtigungen von Dokumenten ändern. Wenn diese Einstellung **aktiviert** ist, können Benutzer Dokumente, für die sie die entsprechenden Berechtigungen haben, öffnen und bearbeiten. Sie können aber keine neuen Inhalte erstellen, deren Rechte verwaltet werden, vorhandenen Dokumenten keine Verwaltung von Informationsrechten hinzufügen, keine vorhandenen IRM-Berechtigungen ändern oder IRM aus Dokumenten entfernen. Diese Konfiguration verhindert möglicherweise eine effektive Nutzung der Verwaltung von Informationsrechten für den Schutz von Dokumenten.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, können 2007 Office-Benutzer IRM-Berechtigungen für Dokumente hinzufügen, entfernen oder ändern, wenn sie über die entsprechende Autorisierung verfügen.
  
**Tabelle 1.187: Benutzer können Berechtigungen für Inhalte, deren Rechte verwaltet werden, nicht ändern**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Eingeschränkte Berechtigungen verwalten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1603</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung setzt die 2007 Office-Standardkonfiguration durch und dürfte daher für die meisten Benutzer keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Hindert Benutzer am Hochladen von Dokumentvorlagen an die Office Online-Community
  
Betrifft: **2007 Office System**
  
Diese Einstellung steuert, ob 2007 Office-Benutzer selbst erstellte Dokumentvorlagen an Microsoft Office Online hochladen können.
  
#### Sicherheitsrisiko
  
Standardmäßig können 2007 Office-Benutzer selbst erstellte Excel 2007-, PowerPoint 2007- und Word 2007-Vorlagen für andere Microsoft Office-Benutzer aus aller Welt freigeben, indem sie die Vorlagen in den Communitybereich der Microsoft Office Online-Website hochladen. Wenn Ihr Unternehmen über Richtlinien für die Regelung der Verwendung externer Ressourcen wie Office Online verfügt, verstoßen Benutzer möglicherweise gegen diese Richtlinien, wenn das Hochladen von Vorlagen zugelassen wird.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, können 2007 Office-Benutzer Vorlagen nicht auf die Office Online-Website hochladen.
  
**Tabelle 1.188: Hindert Benutzer am Hochladen von Dokumentvorlagen an die Office Online-Community**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Extras | Optionen | Allgemein | Weboptionen…</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1401</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung verhindert, dass 2007 Office-Benutzer Vorlagen für die Microsoft Office-Community auf Office Online freigeben können, verursacht aber ansonsten keine Nutzbarkeitsprobleme.
  
### Fehler der Ebene 2 als Fehler, nicht als Warnungen, höher stufen
  
Betrifft: **Outlook**
  
Diese Einstellung steuert, wie Outlook kryptografische Fehler der Ebene 2 verarbeitet.
  
#### Sicherheitsrisiko
  
Kryptografische Fehler werden in Outlook als Ebene 1 (schwerwiegender Fehler) oder Ebene 2 (nicht schwerwiegend) klassifiziert. Standardmäßig erzeugt Outlook statt einer Fehlermeldung eine Warnung, wenn es zu einem Fehler der Ebene 2 kommt: Das Zertifikat, das die Warnung generiert hat, wird als vertrauenswürdig behandelt, und der Benutzer wird nur über das Problem informiert, wenn er das Dialogfeld **Signaturdetails** öffnet und das Zertifikat überprüft. Zu potenziellen Fehler der Ebene 2 zählen:
  
-   Unbekannter Signaturalgorithmus
  
-   Kein Signaturzertifikat gefunden
  
-   Fehlerhafte Attributsätze
  
-   Kein Herausgeberzertifikat gefunden
  
-   Keine Zertifikatsperrliste gefunden
  
-   Veraltete Zertifikatsperrliste
  
-   Stammvertrauensstellungsproblem
  
-   Veralteter CRT (Certificate Revocation Tree)
  
In einigen Fällen kann eine Verarbeitung von Fehlern der Ebene 2 als Warnung dazu führen, dass Benutzer potenziell bedeutende Signaturprobleme übersehen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **deaktiviert** ist, verarbeitet Outlook 2007 Fehler der Ebene 2 als Fehlermeldungen statt als Warnungen. Dem Benutzer wird eine Fehlermeldung angezeigt, und er kann die Arbeit mit dem Zertifikat nicht fortsetzen.
  
![](images/Dd443677.important(de-de,TechNet.10).gif)**Wichtig:**
  
Diese Einstellung funktioniert „umgekehrt“: Trotz des Namens stuft die Deaktivierung und nicht die Aktivierung der Einstellung Anlagen der Ebene 2 höher.
  
**Tabelle 1.189: Fehler der Ebene 2 als Fehler, nicht als Warnungen, höher stufen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office Outlook 2007\Sicherheit\Kryptografie\Dialogfeld „Signaturstatus“</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>outlk12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Nicht konfiguriert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-943</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Deaktivierung dieser Einstellung kann zu Beeinträchtigungen für Benutzer führen, die in Outlook mit digitalen Zertifikaten arbeiten. Diese Benutzer verzeichnen möglicherweise mehr Fehler, die eine effektive Arbeit mit E-Mail-Nachrichten verhindern und zu vermehrten Anfragen an den Desktopsupport führen können.
  
### Dokumentmetadaten für kennwortgeschützte Dateien schützen
  
Betrifft: **2007 Office System**
  
Diese Einstellung bestimmt, ob Metadaten verschlüsselt werden, wenn eine Office Open XML-Datei kennwortgeschützt ist.
  
![](images/Dd443677.important(de-de,TechNet.10).gif)**Wichtig:**
  
Kürzlich durchgeführte Tests dieser Einstellung ergaben, dass sie nicht erwartungsgemäß funktionierte. Weitere Informationen finden Sie in diesem [Microsoft Knowledge Base-Artikel](http://go.microsoft.com/fwlink/?linkid=103521).
  
#### Sicherheitsrisiko
  
Wenn ein Office Open XML-Dokument mit einem Kennwort geschützt ist und gespeichert wird, werden standardmäßig alle mit dem Dokument verknüpften Metadaten gemeinsam mit den restlichen Dokumentinhalten verschlüsselt. Wenn diese Konfiguration geändert wird, könnten potenziell vertrauliche Daten wie der Autor des Dokuments und Hyperlinkverweise an nicht autorisierte Personen gelangen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, verschlüsseln Excel 2007, PowerPoint 2007 und Word 2007 in kennwortgeschützten Office Open XML-Dateien gespeicherte Metadaten und setzen alle Konfigurationsänderungen auf Computern von Benutzern außer Kraft.
  
![](images/Dd443677.note(de-de,TechNet.10).gif)**Hinweis:**
  
Wenn diese Einstellung **deaktiviert** ist, können 2007 Office-Anwendungen Metadaten in kennwortgeschützten Office Open XML-Dateien nicht verschlüsseln. Dadurch kann sich die Sicherheit verringern.
  
**Tabelle 1.190: Dokumentmetadaten für kennwortgeschützte Dateien schützen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1640</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung beeinträchtigt möglicherweise die Funktionsweise von Tools, die Metadateninformationen für Office Open XML-Dateien zusammenstellen und anzeigen, sollte aber ansonsten keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
### Dokumentmetadaten für Office Open XML-Dateien, deren Rechte verwaltet werden, schützen
  
Betrifft: **2007 Office System**
  
Diese Einstellung bestimmt, ob Metadaten in Office Open XML-Dateien, die durch die Verwaltung von Informationsrechten (IRM) geschützt sind, verschlüsselt werden.
  
#### Sicherheitsrisiko
  
Wenn die Verwaltung von Informationsrechten (IRM) verwendet wird, um den Zugriff auf ein Office Open XML-Dokument zu beschränken, werden standardmäßig alle mit dem Dokument verknüpften Metadaten nicht verschlüsselt. Diese Konfiguration könnte potenziell vertrauliche Daten wie den Autor des Dokuments und Hyperlinkverweise für nicht autorisierte Personen zugänglich machen.
  
#### Gegenmaßnahme
  
Wenn diese Einstellung **aktiviert** ist, verschlüsseln Excel 2007, PowerPoint 2007 und Word 2007 Metadaten in Office Open XML-Dateien, deren Rechte verwaltet werden, und setzen alle Konfigurationsänderungen auf Computern von Benutzern außer Kraft.
  
![](images/Dd443677.note(de-de,TechNet.10).gif)**Hinweis:**
  
Wenn diese Einstellung **deaktiviert** ist, können 2007 Office-Anwendungen Metadaten in Office Open XML-Dateien, deren Rechte verwaltet werden, nicht verschlüsseln. Dadurch kann sich die Sicherheit verringern.
  
**Tabelle 1.191: Dokumentmetadaten für Office Open XML-Dateien, deren Rechte verwaltet werden, schützen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Speicherort in Gruppenrichtlinie</strong></p></td>
<td style="border:1px solid black;"><p>Benutzerkonfiguration\Administrative Vorlagen\Klassische administrative Vorlage (ADM)\Microsoft Office 2007 System\Sicherheitseinstellungen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>ADM-Datei</strong></p></td>
<td style="border:1px solid black;"><p>office12.adm</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (EC)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p><strong>Empfohlene Einstellung (SSLF)</strong></p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p><strong>CCE-ID</strong></p></td>
<td style="border:1px solid black;"><p>CCE-1508</p></td>
</tr>
</tbody>
</table>
  
#### Auswirkung
  
Die Aktivierung dieser Einstellung beeinträchtigt möglicherweise die Funktionsweise von Tools, die Metadateninformationen für Office Open XML-Dateien zusammenstellen und anzeigen, sollte aber ansonsten keine wesentlichen Nutzbarkeitsprobleme verursachen.
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/fe58931e-25fa-4a32-8497-416dbe4929c3(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))  
-   Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5  
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))  
-   [Sicherheitseinstellungen für Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))
  
**Download**
  
[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)
  
[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)
  
**Update-Benachrichtigungen**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenmaßnahmen:%20sicherheitseinstellungen%20in%202007%20office%20system)
  
|                                  |                                                                                                                                                                                                                                                                                                                                                                              |  
|----------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [Zum Seitenanfanq](#mainsection) | [![](images/Dd443677.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))6 von 8[![](images/Dd443677.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10)) |
