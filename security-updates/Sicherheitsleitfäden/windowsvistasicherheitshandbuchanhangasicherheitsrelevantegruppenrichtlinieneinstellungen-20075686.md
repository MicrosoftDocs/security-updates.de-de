---
TOCTitle: 'Windows Vista-Sicherheitshandbuch – Anhang A (Sicherheitsrelevante Gruppenrichtlinieneinstellungen)'
Title: 'Windows Vista-Sicherheitshandbuch – Anhang A (Sicherheitsrelevante Gruppenrichtlinieneinstellungen)'
ms:assetid: '4562299d-8a2f-4730-96c0-d0d96206ff3c'
ms:contentKeyID: 20075686
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443743(v=TechNet.10)'
---

Windows Vista-Sicherheitshandbuch
=================================

### Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen

Veröffentlicht: 08. Nov 2006

##### Auf dieser Seite

[](#eeaa)[Übersicht](#eeaa)
[](#edaa)[Domänenrichtlinien](#edaa)
[](#ecaa)[Computerrichtlinien](#ecaa)
[](#ebaa)[Benutzerrichtlinien](#ebaa)
[](#eaaa)[Weitere Informationen](#eaaa)

### Übersicht

In diesem Anhang werden die Sicherheitsrichtlinieneinstellungen für die Unternehmensclient-Umgebung (EC-Umgebung) und die Hochsicherheitsumgebung (SSLF-Umgebung) erläutert. Zudem finden Sie die empfohlenen Einstellungen für die Konfiguration über den automatisierten Prozess, der in Kapitel 1, „Implementieren der Sicherheitsbasis“, und Kapitel 5, „Hochsicherheit (SSLF)“ des *Windows* *Vista-Sicherheitshandbuchs* beschrieben wird. Die als Begleitmaterial zu diesem Handbuch bereitgestellte Datei „Windows Vista Security Guide Settings.xls“ stellt eine weitere Ressource dar, anhand derer Sie die Einstellungswerte vergleichen können.

Die Einstellungen werden in diesem Anhang gemäß ihrem Vorkommen auf der Benutzeroberfläche des Gruppenrichtlinienobjekt-Editors im Betriebssystem Windows Vista™ aufgeführt.

**Hinweis:**   Gruppenrichtlinieneinstellungen, die in Windows Vista neu eingeführt wurden, sind mit dem Symbol § gekennzeichnet.

Die in diesem Handbuch behandelten Sicherheitseinstellungen sind in folgende drei Hauptabschnitte unterteilt:

-   **Domänenrichtlinien:** Die Einstellungen in diesem Abschnitt gelten für die Domäne.

-   **Computerrichtlinien:** Die Einstellungen in diesem Abschnitt gelten für Desktop- und Laptopcomputer in der Domäne.

-   **Benutzerrichtlinien:** Die Einstellungen in diesem Abschnitt gelten für Benutzer in der Domäne.

In den Tabellen der einzelnen Hauptabschnitte werden die Einstellungsnamen aufgelistet und die Baseline-Werte angegeben, die das Technikerteam für die in diesem Handbuch behandelte Unternehmensclient- und Hochsicherheitskonfiguration entwickelt hat.

Die möglichen Werte unterscheiden sich je nach Einstellung beträchtlich. Die meisten Einstellungen werden auf **Aktiviert** oder **Deaktiviert** oder einen anderen im Gruppenrichtlinienobjekt-Editor aufgeführten Wert gesetzt. Bei vielen Einstellungen müssen Sie allerdings auch numerische Werte oder Sicherheitsgruppen angeben.

Bei Einstellungen für Benutzerrechtrichtlinien müssen spezifische Benutzer- und Gruppennamen angegeben werden. Wenn ein bestimmtes Benutzerrecht keinem Benutzer oder keiner Gruppe gewährt wird, wird die Einstellung im Gruppenrichtlinienobjekt-Editor zwar als aktiviert angezeigt, doch es werden keine Gruppen oder Benutzer aufgeführt. Mit dem Wert **Niemand** werden in den Tabellen in diesem Anhang in entsprechender Weise konfigurierte Einstellungen beschrieben.

Einstellungen mit dem Wert **Nicht definiert** oder **Nicht konfiguriert** sind von den in diesem Handbuch enthaltenen Gruppenrichtlinienobjekten (GPOs) nicht betroffen. Dies ist ein ganz anderer Fall als der zuvor beschriebene Einstellungswert **Niemand**. Einstellungen, die nicht durch die Gruppenrichtlinienobjekte dieses Handbuchs geändert werden, können leicht von lokalen Computeradministratoren geändert werden, sofern sie nicht bereits durch ein anderes Gruppenrichtlinienobjekt in Ihrer Umgebung konfiguriert sind. Dies kann zu uneinheitlichen Konfigurationen in Ihrer gesamten Umgebung und dadurch zur Beeinträchtigung der Sicherheit führen. Aus diesem Grund wird durch viele der empfohlenen Einstellungen lediglich die Windows Vista-Standardeinstellung erzwungen.

In der folgenden Tabelle werden einige Beispiele genannt, die Ihnen das Verständnis der verschiedenen möglichen Konfigurationen erleichtern sollen:

**Tabelle A1. Beispiele für die Zuweisung von Benutzerrechten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPO des Handbuchs</th>
<th>SSLF-Computer-GPO des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Anmeldung über Terminaldienste zulassen</td>
<td style="border:1px solid black;">Administratoren, Remotedesktopbenutzer</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anpassen von Speicherkontingenten für einen Prozess</td>
<td style="border:1px solid black;">Administratoren, Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Lokaler Dienst, Netzwerkdienst</td>
</tr>
</tbody>
</table>
  
Beachten Sie die Standardeinstellung für die Option **Anmelden über Terminaldienste zulassen**. Die Einstellung ist im **EC-Computer-GPO** (Computer-Gruppenrichtlinienobjekt für Unternehmensclient-Umgebungen) auf **Nicht definiert** gesetzt. An der Standardeinstellung wurden also keine Änderungen vorgenommen. Im **SSLF-Computer-GPO** (Computer-Gruppenrichtlinienobjekt für Hochsicherheitsumgebungen) bedeutet jedoch die Einstellung **Niemand** (eine aktivierte Einstellung, für die im Gruppenrichtlinienobjekt-Editor kein Wert angegeben ist), dass kein Benutzer und keine Gruppe das Recht hat, sich über Terminaldienste anzumelden. Außerdem kann ein lokaler Computeradministrator diese Einstellung nicht einfach ändern, da sie durch die Gruppenrichtlinie erzwungen wird.
  
Beachten Sie ebenso die Standardeinstellung für die Option **Anpassen von Speicherkontingenten für einen Prozess**. Auch hierbei ändert das **EC-Computer-GPO** nicht die Standardeinstellung. Mit dieser Konfiguration könnte ein lokaler Computeradministrator die Einstellung problemlos ändern. In der Hochsicherheitsumgebung wäre dies jedoch nicht möglich, da das **SSLF-Computer-GPO** die Standardeinstellung erzwingt.
  
Zudem werden in diesem Handbuch mehrere Einstellungen empfohlen, die bestimmte Umgebungsinformationen erfordern, um richtig zu funktionieren. Da es nicht möglich ist, diese Einstellungen in die Gruppenrichtlinienobjekte dieses Handbuchs einzubeziehen, wird in den Tabellen jeweils der Wert **Empfohlen** angegeben. Zu diesen Einstellungen sollten Sie weitere Nachforschungen anstellen, um die richtige Konfiguration zu ermitteln.
  
![](images/Dd443743.warning(de-de,TechNet.10).gif)**Achtung:**
  
Die Funktionalität vieler Einstellungen in diesem Anhang hängt von anderen Einstellungen ab. Diese Abhängigkeiten sind systembedingt. Außerdem ist zu beachten, dass die Werte einiger Einstellungen auf die individuellen Erfordernisse Ihrer Umgebung abgestimmt werden müssen, um ordnungsgemäß zu funktionieren. Wenn Sie also die empfohlenen Einstellungswerte für die Unternehmensclient- oder die Hochsicherheitsumgebung ändern, sollten Sie aus den genannten Gründen darauf vorbereitet sein, die Clientcomputer in Ihrer Umgebung eingehend zu testen, um sicherzugehen, dass sie in vollem Umfang funktionieren.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Domänenrichtlinien
  
Die Sicherheitseinstellungen in diesem Abschnitt des Anhangs gelten für die Domäne. Diese Einstellungen werden im Gruppenrichtlinienobjekt-Editor über den Knoten **Computerkonfiguration** angewendet. Innerhalb dieses Knotens werden im Unterknoten **Windows-Einstellungen** folgende Einstellungsgruppen angezeigt:
  
-   [Einstellungen für Kennwortrichtlinien](#_password_policy_settings)
  
-   [Einstellungen für die Kontosperrungsrichtlinie](#_account_lockout_policy)
  
#### Einstellungen für die Kennwortrichtlinie
  
Durch komplexe, regelmäßig geänderte Kennwörter verringern Sie das Risiko eines erfolgreichen Kennwortangriffs. Kennwortrichtlinieneinstellungen bestimmen die Komplexität und die Lebensdauer von Kennwörtern. Sie konfigurieren Einstellungen für Kennwortrichtlinien auf der Domänenebene nur über die Gruppenrichtlinie.
  
Die Kennwortrichtlinieneinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Kontorichtlinien\\Kennwortrichtlinie**
  
In der nachstehenden Tabelle werden die Empfehlungen zu den Kennwortrichtlinien für die beiden in diesem Handbuch definierten Sicherheitsumgebungen zusammengefasst. In den folgenden Unterabschnitten werden die einzelnen Einstellungen beschrieben.
  
**Tabelle A2: Empfohlene Kennwortrichtlinieneinstellungen**

 
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
<th>Windows Vista-Standardeinstellung</th>
<th>Domänencontroller-Standardeinstellung</th>
<th>EC-Domänen-GPO des Handbuchs</th>
<th>SSLF-Domänen-GPO des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kennwortchronik erzwingen</td>
<td style="border:1px solid black;">0 gespeicherte Kennwörter</td>
<td style="border:1px solid black;">24 gespeicherte Kennwörter</td>
<td style="border:1px solid black;">24 gespeicherte Kennwörter</td>
<td style="border:1px solid black;">24 gespeicherte Kennwörter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Maximales Kennwortalter</td>
<td style="border:1px solid black;">42 Tage</td>
<td style="border:1px solid black;">42 Tage</td>
<td style="border:1px solid black;">90 Tage</td>
<td style="border:1px solid black;">90 Tage</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Minimales Kennwortalter</td>
<td style="border:1px solid black;">0 Tage</td>
<td style="border:1px solid black;">1 Tag</td>
<td style="border:1px solid black;">1 Tag</td>
<td style="border:1px solid black;">1 Tag</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Minimale Kennwortlänge</td>
<td style="border:1px solid black;">0 Zeichen</td>
<td style="border:1px solid black;">7 Zeichen</td>
<td style="border:1px solid black;">8 Zeichen</td>
<td style="border:1px solid black;">12 Zeichen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Kennwort muss Komplexitätsanforderungen entsprechen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kennwörter mit umkehrbarer Verschlüsselung speichern</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Kennwortchronik erzwingen**  
Durch diese Richtlinieneinstellung wird die Anzahl erneuerter, eindeutiger Kennwörter festgelegt, die einem Benutzerkonto zugewiesen werden müssen, bevor Sie ein altes Kennwort wieder verwenden können. Der Wert für diese Richtlinieneinstellung muss zwischen 0 und 24 liegen. Der Standardwert in Windows Vista ist 0, während die Standardeinstellung in einer Domäne 24 lautet. Wenden Sie die Einstellung **Minimales Kennwortalter** an, um die Effektivität dieser Richtlinieneinstellung zu erhalten. Dadurch werden Benutzer daran gehindert, ihr Kennwort wiederholt zu ändern.
  
In den beiden in diesem Handbuch beschriebenen Sicherheitsumgebungen sollte für die Einstellung **Kennwortchronik erzwingen** der Wert **24 Kennwörter** festgelegt werden.
  
**Maximales Kennwortalter**  
Die Werte für diese Richtlinieneinstellung liegen zwischen 1 und 999 Tagen. (Sie können auch den Wert 0 wählen, um festzulegen, dass Kennwörter niemals ablaufen.) Diese Richtlinieneinstellung bestimmt, wie lange ein Benutzer sein Kennwort verwenden kann, bevor es abläuft. Der Standardwert für diese Richtlinieneinstellung beträgt 42 Tage. Da Angreifer Kennwörter knacken könnten, gilt: Je öfter Sie Ihr Kennwort ändern, desto weniger Gelegenheiten hat ein Angreifer, das geknackte Passwort zu verwenden. Je niedriger jedoch der eingestellte Wert ist, desto wahrscheinlicher ist es, dass Benutzer beim Helpdesk um Hilfe bitten, weil sie Ihr Kennwort ändern müssen oder nicht mehr wissen, welches Kennwort das aktuelle ist.
  
In den beiden in diesem Handbuch definierten Sicherheitsumgebungen sollte für die Einstellung **Maximales Kennwortalter** der Wert **90 Tage** festgelegt werden.
  
**Minimales Kennwortalter**  
Diese Richtlinieneinstellung bestimmt, wie viele Tage Sie ein Kennwort verwenden müssen, bevor Sie es ändern können. Der Wertebereich für diese Richtlinieneinstellung beträgt 1 bis 999 Tage. (Sie können auch den Wert 0 wählen, um sofortige Kennwortänderungen zu ermöglichen.) Der Standardwert für diese Einstellung beträgt 0 Tage.
  
Der für die Einstellung **Minimales Kennwortalter** festgelegte Wert muss unter dem Wert der Einstellung **Maximales Kennwortalter** liegen, sofern der Wert in der Einstellung **Maximales Kennwortalter** nicht auf 0 gesetzt wurde, da in diesem Fall das Kennwort immer gültig bleibt. Wenn für **Maximales Kennwortalter** der Wert 0 festgelegt wird, kann der Wert für diese Richtlinieneinstellung auf einen beliebigen Wert zwischen 0 und 999 gesetzt werden.
  
Wenn Sie möchten, dass die Einstellung **Kennwortchronik erzwingen** zur Wirkung kommt, wählen Sie einen höheren Wert als 0. Wenn **Minimales Kennwortalter** auf 0 eingestellt ist, können Benutzer wiederholt zwischen verschiedenen Kennwörtern abwechseln und schließlich ein altes Lieblingskennwort wieder verwenden.
  
In den beiden in diesem Handbuch definierten Sicherheitsumgebungen sollte für die Einstellung **Minimales Kennwortalter** der Wert **1 Tag** festgelegt werden. Durch diesen Wert wird verhindert, dass Benutzer immer wieder das gleiche Kennwort verwenden, da sie nun einen ganzen Tag warten müssen, bevor sie ihr Kennwort erneut ändern können. Darüber hinaus werden Benutzer durch diesen Wert angehalten, sich neue Kennwörter zu merken, da sie diese vor einer erneuten Änderung mindestens einen Tag lang verwenden müssen. Dadurch wird auch verhindert, dass Benutzer die durch **Kennwortchronik erzwingen** auferlegte Einschränkung umgehen.
  
**Minimale Kennwortlänge**  
Durch diese Richtlinieneinstellung wird die Mindestanzahl an Zeichen für das Kennwort eines Benutzerkontos festgelegt. Es gibt viele verschiedene Theorien zur Bestimmung der besten Kennwortlänge für eine Organisation, wobei eventuel „Kennsatz“ oder „Passphrase“ ein besserer Begriff ist als „Kennwort“. In Microsoft® Windows 2000 und späteren Versionen können Kennsätze ziemlich lang sein und auch Leerzeichen enthalten. Daher ist ein Satz wie „Ich möchte einen Milchshake für 5 € trinken“ ein gültiger Kennsatz. Ein solcher Satz ist viel sicherer als eine acht- oder zehnstellige Zeichenfolge aus beliebigen Zahlen und Buchstaben und ist außerdem leichter zu merken. Denken Sie daran, dass Benutzer zur richtigen Auswahl und Pflege von Kennwörtern erzogen werden müssen, insbesondere in Bezug auf die Kennwortlänge.
  
Stellen Sie in der Unternehmensclient-Umgebung sicher, dass der Wert für die Einstellung **Minimale Kennwortlänge** auf **8 Zeichen** gesetzt ist. Diese Richtlinieneinstellung ist lang genug, um angemessene Sicherheit zu gewährleisten. Setzen Sie den Wert in der Hochsicherheitsumgebung auf **12 Zeichen**.
  
**Kennwort muss Komplexitätsanforderungen entsprechen**  
Diese Richtlinieneinstellung sorgt dafür, dass alle neuen Kennwörter daraufhin geprüft werden, ob sie die grundlegenden Voraussetzungen für sichere Kennwörter erfüllen. In Windows Vista ist für diese Richtlinieneinstellung standardmäßig der Wert **Deaktiviert** konfiguriert, in einer Microsoft Windows Server® 2003-Domäne gilt hingegen der Wert **Aktiviert** für beide in diesem Handbuch beschriebenen Umgebungen.
  
Wenn diese Richtlinie aktiviert ist, müssen Kennwörter die folgenden Mindestvoraussetzungen erfüllen:
  
-   Sie dürfen nicht den Kontonamen des Benutzers und nicht mehr als zwei aufeinander folgende Buchstaben aus seinem echten Namen enthalten.
  
-   Sie müssen mindesten sechs Zeichen lang sein.
  
-   Sie müssen Zeichen aus den folgenden vier Kategorien enthalten:
  
    -   Englische Großbuchstaben (A bis Z)
  
    -   Englische Kleinbuchstaben (a bis z)
  
    -   Grundzahlen (0 bis 9)
  
    -   Nicht-alphabetische Zeichen (z. B. !, $, \#, %)
  
Durch jedes zusätzliche Zeichen in einem Kennwort wird dessen Komplexität exponentiell erhöht. Ein alphabetisches Kennwort aus sieben Kleinbuchstaben würde 267 (ungefähr 8 x 109 oder 8 Milliarden) mögliche Kombinationen aufweisen. Bei 1.000.000 Versuchen pro Sekunde (dies ist bei vielen Entschlüsselungsanwendungen möglich) würde es lediglich 133 Minuten dauern, das Kennwort zu knacken. Für ein alphabetisches Kennwort gibt es bei Beachtung der Groß-/Kleinschreibung 527 mögliche Kombinationen. Für ein alphanumerisches Kennwort ohne Interpunktionszeichen sind bei Beachtung der Groß-/Kleinschreibung 627 Kombinationen möglich. Für ein aus acht Zeichen bestehendes Kennwort sind 268 oder 2 x 1011 Kombinationen möglich. Dies scheint eine große Zahl zu sein, doch bei 1.000.000 Versuchen pro Sekunde würde es lediglich 59 Stunden dauern, alle möglichen Kennwörter auszuprobieren. Beachten Sie, dass sich diese Zeiten bei Kennwörtern bedeutend erhöhen, die ALT-Zeichen oder andere Sonderzeichen wie „!“ oder „@“ verwenden. Die richtige Verwendung von Kennworteinstellungen kann es sehr schwierig machen, einen Brute-Force-Angriff durchzuführen.
  
**Kennwörter mit umkehrbarer Verschlüsselung speichern**  
Durch diese Richtlinieneinstellung wird festgelegt, ob das Betriebssystem Kennwörter mit umkehrbarer Verschlüsselung speichert. Dadurch werden Anwendungsprotokolle unterstützt, die zur Authentifizierung das Benutzerkennwort erfordern. Kennwörter, die mit umkehrbarer Verschlüsselung gespeichert sind, sind im Wesentlichen mit den Klartextversionen von Kennwörtern identisch. Aus diesem Grund sollten Sie diese Richtlinieneinstellung nur aktivieren, wenn die Anforderungen von Anwendungen Vorrang vor der Notwendigkeit des Schutzes von Kennwortinformationen haben. Der Standardwert für diese Richtlinieneinstellung lautet **Deaktiviert**.
  
Das Aktivieren dieser Richtlinieneinstellung ist bei Verwendung des Challenge-Handshake Authentication Protocol (CHAP) über Remotezugriff bzw. des Internetauthentifizierungsdienstes (IAS, Internet Authentication Service) erforderlich. Sie ist auch erforderlich, wenn in Internet Information Services (IIS) die Digestauthentifizierung verwendet werden soll.
  
Stellen Sie sicher, dass die Einstellung **Kennwörter mit umkehrbarer Verschlüsselung speichern** für alle Benutzer in der Domäne auf **Deaktiviert** gesetzt ist, wie dies auch beim Standard-Gruppenrichtlinienobjekt der Domäne von Windows Server 2003 und in der lokalen Sicherheitsrichtlinie für Arbeitsstationen und Server der Fall ist. In den beiden in diesem Handbuch definierten Umgebungen ist diese Richtlinieneinstellung ebenfalls **Deaktiviert**.
  
##### Sicherstellen, dass Benutzer ihr Kennwort nur auf Aufforderung ändern
  
Zusätzlich zu diesen Kennwortrichtlinien ist für manche Organisationen eine zentrale Kontrollmöglichkeit über alle Benutzer erforderlich. In diesem Abschnitt wird erläutert, wie Sie verhindern, dass Benutzer ihr Kennwort ändern, ohne dass sie dazu aufgefordert werden.
  
Die zentrale Steuerung der Benutzerkennwörter ist ein Grundstein für ein gut gestaltetes Windows Vista-Sicherheitsschema. Über Gruppenrichtlinien können Sie, wie oben erwähnt, ein minimales und ein maximales Alter für Kennwörter festlegen. Das Erzwingen häufiger Kennwortänderungen kann Benutzer jedoch in die Lage versetzen, die Einstellung **Kennwortchronik erzwingen** in Ihrer Umgebung zu umgehen. Auch kann die Forderung nach zu langen Kennwörtern vermehrte Anfragen beim IT-Helpdesk verursachen, da Benutzer häufiger ihr Kennwort vergessen.
  
Benutzer können ihr Kennwort im Zeitraum zwischen dem in der Einstellung festgelegten minimalen und maximalen Kennwortalter ändern. Das Sicherheitssystem in einer Hochsicherheitsumgebung erfordert jedoch, dass Benutzer ihre Kennwörter nur dann ändern, wenn sie nach Ablauf von 42 Tagen vom Betriebssystem dazu aufgefordert werden. Um dieses Maß an Kontrolle zu erreichen, können Administratoren die Schaltfläche **Kennwort ändern** im Dialogfeld **Windows-Sicherheit** deaktivieren. Dieses Dialogfeld wird angezeigt, wenn Sie STRG+ALT+ENTF drücken.
  
Sie können diese Konfiguration für eine ganze Domäne über die Gruppenrichtlinie implementieren oder die Registrierung bearbeiten und sie für einen oder mehrere bestimmte Benutzer implementieren. Weitere Informationen zu dieser Konfiguration finden Sie im Microsoft Knowledge Base-Artikel 324744, [SO WIRD'S GEMACHT: Kennwortänderungen durch Benutzer nur zulassen, wenn dies in Windows Server 2003 erforderlich ist](http://support.microsoft.com/kb/324744). Wenn Sie über eine Windows 2000-basierte Domäne verfügen, lesen Sie den Knowledge Base-Artikel 309799, [SO WIRD'S GEMACHT: Sicherstellen, dass Kennwörter nur auf Anforderung von Benutzern geändert werden können](http://support.microsoft.com/kb/309799).
  
#### Einstellungen für die Kontosperrungsrichtlinie
  
Die Kontosperrungsrichtlinie ist eine Sicherheitsfunktion des Active Directory®-Verzeichnisdiensts, durch die ein Benutzerkonto gesperrt werden kann. Durch die Sperrung wird verhindert, dass innerhalb eines bestimmten Zeitraums nach einer bestimmten Anzahl erfolgloser Anmeldeversuche eine Anmeldung erfolgt. Die Anmeldeversuche werden von Domänencontrollern erfasst, und die Anzahl zulässiger Versuche und der Zeitraum basieren auf den Werten, die für die Kontosperrungseinstellungen konfiguriert sind. Darüber hinaus können Sie die Dauer der Sperrung festlegen.
  
Durch diese Richtlinieneinstellungen können Angreifer daran gehindert werden, Benutzerkennwörter zu erraten, und die Wahrscheinlichkeit von erfolgreichen Angriffen auf Ihre Netzwerkumgebung wird verringert. Wird eine Kontosperrungsrichtlinie aktiviert, kann dies jedoch zu vermehrten Supportanfragen durch Netzwerkbenutzer führen. Bevor Sie die folgenden Einstellungen aktivieren, sollten Sie sicherstellen, dass Ihre Organisation diesen zusätzlichen Verwaltungsaufwand auf sich nehmen will. Eine verbesserte und kostengünstigere Lösung für viele Organisationen ist das automatische Durchsuchen von Sicherheitsereignisprotokollen für Domänencontroller. Wenn es den Anschein hat, dass jemand Kennwörter für Benutzerkonten zu erraten versucht, werden administrative Warnmeldungen erzeugt.
  
Die Kennwortrichtlinieneinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen**  
**\\Kontorichtlinien\\Kontosperrungsrichtlinien**
  
Die nachstehende Tabelle enthält die empfohlenen Einstellungen für Kontosperrungsrichtlinien für die beiden in diesem Handbuch definierten Sicherheitsumgebungen. In den folgenden Unterabschnitten werden die einzelnen Einstellungen beschrieben.
  
**Tabelle A3: Empfohlene Einstellungen für Kontosperrungsrichtlinien**

 
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
<th>Windows Vista-Standardeinstellung</th>
<th>Domänencontroller-Standardeinstellung</th>
<th>EC-Domänen-GPO des Handbuchs</th>
<th>SSLF-Domänen-GPO des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kontosperrdauer</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">15 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontensperrungsschwelle</td>
<td style="border:1px solid black;">0 ungültige Anmeldeversuche</td>
<td style="border:1px solid black;">0 ungültige Anmeldeversuche</td>
<td style="border:1px solid black;">50 ungültige Anmeldeversuche</td>
<td style="border:1px solid black;">10 ungültige Anmeldeversuche</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zurücksetzungsdauer des Kontosperrungszählers</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">15 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
</tr>
</tbody>
</table>
  
**Kontosperrdauer**  
Durch diese Richtlinieneinstellung wird festgelegt, nach welchem Zeitraum ein gesperrtes Konto wieder freigegeben wird und sich ein Benutzer erneut anmelden kann. Dies wird erzielt, indem in der Einstellung die Anzahl von Minuten festgelegt wird, die ein gesperrtes Konto nicht verfügbar ist. Wenn der Wert für diese Richtlinieneinstellung auf 0 gesetzt wird, bleiben gesperrte Konten so lange gesperrt, bis die Sperre durch einen Administrator manuell wieder aufgehoben wird. Der Standardwert für die Einstellung in Windows Vista lautet **Nicht definiert**.
  
Wenn Sie die Anzahl möglicher Anfragen beim IT-Helpdesk verringern und zugleich zu einer sicheren Infrastruktur beitragen möchten, legen Sie in den beiden in diesem Handbuch definierten Sicherheitsumgebungen (Unternehmensclient- und Hochsicherheitsumgebung) für die Einstellung **Kontosperrdauer** den Wert **15** Minuten fest.
  
Auch wenn es eine gute Idee zu sein scheint, einen hohen Wert für diese Richtlinieneinstellung zu konfigurieren, wird dadurch wahrscheinlich die Anzahl der beim Helpdesk eingehenden Anfragen zur Entsperrung von versehentlich gesperrten Konten erhöht. Der empfohlene Einstellungswert von 15 Minuten hat sich als sinnvolle Wartezeit erwiesen, nach der sich Benutzer wieder anmelden können. Dieser Wert bietet auch ein gewisses Maß an Schutz vor Brute-Force-Kennwortangriffen. Die Benutzer sollten darüber informiert werden, wie lange eine Sperrung dauert, so dass sie wissen, dass sie das Helpdesk nur dann anrufen sollten, wenn ein äußerst wichtiger Grund für einen sofortigen Zugriff auf den Computer besteht.
  
**Kontensperrungsschwelle**  
Diese Richtlinieneinstellung bestimmt, wie viele erfolglose Anmeldeversuche durchgeführt werden können, bis die Sperrung erfolgt. Autorisierte Benutzer können bei ihrem eigenen Konto eine Sperrung hervorrufen, wenn sie ihr Kennwort falsch eingeben oder falsch in Erinnerung haben oder wenn sie an einem Computer ihr Kennwort ändern, während sie an einem anderen Computer angemeldet sind. Der Computer mit dem falschen Kennwort wird wiederholt versuchen, den Benutzer zu authentifizieren, und da das hierzu verwendete Kennwort falsch ist, findet eine Sperrung statt. Legen Sie für die Kontosperrungsschwelle einen hohen Wert fest, um die versehentliche Sperrung autorisierter Benutzer zu vermeiden. Die Standardeinstellung für diese Richtlinieneinstellung ist 0 ungültige Anmeldeversuche. Dadurch wird die Kontosperrung deaktiviert.
  
Setzen Sie den Wert für die Einstellung **Kontosperrungsschwelle** in Unternehmensclient-Umgebungen auf **50** **ungültige Anmeldeversuche** und in Hochsicherheitsumgebungen auf **10 ungültige Anmeldeversuche**.
  
Einem Angreifer ist es möglich, diesen Sperrzustand für einen Denial-of-Service-Angriff (DoS) auszunutzen, indem er bei einer großen Anzahl von Konten eine Sperrung auslöst. Ihre Organisation sollte daher im Hinblick auf identifizierte Bedrohungen und zu mindernde Risiken abwägen, ob diese Richtlinieneinstellung verwendet werden soll. Für diese Richtlinieneinstellung kommen zwei Möglichkeiten in Betracht.
  
-   Legen Sie für die **Kontosperrungsschwelle** den Wert **0** fest, um sicherzustellen, dass keine Konten gesperrt werden. Durch diesen Einstellungswert werden DoS-Angriffe verhindert, bei denen versucht wird, die Konten Ihrer Organisation zu sperren. Dadurch werden auch die Anzahl von Anfragen beim Helpdesk verringert, da die Benutzer ihre Konten nicht unabsichtlich sperren können. Durch diese Einstellungswert können jedoch keine Brute-Force-Angriffe verhindert werden. Die folgenden Verteidigungsmaßnahmen sollten ebenfalls berücksichtigt werden:
  
    -   Eine Kennwortrichtlinie, durch die alle Benutzer gezwungen sind, komplexe Kennwörter mit acht oder mehr Zeichen zu verwenden.
  
    -   Ein wirksamer Überwachungsmechanismus, durch den Administratoren gewarnt werden, wenn in der Umgebung mehrere Kontosperrungen auftreten. Die Überwachungslösung sollte z. B. das Auftreten des Sicherheitsereignisses 539, „Anmeldungsfehler“, überwachen. Dieses Ereignis weist darauf hin, dass das Konto zum Zeitpunkt des Anmeldeversuchs gesperrt war.
  
Die zweite Möglichkeit lautet wie folgt:
  
-   Legen Sie für die **Kontosperrungsschwelle** einen Wert fest, der es Benutzern erlaubt, sich beim Eingeben ihres Kennwortes mehrmals zu vertippen, und der dennoch zur Kontosperrung führt, wenn ein Brute-Force-Angriff stattfindet. Ein Einstellungswert von 50 ungültigen Anmeldeversuchen für Unternehmensclient-Umgebungen und 10 für Hochsicherheitsumgebungen sollte zu angemessener Sicherheit und akzeptabler Benutzerfreundlichkeit beitragen. Durch diese Konfiguration werden zwar versehentliche Kontosperrungen und entsprechende Anfragen beim IT-Helpdesk verringert, ein Denial-of-Service-Angriff kann jedoch nicht verhindert werden.
  
**Zurücksetzungsdauer des Kontosperrungszählers**  
Durch diese Richtlinieneinstellung wird der Zeitraum festgelegt, nach dem die **Kontensperrungsschwelle** auf null zurückgesetzt wird. Der Standardwert für diese Richtlinieneinstellung lautet **Nicht definiert**. Wenn eine **Kontensperrungsschwelle** festgelegt wird, muss diese Zurücksetzungsdauer kleiner oder gleich dem Wert für die Einstellung **Kontosperrdauer** sein.
  
Setzen Sie den Wert für die Einstellung **Zurücksetzungsdauer des Kontosperrungszählers** in der Unternehmensclient- und der Hochsicherheitsumgebung, die in diesem Handbuch definiert sind, auf **15** **Minuten**.
  
Wenn Sie für diese Richtlinieneinstellung den Standardwert verwenden oder den Wert auf ein zu langes Intervall setzen, könnte Ihre Umgebung anfällig für DoS-Angriffen sein. Ein Angreifer könnte bei allen Benutzern in der Organisation eine Reihe ungültiger Anmeldeversuche durchführen, wodurch die Konten wie weiter oben in diesem Anhang beschrieben gesperrt werden. Würde keine Richtlinie zum Zurücksetzen der Kontosperrung festgelegt, müsste ein Administrator die Sperrung manuell zurücksetzen. Entsprechend kann durch Festlegen eines sinnvollen Zeitwertes für diese Richtlinieneinstellung erreicht werden, dass die Benutzerkonten nur für einen festgelegten Zeitraum gesperrt sind und die Sperrung anschließend automatisch wieder aufgehoben wird. Der empfohlene Einstellungswert von 15 Minuten wurde als geeigneter Zeitraum bestimmt, den Benutzer am ehesten akzeptieren. Dadurch sollte sich die Anzahl der Anrufe beim Helpdesk auf ein Minimum reduzieren lassen. Die Benutzer sollten darüber informiert werden, wie lange sie bis zu einem erneuten Anmeldeversuch warten müssen, so dass sie wissen, dass sie das Helpdesk nur dann anrufen sollten, wenn ein äußerst wichtiger Grund für einen sofortigen Zugriff auf den Computer besteht.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Computerrichtlinien
  
Die Sicherheitseinstellungen in diesem Abschnitt des Anhangs gelten für Desktop- und Laptopcomputer in der Domäne. Diese Einstellungen werden im Gruppenrichtlinienobjekt-Editor über den Knoten **Computerkonfiguration** angewendet. Innerhalb dieses Knotens werden diese Einstellungen in den Unterknoten **Windows-Einstellungen** und **Administrative Vorlagen** angezeigt.
  
#### Computerkonfiguration\\Windows-Einstellungen
  
Folgende Einstellungsgruppen werden im Unterverzeichnis Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien angezeigt:
  
-   [Einstellungen für Überwachungsrichtlinien](#_audit_policy_settings_1)
  
-   [Einstellungen für das Zuweisen von Benutzerrechten](#_user_rights_assignment_1)
  
-   [Einstellungen für Sicherheitsoptionen](#_security_options_settings)
  
Folgende Einstellungsgruppen werden im Unterverzeichnis Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen angezeigt:
  
-   [Sicherheitseinstellungen für Ereignisprotokolle](#_event_log_security)
  
-   [Einstellungen für Windows-Firewall mit erweiterten Sicherheit](#_windows_firewall_with)
  
##### Einstellungen für Überwachungsrichtlinien
  
Durch eine Überwachungsrichtlinie wird festgelegt, bei welchen Sicherheitsereignissen die Administratoren benachrichtigt werden, so dass eine Aufzeichnung von Benutzer- und Systemaktivitäten in festgelegten Ereigniskategorien vorhanden ist. Der Administrator kann dann die sicherheitsrelevanten Aktivitäten überwachen. Dazu gehört z. B. die Überwachung der für Objektzugriffe verwendeten Konten, der An- und Abmeldezeiten der Benutzer oder der Änderungen, die an den Einstellungen der Überwachungsrichtlinien vorgenommen werden. Aus diesen Gründen wird das Erstellen einer Überwachungsrichtlinie empfohlen, die der Administrator in Ihrer Umgebung implementieren kann.
  
Bevor Sie jedoch eine Überwachungsrichtlinie implementieren, müssen Sie ermitteln, welche Ereigniskategorien in Ihrer Umgebung zu überwachen sind. Die Überwachungsrichtlinie wird durch die Überwachungseinstellungen definiert, die in den Ereigniskategorien ausgewählt werden. Wenn Sie Überwachungseinstellungen für bestimmte Ereigniskategorien definieren, kann ein Administrator eine Überwachungsrichtlinie erstellen, die den Sicherheitsanforderungen Ihrer Organisation genügt.
  
Wenn Sie keine Überwachungseinstellungen konfigurieren, ist es schwierig bzw. unmöglich, die genauen Umstände einer Sicherheitsverletzung zu bestimmen. Wenn Sie die Überwachungseinstellungen jedoch so konfigurieren, dass für zu viele autorisierte Aktivitäten Ereignisse produziert werden, sind die Sicherheitsereignisprotokolle schnell mit großen Datenmengen überfüllt. Anhand der Informationen in den folgenden Abschnitten können Sie entscheiden, was überwacht werden soll, um die Erfassung relevanter Überwachungsdaten für Ihre Organisation zu erleichtern.
  
Windows Vista enthält dieselben neun Überwachungsrichtlinien-Kategorien wie frühere Windows-Versionen, nämlich:
  
-   [System](#_system_2)
  
-   [Anmeldung/Abmeldung](#_logon/logoff_1)
  
-   [Objektzugriff](#_object_access)
  
-   [Rechteverwendung](#_privilege_use)
  
-   [Detaillierte Überwachung](#_detailed_tracking_1)
  
-   [Richtlinienänderung](#_policy_change)
  
-   [Kontoverwaltung](#_account_management)
  
-   [DS-Zugriff](#_ds_access_1)
  
-   [Kontoanmeldung](#_account_logon)
  
Windows Vista ermöglicht jedoch mit 50 Unterkategorien eine präzisere Handhabung der Überwachungsrichtlinie. Wenngleich nicht alle Unterkategorien für Windows Vista-basierte Computer gelten, können viele von ihnen so konfiguriert werden, dass sie bestimmte Ereignisse aufzeichnen, aus denen wertvolle Informationen hervorgehen.
  
Bisher erfolgte die Konfiguration der neun Überwachungskategorien einfach über Gruppenrichtlinien. Dies ist zwar auch bei Windows Vista noch möglich, doch die neuen Unterkategorien lassen sich nicht einzeln über den Gruppenrichtlinienobjekt-Editor konfigurieren, da sie im Gruppenrichtlinienobjekt-Editor nicht aufgeführt werden. Wenn Sie eine der Überwachungskategorien in Windows Vista über die im Gruppenrichtlinienobjekt-Editor verfügbaren Einstellungen konfigurieren, werden auch sämtliche Unterkategorien entsprechend konfiguriert. Dies führt sehr wahrscheinlich zu einer übermäßigen Überwachungsprotokollierung, so dass die Ereignisprotokolle sehr schnell überfüllt sind.
  
Es empfiehlt sich deshalb, nur die notwendigen Unterkategorien zu konfigurieren. Zum Konfigurieren der einzelnen Unterkategorien ist das in Windows Vista enthaltene Befehlszeilentool *AuditPol.exe* erforderlich.
  
Die Verwendung eines Befehlszeilentools macht es sehr schwierig, die empfohlenen Überwachungsrichtlinien auf zahlreichen Computern zu implementieren. Microsoft hat jedoch eine Lösung zum Konfigurieren von Überwachungsunterkategorien mithilfe von Gruppenrichtlinien entwickelt. Diese Lösung wird automatisch durch die diesem Handbuch beigefügten Skripts und Gruppenrichtlinienobjekte implementiert.
  
Wenn Sie das Skript GPOAccelerator.wsf ausführen, das in den Kapiteln 1 und 5 dieses Handbuchs beschrieben wird, werden automatisch die folgenden Dateien in die Freigabe NETLOGON eines Ihrer Domänencontroller kopiert.
  
Für die Unternehmensclient-Umgebung:
  
-   EC-VSGAuditPolicy.cmd
  
-   EC-VSGApplyAuditPolicy.cmd
  
-   EC-VSGAuditPolicy.txt
  
Für die Hochsicherheitsumgebung:
  
-   SSLF-VSGAuditPolicy.cmd
  
-   SSLF-VSGApplyAuditPolicy.cmd
  
-   SSLF-VSGAuditPolicy.txt
  
Diese Dateien werden dann automatisch in die Freigabe NETLOGON anderer Domänencontroller Ihrer Active Directory-Domäne repliziert. Zu den vom Skript GPOAccelerator.wsf erstellten computerspezifischen Gruppenrichtlinienobjekten gehört auch ein Startskript, das diese Dateien ausführt, um die empfohlenen Einstellungen für die Überwachungsrichtlinien zu konfigurieren. Beim ersten Ausführen dieser Dateien auf einem Computer wird ein geplanter Task mit dem Namen „VSGAudit“ erstellt. Dieser Task wird jede Stunde ausgeführt, um sicherzustellen, dass die Einstellungen für die Überwachungsrichtlinien aktuell sind.
  
Weitere Informationen über die Lösung zur Konfiguration der neuen Überwachungsrichtlinieneinstellungen in Windows Vista in einer Windows Server 2003-basierten Domäne finden Sie im Knowledge Base-Artikel 921469 [Verwenden von Gruppenrichtlinien zur Konfiguration detaillierter Sicherheitsüberwachungseinstellungen für Windows Vista-Clientcomputer in einer Windows Server 2003- oder Windows 2000-Domäne](http://support.microsoft.com/kb/921469).
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für Überwachungsrichtlinien sowohl für Desktop- als auch für Laptopclientcomputer in den beiden sicheren Umgebungen, die in diesem Handbuch behandelt werden. Sie sollten diese Empfehlungen überprüfen und an die Gegebenheiten Ihrer Organisation anpassen. Wie Sie die durch die Gruppenrichtlinienobjekte dieses Handbuchs konfigurierten Einstellungen für Überwachungsrichtlinien ändern können, wird am Ende dieses Abschnitts erläutert.
  
Seien Sie bei den Überwachungseinstellungen jedoch besonders vorsichtig, da sie einen erheblichen Datenverkehr erzeugen können. Wenn Sie beispielsweise die Erfolgs- oder die Fehlerüberwachung für alle Unterkategorien des Typs **Rechteverwendung** aktivieren, wird es aufgrund der großen Menge der generierten Überwachungsereignisse schwierig, andere Arten von Einträgen im Sicherheitsereignisprotokoll zu finden. Eine solche Konfiguration könnte auch beträchtliche Auswirkungen auf die Leistung haben.
  
In den folgenden Abschnitten werden die einzelnen Überwachungsrichtlinien kurz beschrieben. Die Tabellen in sämtlichen Abschnitten enthalten jeweils Empfehlungen für Desktop- und Laptopclientcomputer in den beiden in diesem Handbuch behandelten Sicherheitsumgebungen.
  
**Hinweis:**   Beschreibungen der einzelnen Unterkategorien für Überwachungsrichtlinien konnten aus zeitlichen Gründen nicht in dieses Handbuch aufgenommen werden. Detaillierte Beschreibungen der 50 Unterkategorien werden in einer künftigen Ausgabe des Handbuchs [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10)) zu finden sein.
  
###### System
  
Mithilfe der Überwachungskategorie „System“ können Sie erfolgreiche oder fehlgeschlagene Systemereignisse überwachen und aufzeichnen. Anhand dieser Aufzeichnungen können Sie Fälle von Systemzugriffen durch Unbefugte leichter ermitteln. Zu Systemereignissen gehören das Starten und Herunterfahren von Computern in der Umgebung, zu große Ereignisprotokolldateien oder andere die Sicherheit betreffende Ereignisse mit Auswirkungen auf das gesamte System.
  
In Windows Vista enthält die Überwachungskategorie „System“ die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A4. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „System“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Sicherheitssystemerweiterung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Systemintegrität</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ IPsec-Treiber</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Andere Systemereignisse</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Sicherheitsstatusänderung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Anmeldung/Abmeldung
  
Diese Überwachungskategorie sorgt dafür, dass Ereignisse erzeugt werden, die die Erstellung und Zerstörung von Anmeldesitzungen aufzeichnen. Diese Ereignisse finden auf dem Computer statt, auf den zugegriffen wurde. Bei interaktiven Anmeldungen werden diese Ereignisse auf dem Computer generiert, auf dem die Anmeldung erfolgt. Bei einer Netzwerkanmeldung für den Zugriff auf eine Freigabe werden diese Ereignisse auf dem Computer generiert, der als Host der aufgerufenen Ressource fungiert.
  
Wenn Sie die Einstellung **Anmeldeereignisse überwachen** auf **Keine Überwachung** setzen, ist es schwierig oder unmöglich festzustellen, welcher Benutzer auf Computer in der Organisation zugegriffen bzw. zuzugreifen versucht hat.
  
In Windows Vista enthält die Ereignisüberwachungskategorie „An-/Abmeldung“ die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A5. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „An-/Abmeldung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Anmelden</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Abmelden</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Kontosperrung
<strong>Hinweis: </strong>  Dieser Unterkategorie sind keine Ereignisse zugeordnet.</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ IPsec-Hauptmodus</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ IPsec-Schnellmodus</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ IPsec-Erweiterungsmodus</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Spezielle Anmeldung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Andere Anmelde-/Abmeldeereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Objektzugriff
  
Diese Richtlinieneinstellung allein führt nicht zur Überwachung von Ereignissen. Sie bestimmt, ob überwacht wird, ob ein Benutzer auf ein Objekt zugreift (z. B. eine Datei, einen Ordner, einen Registrierungsschlüssel oder einen Drucker), für das eine Systemzugriffssteuerungsliste (SACL) festgelegt wurde. Dadurch wird die Überwachung tatsächlich aktiviert.
  
Eine SACL besteht aus Zugriffssteuerungseinträgen (Access Control Entries, ACEs). Jeder ACE enthält drei Informationen:
  
-   Das zu überwachende Sicherheitsprinzipal (Benutzer, Computer oder Gruppe)
  
-   Den zu überwachenden Zugriffstyp, die so genannte Zugriffsmaske
  
-   Ein Flag, aus dem hervorgeht, ob fehlgeschlagene Zugriffsereignisse, erfolgreiche Zugriffsereignisse oder beides überwacht werden soll
  
Wenn Sie die Einstellung **Objektzugriffsversuche überwachen** auf **Erfolg** setzen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn ein Benutzer erfolgreich auf ein Objekt mit definierter SACL zugreift. Wenn Sie diese Richtlinieneinstellung auf **Fehler** setzen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn ein Benutzer erfolglos versucht, auf ein Objekt mit definierter SACL zuzugreifen.
  
Organisationen sollten beim Konfigurieren von SACLs nur jene Aktionen definieren, die aktiviert sein sollen. Es kann z. B. sein, dass Sie die Überwachungseinstellung **Daten schreiben und Daten anhängen** für ausführbare Dateien aktivieren möchten, um Ersetzungen oder Änderungen dieser Dateien zu überwachen, weil Viren, Würmer und Trojaner meist ausführbare Dateien angreifen. Ebenso können Sie Änderungen an wichtigen Dokumenten oder den Zugriff auf solche Dokumente überwachen.
  
Die Ereignisüberwachungskategorie „Objektzugriff“ enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A6. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Objektzugriff“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Dateisystem</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Registrierung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Fehler</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Kernelobjekt</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ SAM</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Zertifizierungsdienste</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Anwendung wurde generiert</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Handleänderung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Dateifreigabe</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Filterplattform: Verworfene Pakete</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Filterplattformverbindung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Andere Objektzugriffsereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
Im Folgenden wird die Konfiguration von Überwachungsregeln für eine Datei oder einen Ordner beschrieben. Anschließend wird erklärt, wie die Überwachungsregeln für jedes Objekt in der angegebenen Datei oder dem Ordner getestet werden können.
  
**Hinweis:**   Sie müssen mit *Auditpol.exe* die Unterkategorie „Dateisystem“ so konfigurieren, dass **Erfolg- und Fehler**-Ereignisse hinsichtlich der folgenden Schritte für das Protokollieren von Ereignissen im Sicherheitsereignisprotokoll überwacht werden.
  
**So definieren Sie eine Überwachungsregel für eine Datei oder einen Ordner**
  
1.  Suchen Sie die Datei oder den Ordner in Windows Explorer, und klicken Sie darauf.
  
2.  Klicken Sie im Menü **Datei** auf **Eigenschaften**.
  
3.  Wechseln Sie zur Registerkarte **Sicherheit**, und klicken Sie auf die Schaltfläche **Erweitert**.
  
4.  Klicken Sie auf die Registerkarte **Überwachung**.
  
5.  Wenn Sie zur Eingabe von Administrator-Anmeldeinformationen aufgefordert werden, klicken Sie auf **Weiter**, geben Sie Ihren Benutzernamen und Ihr Kennwort ein, und drücken Sie die Eingabetaste.
  
6.  Klicken Sie auf die Schaltfläche **Hinzufügen**. Das Dialogfeld **Benutzer,** **Computeroder Gruppe wählen** wird angezeigt.
  
7.  Klicken Sie auf die Schaltfläche **Objekttypen**, und wählen Sie anschließend im Dialogfeld **Objekttypen** die zu suchenden Objekttypen aus.
  
    **Hinweis:**   Die Objekttypen **Benutzer**, **Gruppe** und **Integriertes Sicherheitsprinzipal** sind in der Standardeinstellung bereits ausgewählt.
  
8.  Klicken Sie auf die Schaltfläche **Pfade**, und wählen Sie im Dialogfeld **Pfad** entweder Ihre Domäne oder Ihren lokalen Computer aus.
  
9.  Geben Sie im Dialogfeld **Benutzer oder Gruppe wählen** den Namen der zu überwachenden Gruppe bzw. des Benutzers ein. Geben Sie anschließend im Feld **Geben Sie die zu verwendenden Objektnamen ein** den Text **Authentifizierte Benutzer** ein, um die Zugriffe aller authentifizierten Benutzer zu überwachen, und klicken Sie auf **OK**. Das Dialogfeld **Überwachungseintrag** wird angezeigt.
  
10. Geben Sie im Dialogfeld **Überwachungseintrag** an, welche Zugriffe auf die Datei oder den Ordner überwacht werden sollen.
  
    **Hinweis**   Beachten Sie, dass durch jeden Zugriff mehrere Ereignisse im Ereignisprotokoll erzeugt werden können und dass das Protokoll entsprechend schnell anwächst.
  
11. Wählen Sie im Dialogfeld **Überwachungseintrag** neben **Ordner auflisten / Daten lesen** die Option **Erfolgreich und Fehlgeschlagen** aus, und klicken Sie auf **OK**.
  
12. Die aktivierten Überwachungseinträge werden im Dialogfeld **Erweiterte Sicherheitseinstellungen** auf der Registerkarte **Überwachung** angezeigt.
  
13. Klicken Sie zum Schließen des Dialogfelds **Eigenschaften** auf **OK**.
  
**So testen Sie eine Überwachungsregel für die Datei oder den Ordner**
  
1.  Öffnen Sie die Datei oder den Ordner.
  
2.  Schließen Sie die Datei oder den Ordner.
  
3.  Starten Sie die Ereignisanzeige. Im Sicherheitsereignisprotokoll werden mehrere Objektzugriffsereignisse mit **Ereignis-ID 560** angezeigt.
  
4.  Doppelklicken Sie auf ein Ereignis, um die zugehörigen Detailinformationen anzuzeigen.
  
###### Rechteverwendung
  
Durch die Überwachungskategorie „Rechteverwendung“ wird festgelegt, ob jede Ausübung eines Benutzerrechts durch Benutzer überwacht wird. Wenn Sie diesen Wert auf **Erfolg** einstellen, wird bei jeder erfolgreichen Ausübung eines Benutzerrechts ein Überwachungseintrag erzeugt. Wenn Sie diesen Wert auf **Fehler** einstellen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn die Ausübung eines Benutzerrechts fehlschlägt. Diese Richtlinieneinstellung kann bewirken, dass eine sehr große Anzahl von Ereignisdatensätzen erzeugt wird.
  
Die Ereignisüberwachungskategorie **Rechteverwendung** enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A7. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Rechteverwendung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Sensible Verwendung von Rechten</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Nicht sensible Verwendung von Rechten</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Andere Rechteverwendungsereignisse<br />
<strong>Hinweis</strong>   Dieser Unterkategorie sind keine Ereignisse zugeordnet.</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Detaillierte Überwachung
  
Die Überwachungskategorie „Detaillierte Überwachung“ bestimmt, ob detaillierte Informationen zu Ereignissen wie Programmaktivierung, Prozessbeendigung, Handleduplizierung und indirekter Objektzugriff überwacht werden. Da bei Aktivierung von **Prozessverfolgung überwachen** eine große Anzahl von Ereignissen erzeugt wird, wird normalerweise die Einstellung **Keine Überwachung** verwendet. Diese Einstellung kann jedoch aufgrund des detaillierten Protokolls zu gestarteten Prozessen und zugehörigen Startzeiten von großem Vorteil sein, wenn auf Vorfälle reagiert werden muss.
  
Die Ereignisüberwachungskategorie „Detaillierte Überwachung“ enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A8. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Detaillierte Überwachung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPO des Handbuchs</th>
<th>SSLF-Computer-GPO des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Prozessbeendigung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ DPAPI-Aktivität</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ RPC-Ereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Prozesserstellung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Richtlinienänderung
  
Durch die Überwachungskategorie „Richtlinienänderung“ wird festgelegt, ob sämtliche Änderungen in den Zuweisungsrichtlinien von Benutzerrechten, den Richtlinien der Windows-Firewall, den Vertrauensrichtlinien oder den Überwachungsrichtlinien selbst überwacht werden sollen. Die empfohlenen Einstellungen ermöglichen das Anzeigen aller Kontenberechtigungen, die ein Angreifer zu erhöhen versucht, indem er z. B. die Berechtigung **Debuggen von Programmen** oder **Sichern von Dateien und Verzeichnissen** hinzufügt.
  
Die Ereignisüberwachungskategorie **Richtlinienänderung** enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A9. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Richtlinienänderung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Richtlinienänderungen überwachen</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Authentifizierungsrichtlinienänderung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Autorisierungsrichtlinienänderung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ MPSSVC-Richtlinienänderung auf Regelebene</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Filterplattform-Richtlinienänderung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Andere Richtlinienänderungsereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Kontoverwaltung
  
Mit der Überwachungskategorie „Kontoverwaltung“ kann jeder Versuch überwacht werden, neue Benutzer oder Gruppen zu erstellen, Benutzer oder Gruppen umzubenennen, Benutzerkonten zu aktivieren oder zu deaktivieren, Kontokennwörter zu ändern oder die Überwachung der Kontenverwaltung zu aktivieren. Wenn Sie diese Einstellung für Überwachungsrichtlinien aktivieren, können Administratoren Ereignisse überwachen, um die böswillige, zufällige und autorisierte Erstellung von Benutzer- und Gruppenkonten zu erkennen.
  
Die Ereignisüberwachungskategorie **Kontoverwaltung** enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A10. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Kontoverwaltung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontenverwaltung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Computerkontoverwaltung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Sicherheitsgruppenverwaltung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Verteilergruppenverwaltung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Anwendungsgruppenverwaltung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Andere Kontoverwaltungsereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### DS-Zugriff
  
Die Überwachungskategorie „DS-Zugriff“ gilt nur für Domänencontroller. Aus diesem Grund wird für die Überwachungskategorie „DS-Zugriff“ und alle zugehörigen Unterkategorien für beide in diesem Handbuch behandelten Umgebungen der Wert **Keine Überwachung** konfiguriert.
  
Die Ereignisüberwachungskategorie „DS-Zugriff“ enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A11. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „DS-Zugriff“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Verzeichnisdienständerungen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Verzeichnisdienstreplikation</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Detaillierte Verzeichnisdienstreplikation</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Verzeichnisdienstzugriff</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Kontoanmeldung
  
Die Überwachungskategorie „Kontoanmeldung“ generiert Ereignisse für die Überprüfung der Anmeldeinformationen. Diese Ereignisse finden auf dem Computer statt, der für die Anmeldeinformationen autorisierend ist. Für Domänenkonten ist der Domänencontroller autorisierend, für lokale Konten der lokale Computer. In Domänenumgebungen finden die meisten Kontoanmeldeereignisse im Sicherheitsprotokoll der Domänencontroller statt, die für die Domänenkonten autorisierend sind. Diese Ereignisse können jedoch auch auf anderen Computern in der Organisation stattfinden, wenn die Anmeldung über lokale Konten erfolgt.
  
Die Ereignisüberwachungskategorie **Kontoanmeldung** enthält die in der folgenden Tabelle genannten Unterkategorien.
  
**Tabelle A12. Empfehlungen für die Überwachungsrichtlinien-Unterkategorie „Kontoanmeldung“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterkategorie</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Überprüfung der Anmeldeinformationen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Erfolg und Fehler</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Kerberos-Ticketereignisse</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Andere Kontoanmeldungsereignisse
<strong>Hinweis: </strong>  Dieser Unterkategorie sind keine Ereignisse zugeordnet.</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
###### Ändern von Einstellungen für Überwachungsrichtlinien
  
Für Änderungen an den Unterkategorien und Einstellungen der Überwachungsrichtlinien, die durch die Gruppenrichtlinienobjekte dieses Handbuchs konfiguriert werden, muss mit Auditpol.exe die Konfiguration eines einzelnen Computers in Ihrer Umgebung geändert und eine Datei generiert werden, die die Überwachungsrichtlinieneinstellungen für Ihre Umgebung enthält. Die Computer-Gruppenrichtlinienobjekte dieses Handbuchs wenden dann die geänderte Überwachungsrichtlinie auf Computer in Ihrer Umgebung an.
  
**So ändern Sie die Konfiguration Ihrer Überwachungsrichtlinien**
  
1.  Melden Sie sich als Domänenadministrator an einem Computer mit Windows Vista an, der über Active Directory mit der Domäne verbunden ist, in der Sie die Gruppenrichtlinienobjekte erstellen möchten.
  
2.  Klicken Sie auf dem Desktop auf die Windows Vista-Startschaltfläche, klicken Sie auf **Alle Programme** und auf **Zubehör**, klicken Sie mit der rechten Maustaste auf **Eingabeaufforderung**, und klicken Sie dann auf **Als Administrator ausführen**.
  
3.  Löschen Sie die aktuellen Überwachungsrichtlinieneinstellungen. Geben Sie hierzu die folgende Zeile an der Eingabeaufforderung ein, und drücken Sie anschließend die Eingabetaste:
  
    ```  
 auditpol /clear  
```
  
4.  Konfigurieren Sie mit dem Befehlszeilentool Auditpol.exe die gewünschten benutzerdefinierten Überwachungsrichtlinieneinstellungen. Geben Sie beispielsweise die nachstehenden Zeilen an der Eingabeaufforderung ein. Drücken Sie nach jeder Zeile die Eingabetaste.
  
    **Hinweis:** Einige Teile des folgenden Codeausschnitts werden nur aus Gründen der besseren Lesbarkeit in mehreren Zeilen angezeigt. Der Code sollte jedoch in einer einzelnen Zeile eingegeben werden.
  
    ```  
 auditpol /set /subcategory:"IPSEC Main Mode" /failure:enable  
```
  
    **Hinweis:** Wenn Sie alle mögliche Kategorien und Unterkategorien anzeigen möchten, geben Sie die folgende Zeile an der Eingabeaufforderung ein, und drücken Sie die Eingabetaste:  
    **auditpol /list /subcategory:\***
  
    Geben Sie die folgende Zeile an der Eingabeaufforderung ein, und drücken Sie die Eingabetaste:
  
    ```  
 auditpol /backup /file:EC-AuditPolicy.txt (oder SSLF-AuditPolicy.txt)  
```
  
5.  Kopieren Sie die neue Datei **EC-AuditPolicy.txt** (bzw. **SSLF-AuditPolicy.txt** für Hochsicherheitsumgebungen) in die Freigabe NETLOGON eines der Domänencontroller in Ihrer Umgebung, und überschreiben Sie dabei die bestehende Version.
  
Die Computer-Gruppenrichtlinienobjekte dieses Handbuchs verwenden die neue Datei EC-AuditPolicy.txt (bzw. SSLF-AuditPolicy.txt) zum Ändern und Konfigurieren der Überwachungsrichtlinieneinstellungen auf Ihren Computern.
  
###### Entfernen der Überwachungsrichtlinienkonfiguration
  
Wie bereits erwähnt, erstellt die Lösung, die durch die Gruppenrichtlinienobjekte dieses Handbuchs zur Konfiguration der Überwachungsrichtlinien-Unterkategorien implementiert wird, den geplanten Task VSGAudit auf allen Computern in Ihrer Umgebung. Falls Sie die Gruppenrichtlinienobjekte dieses Handbuchs aus Ihrer Umgebung entfernt haben, kann es sinnvoll sein, den geplanten Task VSGAudit zu löschen. Der geplante Task VSGAudit sollte sich nicht auf die Leistung von Computern auswirken, auf denen Windows Vista ausgeführt wird, selbst wenn Sie die Gruppenrichtlinienobjekte dieses Handbuchs aus Ihrer Umgebung entfernt haben.
  
**So löschen Sie den geplanten Task VSGAudit auf allen Computern in Ihrer Umgebung**
  
1.  Löschen Sie je nach Ihrer Umgebung die folgenden drei Dateien aus der Freigabe NETLOGON eines der Domänencontroller in Ihrer Umgebung:
  
    Für die Unternehmensclient-Umgebung:
  
    -   EC-VSGAuditPolicy.cmd
  
    -   EC-VSGApplyAuditPolicy.cmd
  
    -   EC-VSGAuditPolicy.txt
  
    Für die Hochsicherheitsumgebung:
  
    -   SSLF-VSGAuditPolicy.cmd
  
    -   SSLF-VSGApplyAuditPolicy.cmd
  
    -   SSLF-VSGAuditPolicy.txt
  
2.  Erstellen Sie eine leere Textdatei, geben Sie ihr den Namen DeleteVSGAudit.txt, und kopieren Sie sie in die Freigabe NETLOGON eines der Domänencontroller in Ihrer Umgebung. Die Textdatei wird automatisch in allen Domänencontrollern Ihrer Umgebung repliziert.
  
Der geplante Task VSGAudit sucht jedes Mal, wenn er ausgeführt wird, nach der Datei DeleteVSGAudit.txt. Wenn er sie findet, löscht der Task sich selbst. Da der geplante Task VSGAudit so konfiguriert ist, dass er stündlich ausgeführt wird, sollte es nicht allzu lange dauern, bis er auf allen Computern der Umgebung gelöscht ist.
  
###### Überwachungsrichtlinien für Computer mit Windows XP in der Unternehmensclient-Umgebung
  
Die Gruppenrichtlinienobjekte dieses Handbuchs enthalten Einstellungen, mit denen die Überwachungskategorien in früheren Windows-Versionen konfiguriert werden. Wenn Sie das Skript und die Gruppenrichtlinienobjekte dieses Handbuchs verwenden, werden diese Einstellungen nicht auf Computer angewendet, auf denen Windows Vista ausgeführt wird.
  
Die Gruppenrichtlinienobjekte, die für die Verwendung in der Unternehmensclient-Umgebung vorgesehen sind, sind so eingerichtet, dass sie auf Windows XP-basierten Computern funktionieren. Einstellungen für Überwachungskategorien sind in diesen Gruppenrichtlinienobjekten enthalten, so dass Computer mit Windows XP in Ihrer Umgebung die empfohlenen Überwachungsrichtlinieneinstellungen für Windows XP-basierte Computer erhalten.
  
Die Einstellungen für Überwachungsrichtlinien unter Windows Vista können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen**  
**\\Lokale Richtlinien\\Überwachungsrichtlinie**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für Überwachungsrichtlinien sowohl für Desktop- als auch für Laptopclientcomputer in den beiden sicheren Umgebungen, die in diesem Handbuch behandelt werden.
  
**Tabelle A13: Empfohlene Einstellungen für Überwachungsrichtlinien**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Anmeldeversuche überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontenverwaltung überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Verzeichnisdienstzugriff überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anmeldeereignisse überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Objektzugriff überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Richtlinienänderungen überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Rechteverwendung überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prozessverfolgung überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Systemereignisse überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
</tbody>
</table>
  
**Hinweis:** Da Gruppenrichtlinienobjekte für die Unternehmensclient-Umgebung auf Computer mit Windows XP zugeschnitten sind, sind die empfohlenen Überwachungsrichtlinieneinstellungen in diesen Gruppenrichtlinienobjekten enthalten. Da die Hochsicherheits-Gruppenrichtlinienobjekte hingegen nur für Computer mit Windows Vista vorgesehen sind, enthalten sie keine Überwachungsrichtlinieneinstellungen.
  
##### Einstellungen für das Zuweisen von Benutzerrechten
  
In Verbindung mit vielen privilegierten Gruppen von Windows Vista können bestimmten Benutzern oder Gruppen einige Benutzerrechte zugewiesen werden, über die die meisten Benutzer nicht verfügen.
  
Um den Wert eines Benutzerrechts auf **Niemand** zu setzen, aktivieren Sie die Einstellung, ohne ihr jedoch Benutzer oder Gruppen hinzuzufügen. Um den Wert eines Benutzerrechts auf **Nicht definiert** zu setzen, aktivieren Sie die Einstellung nicht.
  
Die Einstellungen für das Zuweisen von Benutzerrechten unter Windows Vista können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Zuweisen von Benutzerrechten**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für das Zuweisen der Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben A bis E beginnen. Die Empfehlungen gelten für Desktop- und Laptopclientcomputer in den beiden sicheren Umgebungen, die in diesem Handbuch behandelt werden. In den folgenden Unterabschnitten finden Sie detaillierte Informationen zu den einzelnen Einstellungen.
  
Empfehlungen für Benutzerrechte, deren englische Bezeichnungen mit den verbleibenden Buchstaben des Alphabets beginnen, sind in Tabelle A15 zusammengefasst. Weitere Informationen zu diesen Benutzerrechten finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Hinweis:** Viele Funktionen in IIS erfordern, dass bestimmte Konten wie zum Beispiel IIS\_WPG, IIS* *IUSR\_*&lt;Computername&gt;* und IWAM\_*&lt;Computername&gt;* über bestimmte Berechtigungen verfügen. Näheres über die erforderlichen Benutzerrechte für Konten, die sich auf IIS beziehen, finden Sie im Artikel [IIS and Built-in Accounts](http://technet2.microsoft.com/windowsserver/en/library/f1727156-e480-4e05-b168-b764a6e13f881033.mspx?mfr=true) (engl.).
  
###### Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben A bis E beginnen
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für das Zuweisen der Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben A bis E beginnen. In den auf die Tabelle folgenden Unterabschnitten werden die einzelnen Einstellungen ausführlicher beschrieben.
  
**Tabelle A14. Empfohlene Einstellungen für die Zuweisung von Benutzerrechten, Teil 1**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Auf diesen Computer vom Netzwerk aus zugreifen</td>
<td style="border:1px solid black;">Jeder, Administratoren, Benutzer, Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Einsetzen als Teil des Betriebssystems</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anpassen von Speicherkontingenten für einen Prozess</td>
<td style="border:1px solid black;">Administratoren, Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lokal anmelden zulassen</td>
<td style="border:1px solid black;">Gast, Administratoren, Benutzer, Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anmeldung über Terminaldienste zulassen</td>
<td style="border:1px solid black;">Administratoren, Remotedesktopbenutzer</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sichern von Dateien und Verzeichnissen</td>
<td style="border:1px solid black;">Administratoren, Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Auslassen der durchsuchenden Überprüfung</td>
<td style="border:1px solid black;">Jeder, Administratoren, Benutzer, Sicherungs-Operatoren, Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Benutzer, Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ändern der Systemzeit</td>
<td style="border:1px solid black;">Lokaler Dienst, Administratoren</td>
<td style="border:1px solid black;">Lokaler Dienst, Administratoren</td>
<td style="border:1px solid black;">Lokaler Dienst, Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Ändern der Zeitzone</td>
<td style="border:1px solid black;">Lokaler Dienst, Administratoren, Benutzer</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Lokaler Dienst, Administratoren, Benutzer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Erstellen einer Auslagerungsdatei</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Erstellen von dauerhaft freigegebenen Objekten</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Erstellen eines Tokenobjekts</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Erstellen globaler Objekte</td>
<td style="border:1px solid black;">Administratoren, Dienst, Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Dienst, Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Erstellen symbolischer Verknüpfungen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Debuggen von Programmen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zugriff vom Netzwerk auf diesen Computer verweigern</td>
<td style="border:1px solid black;">Gast</td>
<td style="border:1px solid black;">Gäste</td>
<td style="border:1px solid black;">Gäste</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anmelden als Batchauftrag verweigern</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Gäste</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lokal anmelden verweigern</td>
<td style="border:1px solid black;">Gast</td>
<td style="border:1px solid black;">Gäste</td>
<td style="border:1px solid black;">Gäste</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anmelden über Terminaldienste verweigern</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Jeder</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ermöglichen, dass Computer- und Benutzerkonten für Delegierungszwecke vertraut wird</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Auf diesen Computer vom Netzwerk aus zugreifen**  
Diese Richtlinieneinstellung ermöglicht es anderen Benutzern im Netzwerk, eine Verbindung zum Computer herzustellen. Sie ist für verschiedene Netzwerkprotokolle erforderlich, wie z. B. SMB-basierte Protokolle (Server Message Block), NetBIOS (Network Basic Input/Output System), CIFS (Common Internet File System) und COM+ (Component Object Model Plus).
  
Die Einstellung **Auf diesen Computer vom Netzwerk aus zugreifen** ist für die Unternehmensclient-Umgebung auf **Administratoren** und **Benutzer** und für die Hochsicherheitsumgebung auf **Administratoren** gesetzt.
  
**Einsetzen als Teil des Betriebssystems**  
Diese Richtlinieneinstellung ermöglicht es einem Prozess, die Identität eines beliebigen Benutzers anzunehmen und dadurch Zugriff auf die dem Benutzer zugänglichen Ressourcen zu erlangen.
  
Aus diesem Grund ist die Einstellung **Einsetzen als Teil des Betriebssystems** für die beiden in diesem Handbuch behandelten Umgebungen auf den Wert **Niemand** beschränkt.
  
**Anpassen von Speicherkontingenten für einen Prozess**  
Diese Richtlinieneinstellung ermöglicht es einem Benutzer, das maximale Arbeitsspeicherkontingent anzupassen, das einem Prozess zur Verfügung steht. Die Möglichkeit, Speicherkontingente festzulegen, ist für die Anpassung des Systems hilfreich, kann aber auch missbraucht werden. In den falschen Hände könnte dieses Recht für einen DoS-Angriff verwendet werden.
  
Aus diesem Grund ist die Einstellung **Anpassen von Speicherkontingenten für einen Prozess** für die Hochsicherheitsumgebung auf **Administratoren**, **Lokaler Dienst** und **Netzwerkdienst** beschränkt und für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt.
  
**Lokal anmelden zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer sich interaktiv bei Computern in Ihrer Umgebung anmelden können. Dieses Benutzerrecht ist für Anmeldungen erforderlich, die durch Drücken der Tastenkombination STRG+ALT+ENTF auf der am Clientcomputer angeschlossenen Tastatur eingeleitet werden. Auch Benutzer, die versuchen, sich über Terminaldienste oder IIS anzumelden, müssen über dieses Benutzerrecht verfügen.
  
Dieses Benutzerrecht wird dem Konto **Gast** standardmäßig zugewiesen. Obwohl dieses Konto standardmäßig deaktiviert ist, empfiehlt Microsoft, diese Einstellung durch Gruppenrichtlinien zu aktivieren. Dieses Benutzerrecht sollte jedoch generell auf die Gruppen **Administratoren** und **Benutzer** beschränkt werden. Weisen Sie dieses Benutzerrecht der Gruppe **Sicherungs-Operatoren** zu, wenn dies für Ihre Organisation erforderlich ist.
  
Die Einstellung **Lokal anmelden zulassen** ist für die beiden in diesem Handbuch behandelten Umgebungen auf die Gruppen **Benutzer** und **Administratoren** beschränkt.
  
**Anmeldung über Terminaldienste zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer oder Gruppen das Recht haben, sich als Terminaldienstclient anzumelden. Dieses Benutzerrecht ist für Remotedesktopbenutzer erforderlich. Wenn Ihre Organisation als Teil der Helpdeskstrategie Remoteunterstützung anbietet, erstellen Sie eine Gruppe, und weisen Sie ihr dieses Recht über Gruppenrichtlinien zu. Wenn in Ihrer Organisation keine Remoteunterstützung verwendet wird, gewähren Sie dieses Recht nur der Gruppe **Administratoren**. Sie können auch mithilfe der Funktion „Eingeschränkte Gruppen“ sicherstellen, dass sich keine Benutzerkonten in der Gruppe **Remotedesktopbenutzer** befinden.
  
Beschränken Sie dieses Benutzerrecht auf die Gruppe **Administratoren** und eventuell auf die Gruppe **Remotedesktopbenutzer**. Dadurch wird sichergestellt, dass nur autorisierte Benutzer über die Remoteunterstützung Zugriff auf Computer in Ihrem Netzwerk erhalten.
  
Die Einstellung **Anmeldung über Terminaldienste zulassen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung ist diese Richtlinieneinstellung zur Erhöhung der Sicherheit auf **Niemand** gesetzt.
  
**Sichern von Dateien und Verzeichnissen**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, Datei- und Verzeichnisberechtigungen zum Sichern des Systems zu umgehen. Dieses Benutzerrecht wird nur dann aktiviert, wenn eine Anwendung wie z. B. NTBACKUP versucht, über die Dateisystemsicherungs-API (Application Programming Interface) für NTFS auf eine Datei oder ein Verzeichnis zuzugreifen. Andernfalls gelten die zugewiesenen Datei- und Verzeichnisberechtigungen.
  
Für die Einstellung **Sichern von Dateien und Verzeichnissen** ist in der Unternehmensclient-Umgebung der Wert **Nicht definiert** und in der Hochsicherheitsumgebung die Gruppe **Administratoren** konfiguriert.
  
**Auslassen der durchsuchenden Überprüfung**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die nicht über die besondere Zugriffsberechtigung „Ordner durchsehen“ verfügen, beim Durchsuchen eines Objektpfads im NTFS-Dateisystem oder in der Registrierung Ordner zu passieren. Dieses Benutzerrecht ermöglicht es Benutzern nicht, den Inhalt eines Ordners anzuzeigen. Die Verzeichnisse können lediglich passiert werden.
  
Die Einstellung **Auslassen der durchsuchenden Überprüfung** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung ist sie auf die Gruppen **Administratoren,Benutzer,** **Lokaler Dienst**und **Netzwerkdienst** gesetzt.
  
**Ändern der Systemzeit**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer und Gruppen die Uhrzeit und das Datum der internen Uhr der Computer in Ihrer Umgebung ändern können. Benutzer, denen dieses Benutzerrecht zugewiesen wird, können den Inhalt der Ereignisprotokolle beeinflussen. Wenn die Zeiteinstellung eines Computers geändert wird, wird bei den protokollierten Ereignissen die neue Uhrzeit wiedergegeben und nicht die tatsächliche Uhrzeit, zu der die Ereignisse stattgefunden haben.
  
Die Einstellung **Ändern der Systemzeit** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Lokaler Dienst** und die Gruppe **Administratoren** gesetzt.
  
**Hinweis:**   Abweichungen zwischen der Uhrzeit auf dem lokalen Computer und auf den Domänencontrollern Ihrer Umgebung führen beim Authentifizierungsprotokoll Kerberos u. U. zu Problemen. Dadurch könnte es sein, dass Benutzer sich nicht mehr an der Domäne anmelden können oder nach der Anmeldung am Netzwerk nicht für den Zugriff auf Domänenressourcen autorisiert werden. Außerdem treten Probleme auf, wenn Gruppenrichtlinien auf Clientcomputer angewendet werden und die Systemzeit nicht mit den Domänencontrollern synchronisiert ist.
  
**Zeitzone ändern**  
Diese Einstellung bestimmt, welche Benutzer die Zeitzone des Computers ändern können. Diese Fähigkeit birgt keine große Gefahr für den Computer und kann für mobile Benutzer nützlich sein.
  
Die Einstellung **Zeitzone ändern** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Administratoren**, **Lokaler Dienst** und **Benutzer** gesetzt.
  
**Erstellen einer Auslagerungsdatei**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Größe der Auslagerungsdatei zu ändern. Wenn die Auslagerungsdatei extrem groß oder klein ist, kann ein Angreifer leicht die Leistung eines Computers beeinflussen, dessen Sicherheit verletzt wurde.
  
Die Einstellung **Auslagerungsdatei erstellen** ist sowohl in der Unternehmensclient-Umgebung als auch in der Hochsicherheitsumgebung auf **Administratoren** gesetzt.
  
**Erstellen von dauerhaft freigegebenen Objekten**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, im Objekt-Manager Verzeichnisobjekte zu erstellen. Dieses Benutzerrecht ist für Kernelmoduskomponenten nützlich, die den Objekt-Namespace erweitern. Komponenten, die im Kernelmodus ausgeführt werden, sind jedoch von vornherein mit diesem Benutzerrecht ausgestattet, so dass es normalerweise nicht erforderlich ist, dieses Benutzerrecht explizit zuzuweisen.
  
Die Einstellung **Erstellen von dauerhaft freigegebenen Objekten** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
**Erstellen eines Tokenobjekts**  
Diese Richtlinieneinstellung ermöglicht es einem Prozess, ein Zugriffstoken zu erstellen, das erhöhte Berechtigungen für den Zugriff auf vertrauliche Daten bereitstellen kann. In Umgebungen, in denen die Sicherheit Priorität hat, sollte dieses Benutzerrecht keinem Benutzer zugewiesen werden. Alle Prozesse, die diese Funktion erfordern, sollten das lokale Systemkonto verwenden, dem dieses Benutzerrecht standardmäßig zugewiesen ist.
  
Die Einstellung **Erstellen eines Tokenobjekts** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
**Erstellen globaler Objekte**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer globale Objekte erstellen können, die für alle Sitzungen verfügbar sind. Benutzer können weiterhin eigene sitzungsspezifische Objekte erstellen, wenn sie nicht über dieses Benutzerrecht verfügen.
  
Benutzer mit der Berechtigung zur Erstellung globaler Objekte können Prozesse beeinflussen, die in den Sitzungen von anderen Benutzern ausgeführt werden. Diese Funktion kann zu verschiedenen Problemen führen, z. B. zum Fehlschlagen von Anwendungen oder zur Beschädigung von Daten.
  
Die Einstellung **Erstellen globaler Objekte** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Administratoren**, **Dienst**, **Lokaler Dienst**, und **Netzwerkdienst** gesetzt.
  
**Erstellen symbolischer Verknüpfungen**  
Diese Richtlinieneinstellung bestimmt, welche Benutzer symbolische Verknüpfungen erstellen können. In Windows Vista kann auf bestehende NTFS-Dateisystemobjekte wie Dateien und Ordner durch Verweis auf eine neue Art von Dateisystemobjekt, eine so genannte symbolische Verknüpfung, zugegriffen werden. Eine symbolische Verknüpfung ist ein Verweis (ähnlich einer herkömmlichen Verknüpfung oder einer .lnk-Datei) auf ein anderes Dateisystemobjekt. Dieses Objekt kann eine Datei, ein Ordner, eine herkömmliche Verknüpfung oder eine andere symbolische Verknüpfung sein. Der Unterschied zwischen einer herkömmlichen Verknüpfung und einer symbolischen Verknüpfung besteht darin, dass eine herkömmliche Verknüpfung nur aus der Windows-Shell heraus funktioniert. Für andere Programme und Anwendungen sind herkömmliche Verknüpfungen nichts anderes als gewöhnliche Dateien. Bei symbolischen Verknüpfungen ist das Konzept einer herkömmlichen Verknüpfung jedoch als Funktion des NTFS-Dateisystems implementiert.
  
Symbolische Verknüpfungen können u. U. Sicherheitsanfälligkeiten in Anwendungen darstellen, die nicht für die Verwendung solcher Verknüpfungen vorgesehen sind. Aus diesem Grund sollten nur vertrauenswürdige Benutzer das Recht erhalten, symbolische Verknüpfungen zu erstellen. Standardmäßig können symbolische Verknüpfungen nur von Administratoren erstellt werden.
  
Die Einstellung **Erstellen symbolischer Verknüpfungen** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf die Gruppe **Administratoren** gesetzt, um die Standardkonfiguration zu erzwingen.
  
**Debuggen von Programmen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzerkonten zum Debuggen von Prozessen oder dem Kernel berechtigt sind, wodurch vollständiger Zugriff auf vertrauliche und kritische Betriebssystemkomponenten gewährt wird. Entwicklern, die ihre eigenen Anwendungen debuggen, braucht dieses Benutzerrecht nicht zugewiesen zu werden. Entwickler, die neue Systemkomponenten debuggen müssen, benötigen hingegen dieses Recht.
  
**Hinweis:**   Microsoft hat im Oktober 2003 mehrere Sicherheitsupdates mit einer Version der Datei Update.exe veröffentlicht, die voraussetzte, dass der Administrator über das Benutzerrecht **Debuggen von Programmen** verfügt. Administratoren, die nicht über dieses Benutzerrecht verfügten, konnten diese Sicherheitsupdates erst installieren, nachdem sie ihre Benutzerrechte neu konfiguriert hatten. Dies ist kein typisches Verhalten von Betriebssystemupdates. Weitere Informationen hierzu finden Sie im Knowledge Base-Artikel 830846, [Windows-Produktaktualisierungen reagieren nicht mehr oder beanspruchen die CPU-Ressourcen vollständig bzw. zum größten Teil](http://support.microsoft.com/kb/830846).
  
Da ein Angreifer dieses Benutzerrecht ausnutzen könnte, wird es standardmäßig nur der Gruppe „Administratoren“ zugewiesen. Die Einstellung **Debuggen von Programmen** ist in der Unternehmensclient-Umgebung auf **Administratoren** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
**Zugriff vom Netzwerk auf diesen Computer verweigern**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer über das Netzwerk eine Verbindung zu einem Computer herstellen können, wodurch sie in die Lage versetzt würden, von Remotestandorten aus auf Daten zuzugreifen und diese möglicherweise zu verändern. In einer Hochsicherheitsumgebung sollte es für Remotebenutzer nicht erforderlich sein, auf Daten auf einem Computer zuzugreifen. Statt dessen sollte die Dateifreigabe über Netzwerkserver erfolgen.
  
Die Einstellung **Zugriff vom Netzwerk auf diesen Computer verweigern** ist für Computer in den beiden in diesem Kapitel behandelten Umgebungen auf die Gruppe **Gäste** gesetzt.
  
**Anmelden als Batchauftrag verweigern**  
Diese Richtlinieneinstellung verhindert Benutzeranmeldungen über eine Warteschlangenfunktion für Batchaufträge. Dies ist eine Funktion unter Windows Server 2003, mit der Aufträge für die künftige ein- oder mehrmalige automatische Ausführung geplant werden.
  
Die Einstellung **Anmelden als Batchauftrag verweigern** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf die Gruppe **Gäste** gesetzt.
  
**Lokal anmelden verweigern**  
Durch diese Richtlinieneinstellung wird verhindert, dass sich Benutzer lokal bei der Computerkonsole anmelden können. Wenn nicht autorisierte Benutzer in der Lage sind, sich lokal bei einem Computer anzumelden, könnten sie schädlichen Code herunterladen oder ihre Berechtigungen auf dem Computer erhöhen. (Wenn Angreifer physischen Zugriff auf die Konsole haben, sind weitere Risiken zu berücksichtigen.) Dieses Benutzerrecht sollte keinem Benutzer zugewiesen werden, der physischen Zugriff auf die Computerkonsole benötigt.
  
Die Einstellung **Lokal anmelden verweigern** ist für beide in diesem Handbuch behandelten Umgebungen auf **Gäste** gesetzt. Außerdem sollte dieses Benutzerrecht in der Hochsicherheitsumgebung allen dem Computer hinzugefügten Dienstkonten zugewiesen werden, um deren Missbrauch zu verhindern.
  
**Anmelden über Terminaldienste verweigern**  
Durch diese Richtlinieneinstellung wird verhindert, dass sich Benutzer über Remotedesktopverbindungen bei Computern in Ihrer Umgebung anmelden können. Wenn Sie dieses Benutzerrecht der Gruppe **Jeder** zuweisen, halten Sie auch Mitglieder der Standardgruppe **Administratoren** davon ab, sich mithilfe von Terminaldiensten bei Computern in Ihrer Umgebung anzumelden.
  
Die Einstellung **Anmeldung über Terminaldienste verweigern** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Jeder** gesetzt.
  
**Ermöglichen, dass Computer- und Benutzerkonten für Delegierungszwecke vertraut wird**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Einstellung **Für Delegierungszwecke vertraut** für ein Computerobjekt in Active Directory zu ändern. Bei einem Missbrauch dieser Berechtigung könnten nicht autorisierte Benutzer die Identität eines anderen Benutzers im Netzwerk annehmen.
  
Aus diesem Grund ist die Einstellung **Ermöglichen, dass Computer- und Benutzerkonten für Delegierungszwecke vertraut wird** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
###### Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben F bis T beginnen
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für die Zuweisung der Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben F bis T beginnen. In den auf die Tabelle folgenden Unterabschnitten werden die einzelnen Einstellungen ausführlicher beschrieben.
  
**Tabelle A15. Empfohlene Einstellungen für die Zuweisung von Benutzerrechten,** **Teil 2**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Erzwingen des Herunterfahrens von einem Remotesystem aus</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Generieren von Sicherheitsüberwachungen</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Annehmen der Clientidentität nach Authentifizierung</td>
<td style="border:1px solid black;">Administratoren, Dienst, Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Dienst, Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Arbeitssatz eines Prozesses vergrößern</td>
<td style="border:1px solid black;">Benutzer</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anheben der Zeitplanungspriorität</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Laden und Entfernen von Gerätetreibern</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Sperren von Seiten im Speicher</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anmelden als Stapelverarbeitungsauftrag</td>
<td style="border:1px solid black;">Administratoren, Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anmelden als Dienst</td>
<td style="border:1px solid black;">Niemand</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Niemand</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verwalten von Überwachungs- und Sicherheitsprotokollen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Verändern der Firmwareumgebungsvariablen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Durchführen von Volumewartungsaufgaben</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Erstellen eines Profils für einen Einzelprozess</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Erstellen eines Profils der Systemleistung</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Entfernen des Computers von der Dockingstation</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ersetzen eines Tokens auf Prozessebene</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
<td style="border:1px solid black;">Lokaler Dienst, Netzwerkdienst</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Wiederherstellen von Dateien und Verzeichnissen</td>
<td style="border:1px solid black;">Administratoren, Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herunterfahren des Systems</td>
<td style="border:1px solid black;">Administratoren, Sicherungs-Operatoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
<td style="border:1px solid black;">Administratoren, Benutzer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Übernehmen des Besitzes von Dateien und Objekten</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Erzwingen des Herunterfahrens von einem Remotesystem aus**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, Windows Vista-basierte Computer von Remotestandorten im Netzwerk aus herunterzufahren. Jeder, dem dieses Benutzerrecht zugewiesen wurde, kann eine DoS-Situation (Denial of Service) herbeiführen und so verhindern, dass der Computer für Benutzeranfragen zur Verfügung steht. Daher empfiehlt Microsoft, dieses Benutzerrecht nur sehr vertrauenswürdigen Administratoren zuzuweisen.
  
Die Einstellung **Erzwingen des Herunterfahrens von einem Remotesystem aus** ist in den beiden in diesem Handbuch behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
**Generieren von Sicherheitsüberwachungen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer oder Prozesse Überwachungseinträge im Sicherheitsprotokoll erzeugen können. Ein Angreifer könnte diese Funktion ausnutzen, um eine große Anzahl überwachter Ereignisse zu erzeugen, die es einem Systemadministrator erschweren würden, unberechtigte Aktivitäten aufzuspüren. Wenn außerdem das Ereignisprotokoll so konfiguriert ist, dass Ereignisse bei Bedarf überschrieben werden, könnte jeder Beweis über unberechtigte Aktivitäten von einer großen Anzahl nicht zugehöriger Ereignisse überschrieben werden.
  
Aus diesem Grund ist die Einstellung **Generieren von Sicherheitsüberwachungen** für die beiden in diesem Handbuch behandelten Umgebungen für die Gruppen **Lokaler Dienst** und **Netzwerkdienst** konfiguriert.
  
**Annehmen der Clientidentität nach Authentifizierung**  
Mit der Richtlinieneinstellung können die im Auftrag eines Benutzers ausgeführten Programme die Identität dieses Benutzers (oder eines anderen angegebenen Kontos) annehmen und Vorgänge in seinem Namen ausführen. Wenn dieses Benutzerrecht für diese Art von Identitätsannahme erforderlich ist, kann ein nicht autorisierter Benutzer einen Client nicht überzeugen, eine Verbindung zu einem von ihm erstellten Dienst zur Identitätsannahme des Clients herzustellen, z. B. durch einen Remoteprozeduraufruf (RPC) oder Named Pipes. Andernfalls kann der nicht autorisierte Benutzer seine Berechtigungen auf Verwaltungs- oder Systemebene erhöhen.
  
Den Zugriffstokens von Diensten, die durch den Dienststeuerungs-Manager gestartetet werden, wird standardmäßig die vordefinierte Gruppe „Dienst“ hinzugefügt. Den Zugriffstokens von COM-Servern, die durch die COM-Infrastruktur gestartet werden und so konfiguriert sind, dass sie unter einem bestimmten Konto ausgeführt werden, wird die Gruppe „Dienst“ ebenfalls hinzugefügt. Dadurch wird diesen Diensten bei ihrem Start dieses Benutzerrecht zugewiesen.
  
Außerdem kann ein Benutzer die Identität eines Zugriffstokens annehmen, wenn eine der folgenden Bedingungen erfüllt ist:
  
-   Das zu imitierende Zugriffstoken ist für diesen Benutzer bestimmt.
  
-   Der Benutzer in dieser Anmeldesitzung hat sich im Netzwerk mit expliziten Anmeldeinformationen angemeldet, um das Zugriffstoken zu erstellen.
  
-   Die angeforderte Ebene liegt unterhalb der Ebene „Identität wechseln“, etwa die Ebene „Anonym“ oder „Identifizieren“.
  
Ein Angreifer mit dem Benutzerrecht **Annehmen der Clientidentität nach Authentifizierung** kann einen Client dazu bringen, eine Verbindung zu einem vom Angreifer erstellten Dienst herzustellen, und anschließend die Identität des Clients annehmen, um seine Berechtigungen auf die Stufe des Clients zu erhöhen.
  
Aus diesem Grund ist die Einstellung **Annehmen der Clientidentität nach Authentifizierung** für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Administratoren,** **Service,** **Lokaler Dienst**und **Netzwerkdienst** gesetzt.
  
**Arbeitssatz eines Prozesses vergrößern**  
Dieses Recht bestimmt, welche Benutzerkonten den Arbeitssatz eines Prozesses vergrößern oder verkleinern können. Der Arbeitssatz eines Prozesses ist die Gruppe der Speicherseiten, die im physischen Arbeitsspeicher momentan für den Prozess sichtbar sind. Diese Seiten sind resident und für die Verwendung durch eine Anwendung verfügbar, ohne dass ein Seitenfehler ausgelöst wird. Die minimale und maximale Größe des Arbeitssatzes wirkt sich bei einem Prozess auf das Auslagerungsverhalten des virtuellen Speichers aus.
  
Dieses Recht wird allen Benutzern standardmäßig gewährt. Eine Vergrößerung des Arbeitssatzes für einen Prozess bedeutet jedoch eine Verringerung des physischen Speichers, der für das übrige System zur Verfügung steht. Es wäre möglich, dass bösartiger Code den Prozessarbeitssatz auf ein Maß erhöht, das die Systemleistung stark beeinträchtigt und zu einer Situation führen könnte, in der keine Anforderungen mehr beantwortet werden können (Denial of Service, DoS). In bestimmten Umgebungen lässt sich dieses Risiko dadurch mindern, dass die Gruppe der Benutzer, die den Prozessarbeitssatz vergrößern können, eingeschränkt wird.
  
Deshalb wird die Einstellung für das Benutzerrecht „Arbeitssatz eines Prozesses vergrößern“ in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Administratoren** gesetzt.
  
**Anheben der Zeitplanungspriorität**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Zeitdauer zu verändern, für die ein Prozess den Prozessor beansprucht. Ein Angreifer könnte diese Möglichkeit ausnutzen, um die Priorität eines Prozesses auf Echtzeit zu erhöhen und eine DoS-Situation für einen Computer herbeizuführen.
  
Aus diesem Grund ist die Einstellung **Anheben der Zeitplanungspriorität** in den beiden in diesem Handbuch behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
**Laden und Entfernen von Gerätetreibern**  
Diese Richtlinieneinstellung ermöglicht Benutzern das dynamische Laden eines neuen Gerätetreibers auf ein System. Ein Angreifer könnte diese Funktion möglicherweise dazu verwenden, schädlichen Code zu installieren, bei dem es sich um einen Gerätetreiber zu handeln scheint. In Windows Vista müssen Benutzer über dieses Recht verfügen, um lokale Drucker oder Druckertreiber hinzufügen zu können.
  
Da diese Benutzerberechtigung von einem Angreifer ausgenutzt werden könnte, ist die Einstellung **Laden und Entfernen von Gerätetreibern** in den beiden in diesem Handbuch behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
**Sperren von Seiten im Speicher**  
Diese Richtlinieneinstellung ermöglicht einem Prozess das Speichern von Daten in einem physischen Speicher, wodurch das System daran gehindert wird, die Daten in einen virtuellen Speicher auf der Festplatte auszulagern. Durch das Zuweisen dieses Benutzerrechts kann die Systemleistung erheblich beeinträchtigt werden.
  
Aus diesem Grund ist die Einstellung **Sperren von Seiten im Speicher** in den beiden in diesem Handbuch behandelten Umgebungen auf **Niemand** gesetzt.
  
**Anmelden als Stapelverarbeitungsauftrag**  
Diese Richtlinieneinstellung ermöglicht es Konten, sich mithilfe des Taskplanerdienstes anzumelden. Da der Taskplaner häufig zu Verwaltungszwecken verwendet wird, wird er möglicherweise in der Unternehmensclient-Umgebung benötigt. In der Hochsicherheitsumgebung sollte seine Verwendung jedoch eingeschränkt werden, um den Missbrauch von Systemressourcen zu verhindern. Außerdem wird so ebenfalls verhindert, dass Angreifer mithilfe des Rechts schädlichen Code starten, nachdem sie Zugriff auf einen Computer auf Benutzerebene erlangt haben.
  
Daher ist das Benutzerrecht **Anmelden als Stapelverarbeitungsauftrag** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
**Anmelden als Dienst**  
Diese Richtlinieneinstellung ermöglicht es Konten, Netzwerkdienste zu starten oder einen Prozess als auf dem System ausgeführten Dienst zu registrieren. Dieses Benutzerrecht sollte auf allen Computern in einer Hochsicherheitsumgebung eingeschränkt werden. Da diese Berechtigung jedoch möglicherweise für viele Anwendungen erforderlich ist, sollte sie sorgfältig bewertet und getestet werden, bevor sie in einer Unternehmensclient-Umgebung konfiguriert wird. Auf Windows Vista-basierten Computern verfügt kein Benutzer standardmäßig über dieses Recht.
  
Die Einstellung **Anmelden als Dienst** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
**Verwalten von Überwachungs- und Sicherheitsprotokollen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Überwachungsoptionen für Dateien und Verzeichnisse ändern und das Sicherheitsprotokoll löschen können.
  
Da diese Möglichkeit eine relativ kleine Bedrohung darstellt, ist die Einstellung **Verwalten von Überwachungs- und Sicherheitsprotokollen** für die beiden in diesem Handbuch behandelten Umgebungen mit dem Standardwert **Administratoren** konfiguriert.
  
**Verändern der Firmwareumgebungsvariablen**  
Mit dieser Richtlinieneinstellung können Benutzer die systemweiten Umgebungsvariablen konfigurieren, die sich auf die Hardwarekonfiguration auswirken. Diese Informationen sind in der Regel in „Letzte als funktionierend bekannte Konfiguration“ gespeichert. Änderungen an diesen Werten könnten zu einem Hardwareversagen führen, was wiederum eine DoS-Situation verursacht.
  
Da diese Möglichkeit eine relativ kleine Bedrohung darstellt, wird für die Einstellung **Verändern der Firmwareumgebungsvariablen** für die beiden in diesem Handbuch behandelten Umgebungen der Standardwert **Administratoren** übernommen.
  
**Durchführen von Volumewartungsaufgaben**  
Mit dieser Richtlinieneinstellung können Benutzer die Konfiguration von Datenträgern oder Laufwerken des Systems verwalten. Dadurch könnte ein Benutzer einen Datenträger löschen und Datenverluste sowie eine DoS-Situation verursachen.
  
Für die Einstellung **Durchführen von Volumewartungsaufgaben** wird für die beiden in diesem Handbuch behandelten Umgebungen der Standardwert **Administratoren** übernommen.
  
**Erstellen eines Profils für einen Einzelprozess**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer mithilfe von Tools die Leistung von systemfremden Prozessen überwachen können. In der Regel müssen Sie dieses Benutzerrecht nicht konfigurieren, um das Snap-In „Leistung“ der Microsoft Management Console (MMC) zu verwenden. Sie benötigen dieses Benutzerrecht jedoch, wenn der Systemmonitor mit der Windows-Verwaltungsinstrumentation (WMI) zum Sammeln von Daten konfiguriert ist. Wenn Sie das Benutzerrecht **Erstellen eines Profils für einen Einzelprozess** beschränken, wird verhindert, dass Angreifer zusätzliche Informationen erhalten, mit deren Hilfe sie das System angreifen können.
  
Die Einstellung **Erstellen eines Profils für einen Einzelprozess** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt und in der Hochsicherheitsumgebung für die Gruppe **Administratoren** konfiguriert.
  
**Erstellen eines Profils der Systemleistung**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, mithilfe von Tools die Leistung verschiedener Systemprozesse anzuzeigen, die von Angreifern missbraucht werden könnten, um die aktiven Prozesse eines Systems zu ermitteln und Einblick in die potenzielle Angriffsfläche des Computers zu erhalten.
  
Für die Einstellung **Erstellen eines Profils der Systemleistung** wird für die beiden in diesem Handbuch behandelten Umgebungen der Standardwert **Administratoren** übernommen.
  
**Entfernen des Computers von der Dockingstation**  
Diese Richtlinieneinstellung ermöglicht es dem Benutzer eines tragbaren Computers, im Menü **Start** auf **PC trennen** zu klicken, um den Computer abzudocken.
  
Die Einstellung **Entfernen des Computers von der Dockingstation** ist für die beiden in diesem Handbuch behandelten Umgebungen für die Gruppen **Administratoren** und **Benutzer** konfiguriert.
  
**Ersetzen eines Tokens auf Prozessebene**  
Diese Richtlinieneinstellung ermöglicht es einem Prozess oder Dienst, einen weiteren Dienst oder Prozess mit einem anderen Sicherheitszugriffstoken zu starten, wodurch das Sicherheitszugriffstoken jenes Unterprozesses geändert und Berechtigungen erhöht werden können.
  
Die Einstellung **Ersetzen eines Tokens auf Prozessebene** ist in den beiden in diesem Handbuch behandelten Umgebungen auf die Standardwerte **Lokaler Dienst** und **Netzwerkdienst** gesetzt.
  
**Wiederherstellen von Dateien und Verzeichnissen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Berechtigungen für Dateien, Verzeichnisse, die Registrierung und andere persistente Objekte umgehen können, wenn sie gesicherte Dateien und Verzeichnisse auf Computern mit Windows Vista in Ihrer Umgebung wiederherstellen. Durch dieses Benutzerrecht wird außerdem festgelegt, welche Benutzer gültige Sicherheitsprinzipale als Objektbesitzer festlegen dürfen. Dieses Benutzerrecht ähnelt dem Benutzerrecht **Sichern von Dateien und Verzeichnissen**.
  
Die Einstellung **Wiederherstellen von Dateien und Verzeichnissen** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt und in der Hochsicherheitsumgebung für die Gruppe **Administratoren** konfiguriert.
  
**Herunterfahren des Systems**  
Durch diese Richtlinieneinstellung wird festgelegt, welche lokal bei den Computern in Ihrer Umgebung angemeldeten Benutzer das Betriebssystem mit dem Befehl „Herunterfahren“ herunterfahren können. Der Missbrauch dieses Benutzerrechts kann zu einer DoS-Situation führen. Microsoft empfiehlt, dieses Recht in Hochsicherheitsumgebungen nur den Gruppen **Administratoren** und **Benutzer** zuzuweisen.
  
Die Einstellung **Herunterfahren des Systems** ist für die beiden in diesem Handbuch behandelten Umgebungen für die Gruppen **Administratoren** und **Benutzer** konfiguriert.
  
**Übernehmen des Besitzes von Dateien und Objekten**  
Diese Richtlinieneinstellung ermöglicht es Benutzern, den Besitz von Dateien, Ordnern, Registrierungsschlüsseln, Prozessen oder Threads zu übernehmen. Mit diesem Benutzerrecht werden alle Berechtigungen umgangen, die Objekte schützen und dem angegebenen Benutzer Besitzrechte zuweisen sollen.
  
Die Einstellung **Übernehmen des Besitzes von Dateien und Objekten** ist für die beiden in diesem Handbuch behandelten Umgebungen mit dem Standardwert **Administratoren** konfiguriert.
  
##### Einstellungen für Sicherheitsoptionen
  
Mithilfe der Einstellungen für Sicherheitsoptionen, die in Ihrer Umgebung über Gruppenrichtlinien auf Computer mit Windows Vista angewendet werden, können Sie Berechtigungen und Funktionen (z. B. Zugriff auf Disketten- und CD-ROM-Laufwerke und Anmeldeaufforderungen) aktivieren und deaktivieren. Diese Einstellungen dienen auch zum Konfigurieren verschiedener anderer Einstellungen, z. B. für die digitale Datensignierung, für Administrator- und Gastkontennamen sowie für die Funktionsweise der Treiberinstallation.
  
Die Einstellungen der Sicherheitsoptionen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Sicherheitsoptionen**
  
Nicht alle in diesem Abschnitt behandelten Einstellungen sind auf sämtlichen Systemtypen vorhanden. Deshalb müssen die in diesem Abschnitt definierten Einstellungen, die den Abschnitt der Sicherheitsoptionen der Gruppenrichtlinien bilden, auf Systemen, auf denen diese Einstellungen vorhanden sind, möglicherweise manuell geändert werden, damit sie vollständig funktionsfähig sind. Sie können die Gruppenrichtlinienvorlagen auch einzeln bearbeiten und die entsprechenden Einstellungsoptionen aufnehmen, so dass die empfohlenen Einstellungen vollständig zum Tragen kommen.
  
In den folgenden Abschnitten werden Empfehlungen zu den Einstellungen der Sicherheitsoptionen bereitgestellt und nach Objekttyp gruppiert. Jeder Abschnitt enthält eine Tabelle mit einer Übersicht über die Einstellungen. In den Unterabschnitten im Anschluss die jeweilige Tabelle werden ausführliche Informationen bereitgestellt. Empfehlungen werden sowohl für Desktop- als auch für Laptopclientcomputer in den beiden sicheren Umgebungen geboten, die in diesem Handbuch behandelt werden: in der Unternehmensclient-Umgebung (EC-Umgebung) und in der Hochsicherheitsumgebung (SSLF-Umgebung).
  
Dieser Abschnitt des Anhangs enthält Tabellen und Empfehlungen zu den folgenden Objekttypeinstellungen im Unterverzeichnis**Sicherheitsverzeichnis**:
  
-   [Konten](#_accounts)
  
-   [Überwachung](#_audit)
  
-   [Geräte](#_devices)
  
-   [Domänenmitglied](#_domain_member)
  
-   [Interaktive Anmeldung](#_interactive_logon)
  
-   [Microsoft-Netzwerk (Client)](#_microsoft_network_client)
  
-   [MSS-Einstellungen](#_mss_settings_1)
  
-   [Microsoft-Netzwerk (Server)](#_microsoft_network_server)
  
-   [Netzwerkzugriff](#_network_access)
  
-   [Netzwerksicherheit](#_network_security)
  
-   [Wiederherstellungskonsole](#_recovery_console)
  
-   [Herunterfahren](#_shutdown)
  
-   [Systemkryptografie](#_system_cryptography)
  
-   [Systemobjekte](#_system_objects)
  
-   [Benutzerkontensteuerung](#_user_account_control)
  
###### Konten
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Konten. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A16: Empfohlene Einstellungen für Sicherheitsoptionen – Konten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Konten: Administratorkontostatus</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konten: Gastkontenstatus</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konten: Administrator umbenennen</td>
<td style="border:1px solid black;">Administrator</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Konten: Gastkonto umbenennen</td>
<td style="border:1px solid black;">Gast</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
</tbody>
</table>
  
**Konten: Administratorkontostatus**  
Durch diese Richtlinieneinstellung wird das Administratorkonto während des normalen Betriebs aktiviert oder deaktiviert. Wenn ein Computer im sicheren Modus gestartet wird, ist das Administratorkonto unabhängig von der Konfiguration dieser Einstellung immer aktiviert.
  
Die Einstellung **Konten: Administratorkontostatus** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Konten: Gastkontenstatus**  
Durch diese Richtlinieneinstellung wird festgelegt, ob das Gastkonto aktiviert oder deaktiviert ist. Das Gastkonto ermöglicht nicht authentifizierten Netzwerkbenutzern den Zugriff auf das System.
  
Die Sicherheitsoption **Konten: Gastkontenstatus** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken**  
Durch diese Richtlinieneinstellung wird festgelegt, ob lokale Konten, die nicht durch ein Kennwort geschützt sind, sich von anderen Orten als der physischen Computerkonsole aus anmelden können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind lokale Konten mit leeren Kennwörtern nicht in der Lage, sich von Remoteclientcomputern aus beim Netzwerk anzumelden. Solche Konten können sich nur über die Tastatur des Computers anmelden.
  
Die Einstellung **Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Konten: Administrator umbenennen**  
Der vordefinierte Name des lokalen Administratorkontos ist ein bekannter Kontoname, auf den viele Angriffe abzielen. Microsoft empfiehlt, einen anderen Namen für dieses Konto zu wählen und Namen zu vermeiden, die auf administrative Konten oder erhöhte Zugriffsrechte hinweisen. Außerdem sollte die Standardbeschreibung für den lokalen Administrator geändert werden (über das Computerverwaltungs-Snap-In).
  
Die Empfehlung, die Einstellung **Konten: Administrator umbenennen** zu verwenden, gilt für beide Umgebungen, die in diesem Handbuch erörtert werden.
  
**Hinweis:**   Diese Richtlinieneinstellung ist in den Sicherheitsvorlagen nicht konfiguriert, und es wird in diesem Handbuch auch kein neuer Benutzername für das Konto vorgeschlagen. Auf Vorschläge für Benutzernamen wird verzichtet, um sicherzustellen, dass Organisationen, die diese Anleitungen umsetzen, in ihrer Umgebung nicht die gleichen Benutzernamen verwenden.
  
**Konten: Gastkonto umbenennen**  
Der Name des vordefinierten lokalen Gastkontos ist Angreifern ebenfalls wohlbekannt. Microsoft empfiehlt, diesem Konto ebenfalls einen Namen zu geben, aus dem sich der Zweck des Kontos nicht erkennen lässt. Selbst wenn Sie dieses Konto deaktivieren (was empfohlen wird), sollten Sie es zur Erhöhung der Sicherheit umbenennen.
  
Die Empfehlung, die Einstellung **Konten: Gastkonto umbenennen** zu verwenden, gilt für beide Umgebungen, die in diesem Handbuch erörtert werden.
  
**Hinweis:**   Diese Richtlinieneinstellung ist in den Sicherheitsvorlagen nicht konfiguriert, und es wird hier auch kein neuer Benutzername für das Konto vorgeschlagen. Auf Vorschläge für Benutzernamen wird verzichtet, um sicherzustellen, dass Organisationen, die diese Anleitungen umsetzen, in ihrer Umgebung nicht die gleichen Benutzernamen verwenden.
  
###### Überwachung
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Überwachungseinstellungen. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A17: Empfohlene Einstellungen für Sicherheitsoptionen – Überwachung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Überwachung: Zugriff auf globale Systemobjekte prüfen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Überwachung: Force audit policy subcategory settings (Windows Vista or later) to override audit policy category settings</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Überwachung: Zugriff auf globale Systemobjekte prüfen**  
Mit dieser Richtlinieneinstellung wird eine standardmäßige Systemzugriffssteuerungsliste (SACL) für Systemobjekte wie z. B. Mutexe (sich gegenseitig ausschließende Objekte), Ereignisse, Semaphore und MS-DOS®-Geräte erstellt. Der Zugriff auf diese Systemobjekte wird daraufhin überwacht.
  
Wenn die Einstellung **Überwachung: Zugriff auf globale Systemobjekte prüfen** aktiviert ist, könnte das Sicherheitsereignisprotokoll schnell mit einer sehr großen Anzahl von Sicherheitsereignissen gefüllt werden. Aus diesem Grund ist diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Verwendung aller Benutzerrechte (einschließlich Sicherung und Wiederherstellung) überwacht wird, wenn die Einstellung **Rechteverwendung überwachen** aktiviert ist. Wenn Sie beide Richtlinien aktivieren, wird für jede gesicherte oder wiederhergestellte Datei ein Überwachungsereignis erzeugt.
  
Wenn die Einstellung **Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen** aktiviert ist, könnte das Sicherheitsereignisprotokoll schnell mit einer sehr großen Anzahl von Sicherheitsereignissen gefüllt werden. Aus diesem Grund ist diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Überwachung: Force audit policy subcategory settings (Windows Vista or later) to override audit policy category settings**  
Mit dieser Richtlinieneinstellung können Administratoren die präziseren Überwachungsfunktionen von Windows Vista aktivieren.
  
Die Überwachungsrichtlinieneinstellungen in Windows Server 2003 Active Directory enthalten noch keine Einstellungen für die Handhabung der neuen Überwachungsunterkategorien. Damit die in diesem Handbuch empfohlenen Überwachungsrichtlinien korrekt angewendet werden können, wird die Einstellung **Überwachung: Force audit policy subcategory settings (Windows Vista or later) to override audit policy category settings** für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können**  
Durch diese Richtlinieneinstellung wird festgelegt, ob das System sofort heruntergefahren wird, wenn es Sicherheitsereignisse nicht protokollieren kann. Diese Einstellung ist für die TCSEC-C2-Zertifizierung (Trusted Computer System Evaluation Criteria) und die Common-Criteria-Zertifizierung erforderlich und verhindert, dass zu überwachende Ereignisse auftreten, wenn sie vom Überwachungssystem nicht protokolliert werden können. Microsoft erfüllt diese Anforderungen durch Anzeigen einer Abbruchmeldung und Herunterfahren des Systems, wenn das Überwachungssystem nicht ordnungsgemäß arbeitet. Wenn diese Richtlinieneinstellung aktiviert ist, wird das System heruntergefahren, wenn eine Sicherheitsüberwachung nicht protokolliert werden kann.
  
Wenn die Einstellung **Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können** aktiviert ist, können ungeplante Systemfehler auftreten. Aus diesem Grund ist diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
###### Geräte
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Geräte. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A18: Empfohlene Einstellungen für Sicherheitsoptionen – Geräte**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Geräte: Entfernen ohne vorherige Anmeldung erlauben</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Geräte: Formatieren und Auswerfen von Wechselmedien zulassen</td>
<td style="border:1px solid black;">Nicht definiert (standardmäßig kein Registrierungswert vorhanden)</td>
<td style="border:1px solid black;">Administratoren, Interaktive Benutzer</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben<br />
(Desktopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben<br />
(Laptopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken</td>
<td style="border:1px solid black;">Nicht definiert (standardmäßig kein Registrierungswert vorhanden)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken</td>
<td style="border:1px solid black;">Nicht definiert (standardmäßig kein Registrierungswert vorhanden)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Geräte: Entfernen ohne vorherige Anmeldung erlauben**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein tragbarer Computer durch einen nicht beim System angemeldeten Benutzer abgedockt werden kann. Wenn diese Einstellung aktiviert ist, entfällt die Anmeldeanforderung, und der Computer kann über eine Schaltfläche zum Trennen externer Hardware abgedockt werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann ein Benutzer den Computer nur dann von der Dockingstation entfernen, wenn ihm das Benutzerrecht **Entfernen des Computers von der Dockingstation** zugewiesen wurde.
  
Die Einstellung **Geräte:** **Entfernen ohne vorherige Anmeldung erlauben** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Geräte: Formatieren und Auswerfen von Wechselmedien zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, wer Wechselmedien formatieren und auswerfen darf. Mit dieser Richtlinieneinstellung können Sie nicht autorisierte Benutzer davon abhalten, Daten von einem Computer zu entfernen und auf diese auf einem anderen Computer zuzugreifen, auf dem die Benutzer lokale Administratorrechte besitzen.
  
Die Einstellung **Geräte:** **Formatieren und Auswerfen von Wechselmedien zulassen** ist zur Erhöhung der Sicherheit in der Unternehmensclient-Umgebung auf die Gruppen **Administratoren** und **Interaktive Benutzer** und in der Hochsicherheitsumgebung auf die Gruppe **Administratoren** beschränkt.
  
**Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben**  
Angreifer verfügen über Möglichkeiten, einen Trojaner als Druckertreiber zu tarnen. Dadurch getäuschte Benutzer verwenden dieses Programm möglicherweise zum Drucken und führen damit schädlichen Code im Netzwerk aus. Zur Verringerung der Wahrscheinlichkeit eines solchen Ereignisses sollten nur Administratoren Druckertreiber installieren dürfen. Da Laptops mobile Geräte sind, kann es für Benutzer von Laptops jedoch notwendig sein, Druckertreiber aus einer Remotequelle zu installieren, um die Arbeit fortsetzen zu können. Diese Einstellung sollte für Laptopbenutzer deaktiviert, jedoch für Desktopbenutzer immer aktiviert werden.
  
Die Einstellung **Geräte:** **Anwendern das Installieren von Druckertreibern nicht erlauben** ist für die Desktopcomputer in den beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** und für Laptopbenutzer in beiden Umgebungen auf **Deaktiviert** gesetzt.
  
**Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken**  
Durch diese Richtlinieneinstellung wird festgelegt, ob sowohl lokale Benutzer als auch Remotebenutzer gleichzeitig auf das CD-ROM-Laufwerk zugreifen können. Wenn Sie diese Richtlinieneinstellung aktivieren, können nur interaktiv angemeldete Benutzer auf Medien im CD-ROM-Laufwerk zugreifen. Wenn diese Richtlinieneinstellung aktiviert und niemand angemeldet ist, kann über das Netzwerk auf das CD-ROM-Laufwerk zugegriffen werden. Bei Aktivierung dieser Einstellung kann das Windows-Sicherungsprogramm nicht erfolgreich ausgeführt werden, wenn für den Sicherungsauftrag Volumeschattenkopien angegeben wurden. Auch Sicherungsprodukte von Drittanbietern, die mit Volumeschattenkopien arbeiten, können nicht erfolgreich ausgeführt werden.
  
Die Einstellung **Geräte:** **Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken**  
Durch diese Richtlinieneinstellung wird festgelegt, ob sowohl lokale Benutzer als auch Remotebenutzer gleichzeitig auf das Diskettenlaufwerk zugreifen können. Wenn Sie diese Richtlinieneinstellung aktivieren, können nur interaktiv angemeldete Benutzer auf Medien in Diskettenlaufwerken zugreifen. Wenn die Einstellung aktiviert und niemand angemeldet ist, kann über das Netzwerk auf Medien im Diskettenlaufwerk zugegriffen werden. Bei Aktivierung dieser Einstellung kann das Windows-Sicherungsprogramm nicht erfolgreich ausgeführt werden, wenn für den Sicherungsauftrag Volumeschattenkopien angegeben wurden. Auch Sicherungsprodukte von Drittanbietern, die mit Volumeschattenkopien arbeiten, können nicht erfolgreich ausgeführt werden.
  
Die Einstellung **Geräte:** **Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
###### Domänenmitglied
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Domänenmitglieder. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A19: Empfohlene Einstellungen für Sicherheitsoptionen – Domänenmitglied**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Domänenmitglied: Maximalalter von Computerkontenkennwörtern</td>
<td style="border:1px solid black;">30 Tage</td>
<td style="border:1px solid black;">30 Tage</td>
<td style="border:1px solid black;">30 Tage</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der gesamte Datenverkehr über den sicheren Kanal, der vom Domänenmitglied initiiert wird, signiert oder verschlüsselt werden muss. Wenn ein System so eingestellt ist, dass es Daten des sicheren Kanals immer verschlüsselt oder signiert, kann kein sicherer Kanal mit einem Domänencontroller hergestellt werden, der nicht in der Lage ist, den gesamten Datenverkehr über den sicheren Kanal zu signieren oder zu verschlüsseln, da der gesamte Datenverkehr über den sicheren Kanal signiert und verschlüsselt wird.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen soll, für den gesamten von ihm initiierten Verkehr über den sicheren Kanal die Verschlüsselung auszuhandeln. Wenn Sie diese Richtlinieneinstellung aktivieren, fordert das Domänenmitglied für den gesamten Verkehr über den sicheren Kanal eine Verschlüsselung an. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann das Domänenmitglied die Verschlüsselung für den sicheren Kanal nicht aushandeln.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen soll, für den gesamten von ihm initiierten Verkehr über den sicheren Kanal die Signierung auszuhandeln. Durch die Signierung wird verhindert, dass der Verkehr geändert wird, wenn er bei der Übertragung über das Netzwerk abgefangen wird.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied sein Computerkontenkennwort regelmäßig ändern kann. Wenn Sie diese Richtlinieneinstellung aktivieren, kann das Domänenmitglied sein Computerkontenkennwort nicht ändern. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann das Domänenmitglied sein Computerkontenkennwort entsprechend der Einstellung für **Domänenmitglied: Maximalalter von Computerkontenkennwörtern ändern**. Der Standardwert dieser Einstellung beträgt 30 Tage. Computer, die ihre Kontenkennwörter nicht automatisch ändern können, sind potenziell anfällig, weil ein Angreifer das Kennwort für das Domänenkonto des Systems ermitteln könnte.
  
Daher ist die Einstellung **Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Domänenmitglied: Maximalalter von Computerkontenkennwörtern**  
Durch diese Richtlinieneinstellung wird das maximal zulässige Alter für Computerkontenkennwörter festgelegt. Standardmäßig ändern Domänenmitglieder ihre Domänenkennwörter automatisch alle 30 Tage. Wenn Sie dieses Intervalls deutlich erhöhen oder auf 0 setzen, damit die Kennwörter von Computern nicht mehr geändert werden müssen, haben Angreifer mehr Zeit, um über Brute-Force-Angriffe das Kennwort von Computerkonten zu erraten.
  
Daher ist die Einstellung **Domänenmitglied: Maximalalter von Computerkontenkennwörtern** für die beiden in diesem Kapitel behandelten Umgebungen auf **30 Tage** gesetzt.
  
**Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)**  
Wenn diese Richtlinieneinstellung aktiviert ist, kann ein sicherer Kanal nur mit Domänencontrollern eingerichtet werden, die Daten des sicheren Kanals mit einem starken Sitzungsschlüssel (128-Bit) verschlüsseln können.
  
Für diese Einstellung ist es erforderlich, dass alle Domänencontroller der Domäne fähig sind, Daten des sicheren Kanals mit einem starken Schlüssel zu verschlüsseln. Dies bedeutet, dass alle Domänencontrollern über Windows 2000 oder höher verfügen müssen. Wenn die Kommunikation mit Domänen erforderlich ist, die nicht auf Windows 2000 basieren, sollte diese Richtlinieneinstellung deaktiviert werden.
  
Die Einstellung **Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows** **2000 oder höher)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
###### Interaktive Anmeldung
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für die interaktive Anmeldung. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A20: Empfohlene Einstellungen für Sicherheitsoptionen – Interaktive Anmeldung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden wollen</td>
<td style="border:1px solid black;">Leer</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten</td>
<td style="border:1px solid black;">Leer</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)<br />
(Desktopcomputer)</td>
<td style="border:1px solid black;">10</td>
<td style="border:1px solid black;">2</td>
<td style="border:1px solid black;">0</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)<br />
(Laptopcomputer)</td>
<td style="border:1px solid black;">10</td>
<td style="border:1px solid black;">2</td>
<td style="border:1px solid black;">2</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern</td>
<td style="border:1px solid black;">14 Tage</td>
<td style="border:1px solid black;">14 Tage</td>
<td style="border:1px solid black;">14 Tage</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich (Desktopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich (Laptopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards</td>
<td style="border:1px solid black;">Keine Aktion</td>
<td style="border:1px solid black;">Arbeitsstation sperren</td>
<td style="border:1px solid black;">Arbeitsstation sperren</td>
</tr>
</tbody>
</table>
  
**Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Kontoname des zuletzt auf den Clientcomputern in Ihrer Organisation angemeldeten Benutzers auf dem Windows-Anmeldebildschirm jedes Computers angezeigt wird. Durch Aktivieren dieser Richtlinieneinstellung können Sie verhindern, dass Eindringlinge Kontonamen von den Bildschirmen der Desktop- oder Laptopcomputer in Ihrer Organisation ablesen können.
  
Die Einstellung **Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich**  
Mit der Tastenkombination STRG+ALT+ENTF wird ein vertrauenswürdiger Pfad zum Betriebssystem hergestellt, wenn ein Benutzer einen Benutzernamen und ein Kennwort eingibt. Wenn diese Richtlinieneinstellung aktiviert ist, ist diese Tastenkombination nicht erforderlich, um sich im Netzwerk anzumelden. Diese Konfiguration stellt jedoch ein Sicherheitsrisiko dar, da sich Benutzer mit geringeren Anmeldeinformationen bei dem Client anmelden können.
  
Die Einstellung **Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden wollen**  
Durch diese Richtlinieneinstellung wird eine Textmeldung festgelegt, die bei der Anmeldung eines Benutzers angezeigt wird. Dieser Text wird häufig aus rechtlichen Gründen verwendet, z. B. um Benutzer auf die Auswirkungen eines Missbrauchs von Firmeninformationen hinzuweisen, oder um sie davor zu warnen, dass ihre Aktionen überwacht werden.
  
**Hinweis:**   Alle Warnmeldungen, die Sie anzeigen lassen, sollten vorher von den juristischen Vertretern und der Personalabteilung der Organisation genehmigt werden. Außerdem müssen die Einstellungen **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden wollen** und **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten***beide* aktiviert sein, damit jede von ihnen richtig funktioniert.
  
**Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten**  
Diese Richtlinieneinstellung ermöglicht das Festlegen von Text für die Titelleiste des Fensters, das Benutzer bei der Anmeldung beim System sehen. Der Grund für diese Richtlinieneinstellung ist derselbe wie für die vorangegangene Meldungstexteinstellung. Organisationen, die auf die Verwendung dieser Einstellung verzichten, sind rechtlich nicht gegen Unbefugte abgesichert, die das System angreifen.
  
**Hinweis:**   Alle Warnmeldungen, die Sie anzeigen lassen, sollten vorher von den juristischen Vertretern und der Personalabteilung der Organisation genehmigt werden. Außerdem müssen die Einstellungen **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden wollen** und **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** beide aktiviert sein, damit jede von ihnen richtig funktioniert.
  
**Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Benutzer sich mit zwischengespeicherten Kontoinformationen bei einer Windows-Domäne anmelden kann. Anmeldeinformationen für Domänenkonten können lokal zwischengespeichert werden, um Benutzern selbst dann die Anmeldung zu ermöglichen, wenn kein Domänencontroller erreichbar ist. Durch diese Einstellung wird die Anzahl von eindeutigen Benutzern festgelegt, für die Anmeldeinformationen lokal zwischengespeichert werden. Der Standardwert für diese Richtlinieneinstellung lautet 10. Wenn dieser Wert auf 0 gesetzt wird, wird der Anmeldecache deaktiviert. Ein Angreifer mit Zugriff auf das Dateisystem des Servers kann nach den zwischengespeicherten Informationen suchen und die Benutzerkennwörter mit einem Brute-Force-Angriff ermitteln.
  
Die Einstellung **Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)** ist in der Unternehmensclient-Umgebung sowohl für Desktop- als auch Laptopcomputer und in der Hochsicherheitsumgebung für Laptopcomputer auf **2** gesetzt. Für Desktops in der Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **0** gesetzt, da diese Computer immer eine sichere Verbindung zum Netzwerk der Organisation haben sollten.
  
**Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern**  
Durch diese Richtlinieneinstellung wird die Zeitspanne festgelegt, die Benutzer im Voraus auf den Ablauf ihrer Kennwörter hingewiesen werden. Microsoft empfiehlt, bei dieser Richtlinieneinstellung eine Frist von 14 Tagen einzugeben, damit Benutzer rechtzeitig über das Ablaufen des Kennworts informiert werden.
  
Die Einstellung **Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **14 Tage** gesetzt.
  
**Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich**  
Bei Aktivierung dieser Einstellung muss ein Domänencontroller das zum Entsperren des Computers verwendete Domänenkonto authentifizieren. Ist diese Richtlinieneinstellung deaktiviert, können zwischengespeicherte Anmeldeinformationen zum Aufheben der Sperrung des Computers verwendet werden. Microsoft empfiehlt, diese Richtlinieneinstellung für Laptopbenutzer in beiden Umgebungen zu deaktivieren, da mobile Benutzer keinen Netzwerkzugriff auf Domänencontrollern haben.
  
Die Einstellung **Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich** ist für Desktopcomputer sowohl in der Unternehmensclient-Umgebung als auch in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Diese Richtlinieneinstellung ist jedoch für Laptops in beiden Umgebungen auf **Deaktiviert** gesetzt, damit diese Benutzer auch außerhalb des Büros arbeiten können.
  
**Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards**  
Durch diese Richtlinieneinstellung wird festgelegt, was geschehen soll, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird. Wenn diese Richtlinieneinstellung auf **Arbeitsstation sperren** gesetzt ist, wird die Arbeitsstation beim Entfernen der Smartcard gesperrt. Auf diese Weise können Benutzer beim Verlassen des Arbeitsplatzes ihre Smartcards mitnehmen und ihre Arbeitsstationen automatisch sperren lassen. Wenn Sie diese Richtlinieneinstellung auf **Abmeldung erzwingen** einstellen, werden Benutzer bei der Entnahme der Smartcard automatisch abgemeldet.
  
Die Einstellung **Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Arbeitsstation sperren** gesetzt.
  
###### Microsoft-Netzwerk (Client)
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Clientcomputer im Microsoft-Netzwerk. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A21: Empfohlene Einstellungen für Sicherheitsoptionen – Microsoft-Netzwerk (Client)**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Client zustimmt)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob die SMB-Clientkomponente die Signierung von Paketen erfordert. Wenn Sie diese Richtlinieneinstellung aktivieren, kann der Microsoft-Netzwerkclient nur dann mit einem Microsoft-Netzwerkserver kommunizieren, wenn der Server der SMB-Paketsignierung zustimmt. In gemischten Umgebungen mit älteren Clients sollte diese Option auf **Deaktiviert** gesetzt werden, da diese Computer sich nicht authentifizieren und nicht auf Domänencontroller zugreifen können. In Umgebungen mit Windows 2000 oder höher kann diese Richtlinieneinstellung jedoch verwendet werden.
  
Die Einstellung **Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)** ist für Computer in beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Wenn diese Richtlinieneinstellung auf Windows Vista-basierten Computern aktiviert ist und diese eine Verbindung zu Datei- oder Druckerfreigaben auf Remoteservern herstellen, muss die Einstellung unbedingt mit ihrer begleitenden Einstellung, **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer),** auf diesen Servern synchronisiert werden. Weitere Informationen zu diesen Einstellungen finden Sie im Abschnitt „Microsoft-Netzwerk (Client und Server): Kommunikation digital signieren (vier in Zusammenhang stehende Einstellungen)“ von Kapitel 5 des Handbuchs [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10)).
  
**Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Client zustimmt)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln. Die Implementierung einer digitalen Signierung in Windows-basierten Netzwerken trägt dazu bei, Sitzungsübernahmen zu verhindern. Wenn Sie diese Richtlinieneinstellung aktivieren, verwendet der Microsoft-Netzwerkclient die Signierung nur dann, wenn der Server, mit dem er kommuniziert, digital signierte Kommunikation akzeptiert.
  
Die Einstellung **Microsoft-Netzwerk (Client): Kommunikationen digital signieren (wenn Server zustimmt)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Aktivieren Sie diese Richtlinieneinstellung auf SMB-Clients in Ihrem Netzwerk, damit sie bei der Paketsignierung mit allen Clients und Servern in Ihrer Umgebung kompatibel sind.
  
**Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden**  
Deaktivieren Sie diese Richtlinieneinstellung, um den SMB-Redirector davon abzuhalten, während der Authentifizierung Klartextkennwörter an SMB-Server von Drittanbietern zu senden, die die Kennwortverschlüsselung nicht unterstützen. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, wenn keine wichtigen geschäftlichen Anforderungen dagegen sprechen. Wenn diese Richtlinieneinstellung aktiviert ist, sind im gesamten Netzwerk unverschlüsselte Kennwörter zugelassen.
  
Die Einstellung **Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
###### Microsoft-Netzwerk (Server)
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Microsoft-Netzwerkserver. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A22: Empfohlene Einstellungen für Sicherheitsoptionen – Microsoft-Netzwerk (Server)**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung</td>
<td style="border:1px solid black;">15 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Server zustimmt)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung**  
Mit dieser Richtlinieneinstellung können Sie die Leerlaufzeitspanne in einer SMB-Sitzung festlegen, nach der die Sitzung aufgrund von Inaktivität angehalten wird. Administratoren können mit dieser Richtlinieneinstellung steuern, zu welchem Zeitpunkt eine nicht aktive Sitzung vom Computer angehalten wird. Wenn der Client seine Aktivität wieder aufnimmt, wird die Sitzung automatisch wiederhergestellt.
  
Die Einstellung **Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung** ist für die beiden in diesem Handbuch behandelten Umgebungen auf eine Zeitspanne von **15 Minuten** gesetzt.
  
**Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob SMB-Pakete vom SMB-Server signiert werden müssen. Aktivieren Sie diese Richtlinieneinstellung in einer gemischten Umgebung, damit Downstream-Clients Arbeitsstationen nicht als Netzwerkserver verwenden können.
  
Die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Server zustimmt)**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der serverseitige SMB-Dienst SMB-Pakete signieren kann, wenn dies von einem Client angefordert wird, der eine Verbindung herzustellen versucht. Wenn vom Client keine Signaturanforderung kommt, wird eine Verbindung ohne Signatur zugelassen, wenn die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** nicht aktiviert ist.
  
Die Einstellung **Microsoft-Netzwerk (Server): Kommunikationen digital signieren (wenn Client zustimmt)** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Aktivieren Sie diese Richtlinieneinstellung auf SMB-Clients in Ihrem Netzwerk, damit sie bei der Paketsignierung mit allen Clients und Servern in Ihrer Umgebung kompatibel sind.
  
**Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Verbindungen zu Benutzern getrennt werden, wenn diese außerhalb der für ihr Konto gültigen Anmeldezeiten mit dem lokalen Computer verbunden sind. Diese Richtlinieneinstellung betrifft die SMB-Komponente. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Clientsitzungen mit dem SMB-Dienst nach Ablauf der Anmeldezeit des Clients beendet. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden bestehende Clientsitzungen nach Ablauf der Anmeldezeit des Clients aufrechterhalten. Wenn Sie diese Richtlinieneinstellung aktivieren, sollte auch die Einstellung **Netzwerksicherheit:** **Abmeldung nach Ablauf der Anmeldezeit erzwingen** aktiviert werden.
  
Die Aktivierung dieser Richtlinieneinstellung ist sinnvoll, wenn in Ihrer Organisation Anmeldezeiten für Benutzer festgelegt wurden.
  
Die Einstellung **Microsoft-Netzwerk (Client): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
###### MSS-Einstellungen
  
Die folgenden Einstellungen enthalten Registrierungswerteinträge, die nicht standardmäßig im Sicherheitskonfigurations-Editor (SCE) angezeigt werden. Diese Einstellungen, die alle das Präfix **MSS:** aufweisen, wurden von der „Microsoft Solutions for Security“-Gruppe für frühere Sicherheitsanleitungen entwickelt. Durch das in Kapitel 1, „Implementieren der Sicherheitsbasis“, behandelte Skript GPOAccelerator.wsf wird der Sicherheitskonfigurations-Editor so verändert, dass er die MSS-Einstellungen korrekt anzeigt.
  
Die folgende Tabelle bietet einen Überblick über die MSS-Einstellungen, die für die einzelnen in diesem Handbuch behandelten Umgebungen empfohlen werden. Im Anschluss an die Tabelle werden weitere Informationen zu den einzelnen Einstellungen bereitgestellt.
  
**Tabelle A23: Empfohlene Einstellungen für Sicherheitsoptionen – MSS-Einstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">MSS: (AutoAdminLogon) Enable Automatic Logon<br />
(nicht empfohlen)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (DisableIPSourceRouting) IP source routing protection level (protects against packet spoofing)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Höchste Schutzebene, Quellrouting vollständig deaktiviert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (EnableDeadGWDetect) Allow automatic detection of dead network gateways (could lead to DoS)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (EnableICMPRedirect) Allow ICMP redirects to override OSPF generated routes</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (Hidden) Hide Computer From the Browse List (not recommended except for highly secure environments)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (KeepAliveTime)How often keep-alive packets are sent in milliseconds</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">30.000 oder 5 Minuten (empfohlen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (NoDefaultExempt) Configure IPSec exemptions for various types of network traffic</td>
<td style="border:1px solid black;">Multicast, Broadcast und ISAKMP sind ausgenommen (beste Einstellung für Windows XP)</td>
<td style="border:1px solid black;">Multicast, Broadcast und ISAKMP sind ausgenommen (beste Einstellung für Windows XP)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (NoDriveTypeAutoRun) Disable Autorun for all drives (recommended)</td>
<td style="border:1px solid black;">255, Autorun für alle Laufwerke deaktivieren</td>
<td style="border:1px solid black;">255, Autorun für alle Laufwerke deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (NoNameReleaseOnDemand) Allow the computer to ignore NetBIOS name release requests except from WINS servers</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (NtfsDisable8dot3NameCreation) Enable the computer to stop generating 8.3 style filenames (recommended)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (PerformRouterDiscovery) Allow IRDP to detect and configure DefaultGateway addresses (could lead to DoS)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (SafeDllSearchMode) Enable Safe DLL search mode (recommended)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (ScreenSaverGracePeriod) The time in seconds before the screen saver grace period expires<br />
(empfohlen: 0)</td>
<td style="border:1px solid black;">0</td>
<td style="border:1px solid black;">0</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (SynAttackProtect) Syn attack protection level (protects against DoS)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Verbindungen werden bei einem SYN-Angriff schneller beendet</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (TCPMaxConnectResponseRetransmissions) SYN-ACK retransmissions when a connection request is not acknowledged</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">3 und 6 Sekunden, halb offene Verbindungen nach 21 Sekunden beendet</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MSS: (TCPMaxDataRetransmissions) How many times unacknowledged data is retransmitted<br />
(empfohlen: 3, Standardwert: 5)</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">3</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MSS: (WarningLevel) Percentage threshold for the security event log at which the system will generate a warning</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">90</td>
</tr>
</tbody>
</table>
  
**MSS: (AutoAdminLogon) Enable Automatic Logon**  
Der Registrierungswert **AutoAdminLogon** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows NT\\CurrentVersion\\Winlogon\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (AutoAdminLogon) Enable Automatic Logon (not recommended)** angezeigt.
  
Diese Einstellung ist vom Begrüßungsbildschirm in Windows XP und Windows Vista getrennt. Wenn dieser deaktiviert ist, ist diese Einstellung nicht deaktiviert. Wenn Sie einen Computer für die automatische Anmeldung konfigurieren, kann jeder, der physischen Zugriff auf den Computer erlangen kann, außerdem Zugriff auf alle auf dem Computer befindlichen Daten erhalten. Dazu gehören auch alle Netzwerke, mit denen der Computer verbunden ist. Wenn Sie die automatische Anmeldung aktivieren, wird das Kennwort in Klartext in der Registrierung gespeichert. Der Registrierungsschlüssel, in dem dieser Wert gespeichert wird, kann von der Gruppe „Authentifizierte Benutzer“ von einem Remotestandort aus gelesen werden. Aus diesen Gründen ist die Einstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt, und in der Hochsicherheitsumgebung wird ausdrücklich die Standardeinstellung **Deaktiviert** erzwungen.
  
Zusätzliche Informationen finden Sie im Knowledge Base-Artikel 315231, [Aktivieren der automatischen Anmeldung in Windows XP](http://support.microsoft.com/kb/315231).
  
**MSS: (DisableIPSourceRouting) IP source routing protection level**  
Der Registrierungswert **DisableIPSourceRouting** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (DisableIPSourceRouting) IP source routing protection level (protects against packet spoofing)** angezeigt.
  
Über das IP-Quellrouting kann ein Sender die IP-Route eines Datagramms im Netzwerk festlegen. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Höchste Schutzebene,** **Quellrouting vollständig deaktiviert** gesetzt.
  
**MSS: (EnableDeadGWDetect) Allow automatic detection of dead network gateways**  
Der Registrierungswert **EnableDeadGWDetect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (EnableDeadGWDetect) Allow automatic detection of dead network gateways (could lead to DoS)** angezeigt.
  
Wenn die Funktion zur Identifizierung deaktivierter Gateways („Dead Gateway Detection“) aktiviert ist, kann das IP-Protokoll zu einem Sicherungsgateway wechseln, wenn bei mehreren Verbindungen Fehler auftreten. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**MSS: (EnableICMPRedirect) Allow ICMP redirects to override OSPF generated routes**  
Der Registrierungswert **EnableICMPRedirect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (EnableICMPRedirect) Allow ICMP redirects to override OSPF generated routes** angezeigt.
  
ICMP-Umleitungen (Internet Control Message Protocol-Umleitungen) bewirken, dass der Stapel Hostrouten einrichtet. Diese Routen setzen die über OSPF (Open Shortest Path First) erstellten Routen außer Kraft. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**MSS: (Hidden) Hide Computer From the Browse List**  
Der Registrierungswert **Hidden** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Lanmanserver\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (Hidden) Hide Computer From the Browse List (not recommended except for highly secure environments)** angezeigt.
  
Sie können einen Computer so konfigurieren, dass er den Browsern in der Domäne keine Ankündigungen sendet. Wenn Sie dies tun, blenden Sie den Computer aus der Suchliste aus. Das bedeutet, dass der Computer seine Anwesenheit vor anderen Computern im gleichen Netzwerk verbirgt. Ein Angreifer, der den Namen eines Computers kennt, kann viel leichter zusätzliche Informationen über das System sammeln. Sie können diese Einstellung aktivieren, um eine Methode zu eliminieren, mit der ein Angreifer Informationen über Computer im Netzwerk erfassen könnte. Außerdem kann die Aktivierung dieser Einstellung zur Verringerung des Netzwerkverkehrs beitragen. Die Sicherheitsvorteile dieser Einstellung sind jedoch gering, da Angreifer alternative Methoden verwenden können, um potenzielle Ziele zu identifizieren und zu finden. Aus diesem Grund empfiehlt Microsoft, diese Einstellung nur in Hochsicherheitsumgebungen zu aktivieren.
  
Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
Zusätzliche Informationen finden Sie im Knowledge Base-Artikel 321710 [HOW TO: Hide a Windows 2000-Based Computer from the Browser List](http://support.microsoft.com/kb/321710/en-us) (engl.).
  
**MSS: (KeepAliveTime) How often keep-alive packets are sent in milliseconds**  
Der Registrierungswert **KeepAliveTime** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (KeepAliveTime) How often keep-alive packets are sent in milliseconds (300,000 is recommended)** angezeigt.
  
Mit diesem Wert wird die Anzahl der TCP-Versuche festgelegt, bei denen durch Senden von Keep Alive-Paketen überprüft wird, ob eine Leerlaufverbindung immer noch hergestellt ist. Wenn die Verbindung mit dem Remotecomputer noch besteht, bestätigt dieser die Keep Alive-Pakete. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **300.000** bzw. **5 Minuten** gesetzt.
  
**MSS: (NoDefaultExempt) Configure IPSec exemptions for various types of network traffic**  
Der Registrierungswert **NoDefaultExempt** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\IPSEC\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (NoDefaultExempt) Configure IPSec exemptions for various types of network traffic** angezeigt.
  
Die Standardausnahmen bei IPsec-Richtlinienfiltern werden in der Onlinehilfe für das jeweilige Betriebssystem dokumentiert. Diese Filter ermöglichen die Funktion des gegenseitigen Schlüsselaustausches (Internet Key Exchange, IKE) und des Kerberos-Authentifizierungsprotokolls. Mit den Filtern kann außerdem das Netzwerk-QoS (Quality of Service) signalisiert werden (RSVP), und zwar sowohl durch IPSec gesicherten Datenverkehr als auch bei nicht durch IPSec gesichertem Datenverkehr (z. B. bei Multicast- und Broadcastverkehr).
  
IPSec wird zunehmend für die grundlegende Hostfirewall-Paketfilterung verwendet, insbesondere in Szenarien mit einer Gefährdung durch Internetverbindungen. Die Auswirkungen dieser Standardausnahmen werden jedoch nicht immer richtig verstanden. Einige IPSec-Administratoren erstellen daher u. U. vermeintlich sichere IPSec-Richtlinien, die jedoch nicht vor eingehenden Angriffen schützen, bei denen die Standardausnahmen verwendet werden. Microsoft empfiehlt, für die beiden in diesem Handbuch behandelten Umgebungen die Standardeinstellung in Windows XP mit SP2, **Multicast,** **Broadcastund ISAKMP sind ausgenommen**, zu verwenden.
  
Zusätzliche Informationen finden Sie im Knowledge Base-Artikel 811832, [IPSec Default Exemptions Can Be Used to Bypass IPsec Protection in Some Scenarios](http://support.microsoft.com/kb/811832/en-us) (engl.).
  
**MSS: (NoDriveTypeAutoRun) Disable Autorun for all drives**  
Der Registrierungswert **NoDriveTypeAutoRun** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\**  
**Policies\\Explorer\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (NoDriveTypeAutoRun) Disable Autorun for all drives (recommended)** angezeigt.
  
Bei Aktivierung von Autorun (AutoAusführen) werden Daten unmittelbar nach dem Einlegen von Medien in ein Laufwerk gelesen. Dies hat zur Folge, dass die Setup-Dateien von Programmen und die Klangwiedergabe von Audiomedien sofort gestartet werden. Diese Einstellung ist für die beiden in diesem Handbuch behandelten Umgebungen auf **255,** **Autorun für alle Laufwerke deaktivieren** gesetzt.
  
**MSS: (NoNameReleaseOnDemand) Allow the computer to ignore NetBIOS name release requests except from WINS servers**  
Der Registrierungswert **NoNameReleaseOnDemand** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Netbt\\**  
**Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (NoNameReleaseOnDemand) Allow the computer to ignore NetBIOS name release requests except from WINS servers** angezeigt.
  
„NetBIOS über TCP/IP“ ist ein Netzwerkprotokoll, das u. a. eine Möglichkeit zur einfachen Auflösung der in Windows-basierten Systemen registrierten NetBIOS-Namen in auf diesen Systemen konfigurierte IP-Adressen bereitstellt. Durch diese Einstellung wird festgelegt, ob der NetBIOS-Name des Computers beim Empfang einer Namensfreigabeanforderung freigegeben wird. Der Wert ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**MSS: (NtfsDisable8dot3NameCreation) Enable the computer to stop generating 8.3 style filenames**  
Der Registrierungswert **NtfsDisable8dot3NameCreation** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Control\\FileSystem\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (NtfsDisable8dot3NameCreation) Enable the computer to stop generating 8.3 style filenames (recommended)** angezeigt.
  
Windows Server 2003 unterstützt 8.3-Dateinamensformate zur Gewährleistung der Abwärtskompatibilität mit 16-Bit-Anwendungen. Bei der 8.3-Dateinamenskonvention handelt es sich um ein Namensformat, bei dem Dateinamen mit maximal acht Zeichen zulässig sind. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**MSS: (PerformRouterDiscovery) Allow IRDP to detect and configure Default Gateway addresses**  
Der Registrierungswert **PerformRouterDiscovery** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (PerformRouterDiscovery) Allow IRDP to detect and configure Default Gateway addresses (could lead to DoS)** angezeigt.
  
Über diese Einstellung wird IRDP (Internet Router Discovery Protocol) aktiviert oder deaktiviert. Dies ermöglicht dem System, wie in RFC 1256 beschrieben Standardgatewayadressen automatisch pro Schnittstelle zu erkennen und zu konfigurieren. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**MSS: (SafeDllSearchMode) Enable Safe DLL Search Order**  
Der Registrierungswert **SafeDllSearchMode** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\ SYSTEM\\CurrentControlSet\\Control\\Session Manager\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (SafeDllSearchMode) Enable Safe DLL search mode (recommended)** angezeigt.
  
Zum Konfigurieren der DLL-Suchreihenfolge für die Suche nach DLLs, die von laufenden Prozessen angefordert werden, stehen zwei Methoden zur Auswahl:
  
-   Zuerst die im Systempfad angegebenen Ordner und dann den aktuellen Arbeitsordner durchsuchen.
  
-   Zuerst den aktuellen Arbeitsordner und dann die im Systempfad angegebenen Ordner durchsuchen.
  
Bei Aktivierung wird der Registrierungswert auf 1 gesetzt. Bei einer Einstellung von 1 werden zuerst die im Systempfad angegebenen Ordner und anschließend der aktuelle Arbeitsordner durchsucht. Bei Deaktivierung wird der Registrierungswert auf 0 gesetzt. Bei dieser Einstellung werden zuerst der aktuelle Arbeitsordner und anschließend die im Systempfad angegebenen Ordner durchsucht. Diese Einstellung ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**MSS: (ScreenSaverGracePeriod) The time in seconds before the screen saver grace period expires**  
Der Registrierungswert **ScreenSaverGracePeriod** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\SYSTEM\\Software\\Microsoft\\**  
**Windows NT\\CurrentVersion\\Winlogon\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (ScreenSaverGracePeriod) The time in seconds before the screen saver grace period expires (0 recommended)** angezeigt.
  
Windows bietet einen Kulanzzeitraum zwischen dem Starten des Bildschirmschoners und der tatsächlichen automatischen Sperrung der Konsole, wenn die Bildschirmschonersperre aktiviert ist. Diese Einstellung ist für die beiden in diesem Handbuch behandelten Umgebungen auf **0** Sekunden gesetzt.
  
**MSS: (SynAttackProtect) Syn attack protection level**  
Der Registrierungswert **SynAttackProtect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (SynAttackProtect) Syn attack protection level (protects against DoS)** angezeigt.
  
Diese Einstellung zwingt das TCP-Protokoll zur Anpassung der Umleitung von SYN-ACKs. Wenn Sie diesen Wert konfigurieren, wird die Verbindungsantwort bei Feststellung eines Verbindungsanforderungsangriffs (SYN-Angriff) schneller beendet. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Verbindungen werden bei einem SYN-Angriff schneller beendet** gesetzt.
  
**MSS: (TCPMaxConnectResponseRetransmissions) SYN-ACK retransmissions when a connection request is not acknowledged**  
Der Registrierungswert **TCPMaxConnectResponseRetransmissions** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\**  
**Services\\Tcpip\\Parameters**\\ hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (TcpMaxConnectResponseRetransmissions) SYN-ACK retransmissions when a connection request is not acknowledged** angezeigt.
  
Durch diese Einstellung wird die Anzahl der erneuten Übertragungen von SYN-Paketen über TCP vor dem Abbruch der Verbindung festgelegt. Das Zeitlimlit für erneute Übertragungen verdoppelt sich im Rahmen eines Verbindungsversuchs mit jeder nachfolgenden erneuten Übertragung. Der Standardwert beträgt 3 Sekunden. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **3 und 6 Sekunden,** **halb offene Verbindungen nach 21 Sekunden beendet** gesetzt.
  
**MSS: (TCPMaxDataRetransmissions) How many times unacknowledged data is retransmitted**  
Der Registrierungswert **TCPMaxDataRetransmissions** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip**  
**\\Parameters\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (TcpMaxDataRetransmissions) How many times unacknowledged data is retransmitted (3 recommended,** **5 is default)** angezeigt.
  
Mit diesem Eintrag wird die Anzahl der Versuche zur Übertragung einzelner Datensegmente vor einem Verbindungsabbruch festgelegt. Das Zeitlimlit für erneute Übertragungen verdoppelt sich bei einer Verbindung mit jeder nachfolgenden erneuten Übertragung. Es wird zurückgesetzt, wenn erneut Antworten eingehen. Der Basiswert für das Zeitlimit wird dynamisch anhand der gemessenen Roundtrip-Zeit bestimmt. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **3** gesetzt.
  
**MSS: (WarningLevel) Percentage threshold for the security event log at which the system will generate a warning**  
Der Registrierungswert **WarningLevel** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\ SYSTEM\\CurrentControlSet\\Services\\Eventlog\\Security\\** hinzugefügt. Im Sicherheitskonfigurations-Editor wird der Eintrag als **MSS: (WarningLevel) Percentage threshold for the security event log at which the system will generate a warning** angezeigt.
  
Durch diese Einstellung kann beim Überschreiten eines benutzerdefinierten Schwellenwerts eine Sicherheitsüberwachung im Sicherheitsereignisprotokoll erzeugt werden. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **90** gesetzt.
  
**Hinweis:**   Wenn Protokolleinstellungen auf **Ereignisse bei Bedarf überschreiben** oder **Ereignisse überschreiben, die älter sind als** ***x*** **Tage** gesetzt sind, wird dieses Ereignis nicht erzeugt.
  
###### Netzwerkzugriff
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für den Netzwerkzugriff. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A24: Empfohlene Einstellungen für Sicherheitsoptionen – Netzwerkzugriff**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann</td>
<td style="border:1px solid black;">netlogon, lsarpc, samr, browser</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">netlogon, lsarpc, samr, browser</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann</td>
<td style="border:1px solid black;">System\CurrentControlSet\<br />
Control\ProductOptions
System\CurrentControlSet\<br />
Control\Server Applications
Software\Microsoft\Windows NT\CurrentVersion</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">System\CurrentControlSet\<br />
Control\ProductOptions
System\CurrentControlSet\<br />
Control\Server Applications
Software\Microsoft\Windows NT\CurrentVersion</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Netzwerkzugriff: Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann</td>
<td style="border:1px solid black;">System\CurrentControlSet\<br />
Control\Print\Printers
System\CurrentControlSet\<br />
Services\Eventlog
Software\Microsoft\OLAP Server
Software\Microsoft\Windows NT\CurrentVersion\Print
Software\Microsoft\Windows NT\CurrentVersion\Windows
System\CurrentControlSet\<br />
ContentIndex
System\CurrentControlSet\<br />
Control\Terminal Server
System\CurrentControlSet\<br />
Control\Terminal Server\User Config
System\CurrentControlSet\<br />
Control\Terminal Server\Default User Config
Software\Microsoft\Windows NT\CurrentVersion\perflib
System\CurrentControlSet\<br />
Services\SysmonLog</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">System\CurrentControlSet\<br />
Control\Print\Printers
System\CurrentControlSet\<br />
Services\Eventlog
Software\Microsoft\OLAP Server
Software\Microsoft\Windows NT\CurrentVersion\Print
Software\Microsoft\Windows NT\CurrentVersion\Windows
System\CurrentControlSet\<br />
ContentIndex
System\CurrentControlSet\<br />
Control\Terminal Server
System\CurrentControlSet\<br />
Control\Terminal Server\User Config
System\CurrentControlSet\<br />
Control\Terminal Server\Default User Config
Software\Microsoft\Windows NT\CurrentVersion\perflib
System\CurrentControlSet\<br />
Services\SysmonLog</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Keine</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten</td>
<td style="border:1px solid black;">Klassisch – lokale Benutzer authentifizieren sich als sie selbst</td>
<td style="border:1px solid black;">Klassisch – lokale Benutzer authentifizieren sich als sie selbst</td>
<td style="border:1px solid black;">Klassisch – lokale Benutzer authentifizieren sich als sie selbst</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer Sicherheits-ID-Attribute anderer Benutzer anfordern können oder eine Sicherheits-ID (SID) verwenden können, um den zugehörigen Benutzernamen zu erhalten. Deaktivieren Sie diese Richtlinieneinstellung, um zu verhindern, dass nicht autorisierte Benutzer Benutzernamen über die zugehörigen Sicherheits-IDs in Erfahrung bringen.
  
Die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben**  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer die Konten in der Sicherheitskontenverwaltung (SAM, Security Accounts Manager) anzeigen lassen können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind Benutzer mit anonymen Verbindungen nicht in der Lage, Domänenkontonamen an einer Arbeitsstation in Ihrer Umgebung anzuzeigen. Durch diese Richtlinieneinstellung werden weitere Einschränkungen für anonyme Verbindungen ermöglicht.
  
Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben**  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer SAM-Konten und -Freigaben anzeigen lassen können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind anonyme Benutzer nicht in der Lage, Domänenkontonamen und Namen für Netzwerkfreigaben an einer Arbeitsstation in Ihrer Umgebung anzuzeigen.
  
Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben**  
Diese Richtlinieneinstellung steuert die Speicherung der Anmeldeinformationen und der Kennwörter auf dem lokalen System.
  
Die Einstellung **Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen**  
Durch diese Richtlinieneinstellung wird festgelegt, welche zusätzlichen Berechtigungen anonymen Verbindungen mit dem Computer gewährt werden. Wenn Sie diese Richtlinieneinstellung aktivieren, können anonyme Windows-Benutzer bestimmte Aktivitäten ausführen, z. B. Auflisten der Namen von Domänenkonten und Netzwerkfreigaben. Ein nicht autorisierter Benutzer könnte Kontennamen und freigegebene Ressourcen anonym auflisten und anhand dieser Informationen Kennwörter erraten oder Social Engineering-Angriffe durchführen.
  
Deshalb ist die Einstellung **Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen** für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann**  
Durch diese Richtlinieneinstellung wird festgelegt, welche Kommunikationssitzungen oder Pipes über Attribute und Berechtigungen verfügen, die anonymen Zugriff zulassen.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann** auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung werden jedoch folgende Standardwerte verwendet:
  
-   Netlogon
  
-   Isarpc
  
-   Samr
  
-   Browser
  
**Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann**  
Durch diese Richtlinieneinstellung wird festgelegt, auf welche Registrierungspfade zugegriffen werden kann, nachdem der Schlüssel WinReg zur Feststellung der Zugriffsberechtigungen für diese Pfade ausgewertet wurde.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann** auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung werden jedoch folgende Standardwerte verwendet:
  
-   System\\CurrentControlSet\\Control\\ProductOptions
  
-   System\\CurrentControlSet\\Control\\Server Applications
  
-   Software\\Microsoft\\Windows NT\\CurrentVersion
  
**Netzwerkzugriff: Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann**  
Durch diese Richtlinieneinstellung wird festgelegt, auf welche Registrierungspfade und -unterpfade zugegriffen werden kann, wenn eine Anwendung oder ein Prozess den Schlüssel **WinReg** zur Feststellung der Zugriffsberechtigungen auswertet.
  
Die Einstellung **Netzwerkzugriff: Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung ist die Einstellung wie folgt konfiguriert:
  
-   System\\CurrentControlSet\\Control\\Print\\Printers
  
-   System\\CurrentControlSet\\Services\\Eventlog
  
-   Software\\Microsoft\\OLAP Server
  
-   Software\\Microsoft\\Windows NT\\CurrentVersion\\Print
  
-   Software\\Microsoft\\Windows NT\\CurrentVersion\\Windows
  
-   System\\CurrentControlSet\\ContentIndex
  
-   System\\CurrentControlSet\\Control\\Terminal Server
  
-   System\\CurrentControlSet\\Control\\Terminal Server\\User Config
  
-   System\\CurrentControlSet\\Control\\Terminal Server\\Default User Config
  
-   Software\\Microsoft\\Windows NT\\CurrentVersion\\perflib
  
-   System\\CurrentControlSet\\Services\\SysmonLog
  
**Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken**  
Wenn diese Richtlinieneinstellung aktiviert ist, wird der anonyme Zugriff auf die Freigaben und Pipes begrenzt, die in den Einstellungen **Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann** und **Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann** genannt werden. Durch diese Richtlinieneinstellung wird der Nullsitzungszugriff auf Computerfreigaben gesteuert, indem **RestrictNullSessAccess** mit dem Wert **1** im Registrierungsschlüssel **HKLM\\System**  
**\\CurrentControlSet\\Services\\LanManServer\\Parameters** hinzugefügt wird. Mit diesem Registrierungswert können Nullsitzungsfreigaben aktiviert bzw. deaktiviert werden. Dadurch wird festgelegt, ob der Serverdienst den nicht authentifizierten Clientzugriff auf die genannten Ressourcen begrenzt. Nullsitzungen sind ein Sicherheitsrisiko, das über die einzelnen Freigaben (einschließlich der Standardfreigaben) auf den Computern in Ihrer Umgebung ausgenutzt werden kann.
  
Die Einstellung **Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann**  
Durch diese Richtlinieneinstellung werden die Netzwerkfreigaben festgelegt, auf die anonyme Benutzer zugreifen können. Die Standardeinstellung für diese Richtlinieneinstellung hat geringe Auswirkungen, da alle Benutzer authentifiziert werden müssen, bevor sie auf freigegebene Ressourcen auf dem Server zugreifen können.
  
Die Einstellung **Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Sie sollten jedoch sicherstellen, dass diese Einstellung für die Hochsicherheitsumgebung auf **Keine** gesetzt ist.
  
**Hinweis**:   Es kann sehr gefährlich sein, dieser Gruppenrichtlinieneinstellung weitere Freigaben hinzuzufügen. Jeder Netzwerkbenutzer kann auf alle aufgelisteten Freigaben zugreifen, wodurch vertrauliche Daten preisgegeben oder beschädigt werden könnten.
  
**Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten**  
Durch diese Richtlinieneinstellung wird festgelegt, wie Netzwerkanmeldungen über lokale Konten authentifiziert werden. Die Option **Klassisch** ermöglicht eine präzise Steuerung des Zugriffs auf Ressourcen, einschließlich der Möglichkeit, verschiedenen Benutzern unterschiedliche Zugriffstypen für dieselbe Ressource zuzuweisen. Die Option **Nur Gast** ermöglicht Ihnen, alle Benutzer gleich zu behandeln. In diesem Fall werden alle Benutzer als **Nur Gast** authentifiziert und haben dieselben Zugriffsrechte auf die jeweilige Ressource.
  
Daher verwendet die Einstellung **Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten** für die beiden in diesem Handbuch behandelten Umgebungen die standardmäßige Option **Klassisch**.
  
###### Netzwerksicherheit
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für die Netzwerksicherheit. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A25: Empfohlene Einstellungen für Sicherheitsoptionen – Netzwerksicherheit**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerksicherheit: LAN Manager-Authentifizierungsebene</td>
<td style="border:1px solid black;">Nur NTLMv2-Antworten senden</td>
<td style="border:1px solid black;">Nur NTLMv2-Antworten senden. LM verweigern</td>
<td style="border:1px solid black;">Nur NTLMv2-Antworten senden. LM und NTLM verweigern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerksicherheit: Signaturanforderungen für LDAP-Clients</td>
<td style="border:1px solid black;">Signatur aushandeln</td>
<td style="border:1px solid black;">Signatur aushandeln</td>
<td style="border:1px solid black;">Signatur aushandeln</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)</td>
<td style="border:1px solid black;">Kein Minimum</td>
<td style="border:1px solid black;">NTLMv2-Sitzungssicherheit erfordern, 128-Bit-Verschlüsselung erfordern</td>
<td style="border:1px solid black;">NTLMv2-Sitzungssicherheit erfordern, 128-Bit-Verschlüsselung erfordern</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)</td>
<td style="border:1px solid black;">Kein Minimum</td>
<td style="border:1px solid black;">NTLMv2-Sitzungssicherheit erfordern, 128-Bit-Verschlüsselung erfordern</td>
<td style="border:1px solid black;">NTLMv2-Sitzungssicherheit erfordern, 128-Bit-Verschlüsselung erfordern</td>
</tr>
</tbody>
</table>
  
**Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern**  
Durch diese Richtlinieneinstellung wird festgelegt, ob die bei der Änderung von Kennwörtern vom LAN Manager (LM) erzeugten Hashwerte für das neue Kennwort gespeichert werden. LM-Hashwerte sind anfälliger für Angriffe, weil für ihre Erzeugung im Vergleich zu Microsoft Windows NT®-Hashwerten ein schwächerer kryptografischer Algorithmus verwendet wird.
  
Aus diesem Grund ist die Einstellung **Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern** für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Ältere Betriebssysteme und einige Anwendungen von Drittanbietern fallen möglicherweise aus, wenn diese Einstellung aktiviert ist. Außerdem müssen Sie nach dem Aktivieren dieser Einstellung die Kennwörter sämtlicher Konten ändern.
  
**Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen**  
Diese Richtlinieneinstellung bestimmt, ob Verbindungen zu Benutzern getrennt werden, wenn diese außerhalb der für ihr Konto gültigen Anmeldezeiten mit dem lokalen Computer verbunden sind. Sie betrifft die SMB-Komponente. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Clientsitzungen mit dem SMB-Server nach Ablauf der Anmeldezeit des Clients beendet. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden bestehende Clientsitzungen nach Ablauf der Anmeldezeit des Benutzers aufrechterhalten.
  
Die Einstellung **Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen** ist für beide in diesem Anhang behandelten Umgebungen auf **Nicht definiert** gesetzt.
  
**Netzwerksicherheit: LAN Manager-Authentifizierungsebene**  
Durch diese Richtlinieneinstellung wird die Art der Anfrage/Antwort-Authentifizierung für Netzwerkanmeldungen festgelegt. Die Authentifizierung über LAN Manager (LM) ist die unsicherste Methode, da verschlüsselte Kennwörter leicht über das Netzwerk abgefangen und entschlüsselt werden können. NT LAN Manager (NTLM) ist etwas sicherer. NTLMv2 ist robuster als NTLM und kann unter Windows Vista, Windows XP Professional, Windows Server 2003, Windows 2000 und Windows NT 4.0 Service Pack 4 oder höher verwendet werden. NTLMv2 ist zusammen mit dem optionalen Client für Verzeichnisdienste auch unter Windows 95 und Windows 98 verfügbar.
  
Microsoft empfiehlt, für diese Richtlinieneinstellung in Ihrer Umgebung die höchste Authentifizierungsebene auszuwählen. Bei Verwendung von Windows 2000 Server oder Windows Server 2003 mit auf Windows Vista oder Windows XP Professional basierenden Arbeitsstationen wird empfohlen, für diese Richtlinieneinstellung die Option **Nur NTLMv2-Antworten senden. LM und NTLM verweigern** zu wählen, um maximale Sicherheit zu gewährleisten.
  
Die Einstellung **Netzwerksicherheit: LAN Manager-Authentifizierungsebene** ist für die Unternehmensclient-Umgebung auf **Nur NTLMv2-Antworten senden. LM verweigern** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf das stärker einschränkende **Nur NTLMv2-Antworten senden. LM und NTLM verweigern** gesetzt.
  
**Netzwerksicherheit: Signaturanforderungen für LDAP-Clients**  
Durch diese Richtlinieneinstellung wird die Datensignaturebene festgelegt, die im Auftrag von Clients angefordert wird, wenn diese LDAP-BIND-Anforderungen ausgeben. Nicht signierter Netzwerkverkehr ist für Man-in-the-Middle-Angriffe anfällig. Ein Angreifer könnte einen Server veranlassen, Entscheidungen zu treffen, die auf falschen Anfragen vom LDAP-Client basieren.
  
Daher wird der Wert für die Einstellung **Netzwerksicherheit: Signaturanforderungen für LDAP-Clients** für die beiden in diesem Handbuch behandelten Umgebungen auf **Signatur aushandeln** gesetzt.
  
**Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)**  
Durch diese Richtlinieneinstellung werden die minimalen Sicherheitsstandards für die Kommunikation zwischen Anwendungen auf Clients festgelegt. Die Optionen für diese Richtlinieneinstellung lauten:
  
-   NTLMv2-Sitzungssicherheit erfordern
  
-   128-Bit-Verschlüsselung erfordern
  
Wenn alle Computer in Ihrem Netzwerk NTLMv2- und 128-Bit-Verschlüsselung unterstützen (z. B. Windows Vista, Windows XP Professional SP2 und Windows Server 2003 SP1), können für maximale Sicherheit alle vier Einstellungsoptionen ausgewählt werden.
  
Die Optionen **NTLMv2-Sitzungssicherheit erfordern** und **128-Bit-Verschlüsselung erfordern** sind für die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)** in beiden in diesem Handbuch behandelten Umgebungen aktiviert.
  
**Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)**  
Diese Richtlinieneinstellung ähnelt der vorherigen Einstellung, wirkt sich aber auf die serverseitige Kommunikation mit Anwendungen aus. Die Optionen für die Einstellung sind dieselben:
  
-   NTLMv2-Sitzungssicherheit erfordern
  
-   128-Bit-Verschlüsselung erfordern
  
Wenn alle Computer in Ihrem Netzwerk NTLMv2- und 128-Bit-Verschlüsselung unterstützen (z. B. Windows Vista, Windows XP Professional SP2 und Windows Server 2003 SP1), können für maximale Sicherheit alle vier Optionen ausgewählt werden.
  
Die Optionen **NTLMv2-Sitzungssicherheit erfordern** und **128-Bit-Verschlüsselung erfordern** sind für die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)** in beiden in diesem Handbuch behandelten Umgebungen aktiviert.
  
###### Wiederherstellungskonsole
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für die Wiederherstellungskonsole. Weitere Informationen finden Sie in den darauf folgenden Unterabschnitten.
  
**Tabelle A26: Empfohlene Einstellungen für Sicherheitsoptionen – Wiederherstellungskonsole**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen**  
Die Wiederherstellungskonsole ist eine Befehlszeilenumgebung, mit der nach Systemproblemen eine Wiederherstellung vorgenommen werden kann. Wenn Sie diese Richtlinieneinstellung aktivieren, wird das Administratorkonto automatisch bei der Wiederherstellungskonsole angemeldet, wenn diese beim Start aufgerufen wird. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, so dass Administratoren ein Kennwort eingeben müssen, um auf die Wiederherstellungskonsole zugreifen zu können.
  
Die Einstellung **Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen**  
Durch diese Richtlinieneinstellung wird in der Wiederherstellungskonsole der Befehl SET verfügbar, mit dem Sie die folgenden Umgebungsvariablen für die Wiederherstellungskonsole einstellen können:
  
-   **AllowWildCards**. Aktiviert die Platzhalterunterstützung für einige Befehle (z. B. für den Befehl DEL).
  
-   **AllowAllPaths**. Ermöglicht den Zugriff auf alle Dateien und Ordner auf dem Computer.
  
-   **AllowRemovableMedia**. Ermöglicht das Kopieren von Dateien auf Wechseldatenträger, z. B. auf Disketten.
  
-   **NoCopyPrompt**. Zeigt beim Überschreiben einer vorhandenen Datei keine Bestätigungsaufforderung an.
  
Die Einstellung **Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Zum Gewährleisten maximaler Sicherheit wird diese Einstellung in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
###### Herunterfahren
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen beim Herunterfahren. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A27: Empfohlene Einstellungen für Sicherheitsoptionen – Herunterfahren**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Herunterfahren: Auslagerungsdatei des virtuellen Arbeitsspeichers löschen (Desktopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Herunterfahren: Auslagerungsdatei des virtuellen Arbeitsspeichers löschen (Laptopcomputer)</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Computer heruntergefahren werden kann, wenn ein Benutzer nicht angemeldet ist. Wenn diese Richtlinieneinstellung aktiviert ist, steht im Windows-Anmeldebildschirm der Befehl „Herunterfahren“ zur Verfügung. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, um nur denjenigen Benutzern das Herunterfahren von Computern zu ermöglichen, die über Anmeldeinformationen im System verfügen.
  
Die Einstellung **Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Herunterfahren: Auslagerungsdatei des virtuellen Arbeitsspeichers löschen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Auslagerungsdatei des virtuellen Arbeitsspeichers beim Herunterfahren des Systems gelöscht wird. Wenn diese Richtlinieneinstellung aktiviert ist, wird die Auslagerungsdatei des Systems bei jedem ordnungsgemäßen Herunterfahren des Systems gelöscht. Bei Aktivierung dieser Sicherheitseinstellung wird die Ruhezustanddatei (hiberfil.sys) gelöscht, wenn die Ruhezustandfunktion auf einem tragbaren Computer deaktiviert ist. Das Herunterfahren und Neustarten des Computers dauert länger, insbesondere auf Computern mit großen Auslagerungsdateien.
  
Aus diesen Gründen ist die Einstellung **Herunterfahren: Auslagerungsdatei des virtuellen Arbeitsspeichers löschen** für Laptopcomputer in der Hochsicherheitsumgebung auf **Aktiviert** und für alle anderen Computer in den in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
###### Systemkryptografie
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Systemkryptografie. Im Anschluss an die Tabelle werden weitere Informationen bereitgestellt.
  
**Tabelle A28: Empfohlene Einstellungen für Sicherheitsoptionen – Systemkryptografie**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Sicherheitsanbieter für TLS/SSL (Transport Layer Security/Secure Sockets Layer) nur die Verschlüsselungssammlung TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA unterstützt. Obwohl durch diese Richtlinieneinstellung die Sicherheit erhöht wird, werden diese Algorithmen von den meisten öffentlichen Websites, die mit TLS oder SSL gesichert sind, nicht unterstützt. Clientcomputer, für die diese Richtlinieneinstellung aktiviert ist, können auch keine Verbindung zu Terminaldiensten auf Servern herstellen, die nicht für die Verwendung der FIPS-konformen Algorithmen konfiguriert sind.
  
Die Einstellung **Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung,** **Hashingund Signatur verwenden** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Hinweis:**   Wenn Sie diese Richtlinieneinstellung aktivieren, verlangsamt sich die Systemleistung des Computers, da durch den Dreifach-DES-Prozess die Verschlüsselung für jeden einzelnen Datenblock in der betreffenden Datei dreimal ausgeführt wird. Diese Richtlinieneinstellung sollte nur aktiviert werden, wenn für Ihre Organisation FIPS-Konformität erforderlich ist.
  
###### Systemobjekte
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für Systemobjekte. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A29: Empfohlene Einstellungen für Sicherheitsoptionen – Systemobjekte**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob für alle Subsysteme das Ignorieren der Groß-/Kleinschreibung erzwungen wird. Für das Microsoft Win32®-Subsystem wird die Groß-/Kleinschreibung ignoriert. Der Kernel unterstützt jedoch die Beachtung der Groß-/Kleinschreibung für andere Subsysteme, z. B. POSIX (Portable Operating System Interface für UNIX). Da unter Windows die Groß-/Kleinschreibung ignoriert wird (das POSIX-Subsystem jedoch die Beachtung der Groß-/Kleinschreibung unterstützt), kann ein Benutzer dieses Subsystems durch Mischen von Groß- und Kleinbuchstaben eine Datei mit einem bereits vorhandenen Namen erstellen, wenn diese Richtlinieneinstellung deaktiviert ist. In einer solchen Situation kann der Zugriff auf diese Dateien durch einen anderen Benutzer blockiert werden, der typische Win32-Tools verwendet, da nur eine der Dateien zur Verfügung steht.
  
Zum Gewährleisten der Konsistenz von Dateinamen ist die Einstellung **Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken**  
Durch diese Richtlinieneinstellung wird die Stärke der standardmäßigen freigegebenen Zugriffssteuerungsliste (DACL) für Objekte festgelegt. Diese Einstellung trägt zur Absicherung von Objekten bei, die zwischen Prozessen gesucht und freigegeben werden können. Die Standardkonfiguration der Einstellung stärkt die Sicherheit der DACL, da sie Benutzern ohne Administratorrechte das Lesen von freigegebenen Objekten ermöglicht, diese jedoch nur die von ihnen selbst erstellten Objekte ändern können.
  
Daher ist die Einstellung **Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken** (z. B. symbolische Verknüpfungen) für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
###### Benutzerkontensteuerung
  
Die Benutzerkontensteuerung (UAC) verringert die Gefährdung und die Angriffsfläche des Betriebssystems, indem sie verlangt, dass alle Benutzer im Standardbenutzermodus ausgeführt werden, auch wenn sie sich mit administrativen Anmeldeinformationen angemeldet haben. Diese Einschränkung hilft zu verhindern, dass Benutzer Änderungen vornehmen, die ihren Computer destabilisieren oder das Netzwerk versehentlich durch Viren gefährden, die den Computer über unerkannte Malware befallen könnten.
  
Wenn ein Benutzer versucht, eine Verwaltungsaufgabe auszuführen, muss das Betriebssystem die Sicherheitsstufe dieses Benutzers erhöhen, damit die Aufgabe ausgeführt werden kann. Die Einstellungen für die Benutzerkontensteuerung in Gruppenrichtlinienobjekten bestimmen, wie das Betriebssystem auf eine Anfrage bezüglich einer Erhöhung der Sicherheitsrechte reagiert.
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen der Sicherheitsoptionen für die Benutzerkontensteuerung. Weitere Informationen finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A30: Empfohlene Einstellungen für Sicherheitsoptionen – Benutzerkontensteuerung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Administratorbestätigungsmodus für das integrierte Administratorkonto</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Verhalten der Benutzeraufforderung mit erhöhten Rechten für Administratoren im Administratorbestätigungsmodus</td>
<td style="border:1px solid black;">Aufforderung zur Eingabe der Zustimmung</td>
<td style="border:1px solid black;">Aufforderung zur Eingabe der Anmeldeinformationen</td>
<td style="border:1px solid black;">Aufforderung zur Eingabe der Anmeldeinformationen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Verhalten der Anhebungsaufforderung für Standardbenutzer</td>
<td style="border:1px solid black;">Aufforderung zur Eingabe der Anmeldeinformationen</td>
<td style="border:1px solid black;">Anforderungen für erhöhte Rechte automatisch ablehnen</td>
<td style="border:1px solid black;">Anforderungen für erhöhte Rechte automatisch ablehnen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Anwendungsinstallationen erkennen und erhöhte Rechte anfordern</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Nur ausführbare Dateien heraufstufen, die signiert und validiert sind</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Nur erhöhte Rechte für UIAccess-Anwendungen, die an sicheren Orten installiert sind</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Alle Administratoren im Administratorbestätigungsmodus ausführen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Bei Benutzeraufforderung nach erhöhten Rechten zum sicheren Desktop wechseln</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benutzerkontensteuerung: Datei- und Registrierungsschreibfehler an Einzelbenutzerstandorte virtualisieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Benutzerkontensteuerung: Administratorbestätigungsmodus für das integrierte Administratorkonto**  
Diese Richtlinieneinstellung bestimmt, ob das integrierte Administratorkonto im Administratorbestätigungsmodus ausgeführt wird. Für diese Einstellung können verschiedene Standardverhalten vorhanden sein, da Windows Vista das integrierte Administratorkonto nach spezifischen Installationskriterien konfiguriert.
  
Bei Neuinstallationen und Aktualisierungen setzt Windows Vista die Einstellung standardmäßig auf **Deaktiviert**, wenn der vordefinierte Administrator *nicht* der einzige aktive lokale Administrator für den Computer ist. Bei Installationen und Aktualisierungen auf Computern, die einer Domäne angehören, deaktiviert Windows Vista standardmäßig das vordefinierte Administratorkonto.
  
Bei Aktualisierungen setzt Windows Vista die Einstellung standardmäßig auf **Aktiviert**, wenn es feststellt, dass es sich bei dem vordefinierten Administratorkonto um den einzigen aktiven lokalen Administrator auf dem Computer handelt. Ist dies der Fall, aktiviert Windows Vista das vordefinierte Administratorkonto im Anschluss an die Aktualisierung.
  
Die Einstellung **Benutzerkontensteuerung: Administratorbestätigungsmodus für das integrierte Administratorkonto** ist für in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Benutzerkontensteuerung: Verhalten der Benutzeraufforderung mit erhöhten Rechten für Administratoren im Administratorbestätigungsmodus**  
Diese Einstellung bestimmt das Verhalten von Windows Vista, wenn ein angemeldeter Administrator eine Aufgabe auszuführen versucht, für die erhöhte Rechte erforderlich sind. Diese Einstellung kann drei verschiedene Werte annehmen:
  
-   **Keine Aufforderung**. Mit diesem Wert werden die Rechte automatisch im Hintergrund erhöht.
  
-   **Aufforderung zur Eingabe der Zustimmung**. Dieser Wert bewirkt, dass die Benutzerkontensteuerung zur Zustimmung auffordert, bevor sie die Rechte erhöht, ohne jedoch Anmeldeinformationen zu verlangen.
  
-   **Aufforderung zur Eingabe der Anmeldeinformationen**. Dieser Wert bewirkt, dass die Benutzerkontensteuerung einen Administrator dazu auffordert, gültige Administrator-Anmeldeinformationen einzugeben, bevor sie die Rechte erhöht.
  
Die Einstellung **Benutzerkontensteuerung: Verhalten der Benutzeraufforderung mit erhöhten Rechten für Administratoren im Administratorbestätigungsmodus** ist für in diesem Handbuch behandelten Umgebungen auf **Aufforderung zur Eingabe der Anmeldeinformationen** gesetzt.
  
**Benutzerkontensteuerung: Verhalten der Anhebungsaufforderung für Standardbenutzer**  
Diese Einstellung bestimmt das Verhalten von Windows Vista, wenn ein angemeldeter Benutzer eine Aufgabe auszuführen versucht, für die erhöhte Rechte erforderlich sind. Diese Einstellung kann zwei verschiedene Werte annehmen:
  
-   **Anforderungen für erhöhte Rechte automatisch ablehnen**. Mit diesem Wert wird verhindert, dass eine Rechteanhebungsaufforderung angezeigt wird. Der Benutzer kann keine Verwaltungsaufgaben ausführen, ohne als Administrator den Befehl **Ausführen** zu verwenden oder sich mit einem Administratorkonto anzumelden.
  
-   **Aufforderung zur Eingabe der Anmeldeinformationen**. Dieser Wert bewirkt, dass die Benutzerkontensteuerung einen Administrator dazu auffordert, gültige Administrator-Anmeldeinformationen einzugeben, bevor die Einstellung erhöht werden kann.
  
Die Einstellung **Benutzerkontensteuerung: Verhalten der Anhebungsaufforderung für Standardbenutzer** ist für beide in diesem Handbuch behandelten Umgebungen auf **Anforderungen für erhöhte Rechte automatisch ablehnen** gesetzt.
  
Diese Einstellung verhindert, dass Standardbenutzer ihre Rechte erhöhen. Ein Standardbenutzer kann also keine Administratorkonto-Anmeldeinformationen eingeben, um eine Verwaltungsaufgabe auszuführen. Standardbenutzer haben nicht die Möglichkeit, mit der rechten Maustaste auf eine Programmdatei zu klicken und **Als Administrator ausführen** zu wählen. Standardbenutzer, die Verwaltungsaufgaben ausführen möchten, müssen sich hierfür erst abmelden und mit ihrem Administratorkonto wieder anmelden. Wenngleich diese Vorgehensweise etwas unbequem ist, sorgt sie für mehr Sicherheit in Ihrer Umgebung.
  
**Benutzerkontensteuerung: Anwendungsinstallationen erkennen und erhöhte Rechte anfordern**  
Diese Einstellung bestimmt, wie Windows Vista auf Anforderungen bezüglich Anwendungsinstallationen reagiert. Für eine Anwendungsinstallation ist eine Erhöhung der Rechte erforderlich. Diese Einstellung kann zwei verschiedene Werte annehmen:
  
-   **Aktiviert**. Mit diesem Wert fordert Windows Vista bei Erkennung eines Installationsprogramms den Benutzer auf, seine Zustimmung zu erklären oder seine Anmeldeinformationen einzugeben, je nachdem, welche Konfiguration für das Verhalten der Rechteanhebungsaufforderung gewählt wurde.
  
-   **Deaktiviert**. Dieser Wert bewirkt, dass Anwendungsinstallationen automatisch oder auf nicht deterministische Weise unterbunden werden.
  
Die Einstellung **Benutzerkontensteuerung: Anwendungsinstallationen erkennen und erhöhte Rechte anfordern** ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Benutzerkontensteuerung: Nur ausführbare Dateien heraufstufen, die signiert und validiert sind**  
Mit dieser Einstellung wird der Schutz vor unsignierten oder ungültigen Anwendungen aktiviert. Vor einer Aktivierung dieser Einstellung müssen sich Administratoren vergewissern, dass alle erforderlichen Anwendungen signiert und gültig sind. Diese Einstellung kann zwei verschiedene Werte annehmen:
  
-   **Aktiviert**. Dieser Wert bewirkt, dass nur signierte ausführbare Dateien gestartet werden dürfen. Damit wird verhindert, dass unsignierte Anwendungen ausgeführt werden.
  
-   **Deaktiviert**. Dieser Wert bewirkt, dass signierte und unsignierte ausführbare Dateien gestartet werden dürfen.
  
Die Einstellung **Benutzerkontensteuerung: Nur ausführbare Dateien heraufstufen, die signiert und validiert sind** ist für beide in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Benutzerkontensteuerung: Nur erhöhte Rechte für UIAccess-Anwendungen, die an sicheren Orten installiert sind**  
Diese Einstellung trägt zum Schutz eines Windows Vista-basierten Computers bei, indem sie das Ausführen mit erhöhten Rechten nur bei Anwendungen zulässt, die an einem sicheren Speicherort im Dateisystem installiert sind, beispielsweise im Ordner „Programme“ oder „Windows\\System32“.
  
Die Einstellung **Benutzerkontensteuerung: Nur erhöhte Rechte für UIAccess-Anwendungen, die an sicheren Orten installiert sind** ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Benutzerkontensteuerung: Alle Administratoren im Administratorbestätigungsmodus ausführen**  
Durch diese Einstellung wird die Benutzerkontensteuerung praktisch deaktiviert. Diese Einstellung kann zwei verschiedene Werte annehmen:
  
-   **Aktiviert**. Mit diesem Wert werden sowohl Administratoren als auch Standardbenutzer zu einer Bestätigung aufgefordert, wenn sie versuchen, Verwaltungsaufgaben auszuführen. Die Art der Eingabeaufforderung hängt von der jeweiligen Richtlinie ab.
  
-   **Deaktiviert**. Mit diesem Wert werden der Benutzertyp „Administratorbestätigungsmodus“ und alle zugehörigen Richtlinien für die Benutzerkontensteuerung deaktiviert. Bei dieser Einstellung zeigt das Sicherheitscenter an, dass die Gesamtsicherheit des Betriebssystems verringert wurde.
  
Die Einstellung **Benutzerkontensteuerung: Alle Administratoren im Administratorbestätigungsmodus ausführen** ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Benutzerkontensteuerung: Bei Benutzeraufforderung nach erhöhten Rechten zum sicheren Desktop wechseln**  
Diese Einstellung hilft zu vermeiden, dass die Rechteanhebungsaufforderung zu bösartigen Zwecken missbraucht wird. Der Windows Vista-Sicherheitsdesktop kann nur SYSTEM-Prozesse ausführen, wodurch Nachrichten aus bösartiger Software im Allgemeinen unterbunden werden. Somit können keine manipulierten Zustimmungen und Anmeldeinformationen in die Eingabeaufforderungen auf dem sicheren Desktop eingegeben werden. Darüber hinaus ist die Zustimmungseingabeaufforderung vor Manipulationen der Ausgabe geschützt. Bei der Verwendung der Eingabeaufforderung für die Anmeldeinformationen besteht jedoch immer noch ein Risiko, da sie durch Malware gefälscht werden könnte. Für diese Einstellung stehen zwei Werte zur Auswahl:
  
-   **Aktiviert**. Mit diesem Wert wird die Rechteanhebungsaufforderung der Benutzerkontensteuerung auf dem sicheren Desktop angezeigt.
  
-   **Deaktiviert**. Dieser Wert bewirkt, dass die Rechteanhebungsaufforderung der Benutzerkontensteuerung auf dem Benutzerdesktop angezeigt wird.
  
Die Einstellung **Benutzerkontensteuerung: Bei Benutzeraufforderung nach erhöhten Rechten zum sicheren Desktop wechseln** ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Benutzerkontensteuerung: Datei- und Registrierungsschreibfehler an Einzelbenutzerstandorte virtualisieren**  
Anwendungen, die keinen Eintrag in der Kompatibilitätsdatenbank oder keine Kennzeichnung der angeforderten Ausführungsebene im Anwendungsmanifest aufweisen, sind mit der Benutzerkontensteuerung nicht kompatibel. Anwendungen, die nicht mit der Benutzerkontensteuerung kompatibel sind, versuchen Daten in geschützte Bereiche zu schreiben, darunter auch in „Programme“ und in „%*systemroot*%“. Das Ausführen solcher Anwendungen wird automatisch unterbunden, wenn der Schreibvorgang nicht durchgeführt werden kann. Wenn Sie diese Einstellung aktivieren, gestatten Sie Windows Vista das Virtualisieren von Datei- und Registrierungsschreibvorgängen an Benutzerspeicherorten, so dass die Anwendung ausgeführt werden kann.
  
Mit der Benutzerkontensteuerung kompatible Anwendungen sollten keine Schreibvorgänge in geschützten Bereichen durchführen und keine Schreibfehler verursachen. Deshalb sollte diese Einstellung in Umgebungen deaktiviert werden, in denen nur mit der Benutzerkontensteuerung kompatible Anwendungen genutzt werden.
  
Diese Einstellung kann zwei verschiedene Werte annehmen:
  
-   **Aktiviert**. Für Umgebungen, in denen auch Software genutzt wird, die nicht mit der Benutzerkontensteuerung kompatibel ist, sollte diese Einstellung auf **Aktiviert** gesetzt werden.
  
-   **Deaktiviert**. Für Umgebungen, in denen nur Software genutzt wird, die mit der Benutzerkontensteuerung kompatibel ist, sollte diese Einstellung auf **Deaktiviert** gesetzt werden.
  
Wenn Sie sich nicht sicher sind, ob alle in Ihrer Umgebung genutzten Anwendungen mit der Benutzerkontensteuerung kompatibel sind, sollten Sie die Einstellung auf **Aktiviert** setzen.
  
Aus diesem Grund ist die Einstellung **Benutzerkontensteuerung: Datei- und Registrierungsschreibfehler an Einzelbenutzerstandorte virtualisieren** für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Sicherheitseinstellungen für Ereignisprotokolle
  
Im Ereignisprotokoll werden Ereignisse im System erfasst, während im Sicherheitsprotokoll Überwachungsereignisse aufgezeichnet werden. Der Ereignisprotokoll-Container der Gruppenrichtlinie dient zum Definieren von Attributen für die Anwendungs-, Sicherheits- und Systemereignisprotokolle, z. B. maximale Protokollgröße, Zugriffsrechte für jedes Protokoll sowie Einstellungen für die Dauer und Methode der Aufbewahrung.
  
Die Ereignisprotokolleinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Ereignisprotokoll**
  
Dieser Abschnitt enthält Informationen zu den empfohlenen Einstellungen für die Umgebungen, die in diesem Handbuch behandelt werden. Eine Zusammenfassung der empfohlenen Einstellungen in diesem Abschnitt finden Sie in der Datei „Windows Vista Security Guide Settings.xls“. Informationen zu den Standardeinstellungen und eine detaillierte Erläuterung zu den Einstellungen in diesem Abschnitt finden Sie im Handbuch [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10)). Dieses Begleithandbuch enthält auch ausführliche Informationen zur Gefahr des Verlusts von Ereignisprotokolldaten, wenn die Protokollgrößen auf sehr große Werte gesetzt sind.
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Sicherheitseinstellungen für Ereignisprotokolle sowohl für Desktop- als auch für Laptopclients in den beiden Umgebungen, die in diesem Handbuch behandelt werden. In den folgenden Unterabschnitten finden Sie detailliertere Informationen zu den einzelnen Einstellungen.
  
**Tabelle A31: Empfohlene Einstellungen für Sicherheitsoptionen – Sicherheitseinstellungen für Ereignisprotokolle**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Maximale Größe des Anwendungsprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend<br />
(Standard = 20480)</td>
<td style="border:1px solid black;">32768 KB</td>
<td style="border:1px solid black;">32768 KB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Maximale Größe des Sicherheitsprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend<br />
(Standard = 20480)</td>
<td style="border:1px solid black;">81920 KB</td>
<td style="border:1px solid black;">81920 KB</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Maximale Größe des Systemprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend<br />
(Standard = 20480)</td>
<td style="border:1px solid black;">32768 KB</td>
<td style="border:1px solid black;">32768 KB</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aufbewahrungsmethode des Anwendungsprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend (Standard = Bei Bedarf überschreiben)</td>
<td style="border:1px solid black;">Bei Bedarf</td>
<td style="border:1px solid black;">Bei Bedarf</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Aufbewahrungsmethode des Sicherheitsprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend (Standard = Bei Bedarf überschreiben)</td>
<td style="border:1px solid black;">Bei Bedarf</td>
<td style="border:1px solid black;">Bei Bedarf</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Aufbewahrungsmethode des Systemprotokolls</td>
<td style="border:1px solid black;">Nicht zutreffend (Standard = Bei Bedarf überschreiben)</td>
<td style="border:1px solid black;">Bei Bedarf</td>
<td style="border:1px solid black;">Bei Bedarf</td>
</tr>
</tbody>
</table>
  
**Maximale Größe des Anwendungsprotokolls**  
Durch diese Richtlinieneinstellung wird die maximale Größe des Anwendungsereignisprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen an die Anwendungsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Anwendungsprotokolls** ist für alle Computer in den beiden in diesem Handbuch behandelten Umgebungen auf **32768** **KB** gesetzt.
  
**Maximale Größe des Sicherheitsprotokolls**  
Durch diese Richtlinieneinstellung wird die maximale Größe des Sicherheitsprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen an die Sicherheitsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Sicherheitsprotokolls** ist für alle Computer in den beiden in diesem Handbuch behandelten Umgebungen auf **81920 KB** gesetzt.
  
**Maximale Größe des Systemprotokolls**  
Durch diese Richtlinieneinstellung wird die maximale Größe des Systemprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen für die Anwendungsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Systemprotokolls** ist für alle Computer in den beiden in diesem Handbuch behandelten Umgebungen auf **32768 KB** gesetzt.
  
**Aufbewahrungsmethode des Anwendungsprotokolls**  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Anwendungsprotokoll festgelegt. Das Anwendungsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen gewährleistet, dass im Protokoll immer die aktuellsten Ereignisse gespeichert werden. Allerdings kann diese Konfiguration bewirken, dass ältere Daten verloren gehen.
  
Die **Aufbewahrungsmethode des Anwendungsprotokolls** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
**Aufbewahrungsmethode des Sicherheitsprotokolls**  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Sicherheitsprotokoll festgelegt. Das Sicherheitsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen gewährleistet, dass im Protokoll immer die aktuellsten Ereignisse gespeichert werden. Allerdings kann diese Konfiguration bewirken, dass ältere Daten verloren gehen.
  
Die **Aufbewahrungsmethode des Sicherheitsprotokolls** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
**Aufbewahrungsmethode des Systemprotokolls**  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Systemprotokoll festgelegt. Das Systemprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen gewährleistet, dass im Protokoll immer die aktuellsten Ereignisse gespeichert werden. Allerdings kann diese Konfiguration bewirken, dass ältere Daten verloren gehen.
  
Die **Aufbewahrungsmethode des Systemprotokolls** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
##### Einstellungen für Windows-Firewall mit erweiterter Sicherheit
  
Die in Windows Vista enthaltene Firewall lässt sich noch präziser konfigurieren.
  
Die Einstellungen für „Windows-Firewall mit erweiterter Sicherheit“ können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen**  
**\\Windows-Firewall mit erweiterter Sicherheit**
  
Zur Steuerung dieser Einstellungen klicken Sie im Abschnitt „Windows-Firewall mit erweiterter Sicherheit“ des Gruppenrichtlinienobjekt-Editors auf die Verknüpfung **Windows-Firewalleigenschaften**. Im Dialogfeld **Windows-Firewall mit erweiterter Sicherheit** können Sie Einstellungen für das Domänenprofil, das private Profil und das öffentliche Profil festlegen. Für jedes Profil können Sie allgemeine Einstellungen im Abschnitt **Status** festlegen und dann im Abschnitt **Einstellungen** auf die Schaltfläche **Anpassen** klicken, um benutzerdefinierte Einstellungen festzulegen. Dieser Abschnitt des Anhangs enthält Tabellen und Empfehlungen für die Profile, die Sie im Dialogfeld **Windows-Firewall mit erweiterter Sicherheit** konfigurieren können.
  
###### Domänenprofil
  
Dieses Profil kommt zur Anwendung, wenn ein Computer mit einem Netzwerk verbunden ist und sich bei einem Domänencontroller in der Domäne authentifiziert, der er angehört.
  
**Tabelle A32: Empfohlene Einstellungen für das Domänenprofil**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Firewallstatus</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Eingehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Ausgehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Benutzerdefinierte Einstellungen</strong></td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benachrichtigung anzeigen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Unicastantwort zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Lokale Firewallregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Lokale Verbindungssicherheitsregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
Die empfohlene Konfiguration der Windows-Firewall mit erweiterter Sicherheit umfasst für die Unternehmensclient-Umgebung Firewallregeln, die die Remotedesktop- und Remoteunterstützungskommunikation zulassen. Zudem können lokale Administratoren von Computern in der Unternehmensclient-Umgebung lokale Firewallregeln konfigurieren, die zusätzliche Kommunikation mit einem Computer zulassen.
  
In der Hochsicherheitsumgebung wird sämtliche eingehende Kommunikation standardmäßig geblockt, und lokale Firewallregeln werden von Computern ignoriert. Hinzufügungen oder Änderungen an den Firewallregeln müssen über den Gruppenrichtlinienobjekt-Editor vorgenommen werden.
  
**Wichtig:**   Die empfohlenen Firewalleinstellungen für die Hochsicherheitsumgebung schränken eingehenden Verbindungen zu Ihren Computern in hohem Maße ein. Sie sollten diese Firewallkonfiguration in Ihrer Umgebung umfassend testen, um sicherzustellen, dass alle Anwendungen wie gewünscht funktionieren.
  
Wenn Sie sehen möchten, welche Regeln für das Domänenprofil definiert sind, klicken Sie innerhalb des Abschnitts „Windows-Firewall mit erweiterter Sicherheit“ des Gruppenrichtlinienobjekt-Editors auf die Verknüpfung **Eingehende Regeln**.
  
###### Privates Profil
  
Dieses Profil gilt nur, wenn es von einem Benutzer mit lokalen Administratorrechten einem Netzwerk zugewiesen wird, für das zuvor das öffentliche Profil festgelegt war. Microsoft empfiehlt, eine Profiländerung auf das private Profil nur bei vertrauenswürdigen Netzwerken vorzunehmen.
  
**Tabelle A33: Empfohlene Einstellungen für das private Profil**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Firewallstatus</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Eingehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Ausgehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Benutzerdefinierte Einstellungen</strong></td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benachrichtigung anzeigen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Unicastantwort zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Lokale Firewallregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Lokale Verbindungssicherheitsregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Ja (Standard)</td>
<td style="border:1px solid black;">Nein</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
Die empfohlene Konfiguration der Windows-Firewall mit erweiterter Sicherheit umfasst für die Unternehmensclient-Umgebung Firewallregeln, die die Remotedesktopkommunikation zulassen. Zudem können lokale Administratoren von Computern in der Unternehmensclient-Umgebung lokale Firewallregeln konfigurieren, die zusätzliche Kommunikation mit einem Computer zulassen.
  
In der Hochsicherheitsumgebung wird sämtliche eingehende Kommunikation standardmäßig geblockt, und lokale Firewallregeln werden von Computern ignoriert. Hinzufügungen oder Änderungen an den Firewallregeln müssen über den Gruppenrichtlinienobjekt-Editor vorgenommen werden.
  
Wenn Sie sehen möchten, welche Regeln für das private Profil definiert sind, klicken Sie innerhalb des Abschnitts „Windows-Firewall mit erweiterter Sicherheit“ des Gruppenrichtlinienobjekt-Editors auf die Verknüpfung **Eingehende Regeln**.
  
###### Öffentliches Profil
  
Dieses Profil ist der standardmäßige Netzwerkstandorttyp, wenn der Computer keiner Domäne angehört. Einstellungen für das öffentliche Profil sollten am stärksten einschränkend sein, da der Computer mit einem öffentlichen Netzwerk verbunden ist, in dem die Sicherheit nicht so nahtlos kontrolliert werden kann wie innerhalb einer IT-Umgebung.
  
**Tabelle A34: Empfohlene Einstellungen für das öffentliche Profil**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>Windows Vista-Standardeinstellung</th>
<th>EC-Computer-GPOs des Handbuchs</th>
<th>SSLF-Computer-GPOs des Handbuchs</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Firewallstatus</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
<td style="border:1px solid black;">Aktiv (empfohlen)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Eingehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
<td style="border:1px solid black;">Blocken (Standard)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Ausgehende Verbindungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
<td style="border:1px solid black;">Zulassen (Standard)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Benutzerdefinierte Einstellungen</strong></td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"> </td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Benachrichtigung anzeigen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Unicastantwort zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Lokale Firewallregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Lokale Verbindungssicherheitsregeln anwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nein</td>
<td style="border:1px solid black;">Nein</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
Sowohl in der Unternehmensclient- als auch in der Hochsicherheitsumgebung wird sämtliche eingehende Kommunikation standardmäßig geblockt, und es sind keine Firewallregeln vorhanden, die eine weitere Kommunikation mit einem Computer zulassen würden. Zudem werden lokale Firewallregeln von Computern in beiden in diesem Handbuch beschriebenen Umgebungen ignoriert. Hinzufügungen oder Änderungen an Firewallregeln, die für das öffentliche Profil gelten, müssen über den Gruppenrichtlinienobjekt-Editor vorgenommen werden.
  
In den folgenden Abschnitten werden in Kurzform die Einstellungen beschrieben, die Sie für die einzelnen Firewallprofile konfigurieren können.
  
**Firewallstatus**  
Wählen Sie **Ein (empfohlen)**, damit die Windows-Firewall mit erweiterter Sicherheit mit den Einstellungen dieses Profils den Netzwerkdatenverkehr filtert. Wenn Sie **Aus** wählen, verwendet die Windows-Firewall mit erweiterter Sicherheit keine der Firewall- oder Verbindungssicherheitsregeln dieses Profils.
  
**Eingehende Verbindungen**  
Diese Einstellung bestimmt das Verhalten für eingehende Verbindungen, die keiner eingehenden Firewallregel entsprechen. Standardmäßig werden Verbindungen geblockt, sofern keine Firewallregeln vorliegen, die diese Verbindungen explizit zulassen.
  
**Ausgehende Verbindungen**  
Diese Einstellung bestimmt das Verhalten für ausgehende Verbindungen, die keiner ausgehenden Firewallregel entsprechen. Standardmäßig werden Verbindungen zugelassen, sofern keine Firewallregeln vorliegen, die diese Verbindungen explizit blocken.
  
**Wichtig:   **Wenn Sie für **Ausgehende Verbindungen** die Einstellung **Blocken** festlegen und dann die Firewallrichtlinie mithilfe eines Gruppenrichtlinienobjekts bereitstellen, können Computer, die die Gruppenrichtlinienobjekt-Einstellungen erhalten, nachfolgend keine Gruppenrichtlinienupdates erhalten, es sei denn, Sie stellen eine ausgehende Regel bereit, die die Gruppenrichtlinie in Kraft setzt. Vordefinierte Kernnetzwerkregeln enthalten auch ausgehende Regeln, die die Gruppenrichtlinie in Kraft setzen. Vergewissern Sie sich, dass diese ausgehenden Regeln aktiv sind, und testen Sie alle Firewallprofile gründlich, bevor Sie sie bereitstellen.
  
**Benachrichtigung anzeigen**  
Wählen Sie diese Option, wenn die Windows-Firewall mit erweiterter Sicherheit den Benutzer benachrichtigen soll, wenn bei einem Programm das Empfangen von eingehenden Verbindungen geblockt ist.
  
**Hinweis:**   Wenn die Einstellung **Lokale Firewallregeln anwenden** auf **Nein** gesetzt ist, empfiehlt es sich, auch die Einstellung **Benachrichtigung anzeigen** auf **Nein** zu setzen. Andernfalls erhalten die Benutzer weiterhin Meldungen mit der Frage, ob die Blockierung einer eingehenden Verbindung aufgehoben werden soll, wobei jedoch die Antwort der Benutzer ignoriert wird.
  
**Unicastantwort zulassen**  
Diese Option ist hilfreich, wenn Sie bestimmen möchten, ob der jeweilige Computer Unicastantworten an seine ausgehenden Multicast- oder Broadcastnachrichten erhalten soll. Wenn Sie diese Einstellung aktivieren und dieser Computer Multicast- oder Broadcastmeldungen an andere Computer sendet, wartet die Windows-Firewall mit erweiterter Sicherheit bis zu drei Sekunden auf Unicast-Antworten von den anderen Computern und blockiert alle späteren Antworten. Wenn Sie diese Einstellung deaktivieren und der Computer eine Multicast- oder Broadcastnachricht an andere Computer sendet, blockiert die Windows-Firewall mit erweiterter Sicherheit die Unicastantworten, die von den anderen Computern gesendet wurden.
  
**Lokale Firewallregeln anwenden**  
Diese Einstellung bestimmt, ob lokale Administratoren berechtigt sind, lokale Firewallregeln zu erstellen, die zusammen mit Firewallregeln gelten, die durch die Gruppenrichtlinie erstellt werden. Wenn Sie diese Einstellung auf **Nein** setzen, können Administratoren zwar weiterhin solche Regeln erstellen, doch diese Regeln werden nicht angewendet. Diese Einstellung ist nur verfügbar, wenn die Regel über die Gruppenrichtline konfiguriert wird.
  
**Lokale Verbindungssicherheitsregeln anwenden**  
Diese Einstellung bestimmt, ob lokale Administratoren berechtigt sind, Verbindungssicherheitsregeln zu erstellen, die zusammen mit Verbindungssicherheitsregeln gelten, die über Gruppenrichtlinien konfiguriert werden. Wenn Sie diese Einstellung auf **Nein** setzen, können Administratoren zwar weiterhin solche Regeln erstellen, doch diese Regeln werden nicht angewendet. Diese Einstellung ist nur verfügbar, wenn die Regel über die Gruppenrichtline konfiguriert wird.
  
#### Computerkonfiguration\\Administrative Vorlagen
  
Die folgenden Einstellungsgruppen für die Computerrichtlinie enthalten Einstellungen, die in diesem Handbuch empfohlen werden. Die Einstellungen werden im Subknoten **Computerkonfiguration\\Administrative Vorlagen** des Gruppenrichtlinienobjekt-Editors angezeigt.
  
-   [Netzwerkverbindungen](#_network_connections)
  
-   [System](#_system)
  
    -   [Anmeldung](#_logon)
  
    -   [Gruppenrichtlinie](#_group_policy)
  
    -   [Remoteunterstützung](#_remote_assistance)
  
    -   [Remoteprozeduraufruf](#_remote_procedure_call)
  
    -   [Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen](#_internet_communication_management--)
  
-   [Windows-Komponenten](#_windows_components_2)
  
    -   [Richtlinien für automatische Wiedergabe](#_autoplay_policies)
  
    -   [Benutzeroberfläche für Anmeldeinformationen](#_credential_user_interface)
  
    -   [Internet Explorer](#_internet_explorer_2)
  
    -   [NetMeeting](#_netmeeting)
  
    -   [Terminaldienste](#_terminal_services)
  
    -   [Windows Messenger](#_windows_messenger)
  
    -   [Windows Update](#_windows_update)
  
##### Netzwerkverbindungen
  
Es gibt keine bestimmten sicherheitsrelevanten Konfigurationen im Netzwerkcontainer der Gruppenrichtlinie. Es gibt jedoch eine Reihe sehr wichtiger Einstellungen im Container **Netzwerkverbindungen\\Windows Firewall**.
  
Es empfiehlt sich, die Windows-Firewall über die Einstellungen für „Windows-Firewall mit erweiterter Sicherheit“ im Gruppenrichtlinienobjekt-Editor zu konfigurieren. Die empfohlenen Einstellungen für die Windows-Firewall mit erweiterter Sicherheit ändern jedoch den Status einiger Einstellungen in diesem Gruppenrichtlinienbereich. Außerdem tragen einige der empfohlenen Einstellungen zur Wahrung der Kompatibilität mit Windows XP-basierten Computern in der in diesem Handbuch beschriebenen Unternehmensclient-Umgebung bei.
  
In Windows XP werden Windows-Firewall-Einstellungen in zwei Profilen konfiguriert: im Domänenprofil und im Standardprofil. Immer wenn eine Domänenumgebung erkannt wird, wird das Domänenprofil verwendet. Wenn keine Domänenumgebung verfügbar ist, wird das Standardprofil genutzt.
  
Wenn eine Einstellung der Windows-Firewall in einer der beiden folgenden Tabellen **Empfohlen** lautet, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Da jede Organisation ihre eigene Liste mit Anwendungen hat, für die bei der Windows-Firewall entsprechende Ausnahmen definiert werden müssen, kann in diesem Handbuch keine allgemeingültige Liste bereitgestellt werden.
  
Wenn Sie ermitteln müssen, welche Anwendungen oder Ports möglicherweise Ausnahmen benötigen, kann es nützlich sein, Windows-Firewall-Protokollierung, Windows Firewall-Überwachung und Ablaufverfolgung für das Netzwerk zu aktivieren. Weitere Informationen hierzu finden Sie im Artikel zum Thema [Configuring a Computer for Windows Firewall Troubleshooting](http://technet2.microsoft.com/windowsserver/en/library/bfdeda55-46fc-4b53-b4cd-c71838ef4b411033.mspx?mfr=true) (engl.).
  
In der Regel wird das Domänenprofil mit weniger Einschränkungen konfiguriert als das Standardprofil, denn eine Domänenumgebung bietet häufig zusätzliche Schutzebenen. Die Namen der Richtlinieneinstellungen sind in beiden Profilen identisch. Die beiden folgenden Tabellen bieten einen Überblick über die Richtlinieneinstellungen für die verschiedenen Profile. In den Unterabschnitten im Anschluss an die Tabellen werden ausführlichere Erklärungen geboten.
  
###### Netzwerkverbindungen\\Windows Firewall\\Domänenprofil
  
Mit den Einstellungen in diesem Abschnitt wird das Domänenprofil der Windows-Firewall konfiguriert. Diese Einstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen**  
**\\Windows Firewall\\Domänenprofil**
  
**Tabelle A35: Empfohlene Windows-Firewall-Einstellungen für das Domänenprofil**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: ICMP-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Remotedesktopausnahmen zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende UPnP-Framework-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Lokale Portausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Lokale Programmausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Portausnahmen definieren</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Programmausnahmen definieren</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Keine Ausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Benachrichtigungen verbieten</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Alle Netzwerkverbindungen schützen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Hinweis:**   Wenn in dieser Tabelle eine Einstellung der Windows-Firewall **Empfohlen** ist, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Beispielsweise verfügt jede Organisation über eine eigene Liste von Anwendungen, die definierte Ausnahmen für die Windows-Firewall erfordern. Deshalb ist es nicht möglich, in diesem Handbuch eine Liste zu definieren, die generell verwendet werden kann.
  
###### Netzwerkverbindungen\\Windows Firewall\\Standardprofil
  
Mit den Einstellungen in diesem Abschnitt wird das Standardprofil der Windows-Firewall konfiguriert. Dieses Profil ist oftmals stärker einschränkend als das Domänenprofil, bei dem davon ausgegangen wird, das die Domänenumgebung bereits für ein gewisses Maß an Sicherheit sorgt. Das Standardprofil ist für Fälle gedacht, in denen sich ein Computer in einem nicht vertrauenswürdigen Netzwerk befindet, etwa in einem Hotelnetzwerk oder an einem öffentlichen Drahtloszugriffspunkt. Solche Umgebungen bergen unvorhersehbare Gefahren und erfordern deshalb zusätzliche Sicherheitsvorkehrungen.
  
**Hinweis:**   Das Standardprofil gilt nur für Computer mit Windows XP. Die folgenden Empfehlungen gelten nur in der diesem Handbuch beschriebenen Unternehmensclient-Umgebung zur Wahrung der Kompatibilität mit Windows XP.
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen**  
**\\Windows Firewall\\Standardprofil**
  
**Tabelle A36: Empfohlene Windows-Firewall-Einstellungen für das Standardprofil**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: ICMP-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Remotedesktopausnahmen zulassen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende UPnP-Framework-Ausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Lokale Portausnahmen zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Lokale Programmausnahmen zulassen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Portausnahmen definieren</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Eingehende Programmausnahmen definieren</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Keine Ausnahmen zulassen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Empfohlen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Benachrichtigungen verbieten</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows-Firewall: Unicast-Antwort auf Multicast- oder Broadcastanfragen verbieten</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows-Firewall: Alle Netzwerkverbindungen schützen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
</tbody>
</table>
  
**Hinweis:**   Wenn in dieser Tabelle eine Einstellung der Windows-Firewall **Empfohlen** ist, ist der zu verwendende Wert von Organisation zu Organisation verschieden. Beispielsweise verfügt jede Organisation über eine eigene Liste von Anwendungen, die definierte Ausnahmen für die Windows-Firewall erfordern. Deshalb ist es nicht möglich, in diesem Handbuch eine Liste zu definieren, die generell verwendet werden kann.
  
**Windows-Firewall: ICMP-Ausnahmen zulassen**  
Durch dieser Richtlinieneinstellung wird der Satz von ICMP-Meldungstypen (Internet Control Message Protocol) definiert, den die Windows-Firewall zulässt. Mithilfe von ICMP-Meldungen können Dienstprogramme den Status anderer Computer bestimmen. Ping verwendet z. B. die Echoanforderungsmeldung.
  
Wenn Sie die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** auf **Aktiviert** setzen, müssen Sie angeben, welchen ICMP-Meldungstyp der Computer durch die Windows-Firewall senden bzw. empfangen kann. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, blockiert die Windows-Firewall alle nicht angeforderten eingehenden ICMP-Meldungstypen sowie die aufgeführten ausgehenden ICMP-Meldungstypen. Demzufolge können Dienstprogramme fehlschlagen, die ICMP verwenden.
  
Viele Angriffstools nutzen Computer aus, die ICMP-Meldungstypen akzeptieren. Diese Meldungen werden für verschiedenartige Angriffe verwendet. Einige Anwendungen erfordern jedoch bestimmte ICMP-Meldungen, um richtig zu funktionieren. Mithilfe von ICMP-Meldungen wird außerdem die Netzwerkleistung eingeschätzt, wenn Gruppenrichtlinien heruntergeladen und verarbeitet werden. Wenn ICMP-Meldungen blockiert werden, kann die Gruppenrichtlinie nicht auf betroffene Systeme angewendet werden. Aus diesem Grund empfiehlt Microsoft, die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** nach Möglichkeit auf **Deaktiviert** zu setzen. Wenn es in Ihrer Umgebung erforderlich ist, dass einige ICMP-Meldungen durch die Windows-Firewall gelangen, legen Sie für die Einstellung die entsprechenden Meldungstypen fest.
  
Wann immer der Computer sich in einem nicht vertrauenswürdigen Netzwerk befindet, sollte die Einstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** auf **Deaktiviert** gesetzt werden.
  
**Hinweis:**   Wenn eine Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows-Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Zu Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, gehören **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** und **Windows-Firewall: Eingehende Portausnahmen definieren**.
  
**Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen**  
Durch diese Richtlinieneinstellung wird eine Ausnahme geschaffen, die die Datei- und Druckerfreigabe zulässt. Dadurch wird die Windows-Firewall so konfiguriert, dass die UDP-Ports 137 und 138 sowie die TCP-Ports 139 und 445 geöffnet werden. Wenn Sie diese Richtlinieneinstellung aktivieren, öffnet die Windows-Firewall diese Ports, damit der Computer Druckaufträge und Anforderungen für den Zugriff auf freigegebene Dateien empfangen kann. Sie müssen die IP-Adressen oder Subnetze angeben, von denen diese Meldungen zulässig sind.
  
Wenn Sie die Einstellung **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen** deaktivieren, blockiert die Windows-Firewall diese Ports und hindert den Computer an der Freigabe von Dateien und Druckern.
  
Die Computer in Ihrer Umgebung, auf denen Windows Vista ausgeführt wird, geben Dateien und Drucker normalerweise nicht frei. Aus diesem Grund empfiehlt Microsoft, die **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen** auf **Deaktiviert** zu setzen.
  
**Hinweis:**   Wenn eine Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows-Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Zu Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, gehören **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** und **Windows-Firewall: Eingehende Portausnahmen definieren**.
  
**Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen**  
Viele Organisationen nutzen im Alltag die Vorteile der Remoteverwaltung von Computern. Bei einigen Angriffsmethoden wurden jedoch die Ports ausgenutzt, die normalerweise von Remoteverwaltungsprogrammen verwendet werden. Die Windows-Firewall kann zum Blockieren dieser Ports beitragen.
  
Um Flexibilität für die Remoteverwaltung bereitzustellen, steht die Einstellung **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** zur Verfügung. Wenn diese Richtlinieneinstellung aktiviert ist, kann der Computer die nicht angeforderte eingehenden Nachrichten, die mit der Remoteverwaltung einhergehen, über die TCP-Ports 135 und 445 empfangen. Außerdem erlaubt diese Richtlinieneinstellung den Dateien SVCHOST.EXE und LSASS.EXE, unerwünscht eingehende Nachrichten zu empfangen. Gehostete Dienste können zusätzlich dynamisch zugewiesene Ports öffnen, in der Regel im Bereich von 1024 bis 1034. Möglich ist jedoch der Bereich zwischen 1024 und 65535. Wenn Sie diese Richtlinieneinstellung aktivieren, müssen Sie die IP-Adressen oder die Subnetze angeben, von denen diese Nachrichten eingehen dürfen.
  
Wenn Sie die Einstellung **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** auf **Deaktiviert** setzen, macht die Windows-Firewall keine der beschriebenen Ausnahmen. Diese Richtlinieneinstellung auf **Deaktiviert** zu setzen, kann Auswirkungen haben, die für viele Organisationen nicht akzeptabel sind, da viele Remoteverwaltungstools und Programme, die nach Sicherheitsanfälligkeiten suchen, fehlschlagen werden. Deshalb empfiehlt Microsoft, dass diese Richtlinieneinstellung nur in Organisationen aktiviert wird, die extrem strenger Sichermaßnahmen bedürfen.
  
Für das Domänenprofil empfiehlt Microsoft, die Einstellung **Windows Firewall: Eingehende Remoteverwaltungsausnahme zulassen** für Computer in der Unternehmensclient-Umgebung nur im Bedarfsfall auf **Aktiviert** zu setzen. Wenn Sie diese Einstellung aktivieren, sollten Computer in Ihrer Umgebung von möglichst wenigen Computern Anforderungen zur Remoteverwaltung annehmen. Um den von der Windows-Firewall gebotenen Schutz zu maximieren, sollten Sie nur die IP-Adressen und Subnetze der Computer angeben, die für die Remoteverwaltung verwendet werden.
  
Microsoft empfiehlt, die Einstellung **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** für alle Computer im Standardprofil auf **Deaktiviert** zu setzen, um bekannte Angriffsmethoden zu vermeiden, die insbesondere die TCP-Ports 135 und 445 ausnutzen.
  
**Hinweis**:   Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows-Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Zu Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, gehören **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** und **Windows Firewall: Eingehende Portausnahmen definieren**.
  
**Windows-Firewall: Eingehende Remotedesktopausnahmen zulassen**  
Viele Organisationen verwenden Remotedesktopverbindungen bei ihren normalen Problembehandlungsverfahren oder -vorgängen. Bei einigen Angriffsmethoden wurden jedoch die Ports ausgenutzt, die normalerweise von Remotedesktop verwendet werden.
  
Um Flexibilität für die Remoteverwaltung bereitzustellen, steht die Einstellung **Windows-Firewall: Eingehende Remoteverwaltungsausnahmen zulassen**zur Verfügung. Wenn Sie diese Richtlinieneinstellung aktivieren, öffnet die Windows-Firewall den TCP-Port 3389 für eingehende Verbindungen. Sie müssen außerdem die IP-Adressen oder Subnetze angeben, von denen diese Meldungen eingehen dürfen.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, blockiert die Windows-Firewall diesen Port und hindert den Computer daran, Anforderungen vom Remotedesktop zu empfangen. Wenn ein Administrator diesen Port einer Liste mit lokalen Portausnahmen hinzufügt, um ihn damit zu öffnen, hält die Windows-Firewall diesen Port geschlossen.
  
Um die erweiterten Verwaltungsmöglichkeiten beizubehalten, die von Remotedesktop bereitgestellt werden, sollten Sie diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Aktiviert** setzen. Sie müssen die IP-Adressen und Subnetze der Computer angeben, die für die Remoteverwaltung verwendet werden. Computer in Ihrer Umgebung sollten Remotedesktopanforderungen von so wenigen Computern wie möglich annehmen.
  
**Windows-Firewall: Eingehende UPnP-Framework-Ausnahmen zulassen**  
Diese Richtlinieneinstellung ermöglicht es einem Computer, nicht angeforderte Plug & Play-Meldungen zu empfangen, die von Netzwerkgeräten gesendet werden, wie z. B. von Routern mit integrierten Firewalls. Um diese Meldungen zu empfangen, öffnet die Windows-Firewall den TCP-Port 2869 und den UDP-Port 1900.
  
Wenn Sie die Einstellung **Windows-Firewall: Eingehende UPnP-Framework-Ausnahmen zulassen** aktivieren, öffnet die Windows-Firewall diese Ports, damit der Computer Plug & Play-Meldungen empfangen kann. Sie müssen die IP-Adressen oder Subnetze angeben, von denen diese Meldungen eingehen dürfen. Wenn Sie diese Richtlinieneinstellung deaktivieren, blockiert die Windows-Firewall diese Ports und hindert den Computer am Empfang von Plug & Play-Meldungen.
  
Das Blockieren des UPnP-Netzwerkdatenverkehrs verringert effektiv die Angriffsfläche der Computer in Ihrer Umgebung. Microsoft empfiehlt, die Einstellung **Windows-Firewall: Eingehende UPnP-Framework-Ausnahme zulassen** in vertrauenswürdigen Netzwerken auf **Deaktiviert** zu setzen, es sei denn, Sie verwenden in Ihrem Netzwerk UPnP-Geräte. In nicht vertrauenswürdigen Netzwerken sollte diese Richtlinieneinstellung immer auf **Deaktiviert** gesetzt werden.
  
**Windows-Firewall: Lokale Portausnahmen zulassen**  
Diese Richtlinieneinstellung ermöglicht es Administratoren, in der Systemsteuerung mithilfe der Windows-Firewall eine Liste lokaler Portausnahmen zu definieren. Die Windows-Firewall kann zwei Portausnahmelisten verwenden. Die andere Liste wird über **Windows-Firewall: Portausnahmen definieren** festgelegt.
  
Wenn Sie die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen** aktivieren, können Administratoren in der Systemsteuerung mithilfe der Windows-Firewall eine Liste lokaler Portausnahmen definieren. Wenn Sie diese Richtlinieneinstellung deaktivieren, erlaubt die Windows-Firewall in der Systemsteuerung Administratoren nicht, eine solche Liste zu definieren.
  
Normalerweise sind lokale Administratoren nicht berechtigt, Unternehmensrichtlinien außer Kraft zu setzen und ihre eigene Liste mit Portausnahmen einzurichten. Aus diesem Grund empfiehlt Microsoft, die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen** auf **Deaktiviert** zu setzen.
  
**Windows-Firewall: Lokale Programmausnahmen zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Administratoren mithilfe der Windows-Firewall in der Systemsteuerung eine Liste lokaler Programmausnahmen definieren können. Wenn Sie diese Richtlinieneinstellung deaktivieren, sind Administratoren nicht in der Lage, eine Liste lokaler Programmausnahmen zu definieren. Außerdem wird durch diese Konfiguration sichergestellt, dass sämtliche Programmausnahmen der Gruppenrichtlinie entstammen. Wenn diese Richtlinieneinstellung aktiviert ist, können lokale Administratoren die Systemsteuerung dazu verwenden, Programmausnahmen lokal zu definieren.
  
Bei Unternehmensclientcomputern kann es Bedingungen geben, die die Definition lokaler Programmausnahmen rechtfertigen. Diese Bedingungen umfassen z. B. Anwendungen, die bei Erstellung der Firewallrichtlinie der Organisation nicht analysiert wurden, sowie neue Anwendungen, die eine nicht standardmäßige Portkonfiguration erfordern. Wenn Sie sich in solchen Situationen dafür entscheiden, die Einstellung **Windows-Firewall: Lokale Programmausnahmen zulassen** zu aktivieren, müssen Sie sich dessen bewusst sein, dass dadurch die Angriffsfläche der betroffenen Computer vergrößert wird.
  
**Windows-Firewall: Eingehende Portausnahmen definieren**  
Die Liste der Portausnahmen für die Windows-Firewall sollte über Gruppenrichtlinien definiert werden. Diese ermöglichen Ihnen, Ihre Portausnahmen zentral zu verwalten und bereitzustellen und stellen sicher, dass lokale Administratoren keine weniger sicheren Einstellungen konfigurieren.
  
Wenn Sie die Einstellung **Windows-Firewall: Eingehende Portausnahmen definieren** aktivieren, können Sie die Liste der Portausnahmen anzeigen und ändern, die durch Gruppenrichtlinien definiert sind. Wenn Sie die Liste der Portausnahmen anzeigen und ändern möchten, setzen Sie die Richtlinieneinstellung auf **Aktiviert**, und klicken Sie anschließend auf die Schaltfläche **Anzeigen**. Wenn Sie eine ungültige Definitionszeichenfolge eingeben, fügt die Windows-Firewall diese der Liste hinzu, ohne eine Fehlerprüfung vorzunehmen. Sie können also versehentlich mehrere Einträge für den gleichen Port erstellen, wobei die Bereichs- oder Statuswerte einander widersprechen.
  
Wenn Sie die Einstellung **Windows Firewall: Eingehende Portausnahmen definieren** deaktivieren, wird die über Gruppenrichtlinien definierte Liste mit Portausnahmen zwar gelöscht, aber andere Einstellungen können weiterhin Ports öffnen oder blockieren. Außerdem wird eine möglicherweise vorhandene Liste lokaler Portausnahmen ignoriert, es sei denn, Sie aktivieren die Einstellung **Windows-Firewall: Lokale Portausnahmen zulassen.**
  
Für Umgebungen mit nicht standardisierten Anwendungen, für die bestimmte Ports geöffnet sein müssen, sollte erwogen werden, Programmausnahmen anstelle von Portausnahmen bereitzustellen. Microsoft empfiehlt, die Einstellung **Windows-Firewall: Eingehende Portausnahmen definieren** nur dann auf **Aktiviert** zu setzen und eine Liste mit Portausnahmen festzulegen, wenn keine Programmausnahmen definiert werden können. Programmausnahmen erlauben der Windows-Firewall, nicht angeforderten Netzwerkverkehr nur dann zu akzeptieren, wenn das angegebene Programm ausgeführt wird. Portausnahmen halten die angegebenen Ports stets offen.
  
**Hinweis:**   Wenn eine beliebige Richtlinieneinstellung den TCP-Port 445 öffnet, lässt die Windows Firewall eingehende ICMP-Echoanforderungsmeldungen zu (wie z. B. diejenigen, die vom Ping-Dienstprogramm gesendet werden). Dies gilt auch dann, wenn sie von der Richtlinieneinstellung **Windows-Firewall: ICMP-Ausnahmen zulassen** blockiert würden. Zu Richtlinieneinstellungen, die den TCP-Port 445 öffnen können, gehören **Windows-Firewall: Eingehende Ausnahme für gemeinsame Datei- und Druckerfreigabe zulassen**, **Windows-Firewall: Eingehende Remoteverwaltungsausnahme zulassen** und **Windows Firewall: Eingehende Portausnahmen definieren**.
  
**Windows-Firewall: Eingehende Programmausnahmen definieren**  
Einige Anwendungen müssen möglicherweise Netzwerkports öffnen und verwenden, die normalerweise nicht von der Windows-Firewall zugelassen sind. Mit der Einstellung **Windows-Firewall: Eingehende Programmausnahmen definieren** können Sie die Liste der Programmausnahmen anzeigen und ändern, die durch die Gruppenrichtlinie definiert ist.
  
Wenn diese Richtlinieneinstellung **Aktiviert** ist, können Sie die Liste der Programmausnahmen anzeigen und ändern. Wenn Sie dieser Liste ein Programm hinzufügen und den entsprechenden Status auf **Aktiviert** setzen, kann dieses Programm über jeden Port, den die Windows-Firewall auf sein Ersuchen hin öffnet, nicht angeforderte eingehende Meldungen empfangen. Dies gilt selbst dann, wenn der Port von einer anderen Richtlinieneinstellung blockiert wird. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, wird die über Gruppenrichtlinien definierte Liste der Programmausnahmen gelöscht.
  
**Hinweis:**   Wenn Sie eine ungültige Definitionszeichenfolge eingeben, fügt Windows-Firewall diese der Liste hinzu, ohne eine Fehlerprüfung vorzunehmen. Da die Eingabe nicht überprüft wird, können Sie Programme hinzufügen, die Sie noch nicht installiert haben. Sie können auch versehentlich mehrere Ausnahmen für dasselbe Programm mit sich widersprechenden Bereichs- oder Statuswerten erstellen.
  
**Windows-Firewall: Keine Ausnahmen zulassen**  
Diese Richtlinieneinstellung sorgt dafür, dass die Windows-Firewall alle nicht angeforderten eingehenden Nachrichten blockiert. Sie setzt alle anderen Einstellungen der Windows-Firewall außer Kraft, die solche Nachrichten zulassen. Wenn Sie diese Richtlinieneinstellung in der Systemsteuerung für die Windows-Firewall aktivieren, wird das Kontrollkästchen **Keine Ausnahmen zulassen** aktiviert. Administratoren können es nicht deaktivieren.
  
Viele Umgebungen enthalten Anwendungen und Dienste, die im Rahmen des normalen Betriebs in der Lage sein müssen, unangeforderte eingehende Kommunikation zu empfangen. In solchen Umgebungen kann es notwendig sein, die Einstellung **Windows-Firewall: Keine Ausnahmen zulassen** auf **Deaktiviert** zu setzen, damit die jeweiligen Anwendungen und Dienste ordnungsgemäß funktionieren. Bevor Sie jedoch diese Richtlinieneinstellung konfigurieren, sollten Sie die Umgebung prüfen und genau ermitteln, welche Kommunikationen Sie zulassen möchten.
  
**Hinweis:**   Diese Richtlinieneinstellung bietet einen sehr guten Schutz vor externen Angreifern. Sie sollte in Situationen auf **Aktiviert** gesetzt sein, in denen Sie vollständigen Schutz vor externen Angriffen benötigen, z. B. beim Ausbruch eines neuen Netzwerkwurms. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, kann die Windows-Firewall andere Richtlinieneinstellungen anwenden, die nicht angeforderte eingehende Meldungen zulassen.
  
**Windows-Firewall: Benachrichtigungen verbieten**  
Die Windows-Firewall kann Benutzern Benachrichtigungen anzeigen, wenn ein Programm die Anforderung stellt, zur Liste mit den Programmausnahmen hinzugefügt zu werden. Diese Situation tritt ein, wenn Programme versuchen, einen Port zu öffnen, den sie aufgrund der aktuellen Regeln der Windows-Firewall nicht öffnen dürfen.
  
Mit der Einstellung **Windows-Firewall: Benachrichtigungen verbieten** wird festgelegt, ob diese Benachrichtigungen Benutzern angezeigt werden. Wenn Sie diese Richtlinie auf **Aktiviert** setzen, wird das Anzeigen dieser Benachrichtigungen von der Windows-Firewall verhindert. Wenn Sie die Richtlinie auf **Deaktiviert** setzen, lässt die Windows-Firewall das Anzeigen dieser Benachrichtigungen zu.
  
**Windows-Firewall: Unicastantwort auf Multicast- oder Broadcastanforderungen nicht zulassen**  
Diese Richtlinieneinstellung hilft zu verhindern, dass ein Computer Unicastantworten auf seine ausgehenden Multicast- oder Broadcastmeldungen empfängt. Wenn diese Richtlinieneinstellung aktiviert ist und der Computer Multicast- oder Broadcastmeldungen an andere Computer sendet, blockiert die Windows-Firewall die Unicast-Antworten, die von den anderen Computern gesendet werden. Wenn diese Richtlinieneinstellung deaktiviert ist und dieser Computer eine Multicast- oder Broadcastmeldung an andere Computer sendet, wartet die Windows-Firewall bis zu drei Sekunden auf Unicast-Antworten von den anderen Computern und blockiert alle späteren Antworten.
  
Normalerweise ist es nicht wünschenswert, auf Multicast- oder Broadcastmeldungen Unicast-Antworten zu erhalten. Solche Antworten können auf einen DoS-Angriff (Denial of Service) oder auf einen Angreifer hindeuten, der versucht, einen bekannten Computer zu untersuchen. Microsoft empfiehlt, die Einstellung **Windows-Firewall: Unicastantwort auf Multicast- oder Broadcastanforderungen nicht zulassen** auf **Aktiviert** zu setzen, um diese Art von Angriff zu verhindern.
  
**Hinweis:**   Diese Richtlinieneinstellung ist wirkungslos, wenn es sich bei der Unicastmeldung um eine Antwort auf eine DHCP-Broadcastmeldung (Dynamic Host Configuration Protocol) handelt, die vom Computer gesendet wurde. Die Windows-Firewall lässt diese DHCP-Antworten immer zu. Diese Richtlinieneinstellung kann sich jedoch störend auf NetBIOS-Nachrichten zur Erkennung von Namenskonflikten auswirken.
  
**Windows-Firewall: Alle Netzwerkverbindungen schützen**  
Durch diese Richtlinieneinstellung wird die Windows-Firewall aktiviert. Sie ersetzt die Internetverbindungsfirewall auf allen Computern, auf denen Windows Vista ausgeführt wird. Es wird empfohlen, diese Richtlinieneinstellung auf **Aktiviert** zu setzen. Dadurch werden für Computer in den in diesem Handbuch behandelten Umgebungen sämtliche Netzwerkverbindungen geschützt.
  
Wenn **Windows-Firewall: Alle Netzwerkverbindungen schützen** auf **Deaktiviert** gesetzt ist, ist die Windows-Firewall deaktiviert, und alle anderen Einstellungen für die Windows-Firewall werden ignoriert.
  
**Hinweis:**   Wenn Sie diese Richtlinieneinstellung aktivieren, wird die Windows-Firewall ausgeführt, und die Einstellung **Computerkonfiguration\\Administrative Vorlagen\\Netzwerk\\Netzwerkverbindungen**  
**\\Verwendung des Internetverbindungsfirewalls im eigenen DNS-Domänennetzwerk nicht zulassen** wird ignoriert.
  
##### System
  
Im Verzeichnis Computerkonfiguration\\Administrative Vorlagen\\System werden zusätzlich folgende Abschnitte konfiguriert:
  
-   [Anmeldung](#_logon)
  
-   [Gruppenrichtlinie](#_group_policy)
  
-   [Remoteunterstützung](#_remote_assistance)
  
-   [Remoteprozeduraufruf](#_remote_procedure_call)
  
-   [Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen](#_internet_communication_management--)
  
###### Anmeldung
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Anmeldung**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für die Anmeldung. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A37: Empfohlene Einstellungen für die Anmeldung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Herkömmliche Ausführungsliste nicht verarbeiten**  
Durch diese Richtlinieneinstellung wird festgelegt, dass die Ausführungsliste mit allen beim Start von Windows Vista automatisch auszuführenden Programmen ignoriert werden soll. Die benutzerdefinierten Ausführungslisten für Windows Vista werden in der Registrierung in folgenden Verzeichnissen gespeichert:
  
-   **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\Run**
  
-   **HKEY\_CURRENT\_USER\\Software\\Microsoft\\Windows\\CurrentVersion\\Run**
  
Durch Aktivieren der Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten** wird weitgehend verhindert, dass ein böswilliger Benutzer bei jedem Start von Windows Vista ein Programm ausführen lässt, das Daten beeinträchtigt oder in anderer Weise Schaden anrichtet. Wenn diese Richtlinieneinstellung aktiviert ist, wird die Ausführung bestimmter Systemprogramme verhindert, z. B. die Ausführung von Antivirensoftware oder von Programmen für Softwareverteilung und -überwachung. Schätzen Sie die Bedrohung für Ihre Umgebung ab, bevor Sie entscheiden, diese Richtlinieneinstellung für Ihre Organisation zu verwenden.
  
Die Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert** und für die Hochsicherheitsumgebung **Aktiviert**.
  
**Einmalige Ausführungsliste nicht verarbeiten**  
Diese Richtlinieneinstellung sorgt dafür, dass die einmalige Ausführungsliste mit allen beim Start von Windows Vista automatisch auszuführenden Programmen ignoriert wird. Diese Richtlinieneinstellung unterscheidet sich von der Einstellung **Herkömmliche Ausführungsliste nicht verarbeiten**, da Programme in dieser Liste beim nächsten Neustart des Clientcomputers einmalig ausgeführt werden. Dieser Liste werden z. B. Setup- und Installationsprogramme hinzugefügt, um Installationen nach einem Neustart des Clientcomputers abzuschließen. Indem Sie diese Richtlinieneinstellung aktivieren, verhindern Sie im Allgemeinen, dass Angreifer über die Liste der einmalig auszuführenden Programme unzulässige Anwendungen starten, was früher eine beliebte Angriffsmethode war. Ein böswilliger Benutzer kann die einmalige Ausführungsliste missbrauchen, um ein Programm zu installieren, mit dem möglicherweise die Sicherheit von Windows Vista-basierten Clientcomputern gefährdet wird.
  
**Hinweis:**   Benutzerdefinierte Listen mit einmalig auszuführenden Programmen werden in der Registrierung in folgendem Verzeichnis gespeichert: **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows\\CurrentVersion\\RunOnce**.
  
Die Einstellung **Einmalige Ausführungsliste nicht verarbeiten** sollte für die Benutzer in Ihrer Umgebung lediglich einen minimalen Funktionalitätsverlust verursachen, insbesondere wenn die Clientcomputer mit der gesamten Standardsoftware Ihrer Organisation konfiguriert wurden, bevor diese Richtlinieneinstellung durch Gruppenrichtlinien angewendet wird. Die Einstellung **Einmalige Ausführungsliste nicht verarbeiten** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert** und für die Hochsicherheitsumgebung **Aktiviert**.
  
###### Gruppenrichtlinie
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Gruppenrichtlinie**
  
**Tabelle A38: Empfohlene Gruppenrichtlinieneinstellungen**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Registrierungsrichtlinienverarbeitung**  
Durch diese Richtlinieneinstellung wird festgelegt, wann Registrierungsrichtlinien aktualisiert werden. Sie betrifft alle Richtlinien im Ordner „Administrative Vorlagen“ sowie alle Richtlinien, mit denen Werte in der Registrierung gespeichert werden. Wenn diese Richtlinieneinstellung aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Während regelmäßiger Hintergrundverarbeitung nicht übernehmen.**
  
-   **Gruppenrichtlinienobjekte auch ohne Änderungen bearbeiten.**
  
Einige der in den administrativen Vorlagen konfigurierten Einstellungen werden in der Registrierung in Bereichen gespeichert, auf die Benutzer Zugriff haben. Änderungen von Benutzern an diesen Einstellungen werden überschrieben, wenn diese Richtlinieneinstellung aktiviert wird.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Registrierungsrichtlinienverarbeitung** auf **Aktiviert** gesetzt.
  
###### Remoteunterstützung
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Remoteunterstützung**
  
In der folgenden Tabelle sind die empfohlenen Einstellungen für die Remoteunterstützung zusammengefasst. Weitere Informationen zu den einzelnen Einstellungen finden Sie in den Unterabschnitten im Anschluss.
  
**Tabelle A39: Empfohlene Einstellungen für die Remoteunterstützung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Remoteunterstützung anbieten**  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Supportmitarbeiter oder ein versierterIT-Administrator Remoteunterstützung für Computer in Ihrer Umgebung anbieten kann, ohne dass ein Benutzer zuvor explizit Unterstützung über Kanäle, z. B. über E-Mail oder Instant Messenger, angefordert hat.
  
**Hinweis:**   Der Experte kann nicht unangekündigt eine Verbindung zum Computer herstellen oder diesen ohne Erlaubnis des Benutzers steuern. Wenn ein Verbindungsversuch erfolgt, kann der Benutzer die Verbindung immer noch verweigern (und damit dem Experten nur Anzeigeberechtigungen gewähren). Der Benutzer muss auf die Schaltfläche **Ja** klicken, um die Remotesteuerung der Arbeitsstation zuzulassen, wenn für die Einstellung **Remoteunterstützung anbieten** die Option **Aktiviert** angegeben wurde.
  
Wenn diese Richtlinieneinstellung aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Helfer dürfen den Computer nur ansehen**
  
-   **Helfer dürfen den Computer remote steuern**
  
Beim Konfigurieren dieser Richtlinieneinstellung können Sie eine Liste mit Benutzern oder Benutzergruppen angeben, die als „Helfer“ Remoteunterstützung anbieten können.
  
**So konfigurieren Sie die Liste der Helfer**
  
1.  Klicken Sie im Einstellungsfenster **Remoteunterstützung anbieten** auf **Anzeigen**. Im daraufhin geöffneten neuen Fenster können Sie die Namen der Helfer eingeben.
  
2.  Verwenden Sie beim Hinzufügen von Benutzern oder Gruppen zur Liste **Helfer** eines der folgenden Formate:
  
    -   *&lt;Domänenname&gt;*\\*&lt;Benutzername&gt;*
  
    -   *&lt;Domänenname&gt;*\\*&lt;Gruppenname&gt;*
  
Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können Benutzer oder Gruppen Computerbenutzern in Ihrer Umgebung keine unangeforderte Remoteunterstützung anbieten.
  
Die Einstellung **Remoteunterstützung anbieten** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Deaktiviert** gesetzt, um den Zugriff auf Windows Vista-Clientcomputer über das Netzwerk zu verhindern.
  
**Angeforderte Remoteunterstützung**  
Durch diese Richtlinieneinstellung wird festgelegt, ob von den Windows Vista-Computern in Ihrer Umgebung Remoteunterstützung angefordert werden kann. Sie können diese Richtlinieneinstellung aktivieren, damit Benutzer Remoteunterstützung von versierten IT-Administratoren anfordern können.
  
**Hinweis:**   Experten können nicht unangekündigt eine Verbindung zum Computer herstellen oder diesen ohne Erlaubnis des Benutzers steuern. Wenn ein Verbindungsversuch erfolgt, kann der Benutzer die Verbindung immer noch verweigern (und damit dem Experten nur Anzeigeberechtigungen gewähren). Der Benutzer muss ausdrücklich auf die Schaltfläche **Ja** klicken, um die Remotesteuerung der Arbeitsstation zuzulassen.
  
Wenn die Einstellung **Angeforderte Remoteunterstützung** aktiviert ist, stehen folgende Optionen zur Verfügung:
  
-   **Helfer dürfen den Computer remote steuern**
  
-   **Helfer dürfen den Computer nur ansehen**
  
Zusätzlich sind folgende Optionen verfügbar, um die Zeitdauer zu konfigurieren, für die die Hilfeanforderung eines Benutzers Gültigkeit behält:
  
-   **Maximale Gültigkeitsdauer der Einladung (Wert):**
  
-   **Maximale Gültigkeitsdauer der Einladung (Einheiten): Stunden,** **Minuten oder Tage**
  
Wenn ein Ticket (Hilfeanforderung) abgelaufen ist, muss der Benutzer eine neue Anforderung senden, damit der Experte eine Verbindung mit dem Computer herstellen kann. Wenn Sie die Einstellung **Angeforderte Remoteunterstützung** deaktivieren, können Benutzer keine Hilfeanforderungen senden, und ein Experte kann keine Verbindung zum Computer des Benutzers herstellen.
  
Wenn die Einstellung **Angeforderte Remoteunterstützung** nicht konfiguriert ist, können Benutzer angeforderte Remoteunterstützung über die Systemsteuerung konfigurieren. Die folgenden Einstellungen sind standardmäßig in der Systemsteuerung aktiviert: **Angeforderte Remoteunterstützung**, **Benutzerunterstützung** und **Remotesteuerung**. Als Wert für die **Maximale Gültigkeitsdauer der Einladung** sind **30 Tage** festgelegt. Wenn diese Richtlinieneinstellung deaktiviert ist, kann niemand über das Netzwerk auf Windows Vista-Clientcomputer zugreifen.
  
Die Einstellung **Angeforderte Remoteunterstützung** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
###### Remoteprozeduraufruf
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\System\\Remoteprozeduraufruf**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für den Remoteprozeduraufruf. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A40: Empfohlene Einstellungen für den Remoteprozeduraufruf**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
<td style="border:1px solid black;">RPC-Endpunktzuordnungs-Clientauthentifizierung</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Einschränkungen für nicht authentifizierte RPC-Clients**  
Diese Richtlinieneinstellung sorgt dafür, dass die RPC-Laufzeit auf einem RPC-Server nicht authentifizierte RPC-Clients daran hindert, eine Verbindung zu RPC-Servern herzustellen Ein Client gilt als authentifizierter Client, wenn er über eine Named Pipe mit dem Server kommuniziert oder wenn er RPC-Sicherheit verwendet. RPC-Schnittstellen, die speziell um Zugriff durch nicht authentifizierte Clients angesucht haben, sind von dieser Einschränkung möglicherweise ausgenommen, je nachdem, welchen Wert Sie für diese Richtlinie gewählt haben. Wenn Sie diese Richtlinieneinstellung aktivieren, sind folgende Werte verfügbar:
  
-   **Keine**. Erlaubt allen RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt.
  
-   **Authentifiziert**. Erlaubt nur authentifizierten RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt. Den Schnittstellen, die um eine Ausnahme von dieser Einschränkung angesucht haben, wird eine Ausnahme gewährt.
  
-   **Authentifiziert ohne Ausnahmen**. Erlaubt nur authentifizierten RPC-Clients, eine Verbindung zu RPC-Servern herzustellen. Diese wiederum müssen auf dem Computer ausgeführt werden, für den die Richtlinie gilt. Es sind keine Ausnahmen zulässig.
  
Da nicht authentifizierte RPC-Kommunikation eine Sicherheitsanfälligkeit verursachen kann, ist für die beiden in diesem Handbuch behandelten Umgebungen die Einstellung **Einschränkungen für nicht authentifizierte RPC-Clients** auf **Aktiviert** und der Wert **RPC-Laufzeit: Einschränkungen für nicht authentifizierte Clients anwenden** auf **Authentifiziert** gesetzt.
  
**Hinweis:**   RPC-basierte Anwendungen, die unerwünscht eingehende Verbindungsanforderungen nicht authentifizieren, funktionieren möglicherweise nicht richtig, wenn diese Konfiguration angewendet wird. Testen Sie die Anwendungen unbedingt, bevor Sie diese Richtlinieneinstellung für Ihre gesamte Umgebung bereitstellen. Obwohl der Wert „Authentifiziert“ für diese Richtlinieneinstellung nicht vollständig sicher ist, kann er für die Bereitstellung von Anwendungskompatibilität in Ihrer Umgebung nützlich sein.
  
**RPC-Endpunktzuordnungs-Clientauthentifizierung**  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden mit diesem Computer kommunizierende Clientcomputer zur Authentifizierung gezwungen, bevor eine RPC-Kommunikation eingerichtet wird. Standardmäßig verwenden RPC-Clients keine Authentifizierung, um mit der RPC-Endpunktzuordnung zu kommunizieren, wenn sie den Endpunkt von einem Server anfordern. Dieser Standard wurde jedoch für die Hochsicherheitsumgebung geändert, um von Clientcomputern eine Authentifizierung zu fordern, bevor eine RPC-Kommunikation zugelassen wird.
  
###### Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen
  
In der Gruppe „Internetkommunikationseinstellungen“ sind mehrere Konfigurationseinstellungen verfügbar. Es wird empfohlen, viele dieser Einstellungen einzuschränken, in erster Linie um die Sicherheit der Daten auf Ihren Computersystemen zu erhöhen. Wenn diese Einstellungen nicht eingeschränkt werden, könnten Informationen durch Angreifer abgefangen und missbraucht werden. Obwohl diese Art von Angriff heutzutage selten ist, können Sie Ihre Umgebung durch die richtige Konfiguration dieser Einstellungen vor zukünftigen Angriffen schützen.
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\System\\Internetkommunikationsverwaltung\\Internetkommunikationseinstellungen**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für die Internetkommunikation. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A41: Empfohlene Einstellungen für die Internetkommunikation**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Aufgabe „Im Web veröffentlichen“ für Dateien und Ordner deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internet-Download für die Assistenten „Webpublishing“ und „Onlinebestellung von Abzügen“ deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Programm zur Verbesserung der Benutzerfreundlichkeit deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Inhaltdateiupdates des Such-Assistenten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Drucken über HTTP deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Download von Druckertreibern über HTTP deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Suche nach Gerätetreibern auf Windows Update deaktivieren</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Aufgabe „Im Web veröffentlichen“ für Dateien und Ordner deaktivieren**  
Durch diese Einstellung wird festgelegt, ob die Aufgaben **Datei im Web veröffentlichen**, **Ordner im Web veröffentlichen** und **Ausgewählte Elemente im Web veröffentlichen** in den Datei- und Ordneraufgaben in Windows-Ordnern zur Verfügung stehen. Mit dem Webpublishing-Assistenten wird eine Liste von Anbietern heruntergeladen, und Benutzer können Inhalte im Internet veröffentlichen.
  
Wenn Sie die Einstellung **Aufgabe „Im Web veröffentlichen“ für Dateien und Ordner deaktivieren** auf **Aktiviert** setzen, werden diese Optionen aus den Datei- und Ordneraufgaben in Windows-Ordnern entfernt. Die Option zur Veröffentlichung im Internet ist standardmäßig verfügbar. Da diese Funktion dazu genutzt werden könnte, gesicherten Inhalt gegenüber einem nicht authentifizierten Webclientcomputer offen zu legen, ist diese Richtlinieneinstellung sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Internet-Download für die Assistenten „Webpublishing“ und „Onlinebestellung von Abzügen“ deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows eine Liste von Anbietern für das Webpublishing und Assistenten für Onlinebestellungen herunterlädt. Wenn diese Richtlinieneinstellung aktiviert ist, wird Windows daran gehindert, Anbieter herunterzuladen. Es werden nur die Dienstanbieter angezeigt, die in der lokalen Registrierung zwischengespeichert sind.
  
Da die Einstellung **Aufgabe„Im Web veröffentlichen“ für Dateien und Ordner deaktivieren** sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung aktiviert wurde (siehe vorherige Einstellung), ist diese Option nicht erforderlich. Die Einstellung **Internet-Download für die Assistenten „Webpublishing“ und „Onlinebestellung von Abzügen“ deaktivieren** ist auf **Aktiviert** gesetzt, um die Angriffsfläche von Clientcomputern zu minimieren und sicherzustellen, dass diese Funktion nicht auf andere Weise ausgenutzt werden kann.
  
**Programm zur Verbesserung der Benutzerfreundlichkeit deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows Messenger anonyme Informationen darüber sammelt, wie Software und Dienste von Windows Messenger verwendet werden. Sie können diese Richtlinieneinstellung aktivieren, um sicherzustellen, dass Windows Messenger keine Nutzungsdaten sammelt. Außerdem wird die Benutzereinstellung, mit der das Sammeln von Nutzungsdaten aktiviert werden kann, nicht angezeigt.
  
In großen Unternehmensumgebungen ist es häufig unerwünscht, dass Informationen von verwalteten Clientcomputern gesammelt werden. Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Programm zur Verbesserung der Benutzerfreundlichkeit deaktivieren** auf **Aktiviert** gesetzt, um das Sammeln von Informationen zu verhindern.
  
**Inhaltdateiupdates des Such-Assistenten deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Such-Assistent bei lokalen Suchen und Internetsuchen automatisch Inhaltsaktualisierungen herunterladen soll. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, hindern Sie den Such-Assistenten daran, im Verlauf von Suchen Inhaltsaktualisierungen herunterzuladen.
  
Die Einstellung **Inhaltdateiupdates des Such-Assistenten deaktivieren** ist sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt, um unnötige Netzwerkkommunikation von den verwalteten Clientcomputern zu kontrollieren.
  
**Hinweis:**   Internetsuchen senden den Suchtext und Informationen zur Suche weiterhin an Microsoft und den ausgewählten Suchprovider. Wenn Sie „Klassische Suche“ auswählen, ist die Funktion Such-Assistent nicht verfügbar. Sie können „Klassische Suche“ auswählen, indem Sie auf **Start**, **Suchen**, **Bevorzugte Einstellungen ändern** und schließlich auf **Internetsuchverhalten ändern** klicken.
  
**Drucken über HTTP deaktivieren**  
Mit dieser Richtlinieneinstellung können Sie verhindern, dass der Clientcomputer über HTTP und damit auf Druckern im Intranet sowie im Internet drucken kann. Wenn Sie diese Richtlinieneinstellung aktivieren, kann der Clientcomputer nicht über HTTP auf Internetdruckern drucken.
  
Informationen, die mithilfe dieser Funktion über HTTP übertragen werden, sind nicht geschützt und können von unbefugten Benutzern abgefangen werden. Aus diesem Grund wird sie nicht oft in Unternehmensumgebungen verwendet. Die Einstellung **Drucken über HTTP deaktivieren** ist sowohl für die Unternehmensclient-Umgebung als auch für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt, um eine potenzielle Sicherheitsverletzung durch einen unsicheren Druckauftrag zu verhindern.
  
**Hinweis:**   Diese Richtlinieneinstellung beim Internetdrucken wirkt sich nur auf den Client aus. Ungeachtet der Konfiguration könnte ein Computer als Internetdruckserver agieren und seine freigegebenen Drucker über HTTP zur Verfügung stellen.
  
**Download von Druckertreibern über HTTP deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Computer Drucktreiberpakete über HTTP herunterladen kann. Für das Einrichten der Druckausgabe über HTTP müssen möglicherweise Druckertreiber über HTTP heruntergeladen werden, die nicht in der Standard-Betriebssysteminstallation enthalten sind.
  
Die Einstellung **Download von Druckertreibern über HTTP deaktivieren** ist auf **Aktiviert** gesetzt, damit keine Druckertreiber über HTTP heruntergeladen werden können.
  
**Hinweis:**   Diese Richtlinieneinstellung hindert den Clientcomputer nicht daran, über HTTP auf Druckern im Intranet oder Internet zu drucken. Sie unterbindet lediglich das Herunterladen von Treibern, die nicht bereits lokal installiert sind.
  
**Suche nach Gerätetreibern auf Windows Update deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows in Windows Update nach Gerätetreibern sucht, wenn lokal keine Treiber für ein Gerät vorhanden sind.
  
Das Herunterladen von Gerätetreibern aus dem Internet birgt gewisse Risiken. Deshalb wird empfohlen, die Einstellung **Suche nach Gerätetreibern auf Windows Update deaktivieren** für Hochsicherheitsumgebungen auf **Aktiviert** und für Unternehmensclient-Umgebungen auf **Deaktiviert** zu setzen. Der Grund für diese Konfiguration ist, dass den Angriffsarten, die einen Treiberdownload ausnutzen, in der Regel durch eine korrekte Verwaltung von Unternehmensanwendungen und Konfigurationen begegnet werden kann. Dies trägt auch zur Kompatibilität und Stabilität der Computer in Ihrer Umgebung bei.
  
**Hinweis:**   Befassen Sie sich außerdem mit **Suchbefehl für Gerätetreiber in Windows Update deaktivieren** in **Administrative Vorlagen/System**. Durch diese Einstellung wird festgelegt, ob ein Administrator um Zustimmung gebeten wird, bevor Windows Update nach einem Gerätetreiber durchsucht wird, der lokal nicht vorhanden ist.
  
##### Windows-Komponenten
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**
  
Im Abschnitt Administrative Vorlagen\\Windows-Komponenten können Sie Einstellungen für Folgendes konfigurieren:
  
-   [Richtlinien für automatische Wiedergabe](#_autoplay_policies)
  
-   [Benutzeroberfläche für Anmeldeinformationen](#_credential_user_interface)
  
-   [Internet Explorer](#_internet_explorer_2)
  
-   [NetMeeting](#_netmeeting)
  
-   [Terminaldienste](#_terminal_services)
  
-   [Windows Messenger](#_windows_messenger)
  
-   [Windows Update](#_windows_update)
  
###### Richtlinien für automatische Wiedergabe
  
Automatische Wiedergabe (Autoplay) ist eine Funktion von Windows, mit der Mediendateien oder Installationsprogramme automatisch geöffnet oder gestartet werden, sobald sie vom Computer erkannt werden. Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**AutoPlay Policies**
  
**Tabelle A42: Empfohlene Einstellungen für die automatische Wiedergabe**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Autoplay deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert –<br />
Alle Laufwerke</td>
<td style="border:1px solid black;">Aktiviert –<br />
Alle Laufwerke</td>
</tr>
</tbody>
</table>
 

**Autoplay deaktivieren**
Die automatische Wiedergabe sorgt dafür, dass der Lesevorgang von einem Laufwerk unmittelbar nach dem Einlegen eines Mediums gestartet wird. Auf dem Medium gespeicherte Setupdateien oder Audiodaten werden dann automatisch ausgeführt bzw. abgespielt. Ein Angreifer kann diese Funktion ausnutzen, um ein Programm zu starten, das einen Computer oder die Daten auf dem Computer beschädigen könnte. Sie können die Einstellung **Autoplay deaktivieren** aktivieren, um die Funktion zur automatischen Wiedergabe zu deaktivieren. Die automatische Wiedergabe ist bei austauschbaren Datenträgern, wie z. B. Disketten- oder Netzlaufwerken, bereits in der Standardeinstellung deaktiviert, aber nicht bei CD-ROM-Laufwerken.

Die Einstellung **Autoplay deaktivieren** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert – Alle Laufwerke** gesetzt.

**Hinweis:**   Sie können diese Einstellung nicht verwenden, um die automatische Wiedergabe für Computerlaufwerke zu aktivieren, bei denen diese Funktion in der Standardeinstellung deaktiviert ist, z. B. bei Disketten- oder Netzlaufwerken.

###### Benutzeroberfläche für Anmeldeinformationen

Die Einstellungen der Benutzeroberfläche für Anmeldeinformationen bestimmen, wie sich die Benutzeroberfläche den Benutzern darstellt, wenn sie zur Eingabe ihres Kontonamens und Kennworts aufgefordert werden, um höhere Aufgaben zu autorisieren, die eine Genehmigung durch den sicheren Desktop erfordern. Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Credential User Interface**

**Tabelle A43: Empfohlene Einstellungen für die Benutzeroberfläche der Benutzerkontensteuerung-Anmeldeinformationen**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Enumerate administrator accounts on elevation (Administratorkonten bei Heraufstufung auflisten)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Require trusted path for credential entry (Vertrauenswürdigen Pfad für die Eingabe von Anmeldeinformationen erfordern)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista
  
**Enumerate administrator accounts on elevation (Administratorkonten bei Heraufstufung auflisten)**  
Standardmäßig werden alle Administratorkonten angezeigt, wenn Sie versuchen, die Rechte bei einer laufenden Anwendung zu erhöhen. Wenn Sie diese Richtlinie aktivieren, müssen die Benutzer immer einen Benutzernamen und ein Kennwort eingeben, um eine Erhöhung durchzuführen. Wenn Sie diese Richtlinie deaktivieren, werden alle lokalen Administratorkonten auf dem Computer angezeigt, so dass der Benutzer eines davon auswählen und das richtige Kennwort eingeben kann.
  
Die Einstellung **Enumerate administrator accounts on elevation** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Require trusted path for credential entry (Vertrauenswürdigen Pfad für die Eingabe von Anmeldeinformationen erfordern)**  
Wenn Sie diese Richtlinieneinstellung deaktivieren, müssen Benutzer mithilfe des vertrauenswürdigen Pfads Windows-Anmeldeeinformationen auf dem sicheren Desktop eingeben. Dies bedeutet, dass Benutzer erst STRG+ALT+ENTF drücken müssen, bevor sie ihren Kontonamen und ihr Kennwort eingeben, um eine Anforderung für erhöhte Rechte zu autorisieren. Das Verlangen eines vertrauenswürdigen Pfads hilft zu verhindern, dass ein Trojaner oder andere Arten von bösartigem Code die Windows-Anmeldeinformationen des Benutzers ausspionieren.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, geben Benutzer während ihrer Desktopsitzung Windows-Anmeldeinformationen ein und ermöglichen dadurch u. U. bösartigem Code den Zugriff auf ihre Windows-Anmeldeinformationen.
  
Die Einstellung **Require trusted path for credential entry** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
###### Internet Explorer
  
Mithilfe der Gruppenrichtlinie für Microsoft Internet Explorer® können Sie die Sicherheitsanforderungen für Windows Vista-Computern umsetzen. Darüber hinaus wird dadurch der Austausch unerwünschter Inhalte über Internet Explorer verhindert. Sichern Sie Internet Explorer nach folgenden Kriterien auf Ihren Arbeitsstationen ab:
  
-   Stellen Sie sicher, dass Anforderungen an das Internet lediglich als direkte Reaktion auf Benutzeraktionen erfolgen.
  
-   Stellen Sie sicher, dass Informationen, die an spezifische Websites gesendet werden, nur zu diesen Sites gelangen, es sei denn, es sind spezielle Benutzeraktionen zugelassen, durch die Informationen an andere Ziele übertragen werden.
  
-   Stellen Sie sicher, dass vertrauenswürdige Kanäle zu Servern/Websites sowie die Besitzer der jeweiligen Server/Websites eindeutig identifiziert werden.
  
-   Stellen Sie sicher, dass alle mit Internet Explorer gestarteten Skripts oder Programme in einer eingeschränkten Umgebung ausgeführt werden. Die über vertrauenswürdige Kanäle übermittelten Programme können so konfiguriert werden, dass sie außerhalb der eingeschränkten Umgebung ausgeführt werden.
  
**Wichtig:**   Bevor Sie die Gruppenrichtlinienobjekte anwenden, die diesem Handbuch beigefügt sind, muss Internet Explorer ordnungsgemäß für den Internetzugriff konfiguriert sein. In vielen Umgebungen sind für einen ordnungsgemäßen Internetzugriff spezielle Proxyeinstellungen erforderlich. Die in diesem Handbuch empfohlenen Einstellungen verhindern, dass Benutzer die Konfiguration von Internet Explorer-Proxyeinstellungen ändern können.
  
Die empfohlenen Computereinstellungen für Internet Explorer können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer**
  
Die folgende Tabelle bietet einen Überblick über zahlreiche empfohlene Einstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A44: Empfohlene Einstellungen für Internet Explorer**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
<td style="border:1px solid black;">Periodische Überprüfungen auf Internet Explorer-Softwareupdates deaktivieren</td>
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
<td style="border:1px solid black;">Aktivierung bzw. Deaktivierung von Add-Ons für Benutzer nicht zulassen</td>
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
<td style="border:1px solid black;">Sicherheitszonen: Benutzer können keine Sites hinzufügen/entfernen</td>
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
<td style="border:1px solid black;">Sicherheitszonen: Nur Computereinstellungen verwenden</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Systemabsturzermittlung deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Automatische Installation von Internet Explorer-Komponenten deaktivieren**  
Wenn Sie diese Richtlinieneinstellung aktivieren, kann Internet Explorer keine Komponenten herunterladen, wenn die Benutzer Websites ansteuern, die für ein vollständiges Funktionieren diese Komponenten erfordern. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, werden die Benutzer bei jedem Besuch der entsprechenden Websites aufgefordert, die Komponenten herunterzuladen oder zu installieren.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung ist die Einstellung **Automatische Installation von Internet Explorer-Komponenten deaktivieren** auf **Aktiviert** gesetzt.
  
**Hinweis:** Microsoft empfiehlt, vor dem Aktivieren dieser Richtlinieneinstellung mit Microsoft Update oder einem ähnlichen Dienst eine alternative Möglichkeit zum Aktualisieren von Internet Explorer einzurichten.
  
**Periodische Überprüfungen auf Internet Explorer-Softwareupdates deaktivieren**  
Wenn Sie diese Richtlinieneinstellung aktivieren, kann durch Internet Explorer nicht mehr festgestellt werden, ob eine neuere Browserversion verfügbar ist, und die Benutzer erhalten keine entsprechende Benachrichtigung mehr. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, wird von Internet Explorer standardmäßig alle 30 Tage geprüft, ob Aktualisierungen vorhanden sind. Ist eine neue Version verfügbar, werden die Benutzer benachrichtigt.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung ist die Einstellung **Periodische Überprüfungen auf Internet Explorer-Softwareupdates deaktivieren** auf **Aktiviert** gesetzt.
  
**Hinweis:** Microsoft empfiehlt, vor dem Aktivieren dieser Richtlinieneinstellung eine alternative Strategie für die Administratoren Ihrer Organisation einzurichten, um sicherzustellen, dass auf den Clients Ihrer Umgebung regelmäßig neue Updates für Internet Explorer ausgeführt werden.
  
**Softwareupdatebenachrichtigungen beim Programmstart deaktivieren**  
Durch diese Richtlinieneinstellung wird festgelegt, dass Programme, die Microsoft Software Distribution Channels verwenden, Benutzer nicht informieren, wenn neue Komponenten installiert werden. Software Distribution Channels werden für die dynamische Aktualisierung von Software auf Benutzercomputern verwendet und basieren auf Open Software Distribution-Technologie (.osd).
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Softwareupdatebenachrichtigungen beim Programmstart deaktivieren** auf **Aktiviert** gesetzt.
  
**Aktivierung bzw. Deaktivierung von Add-Ons für Benutzer nicht zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Möglichkeit haben, Add-Ons mithilfe des Befehls „Add-Ons verwalten“ zuzulassen oder zu verweigern. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** einstellen, können Benutzer Add-Ons nicht über den Befehl „Add-Ons verwalten“ aktivieren oder deaktivieren. Eine Ausnahme ist lediglich dann gegeben, wenn ein Add-On ausdrücklich so in der Richtlinieneinstellung **Add-On-Liste** eingegeben wurde, dass Benutzer das Add-On weiterhin verwalten können. In einem solchen Fall kann der Benutzer das Add-On immer noch über „Add-Ons verwalten“ verwalten. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, kann der Benutzer Add-Ons aktivieren bzw. deaktivieren.
  
Benutzer installieren häufig Add-Ons, die gemäß der Sicherheitsrichtlinien der Organisation nicht zulässig sind. Solche Add-Ons können beträchtliche Sicherheits- und Datenschutzrisiken für Ihr Netzwerk darstellen. Für die beiden in diesem Kapitel behandelten Umgebungen ist diese Richtlinieneinstellung deshalb auf **Aktiviert** gesetzt.
  
**Hinweis:** Sie sollten die Gruppenrichtlinienobjekt-Einstellungen in Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung überprüfen, um sicherzustellen, dass entsprechend autorisierte Add-Ons weiterhin in Ihrer Umgebung ausgeführt werden können. Lesen Sie gegebenenfalls den Knowledge Base-Artikel 555235, [Outlook Web Access and Small Business Server Remote Web Workplace do not function if XP Service Pack 2 Add-on Blocking is enabled via group policy](http://support.microsoft.com/kb/555235/en-us) (engl.).
  
**Proxyeinstellungen pro Computer vornehmen (anstelle von pro Benutzer)**  
Wenn Sie diese Richtlinieneinstellung aktivieren, ist es Benutzern nicht erlaubt, benutzerspezifische Proxyeinstellungen zu ändern. Die Benutzer müssen die Zonen verwenden, die für alle Benutzer eines Computers erstellt wurden.
  
Für Desktopclientcomputer in den beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Proxyeinstellungen pro Computer vornehmen (anstelle von pro Benutzer)** auf **Aktiviert** gesetzt. Für Laptopclientcomputer ist die Richtlinieneinstellung jedoch auf **Deaktiviert** gesetzt, da mobile Benutzer auf Reisen die Proxyeinstellungen u. U. ändern müssen.
  
**Sicherheitszonen: Benutzer können keine Sites hinzufügen/entfernen**  
Aktivieren Sie diese Richtlinieneinstellung, um die Einstellungen für die Siteverwaltung von Sicherheitszonen zu deaktivieren. (Zum Anzeigen der Siteverwaltungseinstellungen für Sicherheitszonen öffnen Sie Internet Explorer, wählen Sie **Extras** und **Internetoptionen**, klicken Sie auf die Registerkarte **Sicherheit** und anschließend auf **Sites**.) Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, sind Benutzer in der Lage, Websites in den Zonen **Vertrauenswürdige** und **Eingeschränkte Sites** hinzuzufügen und zu entfernen und Einstellungen in der Zone **Lokales Intranet** zu ändern.
  
Die Einstellung **Sicherheitszonen: Benutzer können Sites nicht hinzufügen oder entfernen** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Wenn Sie die Einstellung **Sicherheitsseite deaktivieren** (unter \\Benutzerkonfiguration\\  
Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung), wird die Registerkarte **Sicherheit** aus der Benutzeroberfläche entfernt, und die Einstellung **Deaktivieren** erhält Vorrang vor dieser **Sicherheitszonen** -Einstellung.
  
**Sicherheitszonen: Benutzer können keine Einstellungen ändern**  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Schaltfläche **Stufe anpassen** und der Schieberegler **Sicherheitsstufe dieser Zone** auf der Registerkarte **Sicherheit** im Dialogfeld **Internetoptionen** deaktiviert. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können Benutzer die Einstellungen für Sicherheitszonen ändern. Dadurch wird verhindert, dass die Benutzer die vom Administrator vorgegebenen Einstellungen der Sicherheitszonenrichtlinie ändern.
  
Die Einstellung **Sicherheitszonen: Benutzer können Einstellungen nicht ändern** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Wenn Sie die Einstellung **Sicherheitsseite deaktivieren** (unter \\Benutzerkonfiguration\\  
Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung), wird die Registerkarte **Sicherheit** aus Internet Explorer in der Systemsteuerung entfernt, und die Einstellung **Deaktivieren** erhält Vorrang vor dieser **Sicherheitszonen**-Einstellung.
  
**Sicherheitszonen: Nur Computereinstellungen verwenden**  
Durch diese Richtlinieneinstellung wird festgelegt, wie sich Änderungen der Sicherheitszonen auf verschiedene Benutzer auswirken. Dadurch soll sichergestellt werden, dass die Sicherheitszoneneinstellungen auf dem gleichen Computer einheitlich bleiben und sich nicht von Benutzer zu Benutzer ändern. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Änderungen, die der Benutzer an einer Sicherheitszone vornimmt, auf alle Benutzer des betreffenden Computers angewendet. Wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert ist, können die Benutzer eines Computers ihre eigenen Sicherheitszoneneinstellungen festlegen.
  
Die Einstellung **Sicherheitszonen: Nur Computereinstellungen verwenden** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Systemabsturzermittlung deaktivieren**  
Mit dieser Richtlinieneinstellung können Sie die Absturzerkennung in der Add-On-Verwaltung in Internet Explorer verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, hat ein Absturz in Internet Explorer ähnliche Auswirkungen wie ein Absturz auf einem Computer, auf dem Windows XP Professional Service Pack 1 oder eine frühere Version ausgeführt wird: Die Windows-Fehlerberichterstattung wird aufgerufen. Wenn Sie diese Richtlinieneinstellung deaktivieren, ist die Absturzerkennung in der Add-On-Verwaltung aktiviert.
  
Da der Absturzbericht von Internet Explorer vertrauliche Informationen aus dem Speicher des Computers enthalten kann, ist die Einstellung **Absturzerkennung deaktivieren** für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt. Wenn es häufig zu wiederholten Abstürzen kommt, über die Sie für die nachfolgende Problembehandlung Bericht erstatten müssen, können Sie die Richtlinieneinstellung vorübergehend auf **Deaktiviert** setzen.
  
In **Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer** können zusätzlich folgende Einstellungen konfiguriert werden:
  
-   [Internetsystemsteuerung\\Seite „Erweitert“](#_internet_explorer-internet_control)
  
-   [Sicherheitsfunktionen\\MK-Protokoll-Sicherheitsbeschränkung](#_internet_explorer-security_features)
  
-   [Sicherheitsfunktionen\\Konsistente MIME-Verarbeitung](#_security_features-consistent_mime)
  
-   [Sicherheitsfunktionen\\Sicherheitsfunktion für MIME-Sniffing](#_security_features-mime_sniffing)
  
-   [Sicherheitsfunktionen\\Sicherheitseinschränkungen für Skriptfenster](#_security_features-scripted_window)
  
-   [Sicherheitsfunktionen\\Schutz vor Zonenerhöhung](#_security_features-protection_from)
  
-   [Sicherheitsfunktionen\\ActiveX-Installation einschränken](#_security_features-restrict_activex)
  
-   [Sicherheitsfunktionen\\Dateidownload einschränken](#_security_features-restrict_file)
  
-   [Sicherheitsfunktionen\\Add-On-Verwaltung](#_security_features-add-on_management)
  
-   [Einstellung der Add-On-Liste von Internet Explorer](#_internet_explorer_add-on)
  
Die Standardwerte für diese Einstellungen bieten im Vergleich zu früheren Windows-Versionen eine höhere Sicherheit. Sie haben die Möglichkeit, diese Einstellungen zu überprüfen und zu entscheiden, ob Sie sie in Ihrer Umgebung benötigen oder aus Gründen der Benutzerfreundlichkeit oder Anwendungskompatibilität lockern möchten.
  
Beispielsweise können Sie Internet Explorer so konfigurieren, dass Popups standardmäßig für alle Internetzonen blockiert werden. Möglicherweise möchten Sie sicherstellen, dass diese Einstellung auf allen Computern in Ihrer Umgebung durchgesetzt wird, um störende Popupfenster weitgehend zu blockieren und die Möglichkeit der Installation schädlicher Software und Spyware durch Websites zu verringern. Ihre Umgebung könnte aber auch Anwendungen enthalten, bei denen Popupfenster für eine ordnungsgemäße Funktion erforderlich sind. In diesem Fall können Sie diese Richtlinie so konfigurieren, dass Popups für Websites innerhalb Ihres Intranets zugelassen werden.
  
###### Internet Explorer\\Internetsystemsteuerung\\Seite „Erweitert“
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung\\Seite „Erweitert“**
  
**Tabelle A45. Empfohlene Einstellungen für die Seite „Erweitert“**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist**  
Microsoft ActiveX®-Steuerelemente und Dateidownloads verfügen häufig über digitale Signaturen, die ein relativ sicherer Nachweis für die Integrität der Datei und die Identität des Signaturgebers (Erstellers) der Software sind. Solche Signaturen helfen sicherzustellen, dass unmodifizierte Software heruntergeladen wird, und dass Sie aktive Signaturgeber erkennen können. Sie können dann entscheiden, ob Sie dem Signaturgeber genügend vertrauen, um seine Software auszuführen.
  
Durch die Einstellung **Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist** wird festgelegt, ob heruntergeladene Software durch Benutzer installiert oder ausgeführt werden kann, selbst wenn die Signatur ungültig ist. Eine ungültige Signatur kann darauf hinweisen, dass die Datei manipuliert wurde. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer zu einer Bestätigung aufgefordert, dass sie Dateien mit einer ungültigen Signatur installieren oder ausführen möchten. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer keine Dateien mit einer ungültigen Signatur installieren oder ausführen.
  
Da nicht signierte Software eine Sicherheitsanfälligkeit verursachen kann, ist diese Richtlinieneinstellung für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Hinweis:**   Einige zugelassene Softwareprogramme und Steuerelemente können eine ungültige Signatur haben und dennoch in Ordnung sein. Solche Software sollte sorgfältig in einer isolierten Umgebung geprüft werden, bevor Sie deren Verwendung im Netzwerk Ihrer Organisation zulassen.
  
###### Internet Explorer\\Sicherheitsfunktionen\\MK-Protokoll-Sicherheitsbeschränkung
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Sicherheitsfunktionen\\MK-Protokoll-Sicherheitsbeschränkung**
  
**Tabelle A46: Empfohlene Einstellungen für das MK-Protokoll**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Internet Explorer-Prozesse (MK-Protokoll)**  
Durch diese Richtlinieneinstellung wird die Angriffsfläche verringert, weil das selten verwendete MK-Protokoll blockiert wird. Einige ältere Webanwendungen rufen mithilfe des MK-Protokolls Informationen aus komprimierten Dateien ab. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, wird das MK-Protokoll für Windows Explorer und Internet Explorer blockiert. Ressourcen, die das MK-Protokoll verwenden, können dann nicht ausgeführt werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Anwendungen die MK-Protokoll-API verwenden.
  
Da das MK-Protokoll nicht sehr weit verbreitet ist, sollte es überall, wo es nicht gebraucht wird, blockiert werden. Für die beiden in diesem Handbuch behandelten Umgebungen ist diese Richtlinieneinstellung auf **Aktiviert** gesetzt. Microsoft empfiehlt, das MK-Protokoll zu blockieren, sofern es nicht wirklich in Ihrer Umgebung benötigt wird.
  
**Hinweis:**   Wenn Sie diese Einstellung vornehmen, können Ressourcen, die das MK-Protokoll verwenden, nicht ausgeführt werden. Daher sollten Sie sicherstellen, dass keine Ihrer Anwendungen das MK-Protokoll verwendet.
  
###### Internet Explorer\\Sicherheitsfunktionen\\Konsistente MIME-Verarbeitung
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Sicherheitsfunktionen\\Konsistente MIME-Verarbeitung**
  
**Tabelle A47: Empfohlene Einstellungen für die konsistente MIME-Verarbeitung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Internet Explorer-Prozesse (Konsistente MIME-Verarbeitung)**  
Internet Explorer verwendet MIME-Daten (Multipurpose Internet Mail Extensions), um Vorgehensweisen für die Verarbeitung von Dateien zu ermitteln, die über einen Webserver empfangen werden. Durch die Einstellung **Konsistente Mime-Verarbeitung** wird festgelegt, ob Internet Explorer erfordert, dass alle von Webservern bereitgestellten Dateitypinformationen konsistent sind. Weist eine Datei beispielsweise den MIME-Typ „text/plain“ auf, doch die MIME-Daten signalisieren, dass die Datei eigentlich eine ausführbare Datei ist, ändert Internet Explorer ihre Erweiterung entsprechend. Durch diese Möglichkeit wird sichergestellt, dass sich ausführbarer Code nicht als anderer, vertrauenswürdiger Datentyp ausgeben kann.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, untersucht Internet Explorer alle empfangenen Dateien und setzt eine konsistente MIME-Verarbeitung durch. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, erfordert Internet Explorer für keine der empfangenen Dateien konsistente MIME-Daten und verwendet die von der Datei bereitgestellten MIME-Daten.
  
Die Nachahmung von MIME-Dateitypen stellt eine potenzielle Bedrohung für Ihre Organisation dar. Sie sollten sicherstellen, dass diese Dateien konsistent und korrekt bezeichnet sind, um zu verhindern, dass schädliche Dateidownloads Ihr Netzwerk infizieren. Für die beiden in diesem Handbuch behandelten Umgebungen ist diese Richtlinieneinstellung auf **Aktiviert** gesetzt.
  
**Hinweis:**   Diese Richtlinieneinstellung steht mit den Einstellungen für **Sicherheitsfunktion für MIME-Sniffing** in Verbindung, ohne diese jedoch zu ersetzen.
  
###### Internet Explorer\\Sicherheitsfunktionen\\Sicherheitsfunktion für MIME-Sniffing
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Sicherheitsfunktionen\\Sicherheitsfunktion für MIME-Sniffing**
  
**Tabelle A48: Empfohlene Einstellungen für MIME-Sniffing**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Internet Explorer-Prozesse (MIME-Sniffing)**  
Beim MIME-Sniffing wird der Inhalt einer MIME-Datei untersucht, um deren Kontext zu ermitteln, also ob es sich um eine Datendatei, eine ausführbare Datei oder eine andere Art von Datei handelt. Durch diese Richtlinieneinstellung wird festgelegt, ob MIME-Sniffing in Internet Explorer verhindert, dass eine Datei eines Typs zu einem gefährlicheren Dateityp heraufgestuft wird. Wenn diese Richtlinieneinstellung auf **Aktiviert** gesetzt ist, wird durch MIME-Sniffing keine Heraufstufung einer Datei eines bestimmten Typs zu einem gefährlicheren Dateityp durchgeführt. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Internet Explorer-Prozesse so konfiguriert, dass sie MIME-Sniffing zulassen, durch das eine Datei eines bestimmten Typs zu einem gefährlicheren Dateityp heraufgestuft wird. Eine Textdatei kann z. B. zu einer ausführbaren Datei heraufgestuft werden. Dies ist gefährlich, da sämtlicher Code in der vermeintlichen Textdatei ausgeführt werden würde.
  
Die Nachahmung von MIME-Dateitypen stellt eine potenzielle Bedrohung für Ihre Organisation dar. Microsoft empfiehlt, diese Dateien konsistent zu behandeln. Dadurch wird verhindert, dass schädliche Dateidownloads Ihr Netzwerk infizieren.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (MIME-Sniffing)** auf **Aktiviert** gesetzt.
  
**Hinweis:**   Diese Richtlinieneinstellung steht mit den Einstellungen für **Konsistente MIME-Verarbeitung** in Verbindung, ohne diese jedoch zu ersetzen.
  
###### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Sicherheitseinschränkungen für Skriptfenster
  
Die empfohlene System-Computereinstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Sicherheitseinschränkungen für Skriptfenster**
  
**Tabelle A49: Empfohlene Sicherheitsbeschränkungen für Skriptfenster**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Sicherheitseinschränkungen für Skriptfenster)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Internet Explorer-Prozesse (Sicherheitseinschränkungen für Skriptfenster)**  
Internet Explorer ermöglicht Skripts, verschiedene Arten von Fenstern per Programm zu öffnen, in der Größe anzupassen und neu zu positionieren. Oftmals passen Websites von zweifelhaftem Ruf die Größe von Fenstern an, um andere Fenster zu verbergen oder um Sie zur Interaktion mit einem Fenster zu veranlassen, das schädlichen Code enthält.
  
Durch die Einstellung **Internet Explorer-Prozesse** **(Sicherheitseinschränkungen für Skriptfenster)** werden Popupfenster eingeschränkt, und es wird verhindert, dass Skripts Fenster anzeigen, deren Titel- und Statusleisten für den Benutzer nicht sichtbar sind oder die die Titel- und Statusleisten anderer Fenster ausblenden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden in Windows  Explorer- und Internet Explorer-Prozessen keine Popupfenster angezeigt. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, können Skripts weiterhin Popupfenster sowie Fenster, die andere Fenster verbergen, erstellen.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse** **(Sicherheitseinschränkungen für Skriptfenster)** auf **Aktiviert** gesetzt. Wenn diese Richtlinieneinstellung aktiviert ist, wird es schädlichen Websites erschwert, Ihre Internet Explorer-Fenster zu steuern oder Benutzer dazu zu verleiten, in das falsche Fenster zu klicken.
  
###### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Schutz vor Zonenerhöhung
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Schutz vor Zonenerhöhung**
  
**Tabelle A50: Empfohlene Einstellungen für den Schutz vor Zonenerhöhungen**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Internet Explorer-Prozesse (Zonenerhöhungsschutz)**  
Internet Explorer versieht jede Webseite, die geöffnet wird, mit Einschränkungen. Diese Einschränkungen hängen vom Standort der Webseite ab, z. B. Internetzone, Intranetzone oder Zone des lokalen Computers. Webseiten auf einem lokalen Computer haben die wenigsten Sicherheitsbeschränkungen und befinden sich in der Zone des lokalen Computers. Dadurch wird diese Zone zum vorrangigen Ziel für Angreifer.
  
Wenn Sie die Einstellung **Internet Explorer-Prozesse (Zonenerhöhungsschutz)** aktivieren, kann jede Zone vor einer Zonenanhebung durch Internet Explorer-Prozesse geschützt werden. Durch diese Vorgehensweise wird weitgehend verhindert, dass in einer Zone ausgeführter Inhalt die erhöhten Berechtigungen einer anderen Zone erlangt. Wenn Sie diese Richtlinieneinstellung ändern, erhält keine Zone einen solchen Schutz für Internet Explorer-Prozesse.
  
Aufgrund des Schweregrads und der relativen Häufigkeit von Zonenerhöhungsangriffen ist die Einstellung **Internet Explorer-Prozesse (Zonenerhöhungsschutz)** für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
###### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\ActiveX-Installation einschränken
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\ActiveX-Installation einschränken**
  
**Tabelle A51: Einstellungen für das Einschränken der Installation von ActiveX**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (ActiveX-Installation einschränken)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Internet Explorer-Prozesse (ActiveX-Installation einschränken)**  
Diese Richtlinieneinstellung bietet die Möglichkeit, Installationsaufforderungen von ActiveX-Steuerelementen für Internet Explorer-Prozesse zu blockieren. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Aufforderungen zum Installieren von ActiveX-Steuerelementen für Internet Explorer-Prozesse blockiert. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Aufforderungen zum Installieren von ActiveX-Steuerelementen für Internet Explorer-Prozesse nicht blockiert, sondern den Benutzern angezeigt.
  
Benutzer installieren häufig Software wie z. B. ActiveX-Steuerelemente, die von den Sicherheitsrichtlinien ihrer Organisation nicht zugelassen sind. Solche Software kann für Netzwerke ein beträchtliches Sicherheits- und Datenschutzrisiko darstellen. Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (ActiveX-Installation einschränken)** deshalb auf **Aktiviert** gesetzt.
  
**Hinweis:**   Durch diese Einstellung werden Benutzer außerdem daran gehindert, autorisierte, legitime ActiveX-Steuerelemente zu installieren, wodurch wiederum wichtige Systemkomponenten wie Windows Update behindert werden. Wenn Sie diese Richtlinieneinstellung aktivieren, stellen Sie sicher, dass Sicherheitsupdates (z. B. WSUS, Windows Server Update Services) auf andere Weise bereitgestellt werden können. Weitere Informationen über WSUS finden Sie auf der [Windows Server Update Services-Produkthomepage](http://www.microsoft.com/germany/windowsserver2003/technologien/updateservices/default.mspx).
  
###### Internet Explorer\\Sicherheitsfunktionen\\Dateidownload einschränken
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Sicherheitsfunktionen\\Dateidownload einschränken**
  
**Tabelle A52: Empfohlene Einstellungen für das Einschränken von Dateidownloads**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internet Explorer-Prozesse (Dateidownload einschränken)</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Internet Explorer-Prozesse (Dateidownload einschränken)**  
Unter bestimmten Umständen können Websites ohne Benutzereingriff Aufforderungen zum Herunterladen von Dateien einleiten. Dieses Verfahren kann es Websites ermöglichen, nicht autorisierte Dateien auf den Festplatten von Benutzern zu speichern, wenn sie auf die falsche Schaltfläche klicken und das Herunterladen akzeptieren.
  
Wenn Sie die Richtlinieneinstellung **Internet Explorer-Prozesse (Dateidownload einschränken)** auf **Aktiviert** setzen, werden nicht vom Benutzer initiierte Aufforderungen zum Herunterladen von Dateien für Internet Explorer-Prozesse blockiert. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** setzen, können ohne Zustimmung des Benutzers Dateidownloads für Internet Explorer-Prozesse initiiert werden.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Internet Explorer-Prozesse (Dateidownload einschränken)** auf **Aktiviert** gesetzt, um Angreifer davon abzuhalten, beliebigen Code auf den Computern von Benutzern abzulegen.
  
###### Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung
  
Diese empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internet Explorer\\Sicherheitsfunktionen\\Add-On-Verwaltung**
  
**Tabelle A53: Einstellungen für die Add-On-Verwaltung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind**  
Diese Richtlinieneinstellung ermöglicht Ihnen zusammen mit der Richtlinie **Add-On-Liste**, Internet Explorer-Add-Ons zu steuern. Mit der Einstellung **Add-On-Liste** wird standardmäßig eine Liste der Add-Ons definiert, die über Gruppenrichtlinien zugelassen oder gesperrt werden. Die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** gewährleistet, dass alle Add-Ons von vornherein gesperrt werden, wenn sie nicht eigens in der **Add-On-Liste** aufgeführt sind.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, lässt Internet Explorer nur Add-Ons zu, die explizit in der Richtlinieneinstellung **Add-On-Liste** aufgeführt und zugelassen sind. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer über die Add-On-Verwaltung beliebige Add-Ons zulassen oder verweigern.
  
Sie sollten erwägen, sowohl **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** als auch die **Add-On-Liste** zu verwenden, um zu steuern, welche Add-Ons in Ihrer Umgebung verwendet werden können. Dieser Ansatz sorgt dafür, dass nur autorisierte Add-Ons verwendet werden.
  
**Add-On-Liste**  
Mit dieser Richtlinieneinstellung und der Richtlinie **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** können Sie Internet Explorer-Add-Ons steuern. Mit der Einstellung **Add-On-Liste** wird standardmäßig eine Liste der Add-Ons definiert, die über Gruppenrichtlinien zugelassen oder gesperrt werden. Die Einstellung **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** gewährleistet, dass alle Add-Ons von vornherein gesperrt werden, wenn sie nicht eigens in der **Add-On-Liste** aufgeführt sind.
  
Wenn Sie die Einstellung **Add-On-Liste** aktivieren, müssen Sie eine Liste von Add-Ons eingeben, die von Internet Explorer zugelassen oder verweigert werden sollen. Da die spezifische Liste der Add-Ons, die in dieser Liste enthalten sein sollten, je nach Organisation unterschiedlich ist, wird in diesem Handbuch keine ausführliche Liste bereitgestellt. Für jeden Eintrag, den Sie der Liste hinzufügen, müssen Sie folgende Informationen bereitstellen:
  
-   **Name des Wertes**. Die CLSID (Klassen-ID) für das Add-On, das der Liste hinzugefügt werden soll. Die CLSID sollte in Klammern stehen, z. B. {000000000-0000-0000-0000-0000000000000}. Die CLSID für ein Add-On lässt sich aus dem OBJECT-Tag einer Webseite ablesen, auf der auf das Add-On verwiesen wird.
  
-   **Wert**. Eine Zahl, die anzeigt, ob Internet Explorer das Laden des Add-Ons verweigern oder zulassen soll. Folgende Werte sind gültig:
  
    -   **0** Dieses Add-On verweigern
  
    -   **1** Dieses Add-On zulassen
  
    -   **2** Dieses Add-On zulassen und dem Benutzer erlauben, es mithilfe des Befehls „Add-Ons verwalten“ zu verwalten
  
Wenn Sie die Einstellung **Add-On-Liste** deaktivieren, wird die Liste gelöscht. Sie sollten erwägen, sowohl **Alle Add-Ons sperren, soweit diese nicht explizit in der Add-On-Liste aufgeführt sind** als auch die **Add-On-Liste** zu verwenden, um zu steuern, welche Add-Ons in Ihrer Umgebung verwendet werden können. Dieser Ansatz sorgt dafür, dass nur autorisierte Add-Ons verwendet werden.
  
###### NetMeeting
  
Mit Microsoft NetMeeting® können über das Netzwerk Ihrer Organisation virtuelle Besprechungen durchgeführt werden. Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**NetMeeting**
  
**Tabelle A54: Empfohlene NetMeeting-Einstellungen**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Remotedesktop-Freigabe deaktivieren**  
Durch diese Richtlinieneinstellung wird die Remotedesktop-Freigabe von NetMeeting deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer NetMeeting nicht konfigurieren, um eine Remotesteuerung des lokalen Desktops zuzulassen.
  
Die Einstellung **Remotedesktop-Freigabe deaktivieren** ist für die Unternehmensclient-Umgebung **Nicht konfiguriert**. Für die Hochsicherheitsumgebung ist sie jedoch auf **Aktiviert** gesetzt, um Benutzer von der Remotedesktop-Freigabe über NetMeeting abzuhalten.
  
###### Terminaldienste
  
Durch die Terminaldienste werden Optionen für die Umleitung von Clientressourcen auf Servern bereitgestellt, auf die über die Terminaldienste zugegriffen wird. In diesem Abschnitt finden Sie Einstellungen für Folgendes:
  
-   Remotedesktopverbindungsclient
  
-   Terminalserver\\Verbindungen
  
-   Terminaldienste\\Geräte- und Ressourcenumleitung
  
-   Terminalserver\\Sicherheit
  
Terminaldienste\\Remotedesktopverbindungsclient  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Administrative Vorlagen\\Windows-Komponenten\\Terminaldienste**  
**\\Remotedesktopverbindungsclient**
  
**Tabelle A55: Empfohlene Einstellung für „Speichern von Kennwörtern nicht zulassen“**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Speichern von Kennwörtern nicht zulassen**  
Diese Richtlinieneinstellung hilft zu verhindern, dass Terminaldienstclients Kennwörter auf einem Computer speichern. Wenn Sie diese Richtlinieneinstellung aktivieren, wird das Kontrollkästchen zum Speichern von Kennwörtern in Terminaldienstclients deaktiviert. Benutzer sind dann nicht mehr in der Lage, Kennwörter zu speichern.
  
Da gespeicherte Kennwörter zusätzliche Gefährdungen verursachen können, ist die Einstellung **Speichern von Kennwörtern nicht zulassen** für die beiden in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Wenn diese Einstellung zuvor auf **Deaktiviert** bzw. **Nicht konfiguriert** gesetzt war, werden alle zuvor gespeicherten Kennwörter gelöscht, wenn ein Terminaldienstclient zum ersten Mal die Verbindung mit einem beliebigen Server beendet.
  
Terminaldienste\\Terminalserver\\Verbindungen  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Terminaldienste\\Terminalserver\\Verbindungen**
  
**Tabelle A56. Empfohlene Verbindungseinstellung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Remoteverbindungen für Benutzer mit Hilfe der Terminaldienste zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Remoteverbindungen für Benutzer mit Hilfe der Terminaldienste zulassen**  
Mit dieser Richtlinieneinstellung können Sie steuern, ob Benutzer über Terminaldienste oder Remotedesktop eine Verbindung zu einem Computer herstellen können.
  
In der SSLF-Umgebung müssen sich die Benutzer direkt an der physischen Computerkonsole anmelden. Deshalb ist die Einstellung **Remoteverbindungen für Benutzer mit Hilfe der Terminaldienste zulassen** für die SSLF-Umgebung auf **Deaktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung jedoch auf **Nicht konfiguriert** gesetzt.
  
Terminaldienste\\Terminalserver\\Geräte- und Ressourcenumleitung  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Terminaldienste\\Terminalserver\\Geräte- und Ressourcenumleitung**
  
**Tabelle A57: Empfohlene Einstellung für die Geräte- und Ressourcenumleitung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Laufwerkumleitung nicht zulassen**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die lokalen Laufwerke auf ihren Clientcomputern für Terminalserver freigeben, auf die sie Zugriff haben. Zugeordnete Laufwerke werden in der Sitzungsordnerstruktur von Windows Explorer im folgenden Format angezeigt:
  
\\\\TSClient\\*&lt;Laufwerkbuchstabe&gt;*$
  
Wenn lokale Laufwerke freigegeben werden, besteht die Möglichkeit, dass sich Eindringlinge unerlaubt Zugang zu den Daten auf diesen Laufwerken verschaffen. Aus diesem Grund ist die Einstellung **Laufwerkumleitung nicht zulassen** in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung ist diese Richtlinieneinstellung jedoch auf **Nicht konfiguriert** gesetzt.
  
Terminaldienste\\Terminalserver\\Sicherheit  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen**  
**\\Windows-Komponenten\\Terminaldienste\\Terminalserver\\Sicherheit**
  
**Tabelle A58. Empfohlene Terminalserver-Sicherheitseinstellungen**

 
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
<th>EC-Desktop</th>
<th>EC-<br />
Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Clients bei der Verbindungsherstellung immer zur Kennworteingabe auffordern</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verschlüsselungsstufe der Clientverbindung festlegen</td>
<td style="border:1px solid black;">Aktiviert:Höchste Stufe</td>
<td style="border:1px solid black;">Aktiviert:Höchste Stufe</td>
<td style="border:1px solid black;">Aktiviert:Höchste Stufe</td>
<td style="border:1px solid black;">Aktiviert:Höchste Stufe</td>
</tr>
</tbody>
</table>
  
**Clients bei der Verbindungsherstellung immer zur Kennworteingabe auffordern**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Clientcomputer von Terminaldiensten beim Herstellen der Verbindung stets zur Eingabe eines Kennworts aufgefordert wird. Mithilfe dieser Richtlinieneinstellung können sie für Benutzer, die sich bei Terminaldiensten anmelden, eine Aufforderung zur Kennworteingabe erzwingen, auch wenn die Benutzer das Kennwort bereits im Remotedesktopverbindungsclient eingegeben haben. Die Terminaldienste gestatten den Benutzern standardmäßig die automatische Anmeldung, wenn diese ihr Kennwort im Remotedesktopverbindungsclient eingeben.
  
Die Einstellung **Clients bei der Verbindungsherstellung immer zur Kennworteingabe auffordern** ist für beide in diesem Handbuch behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis:**   Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, kann der lokale Computeradministrator mit dem Terminaldienste-Konfigurationsprogramm festlegen, ob Kennwörter automatisch gesendet werden dürfen oder nicht.
  
**Verschlüsselungsstufe der Clientverbindung festlegen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Computer, der die Remoteverbindung soll, für alle zwischen dem Client und dem Remotecomputer gesendeten Daten eine Verschlüsselungsstufe erzwingt.
  
Die Verschlüsselungsstufe ist auf **Höchste Stufe** gesetzt, um für die beiden in diesem Handbuch behandelten Umgebungen eine 128-Bit-Verschlüsselung zu erzwingen.
  
###### Windows Messenger
  
Mit Windows Messenger können Sie Sofortnachrichten an andere Benutzer eines Computernetzwerks versenden. Den Nachrichten können Dateien und andere Anhänge beigefügt sein.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen**  
**\\Windows-Komponenten\\Windows Messenger**
  
**Tabelle A59: Empfohlene Windows Messenger-Einstellung**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
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
  
**Ausführung von Windows Messenger nicht zulassen**  
Sie können die Einstellung **Ausführung von Windows Messenger nicht zulassen** aktivieren, um Windows Messenger zu deaktivieren und zu verhindern, dass das Programm ausgeführt wird. Da diese Anwendung für böswillige Absichten wie z. B. das Versenden von Spam, die Verbreitung schädlicher Software und die Offenlegung vertraulicher Daten verwendet werden kann, empfiehlt Microsoft, die Einstellung **Ausführung von Windows Messenger nicht zulassen** sowohl für die Unternehmensclient- als auch für die Hochsicherheitsumgebung auf **Aktiviert** zu setzen.
  
**Hinweis:**   Diese Einstellung gilt nur für die in Windows XP enthaltene Windows Messenger-Software. Sie hindert die Benutzer nicht am Ausführen von MSN® Messenger oder Windows Live™ Messenger.
  
###### Windows Update
  
Administratoren können über die Einstellungen von Windows Update festlegen, wie Updates und Hotfixes auf Windows Vista-basierten Arbeitsstationen angewendet werden. Updates sind über Windows Update erhältlich. Sie können aber auch eine Intranet-Website einrichten, über die die Updates und Hotfixes in ähnlicher Weise, jedoch unter zusätzlicher Kontrolle des Administrators verteilt werden.
  
Windows Server Update Services (WSUS) ist ein Dienst der Infrastruktur, der auf den erfolgreichen Technologien von Microsoft Windows Update und Software Update Services (SUS) aufbaut. WSUS verwaltet und verteilt wichtige Windows-Updates zur Behebung bekannter Sicherheitsanfälligkeiten und anderer Stabilitätsprobleme in Windows-Betriebssystemen.
  
WSUS macht manuelle Aktualisierungsschritte unnötig. Ein dynamisches Benachrichtigungssystem informiert alle Windows-basierten Clientcomputer über wichtige Updates und stellt diese auf dem Intranetserver bereit. Die Clients müssen keine Internetverbindung aufbauen, um diesen Dienst nutzen zu können. Außerdem wird mit dieser Technologie eine einfache Lösung für die automatische Verteilung von Updates auf Ihren Windows-basierten Arbeitsstationen und -Servern bereitgestellt.
  
Darüber hinaus bietet WSUS folgende Funktionen:
  
-   **Verwaltung und Steuerung der Inhaltssynchronisierung innerhalb des Intranets durch den Administrator**. Dieser Synchronisierungsdienst ist eine serverseitige Komponente, die die jeweils neuesten wichtigen Updates von Windows Update abruft. Wenn neue Updates auf Windows Update gefunden werden, lädt der Server, der WSUS ausführt, diese nach einem vom Administrator definierten Zeitplan automatisch herunter und speichert sie.
  
-   **Verwaltung eines Windows Update-Servers innerhalb des Intranets**. Dieser leicht zu bedienende Server fungiert als virtueller Windows Update-Server für Clientcomputer. Er verfügt über einen Synchronisierungsdienst und über Programme für die Verwaltung der Updates. Er verarbeitet Anforderungen von genehmigten Updates, die von den Clientcomputern ausgegeben werden, die über das HTTP-Protokoll mit dem Server verbunden sind. Dieser Server kann auch wichtige Updates hosten, die vom Synchronisierungsdienst heruntergeladen wurden, und die Clientcomputer an diese Updates verweisen.
  
-   **Kontrolle der Updates durch den Administrator**. Der Administrator kann die über die öffentliche Website von Windows Update bereitgestellten Updates vor der Verteilung im Intranet der Organisation prüfen und genehmigen. Die Verteilung erfolgt nach einem vom Administrator erstellten Zeitplan. Wenn WSUS auf mehreren Servern ausgeführt wird, legt der Administrator fest, welche Computer auf bestimmte Server zugreifen, auf denen der Dienst ausgeführt wird. Administratoren können die genannten Verwaltungsmöglichkeiten über Gruppenrichtlinien in einer Active Directory-Umgebung oder über Registrierungsschlüssel konfigurieren.
  
-   **Automatische Updates auf den Computern (Arbeitsstationen oder Server)**. Die Windows-Funktion „Automatische Updates“ ermöglicht es, automatisch prüfen zu lassen, ob unter Windows Update neu veröffentlichte Updates verfügbar sind. WSUS verwendet diese Windows-Funktion für die Veröffentlichung aller vom Administrator genehmigten Updates in einem Intranet.
  
**Hinweis:**   Wenn Updates mit einer anderen Methode verteilt werden sollen, z. B. über Microsoft Systems Management Server, wird empfohlen, die Einstellung **Automatische Updates konfigurieren** zu deaktivieren.
  
Es gibt mehrere Einstellungen für Windows Update. Damit Windows Update funktioniert, sind mindestens drei Einstellungen erforderlich: **Automatische Updates konfigurieren**, **Kein automatischer Neustart für geplante Installationen automatischer Updates** und **Geplante Installationen automatischer Updates erneut planen**. Eine vierte Einstellung ist optional und hängt von den Anforderungen Ihrer Organisation ab: **Internen Pfad für den Microsoft Updatedienst angeben**.
  
Die folgenden empfohlenen Computereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**\\Windows Update**
  
Die in diesem Abschnitt beschriebenen Einstellungen stehen nicht explizit in Zusammenhang mit bestimmten Sicherheitsrisiken. Sie dienen hauptsächlich einer Anpassung der Umgebung an die vom Administrator festgelegten Konfigurationsvorgaben. Ungeachtet dessen ist die Konfiguration von Windows Update unerlässlich, da zur Sicherheit der Umgebung nur dann beigetragen werden kann, wenn die Clientcomputer möglichst bald nach der Bereitstellung neuer Microsoft-Sicherheitsupdates entsprechend aktualisiert werden.
  
**Hinweis:**   Windows Update ist abhängig von mehreren Diensten, zu denen auch der Remoteregistrierungsdienst und der Intelligente Hintergrundübertragungsdienst gehören.
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Einstellungen für Windows Update. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A60: Empfohlene Einstellungen für Windows Update**

 
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
<th>EC-Desktop</th>
<th>EC-Laptop</th>
<th>SSLF-Desktop</th>
<th>SSLF-Laptop</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Option „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anzeigen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Die Standardoption „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anpassen</td>
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
</tbody>
</table>
  
**Option „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anzeigen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob im Dialogfeld **Windows herunterfahren** die Option **Updates installieren und herunterfahren** angezeigt wird. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird die Option **Updates installieren und herunterfahren** im Dialogfeld **Windows herunterfahren** verfügbar. Dies gilt für den Fall, dass Updates zur Verfügung stehen, wenn der Benutzer im Menü **Start** die Option **Herunterfahren** wählt.
  
Da Updates für die Gesamtsicherheit aller Computer wichtig sind, ist die Einstellung **Option „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anzeigen** für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt. Diese Einstellung steht mit der Einstellung **Die Standardoption „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anpassen** in Verbindung.
  
**Die Standardoption „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anpassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Option **Updates installieren und herunterfahren** als Standardauswahl im Dialogfeld **Windows herunterfahren** zugelassen wird. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird die Option **Updates installieren und herunterfahren** zur Standardoption im Dialogfeld **Windows herunterfahren**, wenn zu dem Zeitpunkt, zu dem der Benutzer im Menü **Start** die Option **Herunterfahren** auswählt, Updates zur Installation zur Verfügung stehen.
  
Da Updates für die Gesamtsicherheit aller Computer wichtig sind, ist die Einstellung **Die Standardoption „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anpassen** für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
**Hinweis:**   Diese Richtlinieneinstellung hat keine Auswirkungen, wenn die Option **Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Windows Update\\Option „Updates installieren und herunterfahren“ im Dialogfeld „Windows herunterfahren“ nicht anzeigen** auf **Aktiviert** gesetzt ist.
  
**Automatische Updates konfigurieren**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Computer in Ihrer Umgebung Sicherheitsupdates von Windows Update oder WSUS empfangen sollen. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, kann das Betriebssystem feststellen, wann eine Netzwerkverbindung verfügbar ist, und anschließend über diese Verbindung die Windows Update-Website oder die ausgewiesene Intranetsite auf relevante Updates überprüfen.
  
Wählen Sie, nachdem Sie diese Richtlinieneinstellung auf **Aktiviert** gesetzt haben, im Dialogfeld **Eigenschaften von Automatische Updates konfigurieren** eine der drei folgenden Optionen für die Funktionsweise des Dienstes aus:
  
-   **Vor dem Download von Updates benachrichtigen und vor deren Installation erneut benachrichtigen**.
  
-   **Updates automatisch downloaden und über installierbare Updates benachrichtigen**. **(Standardeinstellung)**
  
-   **Updates automatisch downloaden und laut angegebenem Zeitplan installieren**.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, müssen alle verfügbaren Updates von Windows Update manuell heruntergeladen und installiert werden.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Automatische Updates konfigurieren** auf **Aktiviert** gesetzt.
  
**Kein automatischer Neustart für geplante Installationen automatischer Updates**  
Wenn diese Richtlinieneinstellung aktiviert ist, muss der Computer von einem angemeldeten Benutzer neu gestartet werden, um eine geplante Installation abzuschließen. Durch Aktivierung dieser Richtlinieneinstellung wird auch verhindert, dass die Funktion „Automatische Updates“ den Computer während einer geplanten Installation automatisch neu startet. Wenn ein Benutzer zu der Zeit an einem Computer angemeldet ist, zu der „Automatische Updates“ einen Neustart erfordert, um die Installation eines Updates abzuschließen, wird der Benutzer darauf hingewiesen. Der Benutzer kann den Neustart dann verschieben. Beachten Sie, dass „Automatische Updates“ bis zum erforderlichen Neustart keine weiteren Updates erkennt.
  
Wenn die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Deaktiviert** oder **Nicht konfiguriert** gesetzt ist, benachrichtigt „Automatische Updates“ den Benutzer, dass der Computer für den Abschluss einer Installation in 5 Minuten automatisch neu gestartet wird. Wenn automatische Neustarts ein Problem darstellen, können Sie die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Aktiviert** setzen. Um den Abschluss durchgeführter Installationen sicherzustellen, richten Sie Ihre Clientcomputer so ein, dass sie nach Ende der normalen Geschäftszeiten automatisch neu gestartet werden, wenn Sie diese Richtlinieneinstellung aktivieren.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Kein automatischer Neustart für geplante Installationen automatischer Updates** auf **Deaktiviert** gesetzt.
  
**Hinweis:**   Diese Richtlinie funktioniert nur, wenn „Automatische Updates“ für die Durchführung von automatischen Updateinstallationen konfiguriert ist. Wenn die Einstellung **Automatische Updates konfigurieren** auf **Deaktiviert** gesetzt ist, hat sie keine Auswirkungen.
  
**Geplante Installationen automatischer Updates erneut planen**  
Durch diese Richtlinieneinstellung wird festgelegt, wie lange nach dem Systemstart gewartet wird, bevor geplante automatische Updateinstallationen fortgesetzt werden. Wenn Sie diese Richtlinieneinstellung auf **Aktiviert** setzen, wird eine zuvor geplante Installation nach Ablauf einer gewissen Zeit (in Minuten) nach dem Start des Computers durchgeführt. Wenn Sie diese Richtlinieneinstellung auf **Deaktiviert** oder **Nicht konfiguriert** setzen, werden zuvor geplante Installationen erst zum nächsten regulär geplanten Installationszeitpunkt durchgeführt.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Geplante Installationen automatischer Updates erneut planen** auf **Aktiviert** gesetzt. Nach dem Aktivieren der Richtlinieneinstellung können Sie die standardmäßige Wartezeit entsprechend den Anforderungen in der Umgebung ändern.
  
**Hinweis:**   Diese Richtlinie funktioniert nur, wenn „Automatische Updates“ für die Durchführung von automatischen Updateinstallationen konfiguriert ist. Wenn die Einstellung **Automatische Updates konfigurieren** auf **Deaktiviert** gesetzt ist, hat die Einstellung **Geplante Installationen automatischer Updates erneut planen** keine Auswirkungen. Sie können die beiden letztgenannten Einstellungen aktivieren, um sicherzustellen, dass zuvor übergangene Installationen bei jedem Neustart des Computers neu angesetzt werden.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Benutzerrichtlinien
  
In den übrigen Abschnitten dieser Anlage werden Empfehlungen für die Benutzerkonfiguration erörtert. Diese Einstellungen müssen auf Benutzer angewendet werden, nicht auf Computer. Sie sollten mit einer Gruppenrichtlinie implementiert werden, die mit der Organisationseinheit verknüpft ist, die die zu konfigurierenden Benutzer enthält. Wenden Sie diese Einstellungen mithilfe eines Gruppenrichtlinienobjekts an, das mit einer Organisationseinheit verknüpft ist, die die Benutzerkonten enthält.
  
**Hinweis:**   Benutzerkonfigurationseinstellungen werden auf jeden Windows Vista-basierten Computer angewendet, bei dem sich ein Benutzer in einer Active Directory-Domäne anmeldet. Computerkonfigurationseinstellungen gelten jedoch für alle Clientcomputer, die von einem Gruppenrichtlinienobjekt in Active Directory gesteuert werden, unabhängig davon, welcher Benutzer sich beim Computer anmeldet.
  
#### Benutzerkonfiguration\\Administrative Vorlagen
  
Die folgenden Einstellungsgruppen für die Benutzerrichtlinie enthalten Einstellungen, die in diesem Handbuch behandelt werden. Die Einstellungen werden im Unterknoten **Benutzerkonfiguration\\Administrative Vorlagen** des Gruppenrichtlinienobjekt-Editors angezeigt.
  
-   [System](#_internet_explorer_1)
  
    -   [Energieverwaltung](#_power_management)
  
-   [Windows-Komponenten](#_windows_components_3)
  
    -   [Anlagen-Manager](#_attachment_manager_1)
  
    -   [Internet Explorer](#_internet_explorer_3)
  
    -   [Windows Explorer](#_windows_explorer)
  
##### System
  
Die folgende empfohlene Einstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\System**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für den Registrierungs-Editor.
  
**Tabelle A61: Empfohlene Benutzerkonfigurationseinstellungen für „System“**

 
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
  
**Zugriff auf Programme zum Bearbeiten der Registrierung verhindern**  
Diese Richtlinieneinstellung deaktiviert die Windows-Registrierungseditoren Regedit.exe und Regedt32.exe. Wenn Sie diese Richtlinieneinstellung aktivieren und Benutzer versuchen, einen Registrierungseditor zu verwenden, wird ihnen in einer Meldung mitgeteilt, dass sie keinen der beiden Editoren verwenden können. Diese Richtlinieneinstellung sorgt dafür, dass Benutzer und Eindringlinge nicht mit diesen Tools auf die Registrierung zugreifen können, verhindert aber nicht den Zugriff auf die Registrierung selbst.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Zugriff auf Programme zum Bearbeiten der Registrierung verhindern** auf **Nicht konfiguriert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt.
  
###### Energieverwaltung
  
Die folgende empfohlene Einstellung kann im Gruppenrichtlinienobjekt-Editor in diesem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\System\\Energieverwaltung**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Konfigurationseinstellungen für **Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus**.
  
**Tabelle A62: Empfohlene Benutzerkonfigurationseinstellungen für „System\\Energieverwaltung“**

 
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
  
**Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Clientcomputer in Ihrer Umgebung gesperrt werden, wenn sie aus dem Ruhezustand oder Standbymodus zurückkehren. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Clientcomputer gesperrt, wenn sie in den Betriebsmodus zurückkehren. Benutzer müssen ihr Kennwort eingeben, um die Sperre aufzuheben. Es können potenziell schwerwiegende Sicherheitsverletzungen auftreten, wenn diese Richtlinieneinstellung deaktiviert oder nicht konfiguriert wird, da in diesem Fall jeder auf die Clientcomputer zugreifen kann.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Kennworteingabe bei der Wiederaufnahme aus dem Ruhezustand bzw. Standbymodus** deshalb auf **Aktiviert** gesetzt.
  
##### Windows-Komponenten
  
Die folgende empfohlene Einstellung kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für den Registrierungs-Editor.
  
###### Anlagen-Manager
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Anlagen-Manager**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für den Anlagen-Manager. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A63: Empfohlene Benutzerkonfigurationseinstellungen für den Anlagen-Manager**

 
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
<td style="border:1px solid black;">Zoneninformationen in Dateianlagen nicht beibehalten</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Mechanismus zum Entfernen von Zoneninformationen ausblenden</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Antivirenprogramme beim Öffnen von Anlagen benachrichtigen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Zoneninformationen in Dateianlagen nicht beibehalten**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Windows-Dateianlagen von Internet Explorer oder Microsoft Outlook® Express mit Informationen zu deren Ursprungszone (z. B. eingeschränkt, Internet, Intranet oder lokal) markiert werden. Für das richtige Funktionieren dieser Einstellung ist es erforderlich, dass Dateien auf NTFS-Festplattenpartitionen heruntergeladen werden. Wenn Zoneninformationen beibehalten werden, kann Windows keine ordnungsgemäßen Risikoanalysen anhand der Zone vornehmen, aus der die Anlage stammt.
  
Wenn die Einstellung **Zoneninformationen in Dateianlagen nicht beibehalten** aktiviert ist, werden Dateianlagen nicht mit ihren Zoneninformationen gekennzeichnet. Wenn diese Richtlinieneinstellung deaktiviert ist, ist Windows gezwungen, Dateianlagen mit ihren Zoneninformationen zu speichern. Da gefährliche Anlagen oft aus nicht vertrauenswürdigen Internet Explorer-Zonen wie etwa der Internetzone heruntergeladen werden, empfiehlt Microsoft, diese Einstellung auf **Deaktiviert** zu setzen. Dadurch wird weitgehend sichergestellt, dass zu jeder Datei so viele Sicherheitsinformationen wie möglich aufbewahrt werden.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Zoneninformationen in Dateianlagen nicht beibehalten** auf **Deaktiviert** gesetzt.
  
**Mechanismus zum Entfernen von Zoneninformationen ausblenden**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer manuell Zoneninformationen von gespeicherten Dateianlagen entfernen können. Normalerweise können Benutzer entweder auf der Seite **Eigenschaften** der Datei auf die Schaltfläche **Zulassen** klicken oder ein Kontrollkästchen im Dialogfeld **Sicherheitswarnung** aktivieren. Das Entfernen von Zoneninformationen ermöglicht es Benutzern, potenziell gefährliche Dateianlagen zu öffnen, obwohl Windows dies zuvor verhindert hat.
  
Wenn die Einstellung **Mechanismus zum Entfernen von Zoneninformationen ausblenden** aktiviert ist, blendet Windows das Kontrollkästchen und die Schaltfläche **Zulassen** aus. Wenn diese Richtlinieneinstellung deaktiviert ist, zeigt Windows das Kontrollkästchen und die Schaltfläche **Zulassen** an. Da gefährliche Anlagen oft aus nicht vertrauenswürdigen Internet Explorer-Zonen wie etwa der Internetzone heruntergeladen werden, empfiehlt Microsoft, diese Richtlinieneinstellung auf **Deaktiviert** zu setzen. Dadurch wird weitgehend sichergestellt, dass zu jeder Datei so viele Sicherheitsinformationen wie möglich aufbewahrt werden.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Mechanismus zum Entfernen von Zoneninformationen ausblenden** auf **Aktiviert** gesetzt.
  
**Hinweis:**   Informationen dazu, wie Sie festlegen können, ob Dateien mit Zoneninformationen gespeichert werden, finden Sie in den vorangegangenen Ausführungen zur Einstellung **Zoneninformationen in Dateianlagen nicht beibehalten**.
  
**Antivirenprogramme beim Öffnen von Anlagen benachrichtigen**  
Antivirenprogramme sind in vielen Umgebungen obligatorisch und stellen einen sehr guten Schutz vor aktuellen Angriffsmethoden dar.
  
Mit der Einstellung **Antivirusprogramme beim Öffnen von Anlagen benachrichtigen** können Sie festlegen, wie registrierte Antivirenprogramme benachrichtigt werden. Wenn diese Richtlinieneinstellung aktiviert ist, ruft Windows das registrierte Antivirenprogramm auf und überprüft Dateianlagen, wenn sie von Benutzern geöffnet werden. Wenn der Virenscan fehlschlägt, wird das Öffnen der Anlagen verhindert. Wenn diese Richtlinieneinstellung deaktiviert ist, ruft Windows das registrierte Antivirenprogramm nicht auf, wenn Dateianlagen geöffnet werden. Um sicherzustellen, dass Antivirenprogramme jede Datei vor dem Öffnen untersuchen, empfiehlt Microsoft, diese Richtlinie in allen Umgebungen auf **Aktiviert** zu setzen.
  
Für die beiden in diesem Handbuch behandelten Umgebungen ist die Einstellung **Beim Öffnen von Anhängen Antivirusprogramme benachrichtigen** auf **Aktiviert** gesetzt.
  
**Hinweis:**   Für das richtige Funktionieren dieser Einstellung muss ein aktualisiertes Antivirenprogramm installiert werden.
  
###### Internet Explorer
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**Internet Explorer**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A64: Empfohlene Benutzerkonfigurationseinstellungen für Internet Explorer**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Outlook Express konfigurieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Disable „Configuring History“ (Konfigurieren des Verlaufs deaktivieren)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:40</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">AutoVervollständigen für Formulare deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Änderung der Einstellungen für automatische Konfiguration deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Änderung der Zertifikateinstellungen deaktivieren</td>
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
<td style="border:1px solid black;">Aktivierung bzw. Deaktivierung von Add-Ons für Benutzer nicht zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Prevent „fix settings“ functionality (Funktionalität für „Einstellungen reparieren“ sperren)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Prevent deletion of „Temporary Internet Files and Cookies“ (Löschen temporärer Internetdateien und Cookies verhindern)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Turn off „Delete Browsing History“ functionality (Funktionalität für „Browserverlauf löschen“ deaktivieren)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">§ Turn off the Security Settings Check feature (Funktion zur Überprüfung der Sicherheitseinstellungen deaktivieren)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">AutoVervollständigen für Benutzernamen und Kennwörter in Formularen verwenden</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista.
  
**Outlook Express konfigurieren**  
Diese Richtlinieneinstellung ermöglicht es Administratoren, für Benutzer von Microsoft Outlook Express® festzulegen, ob sie Anlagen speichern oder öffnen können, die einen Virus enthalten könnten. Benutzer können die Einstellung **Outlook Express konfigurieren** nicht deaktivieren und damit die Sperrung von Anlagen nicht aufheben. Um diese Richtlinieneinstellung zu erzwingen, klicken Sie auf **Aktivieren**, und wählen Sie die Option **Anhänge sperren, die einen Virus enthalten können** aus.
  
Für die in diesem Handbuch behandelte Unternehmensclient-Umgebung ist die Einstellung **Outlook Express konfigurieren** auf die Werte **Aktiviert** und **Anhänge sperren, die einen Virus enthalten können** gesetzt.
  
**Disable „Configuring History“ (Konfigurieren des Verlaufs deaktivieren)**  
Diese Einstellung bestimmt, wie viele Tage Internet Explorer die besuchten Seiten in der Verlaufsliste aufführt. Die Option **Browserverlauf löschen** finden Sie auf der Registerkarte **Extras &gt; Internetoptionen &gt; Allgemein**. In Internet Explorer 7 steht sie außerdem als **Verlauf löschen** direkt unter **Extras &gt; Internetoptionen &gt; Browserverlauf löschen** zur Verfügung.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, kann ein Benutzer nicht festlegen, wie lange Internet Explorer die besuchten Seiten in der Verlaufsliste aufführt. Sie müssen festlegen, wie viele Tage Internet Explorer die besuchten Seiten in der Verlaufsliste aufführen soll. Die Benutzer können den Browserverlauf nicht löschen. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, kann ein Benutzer selbst bestimmen, wie viele Tage lang Internet Explorer die besuchten Seiten in der Verlaufsliste aufführt, und kann bei Bedarf den **Browserverlauf löschen**.
  
Die Einstellung **Disable „Configuring History“** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert:40** gesetzt.
  
**AutoVervollständigen für Formulare deaktivieren**  
Diese Richtlinieneinstellung steuert das automatische Ausfüllen von Feldern in Formularen auf Webseiten. Wenn Sie diese Richtlinieneinstellung aktivieren, macht die Funktion AutoVervollständigen keine Vorschläge für das Ausfüllen von Formularen. Dies ist in bestimmten Umgebungen ein zusätzlicher Schutz für vertrauliche Daten.
  
Die Einstellung **AutoVervollständigen für Formulare deaktivieren** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Änderung der Einstellungen für automatische Konfiguration deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer automatisch konfigurierte Einstellungen ändern können. Administratoren verwenden die automatische Konfiguration zur regelmäßigen Aktualisierung von Browsereinstellungen. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Einstellungen für die automatische Konfiguration in Internet Explorer abgeblendet. (Die Einstellungen befinden sich im Dialogfeld **Einstellungen für lokales Netzwerk (LAN)** im Bereich **Automatische Konfiguration**.) Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden.
  
**So zeigen Sie das Dialogfeld „Einstellungen für lokales Netzwerk (LAN)“ an**
  
1.  Öffnen Sie das Dialogfeld **Internetoptionen**, und klicken Sie auf die Registerkarte **Verbindungen**.
  
2.  Klicken Sie auf die Schaltfläche **Einstellungen**, um die Einstellungen anzuzeigen.
  
Die Einstellung **Änderung der Einstellungen für automatische Konfiguration deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Hinweis:**   Durch die Einstellung **Verbindungsseite deaktivieren** wird die Registerkarte **Verbindungen** aus Internet Explorer in der Systemsteuerung entfernt. Diese Einstellung hat Vorrang vor der Konfigurationsoption **Änderung der Einstellungen für automatische Konfiguration deaktivieren**. Wenn Sie erstere Einstellung aktivieren, wird die letztere Einstellung ignoriert. Die Einstellung **Verbindungsseite deaktivieren** befindet sich im Gruppenrichtlinienobjekt-Editor unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung.
  
**Änderung der Zertifikateinstellungen deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Zertifikatseinstellungen in Internet Explorer ändern können. Zertifikate dienen als Identitätsnachweis für Softwareherausgeber. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Einstellungen im Bereich **Zertifikate** auf der Registerkarte **Inhalte** des Dialogfelds **Internetoptionen** deaktiviert. Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden.
  
Die Einstellung **Änderung der Zertifikateinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Hinweis:**   Wenn diese Richtlinieneinstellung aktiviert ist, können Benutzer weiterhin auf die Datei für Zertifikate von Softwareherausgebern (.spc) doppelklicken, um den Assistenten zum Importieren der Zertifikatverwaltung auszuführen. Dieser Assistent bietet Benutzern die Möglichkeit, noch nicht in Internet Explorer konfigurierte Einstellungen für Zertifikate von Softwareherstellern zu importieren und zu konfigurieren.
  
**Hinweis:**   Durch die Einstellung **Inhaltsseite deaktivieren** wird die Registerkarte **Inhalt** aus Internet Explorer in der Systemsteuerung entfernt. Diese Einstellung hat Vorrang vor der Konfigurationsoption **Änderung der Zertifikateinstellungen deaktivieren**. Wenn Sie erstere Einstellung aktivieren, wird die letztere Einstellung ignoriert. Die Einstellung **Inhaltsseite deaktivieren** befindet sich im Gruppenrichtlinienobjekt-Editor unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung.
  
**Änderung der Verbindungseinstellungen deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer DFÜ-Einstellungen ändern können. Wenn Sie diese Richtlinieneinstellung aktivieren, wird die Schaltfläche **Einstellungen** auf der Registerkarte **Verbindungen** des Dialogfelds **Internetoptionen** deaktiviert. Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden. Diese Richtlinieneinstellung sollte eventuell für Laptopbenutzer deaktiviert werden, wenn diese unterwegs ihre Verbindungseinstellungen ändern müssen.
  
Die Einstellung **Änderung der Verbindungseinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Hinweis:**   Wenn Sie die Einstellung **Verbindungsseite deaktivieren** konfigurieren, müssen Sie diese Richtlinieneinstellung nicht konfigurieren. Durch die Einstellung **Verbindungsseite deaktivieren** wird die Registerkarte **Verbindungen** aus der Benutzeroberfläche entfernt. Die Einstellung **Verbindungsseite deaktivieren** befindet sich im Gruppenrichtlinienobjekt-Editor unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung.
  
**Änderung der Proxyeinstellungen deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Proxyeinstellungen ändern können. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Proxyeinstellungen abgeblendet. (Die Proxyeinstellungen befinden sich im Bereich **Proxyserver** des Dialogfelds **LAN-Einstellungen**, das dem Benutzer angezeigt wird, wenn er im Dialogfeld **Internetoptionen** auf die Registerkarte **Verbindungen** und dann auf die Schaltfläche **LAN-Einstellungen** klickt.) Durch diese Richtlinieneinstellung wird außerdem verhindert, dass Benutzer Einstellungen ändern können, die durch Gruppenrichtlinien definiert wurden. Diese Richtlinieneinstellung sollte eventuell für Laptopbenutzer deaktiviert werden, wenn diese unterwegs ihre Verbindungseinstellungen ändern müssen.
  
Die Einstellung **Änderung der Proxyeinstellungen deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Hinweis:**   Wenn Sie die Einstellung **Verbindungsseite deaktivieren** konfigurieren, müssen Sie diese Richtlinieneinstellung nicht konfigurieren. Durch die Einstellung **Verbindungsseite deaktivieren** wird die Registerkarte **Verbindungen** aus der Benutzeroberfläche entfernt. Diese Einstellung befindet sich im Gruppenrichtlinienobjekt-Editor unter \\Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer\\Internetsystemsteuerung.
  
**Aktivierung bzw. Deaktivierung von Add-Ons für Benutzer nicht zulassen**  
Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Möglichkeit haben, Add-Ons über **Add-Ons verwalten** zuzulassen oder zu verweigern. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer keine Add-Ons über **Add-Ons verwalten** aktivieren oder deaktivieren. Eine Ausnahme ist lediglich dann möglich, wenn ein Add-On speziell in der Richtlinieneinstellung **Add-On-Liste** so eingetragen wurde, dass Benutzer dieses Add-On weiterhin verwalten können. In diesem Fall kann der Benutzer das Add-On immer noch über **Add-Ons verwalten** verwalten.Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, stehen dem Benutzer die entsprechenden Steuerelemente unter **Add-Ons verwalten** zur Verfügung.
  
Die Einstellung **Aktivierung bzw. Deaktivierung von Add-Ons für Benutzer nicht zulassen** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Prevent „fix settings“ functionality (Funktionalität für „Einstellungen reparieren“ sperren)**  
Diese Richtlinieneinstellung verhindert, dass Benutzer die Funktionalität **Einstellungen reparieren** in Zusammenhang mit der Funktion zurÜberprüfung der Sicherheitseinstellungen in Internet Explorer ausführen. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer nicht auf die Option **Einstellungen reparieren** im Kontextmenü der Informationsleiste klicken, das angezeigt wird, wenn Internet Explorer erkennt, dass seine Konfiguration nicht sicher ist.
  
Die Einstellung **Prevent „fix settings“ functionality** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Prevent deletion of „Temporary Internet Files and Cookies“ (Löschen temporärer Internetdateien und Cookies verhindern)**  
Diese Richtlinieneinstellung dient zur Verwaltung temporärer Internetdateien und Cookies in Zusammenhang mit Ihrem Internetbrowserverlauf, in Internet Explorer 7, zu finden unter **Extras &gt; Internetoptionen &gt; Browserverlauf löschen**. Wenn Sie diese Richtlinieneinstellung aktivieren, können die Benutzer temporäre Internetdateien und Cookies nicht löschen. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, können Benutzer temporäre Internetdateien und Cookies löschen.
  
Die Einstellung **Prevent deletion of „Temporary Internet Files and Cookies“** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Turn off „Delete Browsing History“ functionality (Funktionalität für „Browserverlauf löschen“ deaktivieren)**  
Diese Richtlinieneinstellung verhindert, dass Benutzer die Funktion **Browserverlauf löschen** in Internet Explorer verwenden. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer die Funktion **Browserverlauf löschen** in den **Internetoptionen** von Internet Explorer 7 nicht verwenden. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, können Benutzer die Funktion **Browserverlauf löschen** in den **Internetoptionen** von Internet Explorer 7 verwenden.
  
Die Einstellung **Turn off „Delete Browsing History“ functionality** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Turn off the Security Settings Check feature (Funktion zur Überprüfung der Sicherheitseinstellungen deaktivieren)**  
Diese Richtlinieneinstellung deaktiviert die Funktion zurÜberprüfung der Sicherheitseinstellungen, mit der Internet Explorer-Sicherheitseinstellungen daraufhin geprüft werden, ob sie für Internet Explorer ein Risiko darstellen. Wenn Sie diese Richtlinieneinstellung aktivieren, wird keine Überprüfung der Sicherheitseinstellungen durchgeführt. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird eine Überprüfung der Sicherheitseinstellungen durchgeführt. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, kann der Benutzer die Einstellung für die Überprüfung derSicherheitseinstellungen ändern.
  
Die Einstellung **Turn off the Security Settings Check feature** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**AutoVervollständigen für Benutzernamen und Kennwörter in Formularen verwenden**  
Durch diese Richtlinieneinstellung wird das automatische Ausfüllen von Benutzernamen und Kennwörtern in Webseitenformularen und die Abfrage zur Kennwortspeicherung gesteuert. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Kontrollkästchen **Benutzernamen und Kennwörter für Formulare** und **Nachfragen, ob Kennwörter gespeichert werden sollen** abgeblendet. Außerdem werden die Benutzer daran gehindert, Kennwörter lokal zu speichern.
  
Die Einstellung **AutoVervollständigen für Benutzernamen und Kennwörter in Formularen verwenden** ist für die beiden in diesem Handbuch behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
In **Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\Internet Explorer** können zusätzlich folgende Einstellungsbereiche konfiguriert werden:
  
-   [Browser-Menüs](#_browser_menus)
  
-   [Internetsystemsteuerung](#_internet_control_panel)
  
-   [Internetsystemsteuerung\\Seite „Erweitert“](#_internet_control_panel-advanced)
  
-   [Internetsystemsteuerung\\Sicherheitsseite](#_internet_control_panel-security)
  
-   [Internetsystemsteuerung\\Sicherheitsseite\\Internetzone](#_security_page_internet_1)
  
-   [Internetsystemsteuerung\\Sicherheitsseite\\Zone eingeschränkter Sites](#_internet_control_pane-security)
  
-   [Offlineseiten](#_offline_pages)
  
###### Browser-Menüs
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Browsermenüs**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A65: Empfohlene Einstellungen für Browsermenüs**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Option „Das Programm speichern“ deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**Option „Das Programm speichern“ deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Programme oder Dateien speichern können, die Internet Explorer auf die Festplatte heruntergeladen hat. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer Programme nicht mit der Option **Das Programm speichern** auf der Festplatte speichern. Die Programmdatei wird nicht heruntergeladen, und der Benutzer wird darüber informiert, dass dieser Befehl nicht verfügbar ist. Diese Richtlinieneinstellung trägt zum Schutz von Hochsicherheitsumgebungen bei, da Benutzer keine möglicherweise schädlichen Programme über Internet Explorer herunterladen und auf der Festplatte speichern können.
  
Die Einstellung **Option „Das Programm speichern“ deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
###### Internetsystemsteuerung
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internetsystemsteuerung**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A66. Empfohlene Benutzerkonfigurationseinstellungen für die Internetsystemsteuerung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Seite „Erweitert“ deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Sicherheitsseite deaktivieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Prevent ignoring certificate errors (Ignorieren von Zertifikatfehlern verhindern)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista.
  
**Seite „Erweitert“ deaktivieren**  
Diese Richtlinieneinstellung steht mit anderen Einstellungen in Verbindung, um sicherzustellen, dass Benutzer die Einstellungen auf der Registerkarte **Erweitert** von Internet Explorer nicht ändern können.
  
Die Einstellung **Seite „Erweitert“ deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Sicherheitsseite deaktivieren**  
Diese Richtlinieneinstellung steht mit anderen Einstellungen in Verbindung, um sicherzustellen, dass Benutzer keine Einstellungen ändern können, die durch Gruppenrichtlinien konfiguriert wurden. Durch diese Richtlinieneinstellung wird die Registerkarte **Sicherheit** aus dem Dialogfeld **Internetoptionen** entfernt. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer daran gehindert, die Einstellungen für Sicherheitszonen wie Skripterstellung, Downloads und Benutzerauthentifizierung anzuzeigen und zu ändern. Microsoft empfiehlt, diese Richtlinieneinstellung zu aktivieren, damit Benutzer keine Einstellungen ändern und dadurch andere Sicherheitseinstellungen in Internet Explorer beeinträchtigen können.
  
Die Einstellung **Sicherheitsseite deaktivieren** ist nur für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Für die Unternehmensclient-Umgebung lautet diese Richtlinieneinstellung **Nicht konfiguriert**.
  
**Prevent ignoring certificate errors (Ignorieren von Zertifikatfehlern verhindern)**  
Wenn ein Benutzer eine Website besucht, deren SSL- oder TLS-Zertifikat (Secure Socket Layer-/Transport Layer Security-Zertifikat) einen Fehler wie „Abgelaufen“, „Gesperrt“ oder „Name stimmt nicht überein“ aufweist, verhindert Internet Explorer, dass der Benutzer den Besuch der Website fortsetzen kann. Wenn Sie diese Richtlinieneinstellung aktivieren, darf der Benutzer den Besuch der Website nicht fortsetzen. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, kann der Benutzer bestimmen, dass Zertifikatfehler ignoriert werden sollen, um den Besuch der Website fortzusetzen.
  
Die Einstellung **Prevent ignoring certificate errors** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
###### Internetsystemsteuerung\\Seite „Erweitert“
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internetsystemsteuerung\\Seite „Erweitert“**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A67: Empfohlene Einstellungen für die Seite „Erweitert“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">§ Installation bei Bedarf zulassen (Internet Explorer)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Automatische Überprüfung auf Updates von Internet Explorer</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Auf gesperrte Serverzertifikate überprüfen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista.
  
**Installation bei Bedarf zulassen (Internet Explorer)**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Benutzer automatisch **Webkomponenten** (z. B. Schriftarten) herunterladen und durch **Internet Explorer Active Setup** installieren lassen können. Wenn Sie beispielsweise eine Webseite öffnen, die Unterstützung für die Anzeige von japanischem Text erfordert, können Sie von Internet Explorer aufgefordert werden, das **Sprachpaket für Japanisch** herunterzuladen, sofern es noch nicht installiert ist.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden **Webkomponenten** wie etwa Schriftarten bei Bedarf automatisch installiert. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Benutzer zu einer Bestätigung aufgefordert, wenn **Webkomponenten** wie etwa Schriftarten heruntergeladen werden sollen. Wenn Sie diese Richtlinie nicht konfigurieren, werden die Benutzer zu einer Bestätigung aufgefordert, wenn **Webkomponenten** wie etwa Schriftarten heruntergeladen werden sollen.
  
Die Einstellung **Installation bei Bedarf zulassen (Internet Explorer)** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Software wie etwa ActiveX-Steuerelemente und Dateidownloads auch dann vom Benutzer installiert oder ausgeführt werden können, wenn die Signatur ungültig ist. Eine ungültige Signatur kann darauf hinweisen, dass die Datei manipuliert wurde.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, werden die Benutzer zu einer Bestätigung aufgefordert, dass sie Dateien mit einer ungültigen Signatur installieren oder ausführen möchten. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer keine Dateien mit einer ungültigen Signatur installieren oder ausführen. Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer selbst entscheiden, ob Dateien mit einer ungültigen Signatur ausgeführt oder installiert werden sollen.
  
Die Einstellung **Installation bzw. Ausführung von Software zulassen, auch wenn die Signatur ungültig ist** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Automatische Überprüfung auf Updates von Internet Explorer**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Internet Explorer im Internet nach neueren Versionen sucht. Wenn Internet Explorer hierfür eingestellt ist, erfolgt eine Überprüfung etwa alle 30 Tage, und die Benutzer werden dazu aufgefordert, neue Versionen zu installieren, sobald sie verfügbar sind.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, sucht Internet Explorer etwa alle 30 Tage nach einer neuen Version und fordert den Benutzer zum Herunterladen neuer Versionen auf, sobald sie verfügbar sind. Wenn Sie diese Richtlinieneinstellung deaktivieren, sucht Internet Explorer nicht im Internet nach neuen Versionen des Browsers und fordert den Benutzer folglich nicht zu deren Installation auf. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, sucht Internet Explorer nicht im Internet nach neuen Versionen des Browsers und fordert den Benutzer folglich nicht zu deren Installation auf.
  
Die Einstellung **Automatische Überprüfung auf Updates von Internet Explorer** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Auf gesperrte Serverzertifikate überprüfen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Internet Explorer den Sperrstatus von Serverzertifikaten überprüft. Zertifikate werden gesperrt, wenn sie manipuliert wurden oder nicht mehr gültig sind. Diese Option verhindert, dass Benutzer vertrauliche Daten an eine potenziell betrügerische oder unsichere Site senden.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, überprüft Internet Explorer, ob Serverzertifikate gesperrt wurden. Wenn Sie diese Richtlinieneinstellung deaktivieren, überprüft Internet Explorer nicht, ob Serverzertifikate gesperrt wurden. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, überprüft Internet Explorer nicht, ob Serverzertifikate gesperrt wurden.
  
Die Einstellung **Auf gesperrte Serverzertifikate überprüfen** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
###### Internetsystemsteuerung\\Sicherheitsseite
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internetsystemsteuerung\\Sicherheitsseite**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A68: Empfohlene Einstellungen für die Sicherheitsseite**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Intranetsites: Alle Netzwerkpfade (UNCs) einschließen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
**Intranetsites: Alle Netzwerkpfade (UNCs) einschließen**  
Diese Richtlinieneinstellung bestimmt, ob URLs, die für Netzwerkpfade stehen, der Sicherheitszone „Lokales Intranet“ zugeordnet werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden alle Netzwerkpfade der **Intranetzone** zugeordnet. Wenn Sie diese Richtlinieneinstellung deaktivieren, werden Netzwerkpfade nicht unbedingt der **Intranetzone** zugeordnet (die Zuordnung erfolgt ggf. nach anderen Regeln).
  
Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, bestimmen die Benutzer selbst, ob Netzwerkpfade der **Intranetzone** zugeordnet werden.
  
Die Einstellung **Intranetsites: Alle Netzwerkpfade (UNCs) einschließen** ist für die Unternehmensclient-Umgebung auf **Deaktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
###### Internetsystemsteuerung\\Sicherheitsseite\\Internetzone
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internetsystemsteuerung\\Sicherheitsseite\\Internetzone**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Hinweis:**   Die Einstellungen für die Internetzone und die Zone eingeschränkter Sites sind einander sehr ähnlich. Im Folgenden werden die Einstellungen für diese beiden Zonen beschrieben.
  
**Tabelle A69: Empfohlene Einstellungen für die Internetzone**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Auf Datenquellen über Domänengrenzen hinweg zugreifen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Ziehen und Ablegen oder Kopieren und Einfügen von Dateien zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Schriftartdownloads zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Installation von Desktopelementen zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Allow cut, copy, or paste operations from the clipboard via script (Von Skripts durchgeführtes Ausschneiden, Kopieren oder Einfügen aus der Zwischenablage zulassen)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Skript initiierte Fenster ohne Größen- bzw. Positionseinschränkungen zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Internetzone\Statuszeilenaktualisierung über Skript zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Automatische Eingabeaufforderung für Dateidownloads</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Aktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Download von signierten ActiveX-Steuerelementen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Download von unsignierten ActiveX-Steuerelementen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\ActiveX-Steuerelemente initialisieren und ausführen, die nicht sicher sind</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Java-Einstellungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Java deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Programme und Dateien in einem IFRAME starten</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Anmeldeoptionen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Nach Benutzername und Kennwort fragen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Subframes zwischen verschiedenen Domänen bewegen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Dateien basierend auf dem Inhalt und nicht der Dateierweiterung öffnen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Zugriffsrechte für Softwarechannel</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Hohe Sicherheit</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Internetzone\Popupblocker verwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Aktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Internetzone\Websites, die sich in Webinhaltzonen niedriger Berechtigung befinden, können in diese Zone navigieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista.
  
###### Internetsystemsteuerung\\Sicherheitsseite\\Zone eingeschränkter Sites
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Internetsystemsteuerung\\Sicherheitsseite\\Zone eingeschränkter Sites**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Hinweis:**   Die Einstellungen für die Internetzone und die Zone eingeschränkter Sites sind einander sehr ähnlich. Im Folgenden werden die Einstellungen für diese beiden Zonen beschrieben.
  
**Tabelle A70: Empfohlene Einstellungen für die Zone eingeschränkter Sites**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Auf Datenquellen über Domänengrenzen hinweg zugreifen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Active Scripting zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Binär- und Skriptverhalten zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Allow cut, copy, or paste operations from the clipboard via script (Von Skripts durchgeführtes Ausschneiden, Kopieren oder Einfügen aus der Zwischenablage zulassen)</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Ziehen und Ablegen oder Kopieren und Einfügen von Dateien zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Dateidownloads zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Schriftartdownloads zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Installation von Desktopelementen zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\META REFRESH zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Skript initiierte Fenster ohne Größen- bzw. Positionseinschränkungen zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§ Zone eingeschränkter Sites\Statuszeilenaktualisierung über Skript zulassen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Automatische Eingabeaufforderung für Dateidownloads</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Aktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Download von signierten ActiveX-Steuerelementen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Download von unsignierten ActiveX-Steuerelementen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\ActiveX-Steuerelemente initialisieren und ausführen, die nicht sicher sind</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Java-Einstellungen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Java deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Programme und Dateien in einem IFRAME starten</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Anmeldeoptionen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Anonymous-Anmeldung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Subframes zwischen verschiedenen Domänen bewegen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Dateien basierend auf dem Inhalt und nicht der Dateierweiterung öffnen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Nicht mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\ActiveX-Steuerelemente und Plug-Ins ausführen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\ActiveX-Steuerelemente ausführen, die für Scripting sicher sind</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Scripting von Java-Applets</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Zugriffsrechte für Softwarechannel</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Hohe Sicherheit</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Popupblocker verwenden</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Aktivieren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Zone eingeschränkter Sites\Websites, die sich in Webinhaltzonen niedriger Berechtigung befinden, können in diese Zone navigieren</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert:Deaktivieren</td>
</tr>
</tbody>
</table>
  
**§ -** Dieses Symbol kennzeichnet neue Gruppenrichtlinieneinstellungen in Windows Vista.
  
**Auf Datenquellen über Domänengrenzen hinweg zugreifen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Internet Explorer mithilfe von Microsoft XML Parser (MSXML) oder ActiveX Data Objects (ADO) auf Daten aus einer anderen Sicherheitszone zugreifen kann.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer eine Seite in die Zone laden, die mithilfe von MSXML oder ADO auf Daten aus einer anderen Site der Zone zugreift. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob eine Seite in der Zone geladen werden darf, die mithilfe von MSXML oder ADO auf Daten aus einer anderen Site der Zone zugreift.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer keine Seite in die Zone laden, die mithilfe von MSXML oder ADO auf Daten aus einer anderen Site der Zone zugreift.
  
Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können Benutzer keine Seite in die Zone laden, die mithilfe von MSXML oder ADO auf Daten aus einer anderen Site der Zone zugreift.
  
Die Einstellung **Auf Datenquellen über Domänengrenzen hinweg zugreifen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Active Scripting zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob auf den Seiten in der jeweiligen Zone Skriptcode ausgeführt wird. Wenn Sie diese Richtlinieneinstellung aktivieren, kann Skriptcode auf den Seiten in der Zone automatisch ausgeführt werden. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob Skriptcode auf Seiten in der Zone zugelassen werden soll. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird das Ausführen von Skriptcode auf Seiten in der Zone verhindert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, wird das Ausführen von Skriptcode auf Seiten in der Zone verhindert.
  
Die Einstellung **Active Scripting zulassen** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Binär- und Skriptverhalten zulassen**  
Über diese Richtlinieneinstellung können Sie dynamisches Binär- und Skriptverhalten verwalten: Komponenten, die spezifische Funktionalität für die HTML-Elemente einkapseln, an die sie angefügt wurden. Wenn Sie diese Richtlinieneinstellung aktivieren, steht Binär- und Skriptverhalten zur Verfügung. Wenn Sie im Dropdownfeld die Option **Vom Administrator genehmigt** wählen, stehen nur die Verhaltensweisen zur Verfügung, die in der Liste **Vom Administrator zugelassenes Verhalten** unter **Sicherheitseinschränkung für Binärverhalten** aufgeführt sind.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, steht Binär- und Skriptverhalten nur dann zur Verfügung, wenn in den jeweiligen Anwendungen ein benutzerdefinierter Sicherheits-Manager implementiert ist. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, steht Binär- und Skriptverhalten nur dann zur Verfügung, wenn in den jeweiligen Anwendungen ein benutzerdefinierter Sicherheits-Manager implementiert ist.
  
Die Einstellung **Binär- und Skriptverhalten zulassen** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Allow cut, copy, or paste operations from the clipboard via script (Von Skripts durchgeführtes Ausschneiden, Kopieren oder Einfügen aus der Zwischenablage zulassen)**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Skripts Zwischenablagevorgänge (beispielsweise Ausschneiden, Kopieren und Einfügen) in einem bestimmten Bereich durchführen können. Wenn Sie diese Richtlinieneinstellung aktivieren, können Skripts Zwischenablagevorgänge durchführen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer gefragt, ob Zwischenablagevorgänge durchgeführt werden sollen. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Skripts keine Zwischenablagevorgänge durchführen. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können Skripts keine Zwischenablagevorgänge durchführen.
  
Die Einstellung **Allow cut, copy, or paste operations from the clipboard via script** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Ziehen und Ablegen oder Kopieren und Einfügen von Dateien zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Benutzer Dateien aus einer Quelle innerhalb der Zone herüberziehen oder kopieren und einfügen dürfen. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer automatisch Dateien aus dieser Zone herüberziehen oder kopieren und einfügen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob Dateien aus dieser Zone herübergezogen oder kopiert und eingefügt werden sollen. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird verhindert, dass Benutzer Dateien aus dieser Zone herüberziehen oder kopieren und einfügen.
  
Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden die Benutzer aufgefordert zu wählen, ob Dateien aus dieser Zone herübergezogen oder kopiert werden sollen.
  
Die Einstellung **Ziehen und Ablegen oder Kopieren und Einfügen von Dateien zulassen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Dateidownloads zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Dateien aus der jeweiligen Zone heruntergeladen werden dürfen. Diese Option wird durch die Zone bestimmt, in der sich die Seite befindet, die den Download verursacht, nicht durch die Zone, aus der die Datei übertragen wird. Wenn Sie diese Richtlinieneinstellung aktivieren, können Dateien aus der Zone heruntergeladen werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird verhindert, dass Dateien aus der Zone heruntergeladen werden. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, wird verhindert, dass Dateien aus der Zone heruntergeladen werden.
  
Die Einstellung **Dateidownloads zulassen** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Schriftartdownloads zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Seiten der jeweiligen Zone HTML-Schriftarten herunterladen können.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, können HTML-Schriftarten automatisch heruntergeladen werden. Wenn Sie diese Richtlinieneinstellung aktivieren und im Dropdownfeld die Option „Bestätigen“ ausgewählt ist, werden die Benutzer gefragt, ob HTML-Schriftarten heruntergeladen werden dürfen. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird das Herunterladen von HTML-Schriftarten verhindert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden die Benutzer gefragt, ob HTML-Schriftarten heruntergeladen werden dürfen.
  
Die Einstellung **Schriftartdownloads zulassen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Installation von Desktopelementen zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Benutzer Active Desktop-Elemente aus dieser Zone herunterladen dürfen. Für diese Einstellung stehen folgende Option zur Auswahl:
  
**Aktivieren** – Benutzer können automatisch Desktopelemente aus dieser Zone herunterladen.
  
**Bestätigen** – Benutzer werden aufgefordert zu wählen, ob Desktopelemente aus dieser Zone installiert werden sollen.
  
**Deaktivieren** – Benutzer werden daran gehindert, Desktopelemente aus dieser Zone zu installieren.
  
Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden die Benutzer daran gehindert, Desktopelemente aus dieser Zone zu installieren.
  
Die Einstellung **Installation von Desktopelementen zulassen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**META REFRESH zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob ein Benutzerbrowser auf eine andere Webseite umgeleitet werden darf, wenn der Autor der Webseite die **Meta Refresh**-Einstellung verwendet hat, um Browser auf eine andere Webseite umzuleiten. Wenn Sie diese Richtlinieneinstellung aktivieren, kann ein Benutzerbrowser, der eine Seite lädt, die eine aktive **Meta Refresh**-Einstellung enthält, auf eine andere Webseite umgeleitet werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann ein Benutzerbrowser, der eine Seite lädt, die eine aktive **Meta Refresh**-Einstellung enthält, nicht auf eine andere Webseite umgeleitet werden. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, kann ein Benutzerbrowser, der eine Seite lädt, die eine aktive **Meta Refresh**-Einstellung enthält, nicht auf eine andere Webseite umgeleitet werden.
  
Die Einstellung **META REFRESH zulassen** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Skript initiierte Fenster ohne Größen- bzw. Positionseinschränkungen zulassen**  
Mit dieser Richtlinieneinstellung können Sie Einschränkungen bei durch von Skripts initiierten Popupfenstern und Fenstern mit Titel- und Statusleiste verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, werden die **Sicherheitseinschränkungen für Skriptfenster** in dieser Zone nicht angewendet. Die Sicherheitszone wird ohne die durch diese Funktion zur Verfügung gestellte zusätzliche Sicherheitsstufe ausgeführt. Wenn Sie diese Richtlinieneinstellung deaktivieren, können potenziell schädigende Skript-initiierte Popupfenster und Fenster mit Titel- und Statusleisten nicht ausgeführt werden. Diese Sicherheitsfunktion von Internet Explorer wird in dieser Zone gemäß der Steuerungseinstellung der **Sicherheitseinschränkungen für Skriptfenster** aktiviert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können potenziell schädigende durch Skripts initiierte Popupfenster und Fenster mit Titel- und Statusleisten nicht ausgeführt werden. Diese Sicherheitsfunktion von Internet Explorer wird in dieser Zone gemäß der Steuerungseinstellung der **Sicherheitseinschränkungen für Skriptfenster** aktiviert.
  
Die Einstellung **Skript initiierte Fenster ohne Größen- bzw. Positionseinschränkungen zulassen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Statuszeilenaktualisierung über Skript zulassen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob ein Skript die Statusleiste innerhalb der Zone aktualisieren darf. Wenn Sie diese Richtlinieneinstellung aktivieren, darf ein Skript die Statusleiste aktualisieren. Wenn Sie diese Richtlinieneinstellung deaktivieren, darf ein Skript die Statusleiste nicht aktualisieren. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden Aktualisierungen der Statusleiste durch Skripts deaktiviert.
  
Die Einstellung **Statuszeilenaktualisierung über Skript zulassen** ist für die Hochsicherheitsumgebung auf **Deaktiviert** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Automatische Eingabeaufforderung für Dateidownloads**  
Diese Richtlinieneinstellung bestimmt, ob Benutzer zu nicht vom Benutzer eingeleiteten Dateidownloads aufgefordert werden. Unabhängig von dieser Einstellung wird für von Benutzern eingeleitete Downloads ein Dateidownload-Dialogfeld angezeigt. Wenn Sie diese Richtlinieneinstellung aktivieren, wird den Benutzern bei automatischen Downloadversuchen ein Dateidownload-Dialogfeld angezeigt.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, werden nicht vom Benutzer eingeleitete Dateidownloads blockiert, und den Benutzern wird anstelle eines Dateidownload-Dialogfelds eine **Informationsleiste** angezeigt. Die Benutzer können dann auf die **Informationsleiste** klicken, um die Eingabeaufforderung für den Dateidownload zuzulassen.
  
Die Einstellung **Automatische Eingabeaufforderung für Dateidownloads** ist für die Hochsicherheitsumgebung auf **Aktiviert:Aktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Download von signierten ActiveX-Steuerelementen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Benutzer signierte ActiveX-Steuerelemente von einer Seite innerhalb der Zone herunterladen dürfen. Wenn Sie diese Richtlinie aktivieren, können die Benutzer signierte Steuerelemente ohne Benutzereingriff herunterladen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer gefragt, ob Steuerelemente heruntergeladen werden sollen, die von nicht vertrauenswürdigen Herausgebern signiert sind. Von vertrauenswürdigen Herausgebern signierter Code wird automatisch heruntergeladen. Wenn Sie die Richtlinieneinstellungdeaktivieren, können keine signierten Steuerelemente heruntergeladen werden.
  
Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden die Benutzer gefragt, ob Steuerelemente heruntergeladen werden sollen, die von nicht vertrauenswürdigen Herausgebern signiert sind. Von vertrauenswürdigen Herausgebern signierter Code wird automatisch heruntergeladen.
  
Die Einstellung **Download von signierten ActiveX-Steuerelementen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Download von unsignierten ActiveX-Steuerelementen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Benutzer unsignierte ActiveX-Steuerelemente aus der jeweiligen Zone herunterladen dürfen. Solcher Code ist potenziell schädlich, insbesondere, wenn er aus einer nicht vertrauenswürdigen Zone stammt.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer unsignierte Steuerelemente ohne Benutzereingriff ausführen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob die unsignierten Steuerelemente ausgeführt werden dürfen. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer keine unsignierten Steuerelemente ausführen. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können Benutzer keine unsignierten Steuerelemente ausführen.
  
Die Einstellung **Download von unsignierten ActiveX-Steuerelementen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**ActiveX-Steuerelemente initialisieren und ausführen, die nicht sicher sind**  
Mit dieser Richtlinieneinstellung können Sie ActiveX-Steuerelemente verwalten, die als nicht sicher gekennzeichnet sind. Wenn Sie diese Richtlinieneinstellung aktivieren, werden ActiveX-Steuerelemente ausgeführt, mit Parametern geladen und geskriptet, ohne dass die Objektsicherheit für nicht vertrauenswürdige Daten oder Skripts festgelegt wird. Diese Einstellung wird nicht empfohlen, außer für sichere und verwaltete Zonen. Diese Einstellung bewirkt, dass sowohl unsichere als auch sichere Steuerelemente initiiert und geskriptet werden. Dabei wird die Option **ActiveX-Steuerelemente ausführen, die für Scripting sicher sind** ignoriert.
  
Wenn Sie diese Richtlinieneinstellung aktivieren und im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob das Steuerelement mit Parametern geladen oder geskriptet werden darf.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, werden keine ActiveX-Steuerelemente, die nicht sicher gemacht werden können, mit Parametern geladen oder geskriptet. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden keine ActiveX-Steuerelemente, die nicht sicher gemacht werden können, mit Parametern geladen oder geskriptet.
  
Die Einstellung **ActiveX-Steuerelemente initialisieren und ausführen, die nicht sicher sind** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Java-Einstellungen**  
Mit dieser Richtlinieneinstellung können Sie die Berechtigungen für Java-Applets verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, können Sie Optionen aus dem Dropdownfeld wählen. **Benutzerdefiniert** – Hiermit legen Sie die Berechtigungseinstellungen individuell fest. **Niedrige Sicherheit** – Applets dürfen alle Vorgänge durchführen**. Mittlere Sicherheit** – Applets dürfen in ihrer Sandbox (einem Speicherbereich, außerhalb dessen das Programm keine Aufrufe durchführen kann) ausgeführt werden, und es werden Funktionen wie „Scratch Space“ (ein sicherer Speicherbereich auf dem Clientcomputer) und eine benutzergesteuerte Datei-E/A ermöglicht. **Hohe Sicherheit** – Applets dürfen in ihrer Sandbox ausgeführt werden. Java deaktivieren – Damit werden Java-Applets an der Ausführung gehindert. Wenn Sie diese Richtlinieneinstellung deaktivieren, können keine Java-Applets ausgeführt werden. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, gilt die Einstellung **Hohe Sicherheit**.
  
Die Einstellung **Java-Einstellungen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Java deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Programme und Dateien in einem IFRAME starten**  
Über diese Richtlinieneinstellung können Sie festlegen, ob von einem IFRAME-Verweis im HTML der Seiten in dieser Zone aus Anwendungen ausgeführt und Dateien heruntergeladen werden dürfen. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer von IFRAMEs auf den Seiten in dieser Zone ohne Benutzereingriff Anwendungen ausführen und Dateien herunterladen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer gefragt, ob von IFRAMEs auf den Seiten in dieser Zone aus Anwendungen ausgeführt und Dateien heruntergeladen werden dürfen.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, werden die Benutzer daran gehindert, von IFRAMEs auf den Seiten in dieser Zone aus Anwendungen auszuführen und Dateien herunterzuladen. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, werden die Benutzer gefragt, ob von IFRAMEs auf den Seiten in dieser Zone aus Anwendungen ausgeführt und Dateien heruntergeladen werden dürfen.
  
Die Einstellung **Programme und Dateien in einem IFRAME starten** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Anmeldeoptionen**  
Mit dieser Richtlinieneinstellung können Sie die Einstellungen für Anmeldeoptionen verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, können Sie eine der folgenden Anmeldeoptionen wählen:
  
**Anonymous-Anmeldung** – Deaktiviert die HTTP-Authentifizierung und verwendet das Gastkonto nur für das CIFS-Protokoll (Common Internet File System-Protokoll).
  
**Nach Benutzername und Kennwort fragen** – Benutzer werden zur Eingabe von Benutzer-ID und Kennwort aufgefordert. Nach der Eingabe können diese Werte automatisch für den weiteren Verlauf der Sitzung verwendet werden.
  
**Automatisches Anmelden nur in der Intranetzone** – Benutzer werden in anderen Zonen zur Eingabe von Benutzer-ID und Kennwort aufgefordert. Nach der Eingabe können diese Werte automatisch für den weiteren Verlauf der Sitzung verwendet werden.
  
**Automatische Anmeldung mit aktuellem Benutzernamen und Kennwort** – Es wird versucht, die Anmeldung mithilfe der NTLM-Authentifizierung (Windows NT Challenge Response) durchzuführen. Wenn die NTLM-Authentifizierung vom Server unterstützt wird, werden der Netzwerkbenutzername und das Netzwerkkennwort des Benutzers für die Anmeldung verwendet. Wenn die NTLM-Authentifizierung vom Server nicht unterstützt wird, wird der Benutzer zur Eingabe von Benutzername und Kennwort aufgefordert.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, gilt die Einstellung **Automatisches Anmelden nur in der Intranetzone**. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, gilt die Einstellung **Automatisches Anmelden nur in der Intranetzone**.
  
Die Einstellung **Anmeldeoptionen** ist für die Hochsicherheitsumgebung in der **Internetzone** auf **Aktiviert:Nach Benutzername und Kennwort fragen** und in der **Zone eingeschränkter Sites** auf **Aktiviert:Anonymous-Anmeldung** gesetzt.Für die Unternehmensclient-Umgebung ist die Einstellung sowohl in der **Internetzone** als auch in der **Zone eingeschränkter Sites** auf **Nicht konfiguriert** gesetzt.
  
**Subframes zwischen verschiedenen Domänen bewegen**  
Mit dieser Richtlinieneinstellung können Sie das Öffnen von Subframes und den domänenübergreifenden Zugriff verschiedener Anwendungen verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, können Benutzer Subframes aus anderen Domänen öffnen und auf Anwendungen aus anderen Domänen zugreifen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer gefragt, ob Subframes oder der Zugriff auf Anwendungen aus anderen Domänen zugelassen werden sollen.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, können die Benutzer keine Subframes aus anderen Domänen öffnen oder auf Anwendungen aus anderen Domänen zugreifen. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können Benutzer Subframes aus anderen Domänen öffnen und auf Anwendungen aus anderen Domänen zugreifen.
  
Die Einstellung **Subframes zwischen verschiedenen Domänen bewegen** ist für die Hochsicherheitsumgebung in der **Internetzone** auf **Deaktiviert** und in der **Zone eingeschränkter Sites** auf **Aktiviert:Deaktivieren** gesetzt.Für die Unternehmensclient-Umgebung ist die Einstellung sowohl in der **Internetzone** als auch in der **Zone eingeschränkter Sites** auf **Nicht konfiguriert** gesetzt.
  
**Dateien basierend auf dem Inhalt und nicht der Dateierweiterung öffnen**  
Diese Richtlinieneinstellung ermöglicht die Verwaltung von MIME-Sniffing zum Heraufstufen einer Datei von einem Typ zu einem anderen Typ basierend auf einer MIME-Ermittlung. Eine MIME-Ermittlung ist die Ermittlung von Internet Explorer des auf einer Bitsignatur basierenden Dateityps. Wenn Sie diese Richtlinieneinstellung aktivieren, die **Sicherheitsfunktion für MIME-Sniffing** in dieser Zone nicht angewendet. Die Sicherheitszone wird ohne die zusätzliche Sicherheitsstufe ausgeführt, die diese Funktion bietet. Wenn Sie diese Richtlinieneinstellung deaktivieren, können möglicherweise schädigende Aktionen nicht ausgeführt werden. Diese Internet Explorer-Sicherheitsfunktion wird in dieser Zone entsprechend der Funktionssteuerungseinstellung für diesen Prozess aktiviert Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, wird die **Sicherheitsfunktion für MIME-Sniffing** in dieser Zone nicht verwendet.
  
Die Einstellung **Dateien basierend auf dem Inhaltund nicht der Dateierweiterung öffnen** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Nicht mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern**  
Über diese Richtlinieneinstellung können Sie festlegen, ob .NET Framework-Komponenten, die nicht mit Authenticode® signiert sind, mit Internet Explorer ausgeführt werden können. Diese Komponenten enthalten verwaltete Steuerelemente, auf die von einem Objekttag verwiesen wird, und verwaltete ausführbare Dateien, auf die von einem Link verwiesen wird.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, führt Internet Explorer unsignierte verwaltete Komponenten aus. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, wird der Benutzer von Internet Explorer gefragt, ob unsignierte verwaltete Komponenten ausgeführt werden sollen. Wenn Sie diese Richtlinieneinstellung deaktivieren, führt Internet Explorer keine unsignierten verwalteten Komponenten aus. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, führt Internet Explorer keine unsignierten verwalteten Komponenten aus.
  
Die Einstellung **Nicht mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern**  
Über diese Richtlinieneinstellung können Sie festlegen, ob .NET Framework-Komponenten, die mit Authenticode® signiert sind, mit Internet Explorer ausgeführt werden können. Diese Komponenten enthalten verwaltete Steuerelemente, auf die von einem Objekttag verwiesen wird, und verwaltete ausführbare Dateien, auf die von einem Link verwiesen wird.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, führt Internet Explorer signierte verwaltete Komponenten aus. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, wird der Benutzer von Internet Explorer gefragt, ob signierte verwaltete Komponenten ausgeführt werden sollen. Wenn Sie diese Richtlinieneinstellung deaktivieren, führt Internet Explorer keine signierten verwalteten Komponenten aus. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, führt Internet Explorer keine signierten verwalteten Komponenten aus.
  
Die Einstellung **Mit Authenticode signierte Komponenten ausführen, die .NET Framework erfordern** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**ActiveX-Steuerelemente und Plug-Ins ausführen**  
Über diese Richtlinieneinstellung können Sie festlegen, ob ActiveX-Steuerelemente und Plug-Ins auf Seiten aus der angegebenen Zone ausgeführt werden können. Wenn Sie diese Richtlinieneinstellung aktivieren, können Steuerelemente und Plug-Ins ohne Benutzereingriff ausgeführt werden. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob die Steuerelemente oder Plug-Ins ausgeführt werden sollen. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird das Ausführen von Steuerelementen und Plug-Ins verhindert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, wird das Ausführen von Steuerelementen und Plug-Ins verhindert.
  
Die Einstellung **ActiveX-Steuerelemente und Plug-Ins ausführen** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**ActiveX-Steuerelemente ausführen, die für Scripting sicher sind**  
Über diese Richtlinieneinstellung können Sie festlegen, ob ein ActiveX-Steuerelement, das als für Scripting sicher gekennzeichnet ist, mit einem Skript interagieren kann. Wenn Sie diese Richtlinieneinstellung aktivieren, kann die Skriptinteraktion automatisch ohne Benutzereingriff erfolgen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob Skriptinteraktion stattfinden darf. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, wird die Skriptinteraktion verhindert.
  
Die Einstellung **ActiveX-Steuerelemente ausführen, die für Scripting sicher sind** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Scripting von Java-Applets**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Applets für Skripts innerhalb der Zone angezeigt werden. Wenn Sie diese Richtlinieneinstellung aktivieren, können Skripts automatisch ohne Benutzereingriff auf Applets zugreifen. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, werden die Benutzer aufgefordert zu wählen, ob Skripts auf Applets zugreifen dürfen. Wenn Sie diese Richtlinieneinstellung deaktivieren oder nicht konfigurieren, wird die verhindert, dass Skripts auf Applets zugreifen.
  
Die Einstellung **Scripting von Java-Applets** ist in der **Zone eingeschränkter Sites** für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt.
  
**Zugriffsrechte für Softwarechannel**  
Mit dieser Richtlinieneinstellung können Sie Berechtigungen für Softwarechannels verwalten. Wenn Sie diese Richtlinieneinstellung aktivieren, können Sie folgende Optionen aus dem Dropdownfeld wählen:
  
**Niedrige Sicherheit** – Benutzer werden per E-Mail über Softwareupdates benachrichtigt, und Softwarepakete werden automatisch auf die Computer der Benutzer heruntergeladen und dort automatisch installiert.
  
**Mittlere Sicherheit** – Benutzer werden per E-Mail über Softwareupdates benachrichtigt, und Softwarepakete werden automatisch auf die Computer der Benutzer heruntergeladen (aber nicht installiert).
  
**Hohe Sicherheit** – Benutzer werden nicht per E-Mail über Softwareupdates benachrichtigt, und Softwarepakete werden weder automatisch heruntergeladen noch installiert.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, gilt die Einstellung **Hohe Sicherheit**.
  
Die Einstellung **Zugriffsrechte für Softwarechannel** ist für die Hochsicherheitsumgebung auf **Aktiviert:Hohe Sicherheit** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Popupblocker verwenden**  
Über diese Richtlinieneinstellung können Sie festlegen, ob unerwünschte Popupfenster angezeigt werden dürfen. Popupfenster, die geöffnet werden, wenn der Endbenutzer auf einen Link klickt, werden nicht blockiert. Wenn Sie diese Richtlinieneinstellung aktivieren, wird das Anzeigen zahlreicher unerwünschter Popupfenster verhindert. Wenn Sie diese Richtlinieneinstellung deaktivieren, wird das Anzeigen von Popupfenstern nicht verhindert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, wird das Anzeigen zahlreicher unerwünschter Popupfenster verhindert.
  
Die Einstellung **Popupblocker verwenden** ist für die Hochsicherheitsumgebung auf **Aktiviert:Aktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
**Websites, die sich in Webinhaltzonen niedriger Berechtigung befinden, können in diese Zone navigieren**  
Über diese Richtlinieneinstellung können Sie festlegen, ob Websites von Zonen mit niedrigeren Berechtigungen, z. B. **Eingeschränkte Sites**, in diese Zone wechseln dürfen. Wenn Sie diese Richtlinieneinstellung aktivieren, können Websites von Zonen mit niedrigeren Berechtigungen neue Fenster in dieser Zone öffnen oder in diese Zone wechseln. Die Sicherheitszone wird ohne die zusätzliche Sicherheitsstufe ausgeführt, die die Funktion zum **Schutz vor Zonenanhebung** bietet. Wenn Sie im Dropdownfeld die Option **Bestätigen** wählen, wird dem Benutzer eine Warnung angezeigt, die den Benutzer über diese potenziell gefährliche Aktion informiert.
  
Wenn Sie diese Richtlinieneinstellung deaktivieren, werden potenziell schädigende Wechsel verhindert. Die Internet Explorer-Sicherheitsfunktion wird in dieser Zone gemäß der Funktion zum **Schutz vor Zonenanhebung** aktiviert. Wenn Sie diese Richtlinieneinstellung nicht konfigurieren, können Websites von Zonen mit niedrigeren Berechtigungen neue Fenster in dieser Zone öffnen oder in diese Zone wechseln.
  
Die Einstellung **Websites, die sich in Webinhaltzonen niedriger Berechtigung befinden, können in diese Zone navigieren** ist für die Hochsicherheitsumgebung auf **Aktiviert:Deaktivieren** und für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** gesetzt. Dies gilt für die **Internetzone** ebenso wie für die **Zone eingeschränkter Sites**.
  
###### Offlineseiten
  
Diese empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Internet Explorer\\Offlineseiten**
  
Die folgende Tabelle bietet einen Überblick über die empfohlenen Benutzerkonfigurationseinstellungen für Internet Explorer. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Hinweis:   **Diese Einstellungen gelten nicht für Internet Explorer 7. Sie werden nur für die Unternehmensclient-Umgebung konfiguriert, da in dieser Umgebung auch Computer mit Windows XP und Internet Explorer 6.0 vorhanden sein könnten.
  
**Tabelle A71: Empfohlene Einstellungen für Offlineseiten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Einstellung</th>
<th>EC-Benutzer</th>
<th>SSLF-Benutzer</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Hinzufügen von Channels deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hinzufügen von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Alle geplanten Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Channel-Benutzeroberfläche vollständig deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Download von abonnierten Siteinhalten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Bearbeiten von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Trefferprotokollierung für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Entfernen von Channels deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Entfernen von Zeitplänen für Offlineseiten deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
</tr>
</tbody>
</table>
  
**Hinzufügen von Channels deaktivieren**  
Diese Richtlinieneinstellung sorgt dafür, dass Benutzer in Internet Explorer keine Channels hinzufügen können. Channels sind Websites, die auf Computern, auf denen Internet Explorer ausgeführt wird, nach einem vom Channelanbieter vorgegebenen Zeitplan automatisch aktualisiert werden. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen. Als Best Practice-Methode gilt, das Herunterladen von Seiten aus dem Internet auf einen Computer nur zu ermöglichen, wenn ein Benutzer diese Funktion direkt an diesem Computer anfordert.
  
Aus diesen Gründen ist die Einstellung **Hinzufügen von Channels deaktivieren** für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Hinzufügen von Zeitplänen für Offlineseiten deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer festlegen können, dass Webseiten heruntergeladen und offline angezeigt werden können. Diese Funktionalität ermöglicht Benutzern das Anzeigen von Webseiten, wenn ihre Computer nicht mit dem Internet verbunden sind.
  
Die Einstellung **Hinzufügen von Zeitplänen für Offlineseiten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Alle geplanten Offlineseiten deaktivieren**  
Durch diese Richtlinieneinstellung werden alle vorhandenen Zeitpläne deaktiviert, die zum Herunterladen von Webseiten eingerichtet wurden, damit diese offline angezeigt werden können. Wenn Sie diese Richtlinie aktivieren, werden im Dialogfeld **Eigenschaften der Webseite** auf der Registerkarte **Zeitplan** die Kontrollkästchen für Zeitpläne ausgeblendet, damit die Benutzer diese nicht aktivieren können. Benutzer klicken zum Anzeigen dieser Registerkarte im Menü **Extras** auf **Synchronisieren**, wählen eine Webseite aus, klicken dann auf die Schaltfläche **Eigenschaften** und schließlich auf die Registerkarte **Zeitplan**. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Alle geplanten Offlineseiten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Channel-Benutzeroberfläche vollständig deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die Channelleiste anzeigen können. Channels sind Websites, die auf Computern nach einem vom Channelanbieter vorgegebenen Zeitplan automatisch aktualisiert werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer daran gehindert, auf die Channelleiste zuzugreifen und im Dialogfeld **Eigenschaften von Anzeige** auf der Registerkarte **Web** das Kontrollkästchen **Internet Explorer-Channelleiste** zu aktivieren. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Channel-Benutzeroberfläche vollständig deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Download von abonnierten Siteinhalten deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer abonnierte Websiteinhalte herunterladen können. Dennoch erfolgt eine Überprüfung auf Aktualisierung und entsprechende Synchronisierung des Webseiteninhalts, wenn ein Benutzer zu einer zuvor aufgerufenen Seite zurückkehrt. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Download von abonnierten Siteinhalten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer Zeitpläne für die Offlineansicht von abonnierten Webseiten und Webseitengruppen hinzufügen, bearbeiten oder entfernen können. Eine Abonnementgruppe besteht aus einer Favoritenwebseite sowie den damit verknüpften Webseiten. Wenn Sie diese Richtlinie aktivieren, werden im Dialogfeld **Eigenschaften der Webseite** auf der Registerkarte **Zeitplan** die Schaltflächen **Hinzufügen**, **Entfernen** und **Bearbeiten** abgeblendet dargestellt. Um diese Registerkarte anzuzeigen, klicken Benutzer im Menü **Extras** auf **Synchronisieren**, wählen eine Webseite aus, klicken dann auf die Schaltfläche **Eigenschaften** und schließlich auf die Registerkarte **Zeitplan**. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Aus diesen Gründen ist die Einstellung **Das Bearbeiten und Erstellen von geplanten Gruppen deaktivieren** für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Bearbeiten von Zeitplänen für Offlineseiten deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer vorhandene Zeitpläne bearbeiten können, die festgelegt wurden, um Webseiten herunterzuladen und offline anzuzeigen. Wenn Sie diese Richtlinie aktivieren, können Benutzer keine Zeitplaneigenschaften von Seiten anzeigen, die für die Offlineansicht eingerichtet wurden. Es werden keine Eigenschaften angezeigt, wenn Benutzer in Internet Explorer im Menü **Extras** auf **Synchronisieren** klicken, eine Webseite auswählen und dann auf die Schaltfläche **Eigenschaften** klicken. Es wird keine Meldung angezeigt, dass der Befehl nicht verfügbar ist. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Bearbeiten von Zeitplänen für Offlineseiten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Trefferprotokollierung für Offlineseiten deaktivieren**  
Diese Richtlinieneinstellung nimmt Channelanbietern die Möglichkeit aufzuzeichnen, wie oft ihre Channelseiten von Offlinebenutzern angezeigt werden. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Trefferprotokollierung für Offlineseiten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Entfernen von Channels deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer die Channelsynchronisierung in Internet Explorer deaktivieren können. Als Best Practice-Methode gilt, das Herunterladen von Seiten aus dem Internet auf einen Computer nur zu ermöglichen, wenn ein Benutzer diese Funktion direkt an diesem Computer anfordert.
  
Aus diesem Grund ist die Einstellung **Entfernen von Channels deaktivieren** für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
**Entfernen von Zeitplänen für Offlineseiten deaktivieren**  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer vorkonfigurierte Einstellungen löschen können, die dafür sorgen, dass Webseiten für die Offlineansicht heruntergeladen werden. Wenn Sie diese Richtlinieneinstellung aktivieren, werden vorkonfigurierte Einstellungen für Webseiten geschützt. Diese Richtlinieneinstellung ist eine von mehreren Einstellungen, die die Fähigkeit von Internet Explorer blockieren, automatisch Inhalte herunterzuladen.
  
Die Einstellung **Entfernen von Zeitplänen für Offlineseiten deaktivieren** ist für die Unternehmensclient-Umgebung auf **Aktiviert** und für die Hochsicherheitsumgebung auf **Nicht konfiguriert** gesetzt.
  
###### Windows Explorer
  
Windows Explorer dient auf Clientcomputern mit Windows Vista zum Durchsuchen des Dateisystems.
  
Die folgenden empfohlenen Benutzereinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Benutzerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten**  
**\\Windows Explorer**
  
In der folgenden Tabelle sind die empfohlenen Benutzerkonfigurationseinstellungen für Windows-Explorer zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Tabelle A72: Empfohlene Benutzerkonfigurationseinstellungen für Windows-Explorer**

 
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
<td style="border:1px solid black;">Registerkarte „Sicherheit“ entfernen</td>
<td style="border:1px solid black;">Nicht konfiguriert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
**CD-Brennfunktionen entfernen**  
Durch diese Richtlinieneinstellung werden die integrierten Windows Vista-Funktionen entfernt, die es Benutzern erlauben, CDs mithilfe von Windows Explorer zu brennen. Windows Vista ermöglicht es Ihnen, wiederbeschreibbare CDs zu erstellen und zu ändern, wenn an Ihren Computer ein CD-Brenner angeschlossen ist. Mit dieser Funktion können große Datenmengen von einer Festplatte auf eine CD kopiert werden, die dann aus dem Computer genommen werden kann.
  
Die Einstellung **CD-Brennfunktionen entfernen** ist für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
**Hinweis:**   Durch diese Richtlinieneinstellung wird nicht verhindert, dass Anwendungen von Drittanbietern CDs mit einem CD-Brenner erstellen oder ändern können. Dieses Handbuch empfiehlt die Verwendung von Richtlinien für Softwareeinschränkungen, um die Erstellung oder Änderung von CDs durch Anwendungen von Drittanbietern zu blockieren.
  
Eine weitere Möglichkeit, Benutzer am Brennen von CDs zu hindern, besteht darin, die CD-Brenner aus den Clientcomputern Ihrer Umgebung zu entfernen oder sie durch CD-ROM-Laufwerke zu ersetzen, die nicht zum Brennen genutzt werden können.
  
**Registerkarte „Sicherheit“ entfernen**  
Durch diese Richtlinieneinstellung wird im Windows-Explorer die Registerkarte **Sicherheit** in den Eigenschaftendialogfeldern für Dateien und Ordner deaktiviert. Wenn Sie diese Richtlinieneinstellung aktivieren, werden Benutzer bei allen Dateisystemobjekten (wie Ordnern, Dateien, Verknüpfungen und Laufwerken) daran gehindert, im Dialogfeld **Eigenschaften** auf die Registerkarte **Sicherheit** zuzugreifen. Da die Registerkarte **Sicherheit** nicht verfügbar ist, können Benutzer weder Einstellungen ändern noch die Liste der Benutzer anzeigen.
  
Aus diesen Gründen ist die Einstellung **Registerkarte „Sicherheit“ entfernen** für die Unternehmensclient-Umgebung auf **Nicht konfiguriert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Weitere Informationen
  
Die folgenden Links bieten zusätzliche Informationen zu Sicherheitsthemen und ausführlichen Erörterungen der in diesem Handbuch behandelten Konzepte und Sicherheitsempfehlungen für Windows Vista:
  
-   [Configuring a Computer for Windows Firewall Troubleshooting](http://technet2.microsoft.com/windowsserver/en/library/bfdeda55-46fc-4b53-b4cd-c71838ef4b411033.mspx?mfr=true) (engl.)
  
-   [HOW TO: Hide a Windows 2000-Based Computer from the Browser List](http://support.microsoft.com/kb/321710/en-us) (engl.)
  
-   [SO WIRD'S GEMACHT: Kennwortänderungen durch Benutzer nur zulassen, wenn dies in Windows Server 2003 erforderlich ist](http://support.microsoft.com/kb/324744)
  
-   [SO WIRD'S GEMACHT: Sicherstellen, dass Kennwörter nur auf Anforderung von Benutzern geändert werden können](http://support.microsoft.com/kb/309799), Knowledge Base-Artikel 309799.
  
-   [Aktivieren der automatischen Anmeldung in Windows XP](http://support.microsoft.com/kb/315231)
  
-   [Verwenden von Gruppenrichtlinien zum Konfigurieren von detaillierten Sicherheitsüberwachungseinstellungen für Windows Vista-Clientcomputer in einer Windows Server 2003- oder Windows 2000-Domäne](http://support.microsoft.com/kb/921469)
  
-   [IIS and Built-in Accounts](http://technet2.microsoft.com/windowsserver/en/library/f1727156-e480-4e05-b168-b764a6e13f881033.mspx?mfr=true) (engl.)
  
-   [IPSec Default Exemptions Can Be Used to Bypass IPsec Protection in Some Scenarios](http://support.microsoft.com/kb/811832/en-us) (engl.)
  
-   [Outlook Web Access and Small Business Server Remote Web Workplace do not function if XP Service Pack 2 Add-on Blocking is enabled via group policy](http://support.microsoft.com/kb/555235/en-us) (engl.)
  
-   [Update.exe – der Paketinstaller für Windows und Windows-Komponenten](http://www.microsoft.com/germany/technet/datenbank/articles/600338.mspx)
  
-   [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10))
  
-   [Windows-Firewall](http://www.microsoft.com/technet/network/wf/default.mspx) (engl.)
  
-   [Windows Server Update Services – Produkthomepage](http://www.microsoft.com/germany/windowsserver2003/technologien/updateservices/default.mspx)
  
-   [Microsoft Update](http://update.microsoft.com/)
  
#### Support und Feedback
  
Das SASC-Team (Solution Accelerators – Security and Compliance) interessiert sich für Ihre Meinung zu diesem und anderen Solution Accelerators.
  
Veröffentlichen Sie Ihre Kommentare in der Newsgroup [Diskussionen zum Thema Sicherheit](http://windowshelp.microsoft.com/communities/newsgroups/en-us/default.mspx?dg=microsoft.public.windows.vista.security&lang=en&cr=us&r=9dcac6a3-b8e7-4ba3-aa06-4e38b8ee9f35) (engl.) auf der Windows Vista-Hilfe- und Support-Website.
  
Sie können Ihr Feedback auch an die folgende E-Mail-Adresse senden: [secwish@microsoft.com](mailto:secwish@microsoft.com?subject=windows%20vista%20security%20guide).
  
Wir freuen uns, von Ihnen zu hören.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
##### In diesem Beitrag
  
-   [Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)  
-   [Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)  
-   [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)  
-   [Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)  
-   [Kapitel 4: Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)  
-   [Kapitel 5: Hochsicherheit (SSLF)](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx)  
-   Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen
  
**Download**
  
[Windows Vista-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=74028) (engl.)
  
**Update Notifications**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden.](http://go.microsoft.com/fwlink/?linkid=54982) (engl.)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen.](mailto:secwish@microsoft.com?subject=windows%20vista%20security%20guide) (engl.)

 
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
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx"><img src="images/Dd443743.pageLeft(de-de,TechNet.10).gif" /></a> 7 von 7</td>
</tr>
</tbody>
</table>
