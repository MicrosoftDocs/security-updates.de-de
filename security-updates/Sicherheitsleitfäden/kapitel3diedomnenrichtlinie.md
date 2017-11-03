---
TOCTitle: 'Kapitel 3: Die Domänenrichtlinie'
Title: 'Kapitel 3: Die Domänenrichtlinie'
ms:assetid: '70e3e562-9517-4fb9-b617-ef7854a0f03c'
ms:contentKeyID: 20075667
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443724(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 3: Die Domänenrichtlinie

Aktualisiert: 27.12.2005

#### Auf dieser Seite

[](#ehaa)[Überblick](#ehaa)  
[](#egaa)[Domänenrichtlinien](#egaa)  
[](#efaa)[Kontorichtlinien](#efaa)  
[](#eeaa)[Kennwortrichtlinien](#eeaa)  
[](#edaa)[Kontosperrungsrichtlinien](#edaa)  
[](#ecaa)[Kerberos-Richtlinien](#ecaa)  
[](#ebaa)[Sicherheitsoptionen](#ebaa)  
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

In diesem Kapitel wird anhand einer Domänenumgebung veranschaulicht, wie das Thema Sicherheit in einer Infrastruktur für Windows Server™ 2003 mit Service Pack 1 (SP1) bewältigt werden kann.

In diesem Kapitel werden v. a. folgende Themen behandelt:

-   Sicherheitseinstellungen und Gegenmaßnahmen auf Domänenebene.

-   Schützen einer Windows Server 2003-Domäne für Umgebungen mit älteren Clients, Unternehmensclient-Umgebungen und Hochsicherheitsumgebungen, die in Kapitel 1, „Einführung in das Windows Server 2003-Sicherheitshandbuch“, definiert sind.

Diese Informationen stellen eine Grundlage dar und geben Ihnen eine Vorstellung davon, wie Sie innerhalb einer Domäneninfrastruktur von einer Umgebung mit älteren Clients zu einer Hochsicherheitsumgebung wechseln können.

Windows Server 2003 mit SP1 wird mit bekannten, hochsicheren Standardwerten geliefert. Um die Dokumentation überschaubarer zu gestalten, werden in diesem Kapitel nur die Einstellungen behandelt, für die die Standardwerte geändert wurden. Weitere Informationen zu allen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx zur Verfügung steht.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Domänenrichtlinien

Gruppenrichtlinien-Sicherheitseinstellungen können auf unterschiedlichen Ebenen in einer Organisation angewendet werden. In der in Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, behandelten Baseline-Umgebung wurden Gruppenrichtlinien zum Anwenden von Einstellungen auf den folgenden drei Hierarchieebenen der Domäneninfrastruktur verwendet:

-   **Domänenebene**. Für allgemeine Sicherheitsanforderungen wie Konto- und Kennwortrichtlinien, die für alle Server in der Domäne erzwungen werden müssen.

-   **Baseline-Ebene**. Für auf alle Server im Netzwerk zutreffende, bestimmte Sicherheitsanforderungen.

-   **Rollenspezifische Ebene**. Für die Adresssicherheitsanforderungen bei spezifischen Serverrollen. Die Sicherheitsanforderungen für Infrastrukturserver unterscheiden sich z. B. von denen für Server, auf denen Microsoft Internet Information Services (IIS) ausgeführt werden.

In den folgenden Abschnitten dieses Kapitels werden nur die Richtlinien auf Domänenebene ausführlich behandelt. Die meisten beschriebenen Domänensicherheitseinstellungen dienen für Benutzerkonten und -kennwörter. Bedenken Sie beim Überprüfen dieser Einstellungen und Empfehlungen, dass sämtliche Einstellungen für jeden Benutzer innerhalb der Domänengrenze gelten.

#### Übersicht über die Domänenrichtlinie

Gruppenrichtlinien sind ein extrem leistungsstarkes Tool, da sie einem Administrator die Erstellung einer standardmäßigen Netzwerkcomputerkonfiguration ermöglichen. Gruppenrichtlinienobjekte (GPOs) können einen wesentlichen Bestandteil der Konfigurationsverwaltungslösung für jedes Unternehmen darstellen, da sie Administratoren ermöglichen, gleichzeitig auf allen Computern in der Domäne oder Teilmengen der Domäne Sicherheitsänderungen vorzunehmen.

Die folgenden Abschnitte bieten ausführliche Informationen zu den Sicherheitseinstellungen, die im Hinblick auf eine erhöhte Sicherheit von Windows Server 2003 mit SP1 verwendet werden können. In den Tabellen werden die Einstellungen zusammengefasst. Außerdem wird beschrieben, wie die Sicherheitsziele für die einzelnen Einstellungen erreicht werden können. Die Einstellungen sind in Kategorien unterteilt, die ihrer Darstellung in der Benutzeroberfläche des Sicherheitskonfigurations-Editors von Windows Server 2003 (SCE) entspricht.

Die folgenden Arten von Sicherheitsänderungen lassen sich durch die Gruppenrichtlinie gleichzeitig vornehmen:

-   Ändern von Berechtigungen im Dateisystem.

-   Ändern von Berechtigungen für Registrierungsobjekte.

-   Ändern von Einstellungen in der Registrierung.

-   Ändern der Zuweisungen von Benutzerrechten.

-   Konfigurieren von Systemdiensten.

-   Konfigurieren von Überwachungs- und Ereignisprotokollen.

-   Festlegen von Konto- und Kennwortrichtlinien.

In diesem Handbuch wird die Erstellung einer neuen Gruppenrichtlinie auf Domänenstammebene empfohlen, die auf die domänenweiten Richtlinien, die in diesem Handbuch besprochen werden, angewendet werden soll. Dadurch lässt sich die neue Gruppenrichtlinie leichter testen und korrigieren, da sie im Falle einer erforderlichen Rücknahme der Änderungen einfach deaktiviert werden kann. Manche für Active Directory konzipierte Anwendungen ändern jedoch die vordefinierte Standarddomänenrichtlinie. Diese Anwendungen nehmen die neue, von Ihnen implementierte Gruppenrichtlinie nicht zur Kenntnis, wenn Sie die Empfehlungen in diesem Handbuch befolgen. Vor dem Bereitstellen neuer Unternehmensanwendungen müssen Sie sie unbedingt sorgfältig testen. Sollten Probleme auftreten, überprüfen Sie, ob die Kontorichtlinien der Anwendung geändert, neue Benutzerkonten erstellt, Benutzerberechtigungen geändert oder sonstige Änderungen an der Standarddomänenrichtlinie oder an den lokalen Computerrichtlinien vorgenommen wurden.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Kontorichtlinien

Kontorichtlinien (Sicherheitseinstellungen für Kennwortrichtlinien, Kontosperrungsrichtlinien und Kerberos-Richtlinien) sind nur in der Domänenrichtlinie für die drei hier beschriebenen Umgebungen relevant. Kennwortrichtlinien dienen zum Festlegen der Komplexität und Ändern der Pläne für Kennwörter in hochsicheren Umgebungen. Kontosperrungsrichtlinien ermöglichen die Verfolgung von fehlgeschlagenen Anmeldeversuchen, um bei Bedarf Kontosperrungen zu initiieren. Kerberos-Richtlinien werden für Benutzerkonten in einer Domäne verwendet. Sie bestimmen die Einstellungen für das Kerberos-Authentifizierungsprotokoll, wie etwa Gültigkeitsdauer und Durchsetzung von Tickets.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Kennwortrichtlinien

Komplexe Kennwörter, die regelmäßig geändert werden, verringern die Wahrscheinlichkeit eines erfolgreichen Kennwortangriffs. Die Einstellungen der Kennwortrichtlinien steuern die Komplexität und Gültigkeitsdauer von Kennwörtern. In diesem Abschnitt werden alle spezifischen Kennwortrichtlinieneinstellungen und deren Verwendung in den drei in diesem Handbuch definierten Umgebungen beschrieben: die Umgebung mit älteren Clients, die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung.

Strikte Anforderungen für die Kennwortlänge und –komplexität führen nicht automatisch dazu, dass Benutzer und Administratoren sichere Kennwörter verwenden. Obwohl Benutzer aufgrund der Kennwortrichtlinie möglicherweise technische Komplexitätsanforderungen einhalten müssen, ist eine zusätzliche starke Sicherheitsrichtlinie erforderlich, um sicherzustellen, dass Benutzer Kennwörter erstellen, die sicher sind. So würde „Frühstück!“ zwar sämtliche Komplexitätsanforderungen an das Kennwort erfüllen, es wäre aber nicht sehr schwer zu knacken.

Wenn Sie bestimmte Dinge über den Ersteller eines Kennworts wissen, können Sie das Kennwort möglicherweise erraten, wenn Sie sein Lieblingsessen, -auto oder -film kennen. Eine Strategie unternehmensweiter Sicherheitsprogramme, die Benutzer zum Einsatz sicherer Kennwörter anhalten, ist die Erstellung eines Posters mit schlechten Kennwörtern, das dann in Gemeinschaftsräumen, etwa beim Wasserspender oder Kopierer, aufgehängt wird. Ihr Unternehmen sollte beim Erstellen sicherer Kennwortrichtlinien Folgendes beachten:

-   Vermeiden Sie den Gebrauch von Wörtern aus einem Wörterbuch in irgendeiner Sprache, einschließlich häufiger oder raffinierter Falschschreibungen der Wörter.

-   Erstellen Sie kein neues Kennwort, das im Gegensatz zum alten einfach eine neue Ziffer enthält.

-   Vermeiden Sie die Verwendung von Kennwörtern, die mit einer Zahl beginnen oder enden, da sie leichter erraten werden können, als Kennwörter mit einer Zahl in der Mitte.

-   Verwenden Sie keine Kennwörter, die andere durch einen Blick auf Ihren Arbeitsplatz leicht erraten können (Namen von Haustieren, Sportteams und Familienmitgliedern).

-   Verwenden Sie keine Wörter aus dem populären Sprachgebrauch.

-   Ermutigen Sie Benutzer zur Verwendung von Kennwörtern, die sie auf der Tastatur mit beiden Händen eingeben müssen.

-   Ermutigen Sie Benutzer in allen Kennwörtern zur Verwendung von Groß- und Kleinbuchstaben, Zahlen und Symbolen.

-   Ermutigen Sie Benutzer zur Verwendung von Leerzeichen und Zeichen, die nur mithilfe der ALT-Taste erzeugt werden können.

Verwenden Sie diese Richtlinien auch für alle Dienstkontenkennwörter in Ihrem Unternehmen.

#### Kennwortrichtlinieneinstellungen

In der folgenden Tabelle sind Empfehlungen zur Kennwortrichtlinieneinstellung für alle drei in diesem Handbuch enthaltenen Umgebungen enthalten: Die Kennwortrichtlinieneinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Kontorichtlinien\\Kennwortrichtlinien**

Weitere Informationen zu den einzelnen Einstellungen erhalten Sie in den nach der Tabelle angeführten Unterabschnitten.

**Tabelle 3.1 Empfehlungen zur Kennwortrichtlinieneinstellung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kennwortchronik erzwingen</td>
<td style="border:1px solid black;">Erinnerung an 24 Kennwörter</td>
<td style="border:1px solid black;">Erinnerung an 24 Kennwörter</td>
<td style="border:1px solid black;">Erinnerung an 24 Kennwörter</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Maximales Kennwortalter</td>
<td style="border:1px solid black;">42 Tage</td>
<td style="border:1px solid black;">42 Tage</td>
<td style="border:1px solid black;">42 Tage</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Minimales Kennwortalter</td>
<td style="border:1px solid black;">1 Tag</td>
<td style="border:1px solid black;">1 Tag</td>
<td style="border:1px solid black;">1 Tag</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Minimale Kennwortlänge</td>
<td style="border:1px solid black;">8 Zeichen</td>
<td style="border:1px solid black;">8 Zeichen</td>
<td style="border:1px solid black;">12 Zeichen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Kennwörter müssen den Komplexitätsanforderungen entsprechen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kennwort mit umkehrbarer Verschlüsselung speichern</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
#### Kennwortchronik erzwingen
  
Diese Richtlinieneinstellung legt die Anzahl eindeutiger neuer Kennwörter fest, die mit einem Benutzerkonto verbunden werden müssen, bevor ein altes Kennwort erneut verwendet werden darf. Der Wert kann auf 0 bis 24 Kennwörter eingestellt werden.
  
Der Standardwert unter Windows Server 2003 mit SP1 für die Einstellung **Kennwortchronik erzwingen** ist mit 24 Kennwörtern der Höchstwert. Microsoft empfiehlt diesen Wert für alle drei Umgebungen, weil dadurch sichergestellt wird, dass alte Kennwörter nicht immer wieder verwendet werden. Die häufigsten Sicherheitsanfälligkeiten sind nämlich mit der erneuten Verwendung von Kennwörtern verbunden. Außerdem ermöglicht eine niedrige Zahl bei dieser Einstellung die fortwährende Verwendung einiger weniger Kennwörter. In Zusammenhang mit Empfehlungen für Umgebungen mit älteren Clients sind darüber hinaus keine Probleme bekannt.
  
Um die Wirksamkeit dieser Richtlinieneinstellung zu erhöhen, können Sie auch die Einstellung **Minimales Kennwortalter** so konfigurieren, dass Kennwörter nicht sofort geändert werden können. Diese Kombination erschwert es Benutzern, Kennwörter versehentlich oder absichtlich wiederzuverwenden.
  
#### Maximales Kennwortalter
  
Diese Richtlinieneinstellung bestimmt, wie lange ein entschlüsseltes Kennwort von einem Angreifer verwendet werden kann, um auf einen Computer im Netzwerk zuzugreifen. Gültiger Wertebereich für diese Richtlinieneinstellung: 1 bis 365 Tage. Sie können die Einstellung **Maximales Kennwortalter** so konfigurieren, dass Kennwörter so oft ablaufen, wie es Ihre Umgebung erforderlich macht. Der Standardwert für diese Einstellung ist 42 Tage.
  
Regelmäßige Änderungen des Kennworts können verhindern, dass Kennwörter beeinträchtigt werden. Die meisten Kennwörter können entschlüsselt werden, wenn dem Angreifer ausreichend Zeit und Verarbeitungsleistung zur Verfügung steht. Je häufiger Kennwörter geändert werden, desto weniger Zeit bleibt einem Angreifer, das Kennwort zu knacken. Je niedriger der Wert eingestellt ist, desto höher ist jedoch die Wahrscheinlichkeit vermehrter Anfragen beim Helpdesk Ihrer IT-Abteilung.
  
Microsoft empfiehlt, die Einstellung **Maximales Kennwortalter** für alle drei in diesem Handbuch definierten Umgebungen bei ihrem Standardwert von 42 Tagen zu belassen. Diese Konfiguration sorgt dafür, dass Kennwörter regelmäßig geändert werden, erfordert jedoch nicht von den Benutzern, das Kennwort so oft zu ändern, dass sie sich nicht mehr daran erinnern können. Um ein gutes Verhältnis zwischen Sicherheit und Benutzerfreundlichkeit zu schaffen, können Sie den Wert für diese Richtlinieneinstellung in Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen erhöhen.
  
#### Minimales Kennwortalter
  
Diese Richtlinieneinstellung bestimmt die Anzahl der Tage, die ein Kennwort verwendet werden muss, bevor es ein Benutzer ändern kann. Der Wertebereich für die Einstellung **Minimales Kennwortalter** liegt zwischen 0 und 999 Tagen; ein Wert von 0 gestattet die sofortige Änderung eines Kennworts. Der Standardwert für diese Einstellung ist ein Tag.
  
Der Wert von **Minimales Kennwortalter** muss kleiner sein als der Wert von **Maximales Kennwortalter**, sofern die Einstellung **Maximales Kennwortalter** nicht als **0** konfiguriert ist. In dem Fall würde das Kennwort nie ablaufen. Konfigurieren Sie die Einstellung **Minimales Kennwortalter** so, dass der Wert größer als 0 ist, wenn **Kennwortchronik erzwingen** verwendet werden soll. Ohne Angabe eines minimalen Kennwortalters können Benutzer alte Lieblingskennwörter immer wieder verwenden.
  
Microsoft empfiehlt, dass Sie die Standardeinstellung für **Minimales Kennwortalter** von einem Tag für alle drei in diesem Handbuch definierten Umgebungen erzwingen. Wenn diese Einstellung in Verbindung mit einem ähnlichen niedrigen Wert unter **Kennwortchronik erzwingen** verwendet wird, können Benutzer dieselben Kennwörter immer wieder verwenden. Wird z. B. **Minimales Kennwortalter** auf einen Tag gesetzt und **Kennwortchronik erzwingen** als zwei Kennwörter konfiguriert, müssten Benutzer nur zwei Tage warten, bis Sie ein altes Lieblingskennwort wieder verwenden können. Wird **Minimales Kennwortalter** jedoch auf einen Tag gesetzt und **Kennwortchronik erzwingen** auf 24 Tage, müssten Benutzer Ihr Kennwort 24 Tage lang täglich ändern, bevor sie es wiederverwenden können, was sehr unwahrscheinlich ist.
  
#### Minimale Kennwortlänge
  
Durch diese Richtlinieneinstellung wird sichergestellt, dass Kennwörter eine Mindestzeichenanzahl aufweisen. Lange Kennwörter mit acht oder mehr Zeichen sind stärkere Kennwörter als kurze. Bei Einsatz der Einstellung **Minimale Kennwortlänge** können Benutzer keine leeren Kennwörter verwenden, sondern müssen Kennwörter mit einer bestimmten Anzahl an Zeichen erstellen. Der Standardwert für diese Einstellung ist sieben Zeichen.
  
Es wird empfohlen, dass Sie die **Minimale Kennwortlänge** für Umgebungen mit älteren Clients und Unternehmensclients auf acht Zeichen konfigurieren. Diese Konfiguration ist lang genug, um eine zufrieden stellende Sicherheitsebene zu gewährleisten, und kurz genug, um sie leicht in Erinnerung zu behalten. Außerdem stellt diese Konfiguration einen angemessenen Schutz gegen die häufigen Wörterbuch- oder Brute-Force-Angriffe dar.
  
(Wörterbuchangriffe versuchen anhand von Wortlisten, das Kennwort aufzudecken. Bei Brute-Force-Angriffen wird jedes mögliche Kennwort oder sonstige verschlüsselte Textwerte ausprobiert. Die Wahrscheinlichkeit eines Brute-Force-Angriffs auf das Kennwort hängt von der Kennwortlänge, der Größe des möglichen Zeichensatzes und der dem Hacker zur Verfügung stehenden Verarbeitungsleistung ab.)
  
Es wird empfohlen, die Einstellung **Minimale Kennwortlänge** in Clients mit Hochsicher-Umgebung auf zwölf Zeichen einzurichten.
  
Durch jedes zusätzliche Zeichen in einem Kennwort wird dessen Komplexität exponentiell erhöht. So gibt es für ein Kennwort mit sieben Zeichen 267 bzw. 1 x 107 mögliche Kombinationen. Ein alphabetisches Kennwort mit sieben Zeichen unter Berücksichtigung der Groß- und Kleinschreibung weist 527 Kombinationen auf. Für ein Kennwort aus sieben Buchstaben ohne Interpunktionszeichen sind bei Beachtung der Groß-/Kleinschreibung 627 Kombinationen möglich. Bei 1.000.000 Versuchen pro Sekunde würde es ca. 40 Tage dauern, dieses Kennwort zu entschlüsseln. Für ein aus acht Zeichen bestehendes Kennwort sind 268 oder 2 x 1011 Kombinationen möglich. Obwohl dies eine unwahrscheinlich große Anzahl zu sein scheint, werden bei 1.000.000 Versuchen pro Sekunde (dies ist bei vielen Entschlüsselungsanwendungen möglich) nur 59 Stunden benötigt, bis alle möglichen Kennwörter ausprobiert wurden. Bedenken Sie, dass diese Zeiten beträchtlich höher sind, wenn in den Kennwörtern ALT- und andere Sonderzeichen wie z. B. ! oder @ verwendet werden.
  
Kennwörter werden in der Datenbank der Sicherheitskontenverwaltung (SAM) oder in Active Directory gespeichert, nachdem sie durch einen unidirektionalen Hashalgorithmus geleitet wurden. Wenn Sie feststellen möchten, ob Sie das richtige Kennwort verwenden, muss das Kennwort denselben unidirektionalen Hashingalgorithmus durchlaufen. Anschließend vergleichen Sie das Ergebnis. Bei Wörterbuchangriffen werden auf der Suche nach Übereinstimmungen ganze Wörterbücher durch den Verschlüsselprozess gesendet. Diese Angriffe sind ein sehr einfacher, aber doch effektiver Ansatz, um festzustellen, wer allgemeine Wörter wie „Kennwort“ oder „Gast“ als Kontokennwort verwendet.
  
Ältere Versionen von Windows haben einen bestimmten Hashingalgorithmus verwendet, der als LAN Manager-Hash (LMHash) bezeichnet wird. Dieser Algorithmus löst das Kennwort in Blöcke mit sieben oder weniger Zeichen auf und berechnet dann einen getrennten Hashwert für jeden Block. Obwohl Windows 2000 Server, Windows XP und Windows Server 2003 einen neueren Hashingalgorithmus verwenden, können sie den LMHash weiterhin anhand der Abwärtskompatibilität speichern und berechnen.
  
Wenn die LMHashwerte vorhanden sind, stellen sie eine Verknüpfung für Kennwörterangriffe dar. Bei einem Kennwort mit sieben oder weniger Zeichen wird die zweite Hälfte des LMHash in einen bestimmten Wert aufgelöst, an dem ein Angreifer erkennen kann, dass das Kennwort aus weniger als acht Zeichen besteht. Durch Kennwörter mit einer Länge von mindestens acht Zeichen wird selbst ein schwächerer LMHash gestärkt, da Angreifer bei längeren Kennwörtern zwei Teile entschlüsseln müssen und nicht nur einen. Es ist möglich, beide Hälften eines LMHash parallel anzugreifen; die zweite Hälfte des LMHash ist nur ein Zeichen lang. Bei einem Brute-Force-Angriff kann dieses Zeichen in Millisekunden entschlüsselt werden. Es ist daher nur dann sinnvoll, wenn das Zeichen zum ALT-Zeichensatz gehört.
  
Aus diesen Gründen wird von der Verwendung kürzerer Kennwörter abgeraten. Mindestlängenanforderungen, die zu lang sind, können jedoch falsch eingegebene Kennwörter zur Folge haben, was wiederum zu einer Zunahme gesperrter Konten und Helpdeskanfragen führen könnte. Darüber hinaus kann die Forderung übermäßig langer Kennwörter in der Tat auch zu einer Verringerung der Sicherheit eines Unternehmens führen: Die Benutzer schreiben ihre Kennwörter eher auf, um sie nicht zu vergessen.
  
#### Kennwörter müssen den Komplexitätsanforderungen entsprechen
  
Diese Richtlinieneinstellung prüft alle neuen Kennwörter bei deren Erstellung, damit sichergestellt wird, dass sie den Komplexitätsanforderungen entsprechen. Die Richtlinienregeln von Windows Server 2003 können nicht direkt geändert werden. Sie können jedoch eine neue Version der Datei Passfilt.dll erstellen, um einen anderen Regelsatz anzuwenden. Weitere Informationen zum Erstellen einer benutzerdefinierten Passfilt.dll-Datei finden Sie im MSDN®-Artikel über „[Beispielkennwortfilter](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/secmgmt/security/sample_password_filter.asp)“ (in englischer Sprache) unter http://msdn.microsoft.com/library/default.asp?url=/library/en-us/secmgmt/  
security/sample\_password\_filter.asp.
  
Sie können auch Kennwörter mit 20 oder mehr Zeichen verwenden – diese sind möglicherweise für den Benutzer leichter zu merken, und sie sind sicherer als Kennwörter, die aus acht Zeichen bestehen. Nehmen Sie z. B. das 32 Zeichen lange Kennwort: **Ich esse Hamburger für 0.99€** Dieses Kennwort (oder "Kennsatz") ist für den Benutzer wahrscheinlich leichter zu merken als ein kürzeres Kennwort wie P**@55w0rt**.
  
In Kombination mit einer **Minimalen Kennwortlänge** von 8 kann diese Einstellung einen Brute-Force-Angriff beträchtlich erschweren. Wenn Sie Groß- und Kleinbuchstaben sowie Zahlen miteinbeziehen, mit einschließen, erhöht sich die Zahl der verfügbaren Zeichen von 26 auf 62 Zeichen. Für ein aus acht Zeichen bestehendes Kennwort gibt es dann 2,18 x 1014 mögliche Kombinationen. Bei 1.000.000 Versuchen pro Sekunde würden es 6,9 Jahre dauern, alle Möglichkeiten auszuprobieren.
  
Aus diesen Gründen empfiehlt Microsoft, dass die Einstellung **Kennwort muss Komplexitätsvoraussetzungen entsprechen** für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt wird.
  
#### Kennwort mit umkehrbarer Verschlüsselung speichern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob das Betriebssystem Kennwörter mit umkehrbarer Verschlüsselung speichert. Sie unterstützt Anwendungen mit Protokollen, die das Benutzerkennwort zu Authentifizierungszwecken anfordern.
  
Kennwörter, die mit einer umkehrbaren Verschlüsselungsmethode gespeichert sind, können leichter abgerufen werden, als Kennwörter, die mit nicht umkehrbarer Verschlüsselung gespeichert wurden. Wenn diese Einstellung aktiviert wird, ist die Sicherheitsanfälligkeit erhöht.
  
Aus diesem Grund empfiehlt Microsoft, dass Sie die Einstellung **Kennwort mit umkehrbarer Verschlüsselung speichern** auf **Deaktiviert** setzen, sofern nicht die Anwendungsanforderungen wichtiger als der Schutz von Kennwortinformationen sind. Umgebungen, die das CHAP-Protokoll (Challenge Handshake Authentication) über Remotezugriff oder IAS bereitstellen und Umgebungen, die die Digestauthentifizierung für Internet Information Services (IIS) verwenden, müssen diese Richtlinieneinstellung aktivieren.
  
#### Sicherstellen, dass Kennwörter nur auf Anforderung von Benutzern geändert werden können
  
Obwohl die im vorigen Abschnitt erläuterten Kennwortrichtlinieneinstellungen eine Reihe von Optionen bieten, benötigen einige Unternehmen eine zentrale Steuerung aller Benutzer. In diesem Abschnitt wird beschrieben, wie Benutzer daran gehindert werden können, ihr Kennwort zu ändern, sofern die Änderungen nicht ausdrücklich erforderlich sind.
  
Die zentralisierte Steuerung der Benutzerkennwörter ist ein Grundstein in einem gut gestalteten Windows Server 2003-Sicherheitsschema. Mithilfe von Gruppenrichtlinien können die zuvor beschriebenen minimalen und maximalen Kennwortalter festgelegt werden. Bedenken Sie jedoch, dass Benutzer durch häufige Kennwortänderungen in der Lage sind, die Kennwortchronikeinstellung für Ihre Umgebung zu umgehen. Auch kann die Forderung nach zu langen Kennwörtern vermehrte Helpdeskanfragen von Benutzern verursachen, die ihr Kennwort vergessen haben.
  
Benutzer können ihre Kennwörter innerhalb des durch die Einstellungen für das minimale und maximale Kennwortalter festgelegten Zeitraums ändern. Die Struktur der Hochsicher-Umgebung erfordert es jedoch, dass Benutzer ihre Kennwörter nur dann ändern, wenn sie nach Ablauf der Einstellung **Maximales Kennwortalter** von 42 Tagen vom Betriebssystem dazu aufgefordert werden. Um zu verhindern, dass Benutzer ihre Kennwörter ändern (außer wenn sie dazu aufgefordert werden), können Sie die Option **Kennwort ändern** im Dialogfeld **Windows-Sicherheit**, das durch Drücken auf STRG+ALT+ENTF angezeigt wird, deaktivieren. Benutzer mit hohen Sicherheitsanforderungen möchten möglicherweise ihr Kennwort öfter ändern und müssen sich dazu an einen Administrator wenden, wodurch wiederum die Supportkosten erhöht werden.
  
Sie können diese Konfiguration für eine ganze Domäne durch die Gruppenrichtlinie implementieren, oder Sie können die Registrierung bearbeiten und sie für einen oder mehrere bestimmte Benutzer implementieren. Ausführlichere Anweisungen zu dieser Konfiguration finden Sie im Microsoft Knowledge Base-Artikel „[SO WIRD'S GEMACHT: Kennwortänderungen durch Benutzer nur zulassen, wenn dies in Windows Server 2003 erforderlich ist](http://support.microsoft.com/?kbid=324744)“ unter http://support.microsoft.com/?kbid=324744.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Kontosperrungsrichtlinien
  
Die Kontosperrungsrichtlinie ist eine Sicherheitsfunktion von Windows Server 2003 mit SP1, das ein Benutzerkonto nach einer bestimmten Anzahl von fehlgeschlagenen Anmeldeversuchen innerhalb eines definierten Zeitraums sperrt. Die Anzahl der Versuche und der Zeitraum werden durch in der Richtlinie konfigurierte Werte festgelegt. Windows Server 2003 mit SP1 verfolgt Anmeldeversuche, und die Serversoftware kann zum Verhindern von Angriffen dieser Art so konfiguriert werden, dass Konten nach einer voreingestellten Anzahl von fehlgeschlagenen Anmeldeversuchen als Reaktion auf potenzielle Angriffe deaktiviert werden.
  
Diese Richtlinieneinstellungen helfen beim Schützen von Benutzerkennwörtern vor Angreifern, die Kennwörter erraten, und minimieren die Wahrscheinlichkeit erfolgreicher Angriffe auf Ihr Netzwerk. Sie haben jedoch mit höheren Supportkosten zu rechnen, wenn Sie die Kontosperrungsrichtlinie aktivieren, da Benutzer, die das Kennwort vergessen oder falsch eingetippt haben, Ihre Unterstützung benötigen. Bevor Sie die folgenden Einstellungen aktivieren, stellen Sie sicher, dass Ihr Unternehmen bereit ist, diesen zusätzlichen Verwaltungs- und Verarbeitungsaufwand zu übernehmen. Für viele Unternehmen besteht eine verbesserte und kostengünstigere Lösung in der automatischen Überwachung der Sicherheitsereignisprotokolle für Domänencontroller und der Erstellung administrativer Warnmeldungen, wenn offensichtliche Versuche unternommen wurden, die Kennwörter der Benutzerkonten zu erraten. In Kapital 2, „Richtlinien auf Domänenebene“, des Begleithandbuchs [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) finden Sie eine zusätzliche Erörterung dieser Einstellungen und ihrer Auswirkungen aufeinander.
  
#### Einstellungen der Kontosperrungsrichtlinie
  
In der folgenden Tabelle werden die empfohlenen Einstellungen der Kontosperrungsrichtlinie zusammengefasst. Sie können zum Konfigurieren dieser Einstellungen den Gruppenrichtlinienobjekt-Editor in der Domänengruppenrichtlinie in folgendem Verzeichnis verwenden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Kontorichtlinien\\Kontosperrungsrichtlinien**
  
Weitere Informationen zu den einzelnen Einstellungen erhalten Sie in den nach der Tabelle angeführten Unterabschnitten.
  
**Tabellen 3.2 Einstellungen der Kontosperrungsrichtlinie**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Kontosperrdauer</td>
<td style="border:1px solid black;">30 Minuten</td>
<td style="border:1px solid black;">30 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Kontensperrungsschwelle</td>
<td style="border:1px solid black;">50 ungültige Anmeldungsversuche</td>
<td style="border:1px solid black;">50 ungültige Anmeldungsversuche</td>
<td style="border:1px solid black;">10 ungültige Anmeldungsversuche</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zurücksetzungsdauer des Kontosperrungszählers</td>
<td style="border:1px solid black;">30 Minuten</td>
<td style="border:1px solid black;">30 Minuten</td>
<td style="border:1px solid black;">15 Minuten</td>
</tr>
</tbody>
</table>
  
#### Kontosperrdauer
  
Diese Richtlinieneinstellung bestimmt die Zeitdauer, bevor ein Konto entsperrt wird und ein Benutzer einen neuerlichen Anmeldungsversuch starten kann. Sie legt die Anzahl an Minuten fest, die ein gesperrtes Konto unverfügbar ist. Wenn Sie den Wert **Kontosperrdauer** auf null setzen, bleiben Konten solange gesperrt, bis ein Administrator sie entsperrt. In Windows Server 2003 mit SP1 lautet der Standardwert für diese Einstellung **Nicht definiert**.
  
Obwohl es sich als gute Idee erweisen mag, die Einstellung **Kontosperrdauer** so zu konfigurieren, dass sie nie automatisch entsperrt wird, erhöht eine solche Konfiguration die Zahl der Helpdeskanfragen zum Entsperren von Konten, die irrtümlicherweise gesperrt wurden.
  
In diesem Handbuch wird empfohlen, dass Sie die Einstellung **Kontosperrdauer** für Ältere Clients und Unternehmensclients auf **30 Minuten** und für Hochsicher-Umgebungen auf **15 Minuten** setzen. Dadurch wird der Overhead während einer DoS-Attacke verringert. Bei einer DoS-Attacke führt ein Angreifer böswillig eine Reihe von fehlgeschlagenen Anmeldeversuchen für alle Benutzer im Unternehmen aus, um deren Konten zu sperren. Die empfohlenen Einstellungen geben gesperrten Benutzern auch die Möglichkeit, sich nach einer angemessenen Zeitdauer erneut anzumelden, ohne sich an den Helpdesk wenden zu müssen. Informationen zu diesem Einstellungswert müssen allerdings den Benutzern mitgeteilt werden.
  
#### Kontensperrungsschwelle
  
Diese Richtlinieneinstellung legt die Anzahl an Anmeldeversuchen fest, die ein Benutzer unternehmen kann, bevor das Konto gesperrt wird.
  
Autorisierte Benutzer können ihr Konto auf verschiedene Weisen selbst sperren. Sie können ihr Kennwort falsch eingeben oder es auf einem Computer ändern, während Sie bei einem anderen Computer angemeldet sind. Der Computer mit dem falschen Kennwort versucht fortlaufend, den Benutzer zu authentifizieren, und weil das zum Authentifizieren verwendete Kennwort falsch ist, wird das Benutzerkonto schließlich gesperrt. Legen Sie für die **Kontosperrungsschwelle** einen hohen Wert fest, um die Sperrung autorisierter Benutzer zu vermeiden.
  
Da sowohl bei einem konfigurierten wie auch bei einem nicht konfigurierten Wert für die Einstellung **Kontosperrungsschwellen** ein Sicherheitsrisiko besteht, sind für diese beiden Möglichkeiten Gegenmaßnahmen definiert. Je nach den erkannten Risiken, die Ihr Unternehmen zu verringern versucht, sollten Sie sich für eine dieser beiden Möglichkeiten entscheiden.
  
-   Zum Verhindern von Kontosperrungen setzen Sie **Kontensperrungsschwelle** auf 0. Durch diese Konfiguration werden auch die Anfragen beim IT-Helpdesk vermindert, da Benutzer ihre Konten nun nicht mehr versehentlich sperren können. Außerdem schlagen DoS-Attacken, die absichtlich Kontensperrungen in Ihrem Unternehmen hervorzurufen versuchen, fehl. Da Brute-Force-Angriffe hierdurch nicht verhindert werden, sollte diese Einstellung nur verwendet werden, wenn die beiden folgenden Kriterien explizit erfüllt sind:
  
    -   Durch die Kennwortrichtlinien werden alle Benutzer angehalten, komplexe Kennwörter mit acht oder mehr Zeichen zu verwenden.
  
    -   Ein wirksamer Überwachungsmechanismus kann Administratoren vor dem Auftreten mehrerer fehlgeschlagener Anmeldeversuche in der Umgebung warnen. Die Überwachungslösung sollte z. B. das Auftreten des Sicherheitsereignisses 539 „Anmeldungsfehler. Das Konto wurde beim Anmeldeversuch gesperrt“ überwachen. Dieses Ereignis gibt an, dass das Konto bei einem Anmeldeversuch gesperrt wurde. Ereignis 539 zeigt jedoch nicht die fehlgeschlagene Eingabe eines Kennworts an, sondern nur eine Kontosperrung. Daher sollten die Administratoren auch überwachen, ob wiederholt falsche Kennwörter eingegeben werden.
  
-   Wenn diese Kriterien nicht erfüllt werden, kann als zweite Option die Einstellung **Kontensperrungsschwelle** auf einen so hohen Wert eingestellt werden, dass der Benutzer sein Kennwort mehrmals falsch eingeben kann, ohne dass das Konto gesperrt wird. Durch den Wert ist jedoch sichergestellt, dass das Konto bei einem Brute-Force-Angriff gesperrt wird.
  
Es wird empfohlen, dass Sie die Einstellung **Kontensperrungsschwelle** für Umgebungen mit älteren Clients und Unternehmensclients auf **50** setzen, wodurch angemessene Sicherheit und akzeptable Verwendbarkeit gewährleistet werden. Durch diesen Wert werden zwar versehentliche Kontosperrungen und entsprechende Anfragen beim IT-Helpdesk verringert, ein wie zuvor beschriebener Denial-of-Service-Angriff kann jedoch nicht verhindert werden. Es wird allerdings empfohlen, diesen Richtlinieneinstellungswert für Hochsicher-Umgebungen auf **10** zu setzen.
  
#### Zurücksetzungsdauer des Kontosperrungszählers
  
Diese Richtlinieneinstellung bestimmt die Zeitdauer, bevor die **Kontosperrungsschwelle** auf null zurückgesetzt und das Konto entsperrt wird. Wenn Sie eine **Kontensperrungsschwelle** festlegen, muss dieser Zurücksetzungszeitraum kleiner als oder gleich dem Wert von **Kontosperrdauer** sein.
  
Die Einstellung **Zurücksetzungsdauer des Kontosperrungszählers** funktioniert in Verbindung mit anderen Einstellungen. Wenn Sie die Standardeinstellung dieses Wertes übernehmen oder ihn für ein zu langes Intervall konfigurieren, wird die Umgebung möglicherweise für DoS-Attacken anfällig. Wenn für das Zurücksetzen der Kontosperrung keine Richtlinieneinstellung festgelegt wird, müssen Administratoren die Sperrung aller Konten manuell aufheben. Umgekehrt kann durch das Festlegen eines geeigneten Zeitwerts erreicht werden, dass die Benutzerkonten nur für einen definierten Zeitraum gesperrt werden und die Sperrung anschließend automatisch wieder aufgehoben wird.
  
Es wird empfohlen, dass Sie die **Zurücksetzungsdauer des Kontosperrungszählers** für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf 30 Minuten konfigurieren. Mit dieser Konfiguration wird ein angemessener Zeitraum festgelegt, den Benutzer eher akzeptieren, ohne die Unterstützung des Helpdesk in Anspruch nehmen zu müssen. Es wird jedoch empfohlen, diese Richtlinieneinstellung für Hochsicher-Umgebungen auf 15 zu setzen.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Kerberos-Richtlinien
  
Kerberos-Richtlinien werden für Benutzerkonten in einer Domäne verwendet. Durch diese Richtlinien werden Einstellungen festgelegt, die sich auf das Authentifizierungsprotokoll Kerberos Version 5, wie etwa Gültigkeitsdauer und Durchsetzung von Tickets, beziehen. In der Richtlinie für den lokalen Computer werden keine Kerberos-Richtlinien verwendet. Wenn Sie die Gültigkeit von Kerberos-Tickets verringern, wird die Gefahr eines Angriffs, bei dem durch Kennwortdiebstahl die Identität gültiger Benutzerkonten angenommen wird, verringert. Allerdings wird durch die Verwaltung dieser Richtlinien der Verwaltungsaufwand für Autorisierungen höher.
  
In den meisten Umgebungen sollten die Standardwerte für die Richtlinien nicht geändert werden. Da die Kerberos-Einstellungen in der Standarddomänenrichtlinie berücksichtigt und dort angewendet werden, sind sie in den mit diesem Handbuch gelieferten Sicherheitsvorlagen nicht enthalten.
  
Es wird empfohlen, keine Änderungen an den Standardrichtlinien von Kerberos vorzunehmen. Weitere Informationen zu diesen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx zur Verfügung steht.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Sicherheitsoptionen
  
Die drei unterschiedlichen, zuvor in diesem Kapitel erläuterten Kontenrichtlinienarten werden auf Domänenebene festgelegt und durch sämtliche Domänencontroller in der Domäne umgesetzt. Ein Domänencontroller erhält die Kontorichtlinie stets vom Gruppenrichtlinienobjekt der Standarddomänenrichtlinie. Dies gilt auch, wenn auf die Organisationseinheit des Domänencontrollers eine andere Kontorichtlinie angewendet wird.
  
Es gibt drei Sicherheitsoptionseinstellungen, die Kontenrichtlinien ähnlich sind. Es empfiehlt sich, diese Einstellungen auf Ebene der gesamten Domäne und nicht innerhalb einzelner Organisationseinheiten anzuwenden. Sie können diese Einstellungen im Gruppenrichtlinienobjekt-Editor an folgender Stelle konfigurieren:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Sicherheitsoptionen**
  
#### Einstellungen der Sicherheitsoptionen
  
Die folgende Tabelle fasst die empfohlenen Sicherheitsoptionseinstellungen zusammen. Weitere Informationen zu den einzelnen Einstellungen erhalten Sie in den nach der Tabelle angeführten Unterabschnitten.
  
**Tabelle 3.3 Sicherheitsoptionseinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
#### Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Verbindungen zu Benutzern getrennt werden, wenn diese außerhalb der für ihr Konto gültigen Anmeldezeiten mit dem lokalen Computer verbunden sind. Diese Richtlinieneinstellung betrifft die SMB-Komponente (Server Message Block). Ist sie aktiviert, werden Clientsitzungen mit dem SMB-Dienst beendet, wenn die Anmeldezeit des Clients abgelaufen ist. Ist sie deaktiviert, wird eine bestehende Clientsitzung nach Ablauf der Anmeldezeit des Clients aufrechterhalten. Wenn Sie diese Richtlinieneinstellung aktivieren, sollten Sie auch die Einstellung **Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen** aktivieren.
  
Wenn Ihr Unternehmen Anmeldezeiten für Benutzer konfiguriert, liegt es nahe, die Einstellung **Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird** zu aktivieren. Andernfalls können Benutzer, die außerhalb ihrer Anmeldezeiten keinen Zugriff auf das Netzwerk haben sollen, diese Ressourcen über während der zulässigen Verbindungszeit eingerichteten Sitzungen weiter verwenden.
  
Es wird empfohlen, die Einstellung **Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird** für die drei in diesem Handbuch definierten Umgebungen als **Aktiviert** zu konfigurieren. Diese Richtlinieneinstellung hat keine Auswirkungen, wenn keine Anmeldezeiten festgelegt wurden.
  
#### Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein anonymer Benutzer die SID für einen anderen Benutzer anfordern kann.
  
Ist die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** auf einem Domänencontroller aktiviert ist, könnte ein Benutzer mit Kenntnis der standardmäßigen SID-Attribute eines Administrators eine Verbindung mit einem Computer herstellen, auf dem diese Richtlinie ebenfalls aktiviert ist, und die SID dann verwenden, um an den Namen des Administrators zu gelangen. Diese Person könnte den Kontonamen dann zum Erraten des Kennworts verwenden.
  
Weil die Standardkonfiguration für die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** auf Computern von Mitgliedern **Deaktiviert** ist, sind diese von dieser Richtlinieneinstellung nicht betroffen. Die Standardkonfiguration für Domänencontroller lautet jedoch **Aktiviert**. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Computer, auf denen ältere Betriebssysteme ausgeführt werden, möglicherweise nicht mit Domänen kommunizieren, die auf Windows Server 2003 mit SP1 basieren. Zu diesen Computern zählen:
  
-   Microsoft Windows NT® 4.0-basierte RAS-Dienstserver.
  
-   Microsoft SQL Server™, die auf Windows NT 3. x- oder Windows NT 4.0–basierten Computern ausgeführt werden.
  
-   RAS-Server auf Windows 2000-basierten Computern in Windows NT 3.x-Domänen bzw. Windows NT 4.0-Domänen.
  
Es wird empfohlen, dass Sie die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** für alle drei in diesem Handbuch definierten Umgebungen als **Deaktiviert** konfigurieren.
  
#### Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Verbindungen zu Benutzern getrennt werden, wenn diese außerhalb der für ihr Konto gültigen Anmeldezeiten mit einem lokalen Computer verbunden sind. Diese Einstellung betrifft die SMB-Komponente.
  
Wenn Sie die Einstellung **Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen** aktivieren, werden Clientsitzungen mit dem SMB-Server beendet, wenn die Anmeldezeit des Clients abgelaufen ist. Der Benutzer kann sich bis zur nächsten ihm zugewiesenen Benutzerzeit nicht am System anmelden. Wenn Sie diese Richtlinieneinstellung deaktivieren, können Benutzer eine eingerichtete Clientsitzung nach Ablauf der Anmeldezeit aufrechterhalten. Damit diese Einstellung für Domänenkonten gilt, muss sie in der Standarddomänenrichtlinie festgelegt werden.
  
Es wird empfohlen, die Einstellung **Netzwerksicherheit: Abmeldung nach Ablauf der Anmeldezeit erzwingen** für die drei in diesem Handbuch definierten Umgebungen als **Aktiviert** zu konfigurieren.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wird die Notwendigkeit der Überprüfung aller domänenweiten Einstellungen im Unternehmen erläutert. Für jede Domäne kann nur ein Richtliniensatz für Kennwörter, Kontosperrung und das Kerberos-Authentifizierungsprotokoll Version 5 konfiguriert werden. Andere Kennwort- und Kontosperrungseinstellungen betreffen nur die lokalen Konten der Mitgliedsserver. Planen Sie die Konfiguration der Einstellungen, die auf alle Mitgliedsserver der Domäne angewendet werden, und stellen Sie sicher, dass diese Einstellungen im gesamten Unternehmen ein ausreichendes Sicherheitsniveau aufweisen.
  
#### Weitere Informationen
  
Unter den folgenden Links erhalten Sie zusätzliche Informationen zur Domänenrichtlinie für Server, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
  
-   Informationen zur Möglichkeit von anonymen Benutzern, Sicherheitskennungsattribute für andere Benutzer anzufordern, finden Sie auf Seite [Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/299803be-0e85-4c60-b0b5-1b64486559b3.mspx) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/  
    299803be-0e85-4c60-b0b5-1b64486559b3.mspx.
  
-   Informationen zur Netzwerksicherheit und Erzwingung der Abmeldung nach Ablauf der Anmeldezeit finden Sie in „[Mole \#32: Technische Antworten von Microsoft](http://www.microsoft.com/technet/archive/community/columns/inside/techan32.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/archive/community/columns/inside/techan32.mspx.
  
    Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Gastkonto kann bei Deaktivierung des anonymen Zugriffs nicht verwendet werden](http://support.microsoft.com/kb/251171/en-us)“ (in englischer Sprache) unter http://support.microsoft.com/kb/251171/en-us.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))  
-   Kapitel 3: Die Domänenrichtlinie  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))  
-   [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))  
-   [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))  
-   [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))  
-   [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))  
-   [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))  
-   [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))  
-   [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))  
-   [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))  
-   [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))  
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))  
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))  
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))  
-   [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
  
**Download**
  
[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)
  
**Benachrichtigungen über Neuerungen**
  
[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows%20server%202003%20security%20guide)

 
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10)"><img src="images/Dd443724.pageLeft(de-de,TechNet.10).gif" /></a>4 von 19<a href="https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10)"><img src="images/Dd443724.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>