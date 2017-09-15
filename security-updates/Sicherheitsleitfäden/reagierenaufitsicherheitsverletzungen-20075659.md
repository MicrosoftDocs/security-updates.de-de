---
TOCTitle: 'Reagieren auf IT-Sicherheitsverletzungen'
Title: 'Reagieren auf IT-Sicherheitsverletzungen'
ms:assetid: '820c6752-6b33-4958-965a-c3f010f84ff7'
ms:contentKeyID: 20075659
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443716(v=TechNet.10)'
---

Reagieren auf IT-Sicherheitsverletzungen
========================================

##### Auf dieser Seite

[](#ehaa)[Einführung](#ehaa)
[](#egaa)[Bevor Sie beginnen](#egaa)
[](#efaa)[Minimieren der Zahl und des Schweregrads der Sicherheitsverletzungen](#efaa)
[](#eeaa)[Zusammenstellen des Kernteams zur Bekämpfung von Computersicherheitsverletzungen](#eeaa)
[](#edaa)[Definieren eines Vorfallreaktionsplans](#edaa)
[](#ecaa)[Schadensbegrenzung und Risikominimierung](#ecaa)
[](#ebaa)[Verwandte Informationen](#ebaa)

### Einführung

Wie gut sind Ihre Abteilung für Informationstechnologie (IT) oder Ihre Administratoren darauf vorbereitet, Sicherheitsverletzungen abzuwehren? Viele Organisationen lernen erst, nachdem sie solche Angriffe erlitten haben, auf Sicherheitsverletzungen zu reagieren. Dann sind solche Vorfälle allerdings oft viel teurer als nötig. Die angemessene Reaktion auf derartige Angriffe sollte ein wesentlicher Bestandteil Ihrer gesamten Sicherheits- und Schadensbegrenzungsstrategie sein.

Die Reaktion auf Sicherheitsverletzungen hat ganz eindeutig direkte Vorteile. Jedoch können sich daraus auch indirekte finanzielle Vorteile ergeben. Zum Beispiel könnte Ihre Versicherungsgesellschaft Rabatte anbieten, wenn Sie nachweisen, dass Ihre Organisation schnell und kostenwirksam auf Angriffe reagieren kann. Wenn Sie ein Dienstanbieter sind, könnte ein formeller Abwehrplan helfen, zusätzliche Kunden zu gewinnen, weil dies zeigt, dass Sie den Prozess guter Informationssicherheit ernst nehmen.

In diesem Dokument werden ein empfohlener Prozess und die Verfahren beschrieben, mit denen Sie auf erkannte Angriffe in einer kleinen bis mittelgroßen Netzwerkumgebung reagieren können. Es wird erläutert, welche Bedeutung die Bildung eines Teams zur Reaktion auf Sicherheitsverletzungen hat, samt der expliziten Rollen der Teammitglieder. Außerdem wird die Methode zur Definition eines Reaktionsplans für Sicherheitsverletzungen erklärt.

Um erfolgreich auf Vorfälle zu reagieren, müssen Sie:

-   Die Zahl und den Schweregrad der Sicherheitsverletzungen minimieren.

-   Das Kernteam zur Bekämpfung von Computersicherheitsverletzungen (Computer Security Incident Response Team, CSIRT) zusammenstellen.

-   Einen Plan zur Reaktion auf Angriffe definieren.

-   Den Schaden begrenzen und Risiken minimieren.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Bevor Sie beginnen

Systemadministratoren verbringen viel Zeit mit Netzwerkumgebungen und sind sehr vertraut mit Netzwerken. Sie dokumentieren die Umgebungen und haben Sicherungsmechanismen eingerichtet. Ein Prozess sollte bereits eingerichtet sein, um Leistung und Auslastung zu überwachen. Bereits vor der Implementierung eines Angriffsreaktionsteams sollte ein gewisser Kenntnisstand erreicht sein.

Unabhängig davon, wie genau Sie die Netzwerkumgebung kennen, die Gefahr eines Angriffs bleibt bestehen. Jede vernünftige Sicherheitsstrategie muss Angaben dazu enthalten, auf welche Weise auf verschiedene Arten von Angriffen reagiert werden kann.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Minimieren der Zahl und des Schweregrads der Sicherheitsverletzungen

In den meisten Lebensbereichen ist Vorsorge besser als Nachsorge, und Sicherheit bildet dabei keine Ausnahme. Sie sollten möglichst immer versuchen, Sicherheitsverletzungen im Vorfeld zu verhindern. Allerdings ist es unmöglich, alle Sicherheitsverletzungen zu verhindern. Wenn eine Sicherheitsverletzung eingetreten ist, müssen Sie dafür sorgen, dass ihre Auswirkungen minimiert werden. Um die Zahl und die Auswirkung der Sicherheitsverletzungen zu minimieren, sollten Sie folgende Maßnahmen ergreifen:

-   Richten Sie eindeutige Richtlinien und Verfahren ein, und setzen Sie sie durch. Viele Sicherheitsverletzungen werden unbeabsichtigt von IT-Mitarbeitern ermöglicht, die Änderungsverwaltungsverfahren nicht befolgt bzw. nicht verstanden oder Sicherheitseinrichtungen, wie z. B. Firewalls und Authentifizierungssysteme, falsch konfiguriert haben. Ihre Richtlinien und Verfahren sollten gründlich getestet werden, um sicherzustellen, dass sie praktisch und klar sind und die geeignete Sicherheitsstufe bieten.

-   Gewinnen Sie die Unterstützung des Managements für Sicherheitsrichtlinien und Vorfallhandhabung.

-   Bewerten Sie regelmäßig Sicherheitsrisiken in Ihrer Umgebung. Diese Bewertungen sollten von einem Sicherheitsexperten mit der erforderlichen Vollmacht zum Ergreifen der Maßnahmen durchgeführt werden, d. h. einem Experten, der zuverlässig und mit den erforderlichen Administratorrechten für die Systeme ausgestattet ist.

-   Prüfen Sie regelmäßig alle Computersysteme und Netzwerkgeräte, um sicherzustellen, dass darauf alle aktuellen Patches installiert sind.

-   Richten Sie Sicherheitsschulungsprogramme für IT-Personal und Endbenutzer ein. Das größte Sicherheitsrisiko in jedem System ist der unerfahrene Benutzer. Der ILOVEYOU-Wurm hat dieses Sicherheitsrisiko für IT-Personal und Endbenutzer wirksam ausgenutzt.

-   Stellen Sie Sicherheitsbanner auf, um Benutzer an ihre Verantwortlichkeiten und Einschränkungen zu erinnern, zusammen mit einer Warnung hinsichtlich einer möglichen Strafverfolgung bei Verstoß. Diese Banner machen es leichter, Beweise zu sammeln und Angreifer strafrechtlich zu verfolgen. Lassen Sie sich rechtlich beraten, um sicherzustellen, dass die Formulierung Ihrer Sicherheitsbanner angemessen ist.

-   Entwickeln, implementieren und setzen Sie eine Richtlinie durch, die sichere Kennwörter erfordert. Sie können mehr über Kennwörter im Sicherheitsanleitungskit unter „Durchsetzen sicherer Kennwortregeln in Ihrer Organisation“ lernen.

-   Überwachen und analysieren Sie regelmäßig Netzwerkverkehr und Systemleistung.

-   Prüfen Sie regelmäßig alle Protokolle und Protokolliermechanismen, einschließlich der Betriebssystemereignisprotokolle, der anwendungsspezifischen Protokolle und der Systemprotokolle für die Angriffserkennung.

-   Überprüfen Sie Ihre Datensicherungs- und Wiederherstellungsverfahren. Sie sollten wissen, wo Sicherungskopien gepflegt werden, wer darauf zugreifen kann, und Sie sollten Ihre Verfahren zur Daten- und Systemwiederherstellung kennen. Stellen Sie durch selektives Wiederherstellen von Daten sicher, dass Sie Sicherungskopien und Medien regelmäßig überprüfen.

-   Stellen Sie ein Team zur Bekämpfung von Computersicherheitsverletzungen (Computer Security Incident Response Team, CSIRT) zusammen, um auf Angriffe zu reagieren. Sie können mehr über das CSIRT im folgenden Abschnitt dieses Dokuments lernen.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zusammenstellen des Kernteams zur Bekämpfung von Computersicherheitsverletzungen

Das CSIRT ist hauptsächlich verantwortlich für die Reaktion auf Computersicherheitsverletzungen in Ihrer Umgebung. Ihr Team sollte sich aus Personen zusammensetzen, die für die Behandlung von Sicherheitsverletzungen verantwortlich sind. Die Teammitglieder müssen deutlich definierte Aufgaben haben, um zu gewährleisten, dass kein Bereich Ihrer Reaktion unberücksichtigt bleibt.

Die Zusammenstellung eines Teams vor Auftreten einer Sicherheitsverletzung ist für Ihre Organisation sehr wichtig und hat einen positiven Einfluss darauf, wie Vorfälle behandelt werden. Ein erfolgreiches Team erfüllt folgende Aufgaben:

-   Überwachen der Systeme auf Sicherheitsverletzungen.

-   Fungieren als zentraler Kommunikationspunkt, um sowohl Berichte über Sicherheitsverletzungen zu empfangen als auch wichtige Informationen an die entsprechenden Stellen über den Vorfall weiterzuleiten.

-   Dokumentieren und Katalogisieren von Sicherheitsverletzungen.

-   Fördern des Sicherheitsbewusstseins innerhalb des Unternehmens, um zur Vermeidung von Vorfällen in Ihrer Organisation beizutragen.

-   Unterstützen von System- und Netzwerkprüfungen durch Prozesse, wie z. B. Bewertung der Sicherheitsanfälligkeiten und Simulation von Eindringversuchen.

-   Weiterbildung zu neuen Sicherheitsrisiken und Angriffsstrategien.

-   Suchen nach neuen Softwarepatches.

-   Analysieren und Entwickeln neuer Technologien zur Minimierung der Sicherheitsanfälligkeiten und Risiken.

-   Bereitstellen von Sicherheitsberatungsdiensten.

-   Fortlaufendes Verfeinern und Aktualisieren aktueller Systeme und Verfahren.

Wenn Sie ein CSIRT zusammenstellen, bereiten Sie das Team so vor, dass es in der Lage ist, auf Sicherheitsverletzungen zu reagieren. Zur Vorbereitung eines Teams:

-   Informieren Sie die Teammitglieder über die richtige Verwendung und den Speicherort kritischer Sicherheitstools. Sie sollten außerdem in Erwägung ziehen, mobile Computer bereitzustellen, die mit diesen Tools vorkonfiguriert sind, damit keine Zeit mit der Installation und Konfiguration dieser Tools verloren geht und das Team sofort auf einen Vorfall reagieren kann. Diese Systeme und die zugehörigen Tools müssen ordnungsgemäß geschützt werden, wenn sie nicht im Einsatz sind.

-   Stellen Sie alle relevanten Kommunikationsinformationen zusammen. Stellen Sie sicher, dass Sie die Namen und Telefonnummern der Ansprechpartner für die Kollegen in Ihrer Organisation parat haben, die benachrichtigt werden müssen (einschließlich der Mitglieder des CSIRT, die für die Unterstützung Ihrer Systeme und für die Öffentlichkeitsarbeit verantwortlich sind). Außerdem benötigen Sie die Angaben für Ihren Internetdienstanbieter (Internet service provider, ISP) sowie für lokale und nationale Strafvollzugsbehörden. Sprechen Sie mit Ihrer Rechtsberatung darüber, lokale Strafvollzugsbehörden in Anspruch zu nehmen, bevor ein Vorfall geschieht. Das hilft Ihnen sicherzustellen, dass Sie die richtigen Verfahren zur Kommunikation von Vorfällen und Sicherstellung von Beweisen kennen. Ihre Rechtsberatung sollte über Kontakte mit Strafvollzugsbehörten informiert werden.

-   Bewahren Sie alle Notfallsysteminformationen an einem zentralen Ort auf, der offline ist, wie z. B. in einem physischen Ordner oder einem Offlinecomputer. Zu diesen Notfallinformationen gehören Kennwörter zu Systemen, Adressen für Internetprotokolle (IP), Routerkonfigurationsinformationen, Listen mit Firewallregelsätzen, Kopien von Zertifizierungsstellenschlüssel, Namen und Telefonnummern von Ansprechpartnern, Eskalationsverfahren und so weiter. Diese Informationen müssen sofort verfügbar sein und gleichzeitig physisch extrem sicher aufbewahrt werden. Eine Methode, diese Informationen gleichzeitig zu schützen und schnell zugänglich zu machen, ist ihre Verschlüsselung auf einem eigens dafür vorgesehenen, tragbaren Sicherheitscomputer, der sich in einem sicheren Tresor befindet. Der Zugang zu diesem Tresor sollte auf autorisierte Personen, wie z. B. den CSIRT-Leiter und den Abteilungsleiter oder CTO, beschränkt sein.

Die ideale CSIRT-Struktur und geeigneten Mitglieder hängen vom Typ Ihrer Organisation und Ihrer Risikomanagementstrategie ab. Allgemein empfiehlt sich jedoch, dass das Sicherheitsteam Ihrer Organisation teilweise oder ganz aus dem CSIRT besteht. Innerhalb des Kernteams sind Sicherheitsfachleute für die Koordination einer Reaktion auf Vorfälle verantwortlich. Die Anzahl der Mitglieder im CSIRT hängt normalerweise von der Größe und Komplexität Ihrer Organisation ab. Sie sollten jedoch sicherstellen, dass genügend Mitglieder vorhanden sind, um alle Aufgaben des Teams jederzeit ausreichend abzudecken.

#### Festlegen der Teamrollen

Ein erfolgreiches CSIRT besteht aus mehreren Schlüsselmitgliedern.

**CSIRT-Leiter** Innerhalb des CSIRT muss ein Mitglied die Verantwortung für die Aktivitäten des Teams übernehmen. Der CSIRT-Leiter ist im Allgemeinen verantwortlich für die Aktivitäten des CSIRT und koordiniert Prüfungen der Teamaktionen. Dies könnte zu Änderungen in den Strategien und Verfahren für die Behandlung zukünftiger Vorfälle führen.

**CSIRT-Vorfallleiter** Im Falle eines Vorfalls sollten Sie eine Person bestimmen, die für die Koordination der Maßnahmen verantwortlich ist. Der CSIRT-Vorfallleiter ist für diesen besonderen Vorfall oder eine Reihe verwandter Sicherheitsverletzungen zuständig. Jegliche Kommunikation über das Ereignis wird von den Vorfallleitern koordiniert, und bei Gesprächen außerhalb des CSIRT vertreten sie das gesamte CSIRT. Je nach Art des Vorfalls können die Vorfallleiter variieren, und oft unterscheiden sie sich vom CSIRT-Leiter.

**Außerordentliche CSIRT-Mitglieder** Neben dem Kern-CSIRT sollten Sie eine Anzahl bestimmter Personen benennen, die auf besondere Vorfälle reagieren und diese behandeln. Außerordentliche Mitglieder stammen aus den verschiedensten Abteilungen in Ihrer Organisation. Sie sollten in den Bereichen spezialisiert sein, die von Sicherheitsverletzungen betroffen sind, aber nicht direkt vom Kern-CSIRT behandelt werden. Außerordentliche Mitglieder können entweder direkt an einem Vorfall mitarbeiten oder als Anlaufstelle zur Delegierung der Verantwortung an besser geeignete Kollegen innerhalb ihrer Abteilungen dienen. Die folgende Tabelle enthält einige Vorschläge für außerordentliche Mitglieder und ihre Rollen.

**Außerordentliche CSIRT-Mitglieder**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Außerordentliches Mitglied</p></th>
<th><p>Rollenbeschreibung</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>IT-Ansprechpartner</p></td>
<td style="border:1px solid black;"><p>Dieses Mitglied ist hauptsächlich verantwortlich für die Koordination der Kommunikation zwischen dem CSIRT-Vorfallverantwortlichen und der restlichen IT-Gruppe. Die IT-Ansprechpartner haben eventuell nicht die speziellen technischen Fachkenntnisse, um auf den besonderen Vorfall reagieren zu können. Sie sind hauptsächlich verantwortlich dafür, die Kollegen in der IT-Gruppe zu finden, die bestimmte Sicherheitsereignisse behandeln können.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Rechtsvertreter</p></td>
<td style="border:1px solid black;"><p>Dieses Mitglied ist ein Rechtsanwalt, der mit den festgelegten Richtlinien für die Behandlung von Sicherheitsverletzungen sehr vertraut ist. Der Rechtsvertreter bestimmt das Vorgehen bei einer Sicherheitsverletzung mit minimaler gesetzlicher Haftung und maximaler Möglichkeit, Täter strafrechtlich zu verfolgen.</p>
<p>Bevor ein Vorfall stattfindet, sollte der Rechtsvertreter Informationen zu den Überwachungs- und Reaktionsrichtlinien erhalten, um sicherzustellen, dass die Organisation kein rechtliches Risiko während einer Bereinigungs- oder Eindämmungsmaßnahme eingeht. Es ist sehr wichtig festzustellen, welche gesetzlichen Implikationen und möglichen Verstöße gegen Vereinbarungen zum Servicelevel und gegen Mitgliedschaftsabkommen mit Ihren Kunden entstehen können, wenn ein betroffenes System heruntergefahren wird. Außerdem sollte die Frage der Haftung für Schäden untersucht werden, die durch die von diesem System ausgehenden Angriffe entstehen, wenn das System nicht heruntergefahren wird.</p>
<p>Jegliche Kommunikation mit Strafverfolgungsbehörden außerhalb der Organisation oder mit externen Untersuchungseinrichtungen sollte auch mit dem Rechtsvertreter koordiniert werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Beauftragter für Öffentlichkeitsarbeit</p></td>
<td style="border:1px solid black;"><p>Im Allgemeinen gehört dieses Mitglied der Abteilung für an und ist für den Schutz und die Förderung des Images der Organisation verantwortlich.</p>
<p>Diese Person hat zwar möglicherweise keinen direkten Kontakt zu den Medien und den Kunden, ist aber verantwortlich für die Formulierung der Mitteilungen. (Für Inhalt und Ziel der Nachricht ist in der Regel das Management verantwortlich.) Alle Medienanfragen sollten direkt an die Abteilung für Öffentlichkeitsarbeit geleitet werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Management</p></td>
<td style="border:1px solid black;"><p>Je nach Vorfall haben Sie die Wahl, nur die Abteilungsmanager oder aber die abteilungsübergreifenden Manager an der Behandlung des Vorfalls zu beteiligen. Das jeweilige Managementmitglied hängt von den Auswirkungen, dem Ort, dem Schweregrad und der Art des Vorfalls ab.</p>
<p>Wenn Sie einen Ansprechpartner im Management haben, können Sie schnell die am besten geeignete Person für die jeweiligen Umstände identifizieren. Das Management ist verantwortlich für die Genehmigung und Steuerung der Sicherheitsmaßnahmen.</p>
<p>Außerdem ist das Management verantwortlich für die Bestimmung aller (sowohl finanzieller als auch sonstiger) Vorfallauswirkungen auf die Organisation. Das Management weist das Kommunikationspersonal an, welche Informationen den Medien mitgeteilt werden, und bestimmt die Interaktionsebene zwischen dem Rechtsvertreter und den Strafverfolgungsbehörden.</p></td>
</tr>
</tbody>
</table>
<p> </p>

#### Reagieren auf einen Vorfall

Wenn ein Angriff stattgefunden hat, koordiniert das CSIRT eine Reaktion des Kern-CSIRT und kommuniziert mit den außerordentlichen Mitgliedern des CSIRT. Die folgende Tabelle zeigt die Verantwortlichkeiten dieser Personen während des Vorfallreaktionsprozesses.

**Verantwortlichkeiten des CSIRT während des Vorfallreaktionsprozesses**

<table style="width:100%;">
<colgroup>
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
<col width="16%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Aktivität</p></th>
<th><p>Rolle</p></th>
<th></th>
<th></th>
<th></th>
<th></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"> </td>
<td style="border:1px solid black;"><p><strong>CSIRT-Vorfallleiter</strong></p></td>
<td style="border:1px solid black;"><p><strong>IT-Ansprechpartner</strong></p></td>
<td style="border:1px solid black;"><p><strong>Rechtsvertreter</strong></p></td>
<td style="border:1px solid black;"><p><strong>Kommunikationsbeauftragter</strong></p></td>
<td style="border:1px solid black;"><p><strong>Management</strong></p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Erste Bewertung</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Keine</p></td>
<td style="border:1px solid black;"><p>Keine</p></td>
<td style="border:1px solid black;"><p>Keine</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Erste Reaktion</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Sammelt gerichtliche Beweise</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
<td style="border:1px solid black;"><p>Keine</p></td>
<td style="border:1px solid black;"><p>Keine</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Implementiert vorläufige Problembehebung</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Sendet Kommunikation</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Absprechen mit lokaler Strafverfolgungsbehörde</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Implementiert permanente Problembehebung</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
<td style="border:1px solid black;"><p>Implementiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Bestimmt finanzielle Auswirkungen auf das Geschäft</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Berät</p></td>
<td style="border:1px solid black;"><p>Aktualisiert</p></td>
<td style="border:1px solid black;"><p>Besitzer</p></td>
</tr>  
</tbody>  
</table>
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Definieren eines Vorfallreaktionsplans
  
Alle Mitglieder Ihrer IT-Umgebung sollten wissen, welche Maßnahmen bei einem Vorfall ergriffen werden müssen. Das CSIRT führt zwar die meisten Aktionen als Reaktion auf einen Vorfall durch, aber Ihr IT-Personal auf allen Ebenen muss wissen, wie Vorfälle intern zu berichten sind. Endbenutzer sollten dem IT-Personal verdächtige Aktivitäten direkt oder über ein Helpdesk melden, statt sich direkt an das CSIRT zu wenden.
  
Jedes Teammitglied sollte den Vorfallreaktionsplan ausführlich überprüfen. Wenn der Plan allen IT-Mitarbeitern leicht zugänglich ist, wird gewährleistet, dass die richtigen Maßnahmen ergriffen werden, wenn ein Angriff stattfindet.
  
Um einen erfolgreichen Vorfallreaktionsplan in die Wege zu leiten, sollen Sie:
  
-   eine erste Bewertung durchführen.
  
-   den Vorfall kommunizieren.
  
-   den Schaden begrenzen und das Risiko minimieren.
  
-   Typ und Schweregrad der Verletzung identifizieren.
  
-   Beweise schützen.
  
-   bei Bedarf externe Einrichtungen benachrichtigen.
  
-   Systeme wiederherstellen.
  
-   Dokumentation des Vorfalls erstellen und organisieren.
  
-   Vorfallschaden und Kosten beurteilen.
  
-   Maßnahmen und Aktualisierungsrichtlinien prüfen.
  
Diese Schritte sind nicht rein sequenziell. Vielmehr wird ihre Reihenfolge durch den Vorfall bestimmt. So beginnt zum Beispiel die Dokumentation mit dem Eintreten des Vorfalls und wird über seine gesamte Dauer fortgesetzt. Gleichermaßen findet die Kommunikation während des gesamten Vorfalls statt.
  
Andere Aspekte des Prozesses finden parallel zueinander statt. So verschaffen Sie sich zum Beispiel im Zuge Ihrer anfänglichen Bewertung einen Einblick in die allgemeine Natur des Angriffs. Es ist wichtig, den Schaden anhand dieser Informationen zu begrenzen und das Risiko möglichst bald zu minimieren. Wenn Sie schnell handeln, können Sie Zeit und Geld sparen und dazu beitragen, den Ruf Ihrer Organisation zu schützen.
  
Solange Sie jedoch die Art und den Schweregrad des Angriffs nicht genauer verstehen, werden Sie kaum eine wirksame Schadensbegrenzung und Minimierung des Risikos erreichen. Eine zu hastige Reaktion könnte sogar mehr Schaden als der ursprüngliche Angriff verursachen. Wenn Sie diese Schritte parallel durchführen, erzielen Sie den besten Kompromiss zwischen rascher und wirksamer Aktion.
  
**Hinweis:** Es ist sehr wichtig, dass Sie Ihren Vorfallreaktionsprozess gründlich testen, bevor ein Vorfall stattfindet. Ohne eingehende Prüfung können Sie nicht darauf vertrauen, dass die vorgesehenen Maßnahmen Vorfälle wirksam bekämpfen.
  
#### Erstellen einer ersten Beurteilung
  
Viele Aktivitäten könnten ein Hinweis auf einen möglichen Angriff auf Ihre Organisation sein. So könnte zum Beispiel ein Netzwerkadministrator, der eine legitime Systemwartung durchführt, wie jemand erscheinen, der eine Art Angriff startet. In anderen Fällen könnte ein fehlerhaft konfiguriertes System zu einer Reihe falscher Alarme in einem System zur Erkennung von Eindringversuchen führen, was die Feststellung echter Vorfälle erschwert.
  
Als Teil Ihrer ersten Beurteilung sollen Sie:
  
-   Schritte ergreifen, um zu erkennen, ob es sich um einen tatsächlichen Vorfall oder einen falschen Alarm handelt.
  
-   sich einen allgemeinen Überblick über die Art und den Schweregrad des Angriffs verschaffen. Sie sollten zumindest so viele Information sammeln, dass Sie sie zur weiteren Untersuchung kommunizieren und die Schadensbegrenzung sowie die Risikominimierung einleiten können.
  
-   Ihre Aktionen gründlich aufzeichnen. Diese Aufzeichnungen werden später zur Dokumentation des Vorfalls (echt oder falsch) verwendet.
  
**Hinweis:** Falsche Positivmeldungen sollten möglichst vermieden werden. Es ist jedoch immer besser, auf einen falschen Alarm zu reagieren, als einen echten Vorfall zu übersehen. Ihre erste Beurteilung sollte daher so kurz wie möglich sein und trotzdem offensichtlich falsche Positivmeldungen beseitigen.
  
#### Kommunizieren des Vorfalls
  
Wenn Sie vermuten, dass es eine Sicherheitsverletzung gibt, sollten Sie das übrige Kern-CSIRT schnell darüber informieren. Der Vorfallleiter sollte, zusammen mit dem restlichen Team, schnell feststellen, wer außerhalb des Kern-CSIRT angesprochen werden muss. Damit soll sichergestellt werden, dass eine angemessene Steuerungs- und Vorfallkoordination gewährleistet ist und gleichzeitig das Ausmaß des Schadens minimiert werden kann.
  
Denken Sie daran, dass ein Schaden in verschiedenster Form entstehen kann und dass eine Schlagzeile in der Zeitung wesentlich größeren Schaden anrichten kann als viele Systemangriffe. Aus diesem Grund und um zu verhindern, dass ein Angreifer gewarnt wird, sollten vorläufig nur die für die Vorfallreaktion Verantwortlichen informiert werden, bis der Vorfall unter Kontrolle ist. Auf Grund der eindeutigen Lage bestimmt Ihr Team später, wer über den Vorfall informiert werden muss. Dieser Personenkreis könnte bestimmte Einzelpersonen, aber auch die gesamte Organisation und externe Kunden umfassen. Die externe Kommunikation sollte mit dem Rechtsvertreter koordiniert werden.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Schadensbegrenzung und Risikominimierung
  
Durch schnelles Handeln, um die tatsächlichen und potenziellen Auswirkungen eines Angriffs zu verringern, können Sie verhindern, dass sich ein kleiner Angriff zu einem schwerwiegenden Problem entwickelt. Die genaue Reaktion auf einen Angriff hängt von Ihrer Organisation und der Natur des Angriffs ab, dem Sie gegenüberstehen. Die folgenden Prioritäten empfehlen sich jedoch als ein Ausgangspunkt:
  
1.  **Schützen Sie das Leben und die Sicherheit von Personen.** Dies muss selbstverständlich immer Ihre erste Priorität sein.
  
2.  **Schützen Sie geheime und vertrauliche Daten.** Als Teil Ihrer Planung von Maßnahmen bei Sicherheitsverletzungen sollten Sie klar definieren, welche Daten geheim und welche vertraulich sind. Dadurch sind Sie in der Lage, Prioritäten Ihrer Maßnahmen zum Schutz der Daten zu setzen.
  
3.  **Schützen Sie andere Daten, einschließlich proprietärer, wissenschaftlicher und Managementdaten.** Andere Daten in Ihrer Umgebung könnten immer noch von großem Wert sein. Sie sollten die wertvollsten Daten zuerst schützen, bevor Sie sich mit anderen, weniger nützlichen Daten befassen.
  
4.  **Schützen Sie Hardware und Software gegen Angriffe.** Dies umfasst den Schutz vor Verlust oder Veränderung von Systemdateien und physischen Schaden an der Hardware. Schäden an Systemen können zu teurer Ausfallzeit führen.
  
5.  **Minimieren Sie Unterbrechungen der Computerressourcen (einschließlich der Prozesse).** Obwohl die Betriebszeit in den meisten Umgebungen sehr wichtig ist, könnte die Aufrechterhaltung der Systeme während eines Angriffs später zu größeren Problemen führen. Aus diesem Grund sollte die Minimierung von Unterbrechungen der Computerressourcen gewöhnlich eine verhältnismäßig niedrige Priorität haben.
  
Es gibt eine Reihe von Maßnahmen, die Sie ergreifen können, um den Schaden zu begrenzen und das Risiko für Ihre Umgebung zu minimieren. Als Mindestmaßnahmen empfiehlt sich Folgendes:
  
-   Verhindern Sie nach Möglichkeit, dass Angreifer erfahren, dass Sie sich ihrer Aktivitäten bewusst sind Dies kann schwierig sein, weil einige grundlegende Reaktionen Angreifer warnen könnten. Wenn es zum Beispiel eine Notfallbesprechung des CSIRT gibt oder Sie eine unmittelbare Änderung aller Kennwörter verlangen, könnten interne Angreifer wissen, dass Sie sich eines Vorfalls bewusst sind.
  
-   Vergleichen Sie die Kosten, die durch die Außerbetriebsetzung befallener und zugehöriger Systeme entstehen, mit dem Risiko, den Betrieb aufrecht zu erhalten. In der Mehrzahl der Fälle sollten Sie das System sofort aus dem Netzwerk nehmen. Möglicherweise haben Sie jedoch Kundenserviceverträge abgeschlossen, für die eine Verfügbarkeit der Systeme erforderlich ist, selbst mit dem Risiko eines weiteren Schadens. Unter diesen Umständen können Sie sich entscheiden, ein System mit begrenzter Konnektivität online zu lassen, um weitere Beweise während eines laufenden Angriffs zu sammeln.  
    In einigen Fällen könnten der Schaden und das Ausmaß eines Vorfalls so umfangreich sein, dass Sie gezwungen sind, Maßnahmen zu ergreifen, die zu einem Inkrafttreten der Strafklauseln führen, die in Ihren Vereinbarungen zum Servicelevel festgelegt sind. Auf jeden Fall ist es sehr wichtig, dass die Aktionen, die Sie im Falle eines Angriffs durchführen, im Vorfeld in Ihrem Vorfallplan erläutert und definiert werden, damit ein sofortiges Reagieren auf einen Angriff möglich ist.
  
-   Bestimmen Sie die von Angreifern genutzten Zugangspunkte, und implementieren Sie Maßnahmen, um zukünftige Zugriffe zu verhindern. Zu diesen Maßnahmen könnten das Deaktivieren eines Modems, Hinzufügen von Zugriffskontrolleinträgen in einem Router oder einer Firewall oder Verstärken der physischen Sicherheitsmaßnahmen gehören.
  
-   Überlegen Sie, ein frisches System mit neuen Festplatten aufzubauen. (Die existierenden Festplatten sollten ausgebaut und eingelagert werden, da sie als Beweis verwendet werden können, wenn Sie entscheiden, Angreifer strafrechtlich zu verfolgen). Stellen Sie sicher, dass Sie alle lokalen Kennwörter ändern. Auch administrative Kennwörter und die Kennwörter für Dienstkonten anderswo in Ihrer Umgebung sollten geändert werden.
  
#### Identifizieren des Schweregrads des Angriffs
  
Um sich wirksam von einem Angriff erholen zu können, müssen Sie feststellen, wie ernsthaft Ihre Systeme beeinträchtigt worden sind. Dies bestimmt, in welcher Weise Sie den Schaden weiter begrenzen und das Risiko stärker minimieren können, wie Sie Systeme wiederherstellen, wie schnell Sie welche Personen über den Vorfall informieren müssen und ob rechtliche Schritte eingeleitet werden sollen, um Schadensersatz geltend zu machen.
  
Versuchen Sie, nach Möglichkeit:
  
-   die Art des Angriffs zu bestimmen (weicht möglicherweise von der ersten Beurteilung ab).
  
-   den Ursprung des Angriffs zu bestimmen.
  
-   den Zweck des Angriff zu bestimmen. Richtet sich der Angriff speziell an Ihre Organisation, um bestimmte Informationen zu erlangen, oder war er zufällig?
  
-   die betroffenen Systeme zu identifizieren.
  
-   die Dateien zu identifizieren, auf die zugegriffen wurde, und bestimmen Sie die Vertraulichkeit dieser Dateien.
  
Durch diese Aktionen sind Sie in der Lage, die geeigneten Reaktionen für Ihre Umgebung zu bestimmen. Ein guter Vorfallreaktionsplan skizziert bestimmte Verfahren, die Sie durchführen müssen, während Sie mehr über den Angriff erfahren. Im Allgemeinen bestimmt die Art der Angriffssymptome die Reihenfolge, in der Sie die Verfahren durchführen, die in Ihrem Plan definiert sind. Da der Zeitfaktor entscheidend ist, sollten weniger zeitaufwändige Verfahren in der Regel vor langwierigeren ausgeführt werden. Um den Schweregrad eines Angriffs einfacher zu bestimmen, sollten Sie folgende Maßnahmen ergreifen:
  
-   Informieren Sie andere Mitglieder im Reaktionsteam über Ihre Ergebnisse, bitten Sie sie um die Überprüfung Ihrer Ergebnisse, stellen Sie fest, ob ihnen ähnliche oder mögliche andere Angriffsaktivitäten bekannt sind, und unterstützen Sie sie bei der Feststellung, ob der Vorfall ein falscher Alarm ist. Was als ein echter Vorfall erscheinen mag, wird sich in einigen Fällen nach anfänglicher Beurteilung als falscher Alarm erweisen.
  
-   Stellen Sie fest, ob nicht autorisierte Hardware ins Netzwerk eingebunden wurde oder ob es Anzeichen für einen nicht autorisierten Zugriff durch die Beeinträchtigung physischer Sicherheitskontrollelemente gibt.
  
-   Untersuchen Sie Schlüsselgruppen (Domänenadministratoren, Administratoren und so weiter) auf nicht autorisierte Eingaben.
  
-   Suchen Sie nach Sicherheitsbewertungs- oder Ausnutzungssoftware. Während der Beweissammlung können auf befallenen Systemen oft Dienstprogramme zur Umgehung von Sicherheitsmechanismen gefunden werden.
  
-   Suchen Sie nach nicht autorisierten Prozessen oder Anwendungen, die zurzeit laufen oder über die Startordner bzw. Registrierungseingänge zur Ausführung konfiguriert sind.
  
-   Suchen Sie nach Lücken in Systemprotokollen oder fehlenden Systemprotokollen.
  
-   Überprüfen Sie die Systemprotokolle zur Erkennung von Eindringversuchen auf Anzeichen des Eindringens, und stellen Sie fest, welche Systeme betroffen sind, welche Angriffsmethoden angewendet wurden, stellen Sie Zeitpunkt und Länge des Angriffs sowie den Gesamtumfang des möglichen Schadens fest.
  
-   Untersuchen Sie andere Protokolldateien auf ungewöhnliche Verbindungen, Sicherheitsüberwachungsfehler, ungewöhnliche Sicherheitsüberwachungserfolge, fehlgeschlagene Anmeldeversuche, Versuche, sich bei Standardkonten anzumelden, Aktivitäten außerhalb der Arbeitszeiten, Änderungen in den Datei-, Verzeichnis- und Freigabeberechtigungen und höher gesetzte oder geänderte Benutzerberechtigungen.
  
-   Vergleichen Sie Systeme mit vorher durchgeführten Datei-/Systemintegritätsprüfungen. Dies befähigt Sie, Hinzufügungen, Löschungen und Änderungen sowie Berechtigungs- und Kontrolländerungen am Dateisystem und an der Registrierung zu identifizieren. Sie können bei der Reaktion auf Vorfälle viel Zeit sparen, wenn Sie genau feststellen, was beeinträchtigt wurde und welche Bereiche wiederhergestellt werden müssen.
  
-   Suchen Sie nach vertraulichen Daten, wie z. B. Kreditkartennummern und Mitarbeiter- oder Kundendaten, die eventuell verschoben oder zwecks zukünftiger Abrufe oder Änderungen ausgeblendet wurden. Eventuell müssen Sie die Systeme außerdem auf andere Daten als geschäftsbezogene, illegale Kopien der Software und E-Mails oder andere Datensätze überprüfen, die in einer Untersuchung helfen könnten. Wenn die Möglichkeit besteht, dass Sie durch Suchvorgänge auf einem System zu Untersuchungszwecken gegen den Datenschutz oder andere Gesetze verstoßen, setzen Sie sich mit Ihrer Rechtsabteilung in Verbindung, bevor Sie fortfahren.
  
-   Vergleichen Sie die Leistung verdächtiger Systeme mit ihren grundlegenden Leistungswerten. Dies setzt selbstverständlich voraus, dass solche Grundwerte erstellt und ordnungsgemäß aktualisiert wurden.
  
Bei der Feststellung, welche Systeme in welcher Form beeinträchtigt wurden, vergleichen Sie normalerweise Ihre Systeme mit den Grundwerten des gleichen Systems, die vor dem Angriff aufgezeichnet wurden. Vorausgesetzt, dass die neue Schattenkopie eines Systems für einen Vergleich ausreichend ist, könnten Sie sich in einer schwierigen Lage befinden, wenn die vorherige Schattenkopie von einem System kommt, das bereits angegriffen wurde.
  
**Hinweis:** Tools, wie z. B. EventCombMT, DumpEL und Microsoft Operations Manager (MOM), können Ihnen helfen zu bestimmen, wie stark ein System angegriffen worden ist. Drittanbietersysteme zur Erkennung von Eindringversuchen geben Warnungen im Vorfeld der Angriffe, und andere Tools zeigen Dateiänderungen auf Ihren Systemen an.
  
#### Schützen von Beweisen
  
In vielen Fällen werden Sie rechtliche Schritte gegen die Täter ergreifen wollen, wenn Ihre Umgebung vorsätzlich angegriffen wurde. Um sich diese Option zu erhalten, müssen Sie Beweise sammeln, die dann gegen die Angreifer verwendet werden können, selbst wenn letztendlich beschlossen wird, eine solche Maßnahme nicht zu ergreifen. Es ist äußerst wichtig, eine Sicherungskopie der beeinträchtigten Systeme sobald wie möglich zu erstellen. Erstellen Sie eine Sicherungskopie der Systeme, bevor Sie Maßnahmen durchführen, die die Datenintegrität auf den ursprünglichen Medien beeinträchtigen könnten.
  
Eine in der Computerforensik erfahrene Person sollte mindestens zwei vollständige bitweise Sicherungen des ganzen Systems auf einem völlig neuen, unbenutzten Medium erstellen. Mindestens eine Sicherung sollte auf einem einmal beschreibbaren Medium, z. B. CD-R oder DVD-R, gespeichert werden. Diese Sicherung sollte nur für die Strafverfolgung des Täters verwendet und physisch geschützt werden, bis sie benötigt wird.
  
Die andere Sicherung kann zur Datenwiederherstellung verwendet werden. Diese Sicherungen sollten nur zu rechtlichen Zwecken zugänglich sein, deshalb müssen Sie sie physisch schützen. Außerdem müssen Sie Information zu den Sicherungen dokumentieren, z. B. wer die Sicherungskopien der Systeme erstellt hat, wann sie erstellt wurden, wie sie geschützt wurden und wer Zugang dazu hatte.
  
Sobald die Sicherungskopien erstellt sind, sollten Sie die ursprünglichen Festplatten entfernen und an einem physisch sicheren Ort aufbewahren. Diese Datenträger können als gerichtlicher Beweis im Falle einer Strafverfolgung verwendet werden. Für die Wiederherstellung des Systems sollten neue Festplatten verwendet werden.
  
In einigen Fällen könnte der Vorteil des Datenerhalts nicht den Kosten entsprechen, die durch die Verzögerung der Reaktion und Wiederherstellung des Systems entstehen. Die Kosten und Vorteile des Datenerhalts sollten mit den Kosten für eine schnellere Wiederherstellung für jedes Ereignis verglichen werden.
  
Für äußerst große Systeme kann es sein, dass umfassende Sicherungskopien aller beeinträchtigten Systeme nicht durchführbar sind. Stattdessen sollten Sie eine Sicherungskopie aller Protokolle und aller ausgewählten, befallenen Teile des Systems erstellen.
  
Erstellen Sie nach Möglichkeit auch eine Sicherungskopie der Systemstatusdaten. Es kann Monate oder Jahre dauern, bis eine Strafverfolgung stattfindet. Deshalb ist es wichtig, möglichst ausführliche Informationen zu einem Vorfall zur späteren Verwendung zu archivieren.
  
Oft ist der schwierigste gesetzliche Aspekt der strafrechtlichen Verfolgung eines Cyberverbrechens die Zusammenstellung der Beweise in einer Weise, die nach der jeweiligen Rechtsprechung zur Beweiserbringung annehmbar ist. Deshalb ist die wichtigste Komponente im forensischen Prozess die ausführliche und vollständige Dokumentation dazu, wie Systeme von wem und wann behandelt wurden, um zuverlässige Beweis vorzulegen. Unterzeichnen und datieren Sie jede Seite der Dokumentation.
  
Sobald Sie funktionierende, geprüfte Sicherungskopien haben, können Sie die befallenen Systeme bereinigen und wiederherstellen. Dann können Sie damit beginnen, Ihren Geschäftsbetrieb wieder aufzunehmen. Die Sicherungskopien stellen den entscheidenden, unverfälschten Beweis dar, der zur Strafverfolgung erforderlich ist. Eine andere Sicherungskopie als die forensische sollte verwendet werden, um Daten wiederherzustellen.
  
#### Benachrichtigen externer Einrichtungen
  
Nachdem der Schaden begrenzt und Daten zwecks möglicher Strafverfolgung konserviert wurden, sollten Sie überlegen, ob Sie die entsprechenden externen Einrichtungen benachrichtigen müssen. Alle externen Veröffentlichungen sollten mit Ihrem Rechtsvertreter koordiniert werden. Mögliche Einrichtungen umfassen lokale und nationale Strafverfolgungsbehörden, externe Sicherheitsagenturen und Virenfachleute. Externe Einrichtungen können technische Hilfe, schnellere Lösungen und Informationen bieten, die aus ähnlichen Vorfällen gewonnen wurden, um Ihnen zu helfen, eine vollständige Wiederherstellung nach einem Vorfall zu erreichen und ein erneutes Eintreten in Zukunft zu verhindern.
  
In besonderen Branchen und bei bestimmten Angriffsarten müssen Sie eventuell die Kunden und die Allgemeinheit benachrichtigen, besonders, wenn Kunden durch den Vorfall direkt betroffen sind.
  
Wenn das Ereignis erhebliche finanzielle Auswirkungen hat, sollten Sie den Strafverfolgungsbehörden den Vorfall melden.
  
Für Unternehmen und Vorfälle mit höherem Profil müssen gegebenenfalls die Medien beteiligt werden. Es ist selten wünschenswert, die Aufmerksamkeit der Medien auf eine Sicherheitsverletzung zu lenken, aber oft ist es unvermeidlich. Durch die Aufmerksamkeit der Medien kann Ihre Organisation eine proaktive Haltung beim Kommunizieren des Vorfalls einnehmen. Die Vorfallreaktionsverfahren sollten zumindest die Personen eindeutig definieren, die autorisiert sind, mit Medienvertretern zu sprechen.
  
Normalerweise ist die Abteilung für Öffentlichkeitsarbeit innerhalb Ihrer Organisation der Ansprechpartner für die Medien. Sie sollten nicht versuchen, den Vorfall den Medien gegenüber zu verschweigen, denn dadurch erleidet der Ruf Ihrer Organisation größeren Schaden, als ein proaktives Eingeständnis und sichtbare Reaktionen es je können. Dies bedeutet nicht, dass Sie die Medien über jeden einzelnen Vorfall ohne Rücksicht auf seine Natur oder seinen Schweregrad benachrichtigen müssen. Die angemessene Medienreaktion sollte von Fall zu Fall beurteilt werden.
  
#### Wiederherstellen der Systeme
  
Wie Sie Ihr System wiederherstellen, hängt gewöhnlich vom Umfang der Sicherheitsverletzung ab. Sie müssen entscheiden, ob Sie das vorhandene System wiederherstellen und es dabei so unversehrt wie möglich lassen können oder ob es vollständig neu zusammengestellt werden muss.
  
Die Wiederherstellung von Daten setzt voraus, dass Sie über saubere Sicherungskopien verfügen, d. h. Sicherungskopien, die vor dem Vorfall erstellt wurden. Dateiintegritätssoftware kann helfen, das erste Eintreten des Schadens festzustellen. Wenn die Software Sie auf eine geänderte Datei hinweist, dann wissen Sie, dass die vor dieser Warnung erstellte Sicherungskopie in Ordnung ist und für den Einsatz bei der Wiederherstellung des betroffenen Systems aufbewahrt werden sollte.
  
Ein Vorfall kann die Daten bereits viele Monate vor seiner Entdeckung beschädigen. Es ist daher sehr wichtig, dass Sie die Dauer des Vorfalls als Teil Ihres Vorfallreaktionsprozesses bestimmen. (Datei-/Systemintegritätssoftware und Systeme zur Erkennung von Eindringversuchen können Ihnen dabei helfen.) In einigen Fällen könnten die aktuellsten oder sogar mehrere ältere Sicherungskopien nicht weit genug zurückreichen, um einen sauberen Systemzustand herzustellen. Deshalb sollten Sie die Datensicherungen regelmäßig an einem sicheren Ort entfernt vom Arbeitsplatz archivieren.
  
#### Kompilieren und Organisieren von Vorfallbeweisen
  
Das CSIRT sollte alle Prozesse gründlich dokumentieren, wenn es einen Vorfall behandelt. Dies sollte eine Beschreibung der Verletzung und Angaben zu jeder ergriffenen Maßnahme beinhalten (wer hat die Maßnahme wann und warum durchgeführt). Alle beteiligten Personen mit Zugriffsberechtigung müssen im gesamten Reaktionsprozess notiert werden.
  
Danach sollte die Dokumentation chronologisch geordnet, auf Vollständigkeit geprüft und vom Management sowie vom Rechtsvertreter unterschrieben und überprüft werden. Sie müssen außerdem die Beweise in der entsprechenden Phase schützen. Sie sollten überlegen, zwei Personen in allen Phasen hinzuzuziehen, die jeden Schritt abzeichnen können. Dadurch wird die Wahrscheinlichkeit verringert, dass die Beweise unzulässig sind und nachträglich geändert werden können.
  
Bedenken Sie, dass der Täter ein Arbeitnehmer, Auftragnehmer, eine vorübergehend angestellte Person oder ein anderer Insider innerhalb Ihrer Organisation sein könnte. Ohne eingehende, ausführliche Dokumentation ist es sehr schwierig, einen internen Täter zu identifizieren. Die richtige Dokumentation gibt Ihnen auch die beste Chance, Täter strafrechtlich zu verfolgen.
  
#### Beurteilen des Vorfallschadens und der Kosten
  
Bei der Beurteilung des Schadens für Ihre Organisation sollten Sie sowohl die direkten als auch die indirekten Kosten berücksichtigen. Schaden und Kosten eines Vorfalls sind wichtige Beweise, die benötigt werden, um gerichtliche Schritte einzuleiten. Diese können folgende Aspekte umfassen:
  
-   Kosten durch Verlust des Wettbewerbsvorteils, der aufgrund der Veröffentlichung gesetzlich geschützter oder vertraulicher Informationen entsteht.
  
-   Kosten für Rechtsbeistand.
  
-   Lohnkosten für die Analyse des Verstoßes, erneute Installation der Software und Wiederherstellung der Daten.
  
-   Kosten aufgrund der Systemausfallzeit (z. B. verlorene Arbeitnehmerproduktivität, verlorene Umsätze, Ersatz der Hardware, Software und Ersatz für anderes Eigentum).
  
-   Kosten für Reparaturen und mögliche Aktualisierung beschädigter oder unwirksamer physischer Sicherheitsmaßnahmen (Schlösser, Wände, Behälter und so weiter).
  
-   Andere indirekte Schäden, wie z. B. Verlust des Rufs oder des Kundenvertrauens.
  
#### Überprüfen der Reaktions- und Aktualisierungsrichtlinien
  
Nachdem die Dokumentations- und die Wiederherstellungsphasen abgeschlossen sind, sollten Sie den Prozess gründlich überprüfen. Bestimmen Sie mit Ihrem Team, welche Schritte erfolgreich durchgeführt und welche Fehler gemacht wurden. In fast allen Fällen werden Sie einige Prozesse finden, die geändert werden müssen, damit Sie zukünftige Vorfälle besser behandeln können.
  
Sie werden Schwächen in Ihrem Vorfallantwortplan finden. Zweck dieses „Autopsieschritts“ ist es, Möglichkeiten zur Verbesserung zu finden und damit einen neuen Zyklus im Vorfallreaktionsplanungsprozess einzuleiten.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Verwandte Informationen
  
Vieles in diesem Dokument betrifft Maßnahmen, die Sie ergreifen können, um die Gefahr eines Angriffs zu minimieren. Jedoch erreichen Organisationen ihre Sicherheitsziele mit dem größten Erfolg, wenn sie alles in ihrer Macht stehende unternehmen, um ihre Angriffsfläche zu minimieren, und dann die Maßnahmen für den Fall eines Angriffs planen. Teil dieses Prozesses sollte eine sorgfältige Überwachung sein. Ein anderer, gleichermaßen wichtiger Aspekt stellt die Bereitstellung einer Reihe deutlich definierter, gut geprobter Maßnahmen dar, die ergriffen werden können, wenn ein Angriff stattfindet.
  
Weitere Informationen zum Erstellen eines Angriffsmaßnahmenplans finden Sie hier:
  
-   *Hacking Exposed Windows 2000* von Joel Scambray und Stuart McClure (McGraw-Hill Professional Publishing, ISBN: 007292623).
  
-   [Handbook for Computer Security Incident Response Teams](http://go.microsoft.com/fwlink/?linkid=22398) auf der SEI-Website unter [http://go.microsoft.com/fwlink/?LinkId=22398](http://go.microsoft.com/fwlink/?linkid=22398).
  
-   [Forum of Incident Response and Security Teams (FIRST)](http://go.microsoft.com/fwlink/?linkid=22399) auf der FIRST-Website unter [http://go.microsoft.com/fwlink/?LinkId=22399](http://go.microsoft.com/fwlink/?linkid=22399).
  
-   *Incident Response: Investigating Computer Crime* von Chris Prosise und Kevin Mandia (McGraw-Hill Professional Publishing, ISBN: 00723829).
  
Weitere Informationen zum Thema Sicherheit finden Sie hier:
  
-   *The Internet Security Guidebook: &gt;From Planning to Deployment* von Juanita Ellis und Tim Speed (Academic Press, ISBN: 0223747).
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
