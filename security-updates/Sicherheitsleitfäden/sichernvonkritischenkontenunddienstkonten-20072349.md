---
TOCTitle: Sichern von kritischen Konten und Dienstkonten
Title: Sichern von kritischen Konten und Dienstkonten
ms:assetid: 'aed37382-e798-437b-8740-8a03412ed1ef'
ms:contentKeyID: 20072349
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc875826(v=TechNet.10)'
---

Sichern von kritischen Konten und Dienstkonten
==============================================

Veröffentlicht: 26. Sep 2006

##### Auf dieser Seite

[](#ehaa)[Einführung](#ehaa)
[](#egaa)[Definition](#egaa)
[](#efaa)[Herausforderungen](#efaa)
[](#eeaa)[Lösungen](#eeaa)
[](#edaa)[Zusammenfassung](#edaa)
[](#ecaa)[Anhang A: Gängige Dienste](#ecaa)

### Einführung

Der erste Schritt zur Sicherung des Netzwerks eines mittelgroßen Unternehmens besteht darin, sich darüber im Klaren zu sein, welche Schwachstellen ein Angreifer wahrscheinlich ausnutzen wird. Die Hauptaufgabe eines Angreifers, der in ein Netzwerk eingedrungen ist, besteht darin, eine Erhöhung von Berechtigungen zu bewirken. Auf diese Weise versucht ein Angreifer, die von ihm geöffnete Sicherheitslücke zu nutzen, um mehr Zugriffsrechte zu erhalten. Im Anschluss an eine Erhöhung von Berechtigungen gibt es kaum noch eine Möglichkeit, einen Eindringling von seinen Zielen abzuhalten, wie auch immer diese aussehen mögen. Angreifer können eine Erhöhung von Berechtigungen mit vielen verschiedenen Methoden bewirken, doch hauptsächlich ist damit die Manipulation von bestehenden Konten verbunden, insbesondere von Konten mit administratorähnlichen Rechten.

Bei Netzwerken mittelgroßer Unternehmen werden standardmäßige Benutzerkonten häufig einer gewissen Sicherheitskontrolle unterzogen. Dienstkonten erfahren dagegen oft nur wenig Kontrolle. Dadurch weisen sie Sicherheitsanfälligkeiten auf und werden so zu beliebten Zielen für Angreifer. Nachdem ein Angreifer sich soweit Zugang zu einem Netzwerk verschafft hat, dass dabei kritische Konten mit hohen Berechtigungen in Mitleidenschaft gezogen werden, kann das gesamte Netzwerk nie wieder als vollständig vertrauenswürdig eingestuft werden, solange es nicht von Grund auf neu aufgebaut wird. Aus diesem Grund ist der Sicherheitsgrad von jeder Art von Konto ein sehr wichtiger Aspekt bei Netzwerksicherheitsinitiativen.

Neben den durch externe Bedrohungen verursachten Risiken für die Netzwerke mittelgroßer Unternehmen können auch interne Bedrohungen sehr großen Schaden anrichten. Interne Bedrohungen gehen nicht nur von Benutzern mit böswilligen Absichten aus, sondern auch von solchen, die unbeabsichtigt Schaden anrichten könnten. Die scheinbar harmlosen Versuche von Benutzern, sich unter Umgehung von Sicherheitsmaßnahmen Zugriff auf Ressourcen zu verschaffen, sind dabei nur ein Beispiel. Aus praktischen Gründen erhalten Benutzer und Dienste viel zu häufig Zugriff auf höhere Rechte, als es erforderlich wäre. Diese Praktik stellt zwar sicher, dass Benutzer Zugriff auf die von ihnen zur Ausführung ihrer Aufgaben benötigten Ressourcen erhalten, erhöht aber gleichzeitig das Risiko, dass ein Angriff auf das Netzwerk Erfolg zeigt.

#### Kurzzusammenfassung

Wie in der Einführung bereits dargestellt wurde, ist das Sicherheitsmanagement bei allen Kontentypen innerhalb eines Netzwerks von größter Wichtigkeit, um Risiken für Netzwerke mittelgroßer Unternehmen in den Griff zu bekommen. Interne und externe Bedrohungen müssen gleichermaßen berücksichtigt werden. Die entsprechenden Maßnahmen müssen dabei so ausgerichtet sein, dass kein Konflikt zwischen den Sicherheitsanforderungen und der Funktionalität entsteht, die ein mittelgroßes Unternehmen von seinen Netzwerkressourcen erwartet.

Mithilfe dieses Dokuments können mittelgroße Unternehmen ein besseres Verständnis der Risiken erlangen, die mit Administrator-, Dienst-, anwendungsbezogenen und Standardkonten verbunden sind. Anhand dieser Informationen können dann Maßnahmen entwickelt und umsetzt werden, über die sich diese Risiken verringern lassen. Dazu ist es notwendig, auf die Beschaffenheit dieser Konten einzugehen: Wie lassen sie sich identifizieren? Wie lassen sich die zur Funktionsfähigkeit der Konten erforderlichen Berechtigungen festlegen? Wie können die Risiken verringert werden, die mit Dienstkonten und Konten auf Administratorebene verbunden sind?

Im Rahmen der Trustworthy Computing Initiative von Microsoft wurden die Standardeinstellungen von Microsoft® Windows Server™ 2003 darauf ausgerichtet, den Verzeichnisdienst Active Directory® vor vielen unterschiedlichen Bedrohungen zu schützen. Einige Einstellungen für Administratorkonten lassen sich jedoch noch weiter optimieren, um das Sicherheitsniveau der Netzwerkumgebung eines mittelgroßen Unternehmens zu erhöhen. Darüber hinaus müssen auch die Dienste gesichert werden, die nicht Teil des Betriebssystems Windows Server 2003 sind und im Zusammenhang mit anderen Anwendungen installiert wurden. In diesem Dokument werden Methoden zur Sicherung dieser Konten und Dienste erläutert sowie Best Practices (bewährte Methoden) zur Bereitstellung und Verwaltung von Administratorrechten.

#### Übersicht

Dieses Dokument ist in vier Hauptteile untergliedert, in denen Sie Informationen zur Sicherung von Administrator- und Dienstkonten in mittelgroßen Unternehmen finden. Der erste Abschnitt ist die Einführung, die Sie gerade lesen. Die übrigen Teile des Dokuments sind folgendermaßen gegliedert:

-   **Definition**: In diesem Abschnitt finden Sie Hintergrundinformationen sowie einige Erläuterungen zur Terminologie, die in diesem Dokument Verwendung findet.

-   **Herausforderungen**: In diesem Abschnitt werden einige der häufig auftretenden Probleme beschrieben, die mittelgroße Unternehmen bei der Ermittlung des Sicherungsbedarfs von Konten zu bewältigen haben. Daneben werden einige der mit der Sicherung von Administrator- und Dienstkonten verbundenen Probleme behandelt.

-   **Lösungen**: Dieser Abschnitt ist in drei Unterabschnitte aufgegliedert, in denen Sie Informationen zur Abfolge der Maßnahmen finden, mit denen sich kritische Konten und Dienstkonten in einem mittelgroßen Unternehmen sichern lassen. Diese Unterabschnitte umfassen folgende Elemente:

    -   **Einschätzung**: Dieser Unterabschnitt zeigt, welche grundsätzlichen Überlegungen bei der Sicherung von kritischen Konten und Dienstkonten angestellt werden müssen. Daneben wird die Grundlage für das Planen von Lösungen geschaffen.

    -   **Entwicklung**: In diesem Unterabschnitt werden auf der Grundlage der im Abschnitt „Einschätzung“ dargestellten Informationen Lösungen bereitgestellt, mit deren Hilfe Pläne aufgestellt werden können, über die sich die Sicherheit von kritischen Konten und Dienstkonten erhöhen lässt.

    -   **Bereitstellung und Verwaltung**: In diesem Unterabschnitt werden empfehlenswerte Methoden zur Implementierung gesicherter Administrator- und Dienstkonten in einem mittelgroßen Unternehmen beschrieben.

#### Zielgruppe dieses Dokuments

Dieses technische Dokument ist zur Unterstützung von Fachleuten und Managern im technischen Bereich gedacht, die um die Sicherheit von Konten auf Dienst-, Anwendungs- und Administratorebene innerhalb eines Microsoft-Netzwerks bedacht sind. Obgleich auch ein Leser ohne technischen Hintergrund aus diesem Dokument einen Informationszugewinn hinsichtlich der Prinzipien einer sicheren Kontoverwaltung erzielen kann, ist dennoch ein Verständnis der Kontoverwaltungskonzepte von Microsoft Windows® und Active Directory erforderlich, um den größtmöglichen Nutzen aus den in diesem Dokument dargestellten Informationen zu ziehen.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Definition

In diesem Abschnitt werden einige Begriffen definiert, die in diesem Dokument Verwendung finden und möglicherweise näher erläutert werden müssen.

-   **Dienste**: Dienste sind ausführbare Dateien, die beim Systemstart ausgeführt werden bzw. durch andere Ereignisse oder geplante Instanzen ausgelöst werden können. Dienste werden häufig im Hintergrund ausgeführt. Der Benutzer wird dabei kaum zu Eingaben bzw. anderen Interaktionen aufgefordert.

-   **Dienstkonten**: Unter einem Dienstkonto versteht man – einfach ausgedrückt – jede Art von Konto, das nicht einer Person zugeordnet ist. Dabei handelt es sich häufig um integrierte Konten, über die Dienste auf Ressourcen zugreifen, die zur Ausführung der für den jeweiligen Dienst festgelegten Aktionen erforderlich sind. Für einige Dienste werden jedoch tatsächliche Benutzerkonten zur Ausführung bestimmter Funktionen benötigt, und zahlreiche Unternehmen verwenden auch für die Ausführung von Diensten noch immer Domänenkonten.

-   **Administratorkonto**: Auch wenn bei jeder Neuinstallation einer Microsoft Windows- oder Active Directory-Domäne ein standardmäßiges Administratorkonto eingerichtet wird, bezieht sich der Begriff „Administratorkonto“ häufig ganz allgemein auf jede Art von Konto, das Rechte auf Administratorebene gewährt. Aus Gründen der Klarheit wird in diesem Dokument zwischen diesen beiden Verwendungszusammenhängen unterschieden.

-   **Administrative Gruppen**: Diese Gruppen können in Abhängigkeit von den installierten Diensten variieren. Dennoch können sie auch die Gruppen umfassen, die automatisch in den vordefinierten Containern und den Benutzercontainern erstellt wurden. Dazu zählen auch alle Gruppen, denen bei ihrer Erstellung Administratorrechte gewährt wurden.

-   **Kritische Konten**: Der Begriff „kritische Konten“ wird in diesem Dokument zur Beschreibung von Standardkonten verwendet, die als sehr risikoreich eingestuft werden, da sie mit hohen Berechtigungen verbunden sind. Auch aufgrund der Tatsache, dass diese Konten praktisch ständig und überall zum Einsatz kommen, stellen sie ein erhöhtes Risiko dar.

-   **Eingeschränkte Konten**: Unter einem eingeschränkten Konto versteht man ein Konto, das nicht zu einer administrativen Gruppe gehört und mit dem keine erhöhten Berechtigungen verbunden sind, die denen eines lokalen oder eines Domänenadministratorkontos entsprechen. In der Regel ist ein eingeschränktes Konto Mitglied der Gruppe „Domänenbenutzer“ oder der lokalen Benutzergruppe.

-   **Prinzip der geringsten Rechte**: Bei den Kriterien des amerikanischen Verteidigungsministeriums zur Beurteilung eines vertrauenswürdigen Computersystems („Department of Defense Trusted Computer System Evaluation Criteria“, DOD-5200.28-STD) – dem so genannten „Orange Book“ – handelt es sich um einen anerkannten Computersicherheitsstandard. Das Prinzip der „geringsten Rechte“ sieht entsprechend dieser Publikation vor, „dass jedem Benutzer innerhalb eines Systems nur die eingeschränktesten Rechte (bzw. die niedrigsten Freigabestufen) zugewiesen werden, die er zur Ausführung der Aufgaben benötigt, zu denen er berechtigt ist. Durch die Anwendung dieses Prinzips lassen sich Schäden, die durch Unfälle, Fehler oder unberechtigte Nutzung verursacht werden, begrenzen.“

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Herausforderungen

Wie bereits im vorangegangenen Abschnitt erwähnt wurde, stellen ungesicherte Konten auf Administratorebene sowie ungesicherte Dienstkonten ein beträchtliches Risiko für die Sicherheit des Netzwerks eines mittelgroßen Unternehmens dar. Angesichts der Komplexität von Netzwerkumgebungen und der hohen Wachstumsraten, die in den meisten Unternehmensnetzwerken zu verzeichnen sind, weisen Kontoverwaltungsverfahren häufig große Sicherheitsrisiken auf. Aufgrund dieser Faktoren kann die Sicherung der kritischen Konten und der Dienste, die in einem Netzwerk ausgeführt werden, eine echte Herausforderung sein.

Im Folgenden sind einige häufig anzutreffende Probleme aufgelistet, die sich für mittelgroße Unternehmen ergeben, wenn die richtige Vorgehensweise zur Lösung dieser Sicherheitsfragen bestimmt werden soll:

-   Schützen des Unternehmens gegen interne und externe Bedrohungen, die sich aus der Kontoverwaltung ergeben oder daraus, dass Mitarbeiter versuchen, Sicherheitsvorkehrungen zu umgehen

-   Identifizieren aller Dienstkonten und anwendungsbezogenen Konten, die im Netzwerk und auf den lokalen Computern verwendet werden

-   Sichern von sicherheitskritischen Dienst-, Administrator- und anwendungsbezogenen Konten

-   Bestimmen, welche Konten mit Diensten und Anwendungen verbunden sind

-   Trennen der Dienstkonten von Benutzerkonto-Kennwortrichtlinien

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Lösungen

Die in diesem Dokument dargestellten Lösungen orientieren sich am Prinzip der geringsten Rechte sowie an der Methode der Vergabe von Benutzerkonten mit möglichst geringen Berechtigungen bei der Verwaltung von Dienst-, Administrator- und kritischen Konten.

Beim Training und in Dokumentationsunterlagen im Zusammenhang mit Sicherheitsfragen wird in den meisten Fällen auf das Prinzip der geringsten Rechte hingewiesen. Auch wenn dieses Prinzip relativ leicht zu verstehen ist, lassen sich damit beträchtliche Verbesserungen am Sicherheitsprofil eines jeden Unternehmens erreichen, das es umsetzt. Einfach ausgedrückt besagt dieses Prinzip, dass sämtliche Konten lediglich das absolute Mindestmaß an Berechtigungen aufweisen sollten, das erforderlich ist, um die derzeit unter dem jeweiligen Konto zu bearbeitenden Aufgaben auszuführen. Dieses Prinzip hat nicht nur für Benutzer Gültigkeit, sondern auch für Computer und die Dienste, die auf ihnen ausgeführt werden.

Die Befolgung dieses Prinzips ermöglicht nicht nur den Schutz vor böswilligen Angreifern und Malware, sondern trägt auch zur Verbesserung des Sicherheitsprofils eines Unternehmens bei, da Technologieexperten umfassende Ermittlungen durchführen müssen, um zu bestimmen, welche Zugriffsrechte für Benutzer, Computer und Anwendungen erforderlich sind. Anhand dieser Informationen lässt sich erkennen, welche Prozesse oder Einstellungen als unsicher einzustufen sind und einen besseren Schutz benötigen. Damit bilden diese Informationen die Grundlage für jede erfolgreiche Sicherheitsinitiative.

Beispielsweise sollte entsprechend dem Prinzip der geringsten Rechte eine Person, die die Funktion des Domänenadministrators ausübt, nur dann ein Konto verwenden, das über Berechtigungen auf Domänenadministratorebene verfügt, wenn Aufgaben ausgeführt werden, die Zugriffsrechte auf dieser Ebene erfordern. Wenn dagegen keine Aufgaben ausgeführt werden, die höhere Berechtigungen erfordern, sollte ein Administrator ein Konto mit Standardzugriffsrechten verwenden. Mit dieser Verfahrensweise ließen sich Sicherheitsbedrohungen verringern, die auf menschlichen Fehlern beruhen. Daneben würde auch weniger Schaden entstehen, wenn die Arbeitsstation eines Administrators mit Malware infiziert würde.

#### Einschätzung

Für die Sicherung von Dienstkonten und kritischen Konten muss bestimmt werden, wie diese Konten definiert sind und welche Bedrohungen mit ihnen verbunden sind. Es muss jedoch auch klar ersichtlich sein, welche Folgen sich im Falle der Modifizierung dieser Konten ergeben, so dass negative Auswirkungen auf das Unternehmen auf ein erträgliches Maß begrenzt bleiben.

##### Verwaltung von kritischen Konten und Administratorkonten

Um kritische Konten und Administratorkonten sowie die ihnen zugeordneten Gruppen sichern zu können, muss bekannt sein, welche Konten und Gruppen dieses Kriterium erfüllen. Auch ist es wichtig zu wissen, welchen Umfang Rechte auf Administratorebene haben und auf welche Systeme sie sich erstrecken, insbesondere dann, wenn über sie Domänencontroller gesteuert werden.

Daher ist es maßgeblich, dass die Leser dieses Dokuments genaue Kenntnisse über die Konten auf Administratorebene in ihrer Systemumgebung haben. Daneben müssen sie sämtliche Domänencontroller kennen sowie die Konten, die von diesen verwaltet werden.

###### Administratorkonten und administrative Gruppen

Folgende Konten zählen zu den Konten auf Administratorebene in einem Active Directory-Netzwerk:

-   Das Standardadministratorkonto, das erstellt wird, wenn Active Directory auf dem ersten Domänencontroller einer Domäne installiert wird. Dieses Konto ist das höchste Konto in einer Domäne. Bei der Erstellung des Kontos muss ein Kennwort dafür eingerichtet werden.

-   Zu einem späteren Zeitpunkt erstellte Konten, denen Administratorrechte entweder auf direktem Weg oder durch die Aufnahme in einer administrative Gruppe gewährt werden.

Administrative Gruppen innerhalb einer Active Directory-Domäne variieren in Abhängigkeit von den in dieser Domäne installierten Diensten. Eine Active Directory-Domäne in der Basisausführung umfasst folgende Elemente:

-   Automatisch im vordefinierten Container erstellte administrative Gruppen

-   Automatisch im Benutzercontainer erstellte administrative Gruppen

-   Zu einem späteren Zeitpunkt erstellte Gruppen, die entweder in Gruppen mit Administratorrechten aufgenommen werden oder denen Administratorrechte zugewiesen werden.

###### Dienstadministratoren und Datenadministratoren

In einer Windows Server 2003 Active Directory-Umgebung gibt es zwei unterschiedliche Arten von Administratorrechten: Dienstadministratoren und Datenadministratoren.

-   Über Dienstadministratorkonten wird die Verwaltung und Bereitstellung von Verzeichnisdiensten gesteuert, einschließlich der Verwaltung von Domänencontrollern und Active Directory.

-   Über Datenadministratorkonten werden die im Verzeichnisdienst gespeicherten Daten auf Domänenmitgliedsservern und Arbeitsstationen in der Domäne verwaltet.

Auch wenn Personen in jeder Umgebung beide Rollen einnehmen können, ist es entscheidend, die Standardkonten und -gruppen zu kennen, die dem Kompetenzbereich nach Dienstadministratoren entsprechen. Dienstadministratorkonten haben innerhalb einer Netzwerkumgebung eine große Handlungsfreiheit und müssen daher am stärksten geschützt werden. Diese Konten sind verantwortlich für Einstellungen, die das gesamte Verzeichnis betreffen, für die Installation und Verwaltung von Software sowie für die Installation von Service Packs und Updates für Betriebssysteme auf Domänencontrollern.

**Tabelle 1 – Standardmäßige Dienstadministratorgruppen und -konten**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Name</p></th>
<th><p>Container</p></th>
<th><p>Beschreibung</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Vordefiniert</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe hat Vollzugriff auf alle Domänencontroller sowie auf sämtliche in einer Domäne gespeicherten Verzeichnisinhalte. Bei dieser Gruppe handelt es sich um die höchste Dienstadministratorgruppe. Sie kann die Mitgliedschaft aller anderen administrativen Gruppen verändern.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Organisations-Admins</p></td>
<td style="border:1px solid black;"><p>Benutzer</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe wird in jeder Domäne automatisch der Gruppe „Administratoren“ hinzugefügt und hat Vollzugriff auf die Konfiguration sämtlicher Domänencontroller.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Domänen-Admins</p></td>
<td style="border:1px solid black;"><p>Benutzer</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe wird in jeder Domäne einer Gesamtstruktur automatisch der Gruppe „Administratoren“ hinzugefügt Daher haben die Domänen-Admins Zugriffsrechte auf alle Domänencontroller sowie auf Daten, die im Verzeichnis einer Domäne gespeichert sind. Sie können die Mitgliedschaft aller administrativen Gruppen modifizieren.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Schema-Admins</p></td>
<td style="border:1px solid black;"><p>Benutzer</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe verfügt über volle Administratorrechte für das Active Directory-Schema.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Konten-Operatoren</p></td>
<td style="border:1px solid black;"><p>Vordefiniert</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe kann Konten und Gruppen in der Domäne erstellen und verwalten, jedoch keine Dienstadministratorkonten verwalten. Diese Gruppe hat standardmäßig keine Mitglieder und sollte bei einer auf Best Practices basierenden Verfahrensweise nicht zur Delegierung von Verwaltungsaufgaben verwendet werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Sicherungs-Operatoren</p></td>
<td style="border:1px solid black;"><p>Vordefiniert</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe gewährt Berechtigungen zur Ausführung von Sicherungs- und Wiederherstellungsaufgaben auf Domänencontrollern. Sie hat standardmäßig keine Mitglieder.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Server-Operatoren</p></td>
<td style="border:1px solid black;"><p>Vordefiniert</p></td>
<td style="border:1px solid black;"><p>Diese Gruppe kann Wartungsaufgaben auf Domänencontrollern ausführen. Sie hat standardmäßig keine Mitglieder.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DS-Wiederherstellungsmodus-Administrator</p></td>
<td style="border:1px solid black;"><p>Nicht in Active Directory gespeichert</p></td>
<td style="border:1px solid black;"><p>Dieses Konto wird während des Active Directory-Installationsvorgangs erstellt. Dieses Konto wird verwendet, um den Domänencontroller im Modus „Verzeichnisdienste wiederherstellen“ zu starten. Auch wenn dieses Konto nicht dem Administratorkonto entspricht, verfügt es über Vollzugriff auf den Domänencontroller, solange dieser sich im Modus „Verzeichnisdienste wiederherstellen“ befindet.</p></td>
</tr>
</tbody>
</table>
  
Die in der vorangehenden Tabelle aufgeführten Dienstadministratorgruppen und -konten werden durch einen Hintergrundprozess geschützt, der in gewissen Zeitabständen eine bestimmte Sicherheitsbeschreibung prüft und anwendet, die diesem geschützten Objekt zugeordnete Sicherheitsinformationen enthält. Dieser Prozess erstreckt sich alle Mitglieder einer Dienstadministratorgruppe und gewährleistet, dass jeder erfolgreiche unbefugte Versuch, diese Sicherheitsbeschreibung für ein Mitglied einer administrativen Gruppe zu verändern, mit den geschützten Einstellungen aus der Datenstruktur der Sicherheitsbeschreibung überschrieben wird.
  
Die Datenstruktur der Sicherheitsbeschreibung befindet sich im Objekt „AdminSDHolder“. Um also die Berechtigungen einer Dienstadministratorgruppe oder eines ihrer Mitgliederkonten zu verändern, muss die Sicherheitsbeschreibung im Objekt „AdminSDHolder“ so modifiziert werden, dass die Änderungen einheitlich vorgenommen werden. Alle an der Sicherheitsbeschreibung vorgenommenen Änderungen werden auf die Standardeinstellungen für sämtliche geschützte Administratorkonten angewendet. Berechtigungen dürfen auf diese Weise also nur mit größter Vorsicht verändert werden.
  
Weitere Informationen zum Ändern von Berechtigungen für Dienstadministratorkonten finden Sie im [Leitfaden mit Best Practices zur Sicherung von Active Directory-Installationen](http://www.microsoft.com/downloads/details.aspx?familyid=4e734065-3f18-488a-be1e-f03390ec5f91&displaylang=en) (möglicherweise in Englisch). Diese Veröffentlichung kann unter der folgenden Adresse heruntergeladen werden: www.microsoft.com/downloads/details.aspx?FamilyID=4e734065-3f18-488a-be1e-f03390ec5f91&DisplayLang=en.
  
#### Verwaltung von Dienst- und Anwendungskonten
  
Dienste sind ausführbare Dateien, bei deren Ausführung häufig keine Interaktion mit dem Benutzer stattfindet. Ihr Start erfolgt automatisch mit dem Start eines Betriebssystems. Aus diesem Grund werden Dienste und Dienstkonten als beträchtliches Sicherheitsrisiko in einem Unternehmensnetzwerk oft übersehen. Auch wenn die Sicherheitsrisiken erkannt werden, kann sich die Dienstkontenverwaltung als ziemlich komplexes Unterfangen erweisen, wenn man bedenkt, dass selbst die einfache Änderung eines Kennworts möglicherweise einige weitere Änderungen erfordert, damit es nicht zu einem Systemausfall kommt.
  
Windows Server 2003 verfügt zwar über standardmäßige Dienste und Dienstkonten, die vor Bedrohungen geschützt sind, doch zahlreiche Dienste von Drittanbietern und selbst andere Zusatzdienste von Microsoft müssen geschützt werden, da sie zum ordnungsgemäßen Betrieb Dienstkonten erfordern. Dies trifft besonders auf Unternehmensverwaltungstools wie Microsoft Systems Management Server oder IBM Tivoli zu, da diese oft die Verwendung eines Kontos voraussetzen, das mit Rechten für die gesamte Domäne oder sogar für andere Domänen mit Vertrauensstellung ausgestattet ist.
  
Darüber hinaus werden für das Ausführen von Diensten häufig immer noch Domänenkonten eingesetzt, da es – ungeachtet der mit dieser Methode verbundenen Sicherheitsrisiken – bisher als einfacher angesehen wurde, Dienste domänenübergreifend zu verwalten statt auf einzelnen Servern. Dienste speichern die Informationen zu den von ihnen verwendeten Benutzerkonten und Kennwörtern in der Registrierung, unabhängig davon, ob lokale Konten oder Domänenkonten verwendet werden. Wenn also die Sicherheit eines einzelnen Computers verletzt wird, kann der Angreifer diese Informationen nutzen, um seine Berechtigungen zu erhöhen, wenn diese Dienste Domänenkonten verwenden. Wenn ein Dienst ein Domänenkonto auf Administratorebene verwendet, könnte ein derartiges Szenario das gesamte Netzwerk gefährden.
  
##### Szenarien hinsichtlich der Sicherheitsanfälligkeit von Dienstkonten
  
Die Praktik, Dienste so zu konfigurieren, dass sie Domänenkonten zur Authentifizierung verwenden, führt zu potenziellen Sicherheitsanfälligkeiten. Das Ausmaß der möglichen Risiken hängt von zahlreichen Faktoren ab:
  
-   **Die Anzahl der Server, auf denen Dienste für eine Verwendung von Dienstkonten konfiguriert sind**: Das Sicherheitsanfälligkeitsprofil eines Netzwerks erhöht sich mit jedem Server, der über Dienste verfügt, die über das Domänenkonto authentifiziert und auf diesem Server ausgeführt werden. Mit steigender Anzahl solcher Server steigt auch die Wahrscheinlichkeit, dass ein Angreifer Zugriff auf diesen Server erhält und so anderen Netzwerkressourcen höhere Berechtigungen zuweisen kann.
  
-   **Der Wirkungsbereich der Berechtigungen eines Domänenkontos, das von Diensten verwendet wird**: Je größer der Wirkungsbereich der mit einem Dienstkonto verbundenen Rechte ist, desto mehr Ressourcen können durch dieses Konto in ihrer Sicherheit verletzt werden. Berechtigungen auf Domänenadministratorebene stellen ein besonders hohes Risiko dar, da jeder Computer des Netzwerks, einschließlich des Domänencontrollers, vom Ausmaß der Sicherheitsanfälligkeit solcher Konten betroffen ist. Da diese Konten über Administratorrechte für sämtliche Mitgliederserver verfügen, hätte eine Sicherheitsverletzung bei einem solchen Konto schwerwiegende Folgen, da sämtliche Computer und Daten der Domäne dann nicht mehr vertrauenswürdig wären.
  
-   **Die Anzahl der Dienste, die auf einem bestimmten Server für die Verwendung von Domänenkonten konfiguriert sind**: Einige Dienste weisen besondere Sicherheitsanfälligkeiten auf, die sie leichter zum Ziel von Angriffen werden lassen. Angreifer versuchen in der Regel zuerst, bekannte Sicherheitsanfälligkeiten auszunutzen. Wenn ein Domänenkonto einen Dienst verwendet, der Sicherheitsanfälligkeiten aufweist, bedeutet dies ein erhöhtes Risiko für andere Systeme, das andernfalls auf einem einzelnen Server hätte isoliert werden können.
  
-   **Die Anzahl der Domänenkonten, die zum Ausführen von Diensten in einer Domäne verwendet werden**: Die Sicherheit von Dienstkonten muss mit mehr Sorgfalt überwacht und verwaltet werden als die Sicherheit von gewöhnlichen Benutzerkonten. Mit jedem zusätzlichen, von Diensten verwendeten Domänenkonto wird auch die Verwaltung dieser Konten weiter verkompliziert. Die Tatsache, dass Administratoren und Sicherheitsadministratoren wissen müssen, wo das jeweilige Dienstkonto verwendet wird, wenn sie verdächtige Vorgänge identifizieren möchten, unterstreicht noch einmal mehr, wie wichtig es ist, die Anzahl solcher Konten zu minimieren.
  
Ausgehend von den oben genannten Faktoren sind im Hinblick auf Sicherheitsanfälligkeiten verschiedene Szenarien denkbar. Jedes dieser Szenarien ist mit einem unterschiedlich hohen potenziellen Sicherheitsrisiko verbunden. Diese Szenarien werden in der im Folgenden abgebildeten Grafik und Tabelle beschrieben.
  
Diese Beispiele gehen davon aus, dass es sich bei den Dienstkonten um Domänenkonten handelt und dass jedes Konto über mindestens einen Dienst auf jedem Server verfügt und diesen zur Authentifizierung verwendet. Die folgenden Informationen beschreiben die unten dargestellten Domänenkonten.
  
-   Konto A verfügt über administratorähnliche Rechte für mehr als einen Domänencontroller.
  
-   Konto B verfügt über administratorähnliche Rechte für alle Mitgliedsserver.
  
-   Konto C verfügt über administratorähnliche Rechte für Server 2 und 3.
  
-   Konto D verfügt über administratorähnliche Rechte für Server 4 und 5.
  
-   Konto E verfügt nur für einen einzigen Mitgliedsserver über administratorähnliche Rechte.
  
    ![](images/Cc875826.SCASA1(de-de,TechNet.10).gif)
  
    **Abbildung 1 – Szenarien hinsichtlich der Sicherheitsanfälligkeit von Domänendienstkonten**
  
Die folgende Tabelle beschreibt die oben in Text und Bild dargestellten Szenarien und ordnet sie nach den mit ihnen verbundenen Sicherheitsanfälligkeiten.
  
**Tabelle 2 – Rangordnung der Szenarien hinsichtlich unterschiedlicher Sicherheitsanfälligkeiten**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Szenario</p></th>
<th><p>Beschreibung</p></th>
<th><p>Risikostufe</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Konto A wird von einem Dienst auf Server 1 verwendet. Nach einer Sicherheitsverletzung auf Server 1 werden die Authentifizierungsdaten für Konto A offen gelegt. Daraufhin hat der Angreifer Zugriff auf den DC1-Domänencontroller. Ausgehend von diesem werden alle Ressourcen auf der Domäne und alle darin enthaltenen Daten anfällig gegenüber Sicherheitsverletzungen.</p>
<p>Diese Situation stellt ein kritisches Risikoszenario dar. Domänenkonten mit administratorähnlichen Rechten für die Domäne oder den Domänencontroller sollten nie eingesetzt werden, um Dienste auf einem Mitgliedsserver auszuführen.</p></td>
<td style="border:1px solid black;"><p>Kritisch</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>2</p></td>
<td style="border:1px solid black;"><p>Konto B wird von einem Dienst auf Server 2 verwendet. Konto B verfügt auch über Berechtigungen für Server 1, auf dem Konto A einen Dienst ausführt. Nachdem eine Sicherheitsverletzung von Konto B auf Server 2 aufgetreten ist, verfügt der Angreifer über denselben Zugriff wie in Szenario 1. Damit ist der Domänencontroller sowie die gesamte Domäne für Angriffe anfällig.</p>
<p>Konto C setzt das Netzwerk demselben Risiko aus, da es über einen Angriff auf Server 3 für eine Sicherheitsverletzung auf Server 2 verwendet werden kann. Dadurch wird Konto A anfällig für eine Ausnutzung, was wiederum die gesamte Domäne gefährdet.</p>
<p>Hierbei handelt es sich um Szenarien mit hohem Risiko, doch sind in dieser Situation Lösungen möglich, wenn Maßnahmen gegen die potenziellen Bedrohungen aus Szenario 1 ergriffen wurden.</p></td>
<td style="border:1px solid black;"><p>Hoch</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>3</p></td>
<td style="border:1px solid black;"><p>Konto D wird von einem auf Server 4 und 5 ausgeführten Dienst verwendet. Nach einer Sicherheitsverletzung von Konto D erhält ein Angreifer Zugriff auf sämtliche Server, auf denen Konto D über Berechtigungen verfügt. Wenn auf diesen Servern keine Dienste ausgeführt werden, die Konten mit höheren oder umfangreicheren Rechten verwenden, stellt dieses Szenario eine Gefahr mittlerer Priorität dar, weil die Durchlässigkeit für Sicherheitsverletzungen aus Szenario 2 nicht vorhanden ist.</p></td>
<td style="border:1px solid black;"><p>Mittel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>4</p></td>
<td style="border:1px solid black;"><p>Konto E wird von einem Dienst verwendet, der auf einem einzigen Server – Server 5 – ausgeführt wird, und verfügt über keine weiteren Berechtigungen oder zugeordneten Dienste. Dieses Szenario stellt eine geringe Bedrohung dar, denn hier ist es nicht möglich, Berechtigungen über einen einzigen Server hinaus zu erhöhen.</p></td>
<td style="border:1px solid black;"><p>Gering</p></td>
</tr>
</tbody>
</table>
  
Die jeweilige Risikostufe der oben beschriebenen Szenarien lässt sich am besten wie folgt erklären:
  
-   **Kritische Risikostufe**: Dieses Risiko würde die Sicherheit des gesamten Netzwerks und Unternehmens unmittelbar gefährden.
  
-   **Hohe Risikostufe**: Dieses Risiko kann potenziell zu Verletzungen der Sicherheit des gesamten Netzwerks führen, ist jedoch nicht so unmittelbar wie ein kritisches Risiko.
  
-   **Mittlere Risikostufe**: Es ist wichtig, dieses Risiko zu thematisieren. Es könnten mehrere Server davon betroffen sein, doch es wird kein kritischer Server einer Sicherheitsgefahr ausgesetzt.
  
-   **Geringe Risikostufe**: Hierbei könnte es zu einer Sicherheitsverletzung auf einem einzigen Server kommen, doch kritische Server werden nicht gefährdet.
  
#### Systemkonten
  
Dienste erfordern Konten, um auf Ressourcen und Objekte zuzugreifen, die von dem Betriebssystem verwaltet werden, auf dem die Dienste ausgeführt werden. Wenn ein von einem Dienst verwendetes Konto nicht über ausreichende Berechtigungen zur Anmeldung verfügt, gewährt das Snap-In „Dienste“ in der Microsoft Management Console (MMC) automatisch das für das Konto benötigte Benutzerrecht „Als Dienst anmelden“ auf dem verwalteten Computer.
  
Windows Server 2003 bietet die folgenden drei vordefinierten lokalen Konten, die als Anmeldekonten für eine Reihe von Systemdiensten verwendet werden.
  
-   **Lokales System**: Das lokale Systemkonto, das im Netzwerk als DOMAIN*\\&lt;Computername&gt;*$ und lokal als NT AUTHORITY\\System dargestellt wird, ist ein vordefiniertes lokales Konto, mit dem Dienste gestartet werden können und das den Sicherheitskontext für den betreffenden Dienst bietet. Diesem mit hohen Rechten ausgestatteten Konto hat Vollzugriff auf den lokalen Computer. Im Falle einer Verwendung auf Domänencontrollern besteht zudem Vollzugriff auf die Verzeichnisdienste. Auch wenn einige Dienste so konfiguriert sind, dass sie dieses Konto unter Windows Server 2003 standardmäßig verwenden, sollte es nicht anderweitig verwendet werden, da es ein offensichtliches Sicherheitsrisiko darstellt, insbesondere auf Domänencontrollern.
  
-   **Lokaler Dienst**: Das lokale Dienstkonto (NT AUTHORITY\\LocalService) ist ein vordefiniertes Konto, das mit eingeschränkten Rechten ausgestattet ist, die einem authentifizierten lokalen Benutzerkonto entsprechen. Dieser eingeschränkte Zugriff dient als Sicherungsmechanismus für den Fall, dass der Dienst oder Prozess, der das Konto verwendet, Ziel einer Sicherheitsverletzung geworden ist. Dienste, die als das lokale Dienstkonto ausgeführt werden, greifen als NULL-Sitzung auf Netzwerkressourcen zu. Anders ausgedrückt, verwenden sie anonyme Anmeldeinformationen.
  
-   **Netzwerkdienst**: Beim Netzwerkdienstkonto (NT AUTHORITY\\NetworkService) handelt es sich um ein vordefiniertes Konto, das ähnlich wie das lokale Dienstkonto über eingeschränkte Rechte verfügt. Die Dienste und Prozesse, die dieses Konto verwenden, nutzen für den Zugriff auf Netzwerkressourcen jedoch keine anonymen Anmeldeinformationen, sondern die des Computerkontos.
  
**Hinweis:**   Die Änderung der Standardeinstellungen von Diensten kann möglicherweise die Funktionsfähigkeit von wichtigen Diensten beeinträchtigen. Die Einstellungen **Starttyp** und **Anmelden als** für Dienste, die standardmäßig automatisch beim Systemstart gestartet werden, sollten nur mit Vorsicht geändert werden.
  
#### Standardsicherheitseinstellungen für Windows Server 2003-Dienste
  
Vor Windows XP und Windows Server 2003 verwendeten fast alle vom Betriebssystem erstellten Dienste standardmäßig das lokale Systemkonto. Mit dieser Funktionalität waren einige offensichtliche Sicherheitsrisiken verbunden, da solche Dienste mit unbeschränkten Rechten für den lokalen Computer ausgestattet waren. Die Standardeinstellungen wurden mit der Entwicklung von Windows Server 2003 geändert, um die inhärente Sicherheit des Betriebssystems zu verbessern. Demzufolge verwenden nun viele derselben Dienste standardmäßig die Konten „Lokaler Dienst“ oder „Netzwerkdienst“ und stellen so ein geringeres Sicherheitsrisiko dar.
  
Es sind noch immer einige Dienste vorhanden, die die Verwendung des lokalen Systemkontos erfordern. Dazu gehören die Dienste „Automatische Updates“, „Computerbrowser“, „Nachrichtendienst“ und „Windows Installer“. Dienste, die immer noch das lokale Systemkonto zur Authentifizierung verwenden, sollten nicht dahingehend geändert werden, dass sie andere Konten verwenden. Dies könnte nämlich schwerwiegende Probleme verursachen und potenziell die Funktionsfähigkeit solcher Dienste beeinträchtigen.
  
In der folgenden Tabelle sind Dienstkonten aufgelistet, die unter Windows Server 2003 nicht mehr das lokale Systemkonto verwenden. Daneben wird der nun verwendete Kontotyp angegeben:
  
**Tabelle 3 – Windows Server 2003: Neue Dienstkontoeinstellungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Service</p></th>
<th><p>Anmelden als</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Warndienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Gatewaydienst auf Anwendungsebene</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Remoteregistrierung</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Smartcard</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TCP/IP-NetBIOS-Hilfsprogramm</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Telnet</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Unterbrechungsfreie Stromversorgung (USV)</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WebClient</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Windows-Bilderfassung</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Windows-Zeitgeber</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WinHTTP-Web Proxy Auto-Discovery-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DHCP-Client</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Distributed Transaction Coordinator</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DNS-Client</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lizenzprotokollierung</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Leistungsprotokollierung</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Remote Procedure Call (RPC) Locator</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
</tr>
</tbody>
</table>
  
#### Entwicklung
  
Für die Entwicklung eines Plans zur Sicherung von Administratorkonten und kritischen Konten ist es wichtig, die grundlegenden Elemente zu verstehen, auf denen sämtliche Best Practices aufgebaut sind. Jeder Schritt, der zur Sicherung von Konten und Diensten unternommen wird, beruht auf denselben Grundprinzipien. Diese Grundprinzipien sind wiederum Teil der Prozesse und Verfahrensweisen sämtlicher Best Practice-Prozesse und -Verfahren. In diesem Abschnitt werden diese Prinzipien und Grundüberlegungen dargestellt.
  
##### Verwaltung von kritischen Konten und Administratorkonten
  
Best Practice-Richtlinien für die Sicherung von Administratorkonten unter Windows Server 2003 beruhen auf der Anwendung des Prinzips der geringsten Rechte und der Verwendung von Benutzerkonten mit eingeschränkten Rechten. Der erste Schritt bei diesem Prozess besteht darin, die aktuelle Systemumgebung gründlich zu erfassen. Den folgenden drei Punkten kommt eine Schlüsselbedeutung bei der Entwicklung eines effektiven Plans zur Verbesserung der Sicherheit von Administratorkonten und kritischen Konten zu:
  
-   Erfassen und Dokumentieren der Systemumgebung
  
-   Anwendung des Prinzips der geringsten Rechte
  
-   Vergabe von Benutzerkonten mit möglichst geringen Berechtigungen
  
###### Erfassen und Dokumentieren der Systemumgebung
  
Auch wenn dieser erste und wichtigste Schritt zur Verbesserung der Sicherheit von Konten mit administratorähnlichen Rechten offensichtlich scheint, kann darin manchmal der schwierigste Schritt in diesem Prozess bestehen. Wenn ein Unternehmen die Verwendung von Berechtigungen auf Administratorebene nicht beschränkt und dokumentiert hat, kann es sich als ziemlich schwierig erweisen festzustellen, wo Berechtigungen auf Administratorebene bestehen – insbesondere im Hinblick auf lokale Konten.
  
In Bezug auf Konten auf Administratorebene und andere sicherheitskritische Konten geht es beim Erfassen und Dokumentieren einer Netzwerkumgebung um die Klärung folgender Fragen: Wer, weshalb, was und wo. Das heißt: *Wer* ist berechtigt, Administratorkonten zu verwenden? *Weshalb* verfügen die betreffenden Personen über den Zugriff auf Administratorkonten? Für *welche* Aufgaben ist die Gewährung von administrativen Anmeldeinformationen angemessen? *Wo* ist die Sicherheit für den Einsatz solcher Anmeldeinformationen gewährleistet?
  
Der wichtigste Aspekt beim Dokumentieren dieser Informationen besteht in der Festlegung von Prozessen und Verfahrensweisen, über die geprüft wird, wo Administratorkonten verwendet werden, weshalb sie verwendet werden, wer sie verwendet hat und welche Aufgaben bei ihrer Verwendung ausgeführt wurden. Die Aufzeichnung dieser Informationen erfolgt am besten proaktiv durch den Einsatz von Bereitstellungs-, Änderungssteuerungs- und Vorfallsmanagementprozessen, über die erreicht wird, dass jede Aktion autorisiert und aufgezeichnet werden muss, bevor eine Aufgabe abgeschlossen wird. Derartige Prozesse ermöglichen die genaue Überprüfung der Nutzung von Administratorrechten, was es zudem wesentlich einfacher macht, verdächtige Vorgänge zu identifizieren.
  
Wie aus der weiteren Lektüre dieses Dokuments noch ersichtlich wird, ist das Erfassen und Dokumentieren einer Netzwerkumgebung der wichtigste Schritt zur Verbesserung der Sicherheit von kritischen Konten. Ein grundlegender Teil dieses Prozesses besteht darin, für die Verwendung und Vergabe von sicherheitskritischen Konten an Best Practices ausgerichtete Prozesse und Verfahrensweisen festzulegen. Dies sollte noch vor der Implementierung aller weiteren in diesem Dokument enthaltenen Richtlinien erfolgen.
  
###### Anwendung des Prinzips der geringsten Rechte
  
Einer der wohl wichtigsten Schritte, den ein Unternehmen zur Optimierung seiner Netzwerkumgebung ergreifen kann, besteht in der Anwendung des Prinzips der geringsten Rechte. Die Vergabe von Berechtigungen auf Administratorebene ist zwar häufig der einfachste und schnellste Weg, um komplexe Probleme im Zusammenhang mit Rechten bzw. Berechtigungen zu lösen, doch gleichzeitig ist dies auch die mit den größten Risiken verbundene Methode. Gleichfalls ist es für Systemadministratoren zwar wesentlich leichter, für alle Aufgaben ein Konto mit Administratorberechtigungen zu verwenden, doch erhöht sich durch eine solche Vorgehensweise auch das Risikoprofil des Netzwerks, für das die Systemadministratoren verantwortlich sind.
  
In seiner grundlegendsten Form lässt sich das Prinzip folgendermaßen anwenden: Die Verwendung von Berechtigungen auf Administratorebene sollte auf die berechtigten Mitarbeiter beschränkt bleiben und nur dann erfolgen, wenn die Bearbeitung der anstehenden Aufgabe derartig hohe Berechtigungen erfordert. Auch wenn eine Implementierung von Verfahrensweisen, bei denen dieses Prinzip berücksichtigt wird, beschwerlich scheint, dürfen die mit einer Nichtbefolgung dieses Prinzips verbundenen Risiken nicht ignoriert werden.
  
Bei Anwendung dieses Prinzips lässt sich das Risiko im Zusammenhang mit den häufigsten Sicherheitsanfälligkeiten, denen ein Netzwerk ausgesetzt sein kann, reduzieren. Im Folgenden sind einige Beispiele für diese Sicherheitsanfälligkeiten aufgelistet:
  
-   Kernelmodusrootkits
  
-   Programme zur Aufzeichnung von Tastaturanschlägen, die auf Systemebene ausgeführt werden
  
-   Versuche, Kennwörter abzufangen
  
-   Vorfälle in Zusammenhang mit Spyware und Adware
  
-   Nicht autorisierter Zugriff auf Daten
  
-   Installation von Trojanern
  
-   Ereignisprotokollmanipulationen
  
Bei reduziertem Einsatz von Administratorkonten bestehen auch weniger Möglichkeiten, die mit solchen Konten verbundenen hohen Berechtigungen für bösartige Aktivitäten zu missbrauchen. Dadurch wird das Sicherheitsprofil des Netzwerks verbessert. Wenn die Möglichkeit zur Vornahme größerer Änderungen am Betriebssystem nicht mehr gegeben ist, werden damit auch die Möglichkeiten zur Installation und Ausführung von Malware und Spyware beschränkt. Aus diesen Gründen kann sich die Anwendung des Prinzips der geringsten Rechte derartig stark auf die Netzwerksicherheit auswirken.
  
###### Vergabe von Benutzerkonten mit möglichst geringen Berechtigungen
  
In vielen Unternehmen ist es üblich, den Benutzern Administratorrechte für ihre eigenen Computer zu gewähren, insbesondere bei tragbaren Computern. Auch wenn es durchaus gute Gründe für die Gewährung solch hoher Berechtigungen geben mag, wird das Unternehmen dadurch einem höheren Risiko ausgesetzt.
  
Bei der Vergabe von Benutzerkonten mit möglichst geringen Berechtigungen werden Empfehlungen auf der Grundlage von Best Practices kombiniert, durch die es Unternehmen ermöglicht wird, Konten ohne Administratorrechte für die Bedienung von Windows XP-basierten Computern zu verwenden. Diese Verfahrensweisen führen zu einer praktischen Anwendung des Prinzips der geringsten Rechte für Windows XP-Clientgeräte.
  
In diesem Dokument werden die Grundsätze der Vergabe von Administratorkonten erörtert, wobei Berechtigungen auf Netzwerkebene eine besondere Berücksichtigung erfahren. Deshalb ist es ebenfalls wichtig zu bedenken, welche Konsequenzen sich für lokale Benutzerkonten auf Arbeitsstationen ergeben. Ein derartig konzentrierter Ansatz geht zwar über den Rahmen dieses Dokuments hinaus, doch können Sie ausführlichere Erläuterungen zur Vergabe von Benutzerkonten mit möglichst geringen Berechtigungen auf der Website von Microsoft finden. Weitere Informationen hierzu finden Sie im Whitepaper zur [Anwendung des Prinzips der geringsten Rechte für Benutzerkonten unter Windows XP](http://go.microsoft.com/fwlink/?linkid=58445) (möglicherweise in Englisch) unter http://go.microsoft.com/fwlink/?LinkId=58445 sowie im Artikel über die [Verwendung eines Benutzerkontos mit möglichst geringen Berechtigungen](http://www.microsoft.com/technet/security/secnews/articles/lpuseacc.mspx) (möglicherweise in Englisch) unter www.microsoft.com/technet/security/secnews/articles/lpuseacc.mspx.
  
##### Dienstkontenverwaltung
  
Wie bei der Verwaltung von Administratorkonten und kritischen Konten gibt es auch hier drei grundlegende Punkte, denen für die Entwicklung eines erfolgreichen Plans zur Verbesserung der Sicherheit von Diensten in einem mittelgroßen Unternehmen eine Schlüsselbedeutung zukommt. Es ist wichtig, dass die folgenden drei Punkte während der Entwicklungsphasen thematisiert und in Sicherheitsrichtlinienverfahren integriert werden.
  
-   Erfassen und Dokumentieren der Systemumgebung
  
-   Anwendung des Prinzips der geringsten Rechte
  
-   Anwendung des Prinzips der geringsten Dienstanzahl
  
###### Erfassen und Dokumentieren der Systemumgebung
  
Dieser empfohlene Schritt mag offensichtlich erscheinen, doch zahlreiche Unternehmen sind sich nicht sämtlicher Rollen und Dienste bewusst, die in ihrer Netzwerkumgebung vorhanden sind. Die Tatsache, dass die Rollen und Dienste nicht bekannt und dokumentiert sind, kann eine Reihe von Gründen haben. Meistens besteht der Grund jedoch im raschen Wachstum von Netzwerkumgebungen sowie einem Mangel von Zeit und Ressourcen, um sich in angemessener Weise der Notwendigkeit einer Dokumentierung zu widmen.
  
Um zu erkennen, ob die Sicherheit von Computern gewährleistet ist, muss bekannt sein, welche Dienste auf diesen Computern ausgeführt werden und welche Folgen sich aus den Eigenschaften dieser Dienste ergeben könnten. Diese Informationen sind überaus wichtig, um sowohl die Server und ihre jeweiligen Dienste zu sichern als auch die Konten, die diese Dienste erfordern könnten. Zu diesem Zweck ist es normalerweise hilfreich, eine Tabelle von Diensten, Diensteigenschaften und Computern zu erstellen, auf denen diese Dienste verwendet werden. Die Erstellung solch einer Liste mag eine gewisse Herausforderung darstellen, aber die Ergebnisse sind der Mühe wert. Nachdem die Tabelle erstellt wurde und einen Bestandteil des Prozesses zur Serverkonfiguration und Anwendungsbereitstellung darstellt, ist es zudem relativ einfach, sie auf aktuellem Stand zu halten.
  
Es sind einige Tools verfügbar, die die Dokumentierung der Dienste und Diensteigenschaften innerhalb eines Netzwerks erleichtern. Im Folgenden sind einige dieser Tools aufgelistet:
  
-   **Service Controller Tool (sc.exe)**: Dieses Befehlszeilenprogramm ist in Windows Server 2003 und Windows XP integriert. Dieses Tool bietet eine einfache Methode, um zum Abfragen und Einstellen von Diensteigenschaften über die Befehlszeile mit der Dienststeuerungs-Manager-Komponente zu kommunizieren.
  
-   **Service Controller List Tool (sclist.exe)**: Windows 2000 Server Resource Kit bietet ein Tool, das die auf lokalen oder Remotecomputern ausgeführten und angehaltenen Dienste auflistet. Mithilfe von Sclist.exe können Dienste identifiziert werden, die auf Remoteservern ausgeführt werden und nicht über Bildschirme verfügen bzw. vom Administrator räumlich getrennt sind.
  
-   **Windows-Verwaltungsinstrumentation (Windows Management Instrumentation, WMI)**: Diese Komponente ist in Windows Server 2003 und Windows XP integriert und stellt Verwaltungsinformationen und Verwaltungssteuerungsmechanismen in Unternehmensumgebungen bereit. WMI kann von Administratoren genutzt werden, um auf Computern, in Netzwerken, Anwendungen und Diensten Daten abzufragen und Einstellungen vorzunehmen. Neben der Möglichkeit, Skripts für die Bewältigung von Verwaltungsaufgaben zu verwenden, können Administratoren mithilfe von WMI Abhängigkeiten von Diensten sowie Dienste identifizieren, von denen diese Dienste ihrerseits abhängen.
  
-   **Windows-Verwaltungsinstrumentations-Befehlszeile (Windows Management Instrumentation Command Line, WMIC)**: WMI enthält auch ein Befehlszeilenprogramm namens WMIC. Dieses Tool bietet eine einfache WMI-Befehlszeilenschnittstelle für Abfragen und Remotecomputerverwaltung. Abfrageergebnisse von WMIC lassen sich als leicht lesbare HTML-Tabellen formatieren, die mit einem Browser wie Internet Explorer angezeigt werden können.
  
###### Anwendung des Prinzips der geringsten Rechte
  
Wir bei Microsoft verstehen, wie wichtig das Thema Sicherheit ist und welche Bedeutung dem Prinzip der geringsten Rechte bei der Sicherung von Netzwerkumgebungen zukommt. Bei Microsoft wurde das Prinzip der geringsten Rechte bei der Entwicklung von Windows Server 2003 angewendet, um sicherzustellen, dass die Dienste im Betriebssystemkern bereits das Konto mit den geringsten Rechten verwenden. Aus diesem Grund sollte keine weitere Konfiguration dieser Dienste erforderlich sein. Dieser Ansatz sollte sich schwerpunktmäßig darauf konzentrieren, Dienste zu sichern, die nicht zum Betriebssystem gehören. Dazu zählen die Dienste, die als Komponenten anderer Produkte bereitgestellt werden, beispielsweise Microsoft SQL Server, Microsoft Operations Manager oder andere Softwareprodukte von Drittanbietern.
  
Dementsprechend sollte das Prinzip der geringsten Rechte ebenfalls angewendet werden, wenn andere Dienste ausgeführt werden, selbst wenn es häufig leichter ist, bei Einführung neuer Produkte einfach höhere Berechtigungen zu gewähren. Dienste sollten z. B. überall, wo dies möglich ist, das lokale Dienstkonto verwenden, um einen Angriff in seinem Erfolg auf den lokalen Computer zu beschränken und nicht die gesamte Domäne in Mitleidenschaft zu ziehen. Dienste, die einen authentifizierten Netzwerkzugriff erfordern, sollten den Netzwerkdienst verwenden, wann immer dies möglich ist. Für Dienste, die breit angelegte Berechtigungen erfordern, sollte das lokale Dienstkonto verwendet werden. Wenn ein Dienst schließlich die Verwendung eines Administratorkontos auf Domänenebene erfordert, sollten die Server, auf denen dieser Dienst ausgeführt wird, als Hochsicherheitssysteme betrachtet werden, die auf dieselbe Weise geschützt werden wie andere vertrauliche bzw. kritische Netzwerkressourcen und Domänencontroller.
  
Gruppenrichtlinien können ebenfalls zur Steuerung bestimmter Dienste verwendet werden, die auf Computern ausgeführt werden dürfen. Zahlreiche Eigenschaften können unter **Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Systemdienste** gesteuert werden, indem dort die Seite **Eigenschaften** für den entsprechenden Dienst geöffnet wird. Einstellungen wie etwa der Startmodus und die Berechtigungen dafür, welche Konten verwendet werden dürfen, um bestimmte Vorgänge für diesen Dienst auszuführen (z. B. Starten oder Beenden), können geändert werden.
  
Die Implementierung des Prinzips der geringsten Rechte setzt eine genaue Kenntnisse der Systeme in der jeweiligen Umgebung voraus. Durch die Kombination dieser beiden zentralen Konzepte ist es möglich festzustellen, welche Dienste auf welchen Computern ausgeführt werden. Darüber hinaus ist der Status der Dienste zu erkennen sowie die Anmeldeinformationen, die für jeden Dienst bzw. für jeden Server verwendet werden. Nur dann ist es möglich, über Änderungssteuerungsprozesse methodisch und effektiv jeden einzelnen Dienst auf die Verwendung der geringsten Rechte zu beschränken, die für die weitere Funktionsfähigkeit erforderlich sind. Auf diese Weise wird zudem die Dokumentierung der Umgebung erleichtert.
  
###### Anwendung des Prinzips der geringsten Dienstanzahl
  
Abschließend ist noch das Prinzip der geringsten Dienstanzahl zu nennen. Es sagt aus, dass die für Netzwerkressourcen verfügbaren Betriebssystem- und Netzwerkprotokolle nur genau die Dienste und Protokolle ausführen sollten, die für das Funktionieren der Betriebsabläufe erforderlich sind. Wenn ein Server beispielsweise nicht als Host für Internetanwendungen benötigt wird, sollte der WWW-Dienst (World Wide Web) deaktiviert oder deinstalliert werden.
  
Bei der Standardinstallation der meisten Betriebssysteme und Programme werden weit mehr Dienste und Protokolle installiert, als tatsächlich für gängige Nutzungsszenarien erforderlich sind. Daher sollte, wann immer möglich, ein benutzerdefinierter Installationsvorgang gewählt werden, damit gesteuert werden kann, welche Dienste und Protokolle während eines Anwendungsprozesses aktiviert bzw. installiert werden. Auf diese Weise ist es möglich zu dokumentieren, welche Prozesse während der Installation erstellt werden. Dies ist nützlich für den Fall, dass zu einem späteren Zeitpunkt festgestellt wird, dass ein bei der Installation erstellter Dienst nicht mehr benötigt wird.
  
Bei der Bereitstellung von neuen Servern oder der Entwicklung von Serverimages gilt es als Best Practice, Schritte in das Verfahren aufzunehmen, bei denen der Systemadministrator alle bis auf die vom Betriebssystem benötigten Dienste herunterfährt. Die deaktivierten Dienste können zu einem späteren Zeitpunkt für jede Anwendung, die auf dem Server ausgeführt werden muss, erneut aktiviert werden. So war es z. B. vor Windows Server 2003 üblich, die Warn- und Nachrichtendienste von Windows-Betriebssystemen zu deaktivieren, da derartige Dienste im Allgemeinen nicht benötigt wurden. Durch das Deaktivieren dieser Dienste wurde das Sicherheitsprofil des bereitgestellten Servers erhöht, ohne dabei die Funktionalität zu beeinträchtigen.
  
Ein weiterer wichtiger Bestandteil dieses Prinzips ist auch der jeweilige Installationsort von Diensten. Der Routing- und RAS-Dienst oder der Internetinformationsdienst sollten beispielsweise nie auf Domänencontrollern installiert werden, da diese Hintergrunddienste die Sicherheitsanfälligkeit von Domänencontrollern erhöhen. Nach einer aufgetretenen Sicherheitsverletzung könnte ein Domänencontroller uneingeschränkten Zugriff auf die übrige Domäne gewähren. Auf der Grundlage der Best Practices von Microsoft empfiehlt es sich deshalb, nur die Dienste auf einem Domänencontroller bereitzustellen, die für dessen Betrieb absolut erforderlich sind.
  
#### Bereitstellung und Verwaltung
  
Nach der Darstellung der zentralen Überlegungen und grundlegenden Prinzipien kann nun eine Reihe von speziellen Empfehlungen betrachtet werden, die auf diesen Konzepten beruhen. Schon durch das Ergreifen einer einzigen dieser Maßnahmen lässt sich die Sicherheit eines Unternehmensnetzwerks erhöhen, doch in der Kombination können die Maßnahmen Teil eines umfassenden Sicherheitsframeworks werden, über das die Sicherheitsanfälligkeit des Netzwerks eines mittelgroßen Unternehmens erheblich reduziert werden kann.
  
##### Verwaltung von kritischen Konten und Administratorkonten
  
Es kann eine Reihe von auf Best Practices basierenden Ansätzen zur Sicherung von Administratorkonten in einem Microsoft Windows-Netzwerk umgesetzt werden. Mithilfe der folgenden Methoden lässt sich erwiesenermaßen die mit derartigen Konten verbundene Sicherheitsanfälligkeit reduzieren. Die Methoden werden häufig bei Netzwerken von mittelgroßen Unternehmen eingesetzt.
  
###### Trennen von Domänenadministrator- und Unternehmensadministratorrollen
  
Die Unternehmensadministratorrolle ist die höchste Rolle innerhalb einer Active Directory-Gesamtstruktur. Es müssen Schritte unternommen werden, um zu gewährleisten, dass dieser Kontotyp gesichert und seine Verwendung genauen Regelungen unterworfen wird. Es bestehen zwei Möglichkeiten zur Verwaltung dieses Kontotyps:
  
-   **Kontrolliertes Einzelkonto**: Die erste Methode besteht darin, diese Rolle auf ein einzelnes Konto zu beschränken, das streng überwacht und kontrolliert wird, um zu gewährleisten, dass das Konto nur verwendet wird, wenn autorisierte Anforderungen zur Änderungssteuerung für Aufgaben bestehen, die seine Verwendung erfordern würden. Jedes überwachte Ereignis, das im Namen dieses Kontos stattfindet, erfordert eine unmittelbare Nachforschung und muss in irgendeiner Form von autorisiertem Änderungsanforderungsereignis begleitet sein.
  
-   **Temporäres Konto**: Ein anderer Ansatz besteht darin, ein derartiges Konto erst dann zu erstellen, wenn es zur Ausführung einer autorisierten Aufgabe benötigt wird. In so einem autorisierten Fall kann dann ein temporäres Konto erstellt werden, das zur Ausführung der Aufgabe genutzt und anschließend wieder gelöscht wird. Da nur selten die Notwendigkeit für ein Konto mit derartig hohen Berechtigungen besteht, würden solche Schritte den Verwaltungsaufwand nur unwesentlich erhöhen.
  
###### Trennen von Benutzer- und Administratorkonten
  
Konten werden normalerweise Benutzern zugeordnet. Bei der Anwendung des Prinzips der geringsten Rechte können Konten nicht nur mit Rollen, sondern auch mit Aufgaben verknüpft werden, insbesondere dann, wenn es um Verwaltungsfunktionen geht. Für jede Person, die eine Administratorrolle erfüllt, sollten zwei Konten bestehen: eines für den täglichen Gebrauch – ein typisches Benutzerkonto – und ein weiteres mit Administratorrechten, das nur zur Ausführung von Verwaltungsaufgaben an der Arbeitsstation eines Administrators verwendet wird.
  
Administratorkonten sollten auf die Ausführung von Verwaltungsaufgaben und die Verwendung an Administratorarbeitsstationen eingeschränkt werden, die – ähnlich wie Domänencontroller – zu einem vertrauenswürdigen Netzwerk gehören. Administratorkonten und die damit verbundenen Arbeitsstationen sollten keinen Zugriff auf E-Mail oder das Internet haben. Zudem sollten diese Konten nur dann angemeldet sein, wenn sie auch genutzt werden. Administratoren sollten über unterschiedliche Kennwörter für ihre Standardbenutzer- und Administratorkonten verfügen. Administratorkennwörter sollten den höchstmöglichen Sicherheitsstandard innerhalb eines Netzwerks aufweisen.
  
Diese einfachen Vorsichtsmaßnahmen senken deutlich die Sicherheitsgefahren, die mit derartigen Konten verbunden sind, da sie weniger Angriffsfläche nach außen bieten und sie für kürze Zeiträume genutzt werden.
  
###### Verwenden des sekundären Anmeldedienstes
  
Programme können unter einem anderen als dem aktuell angemeldeten Konto ausgeführt werden, wenn Microsoft Windows 2000 Run als Dienst verwendet wird. Bei Windows Server 2003 und Windows XP Professional hat diese Funktionalität den neuen Namen „sekundärer Anmeldedienst“ erhalten.
  
Der sekundäre Anmeldedienst ermöglicht es Administratoren, sich mit einem Konto ohne Administratorrechte an einem Computer anzumelden und Verwaltungsaufgaben auszuführen. Dabei werden, vertrauenswürdige Verwaltungsaufgaben mit einer Administratoranmeldung ausgeführt, ohne dass zuvor eine Abmeldung erfolgen muss. Mithilfe dieser Funktionalität lassen sich die mit einer Administratoranmeldung verbundenen Risiken verringern, indem eine Form des weiter oben beschriebenen Konzepts der Trennung von Benutzer- und Administratorkonten eingesetzt wird.
  
###### Ausführen separater Terminaldienstsitzungen für die Administration
  
Terminaldienste und Remotedesktopverbindungen werden häufig zur Serververwaltung verwendet, ohne dass dabei ein physischer Zugriff auf die Serverkonsole erforderlich ist. Diese Methode ist nicht nur effizienter, sondern auch sicherer als die Verwendung eines Administratorkontos, um sich interaktiv am Server anzumelden. Dies gilt besonders dann, wenn an dem Computer, von dem aus die Verbindung hergestellt wurde, kein Konto auf Administratorebene verwendet wird. Wenn eine Verwaltungsaufgabe abgeschlossen ist, sollte eine Abmeldung des Administratorkontos erfolgen und die Verbindung der Sitzung beendet werden.
  
###### Umbenennen der standardmäßigen Administratorkonten
  
Das Umbenennen des standardmäßigen Administratorkontos bleibt in zahlreichen mittelgroßen Unternehmen eine häufig angewendete Methode und trägt bis zu einem gewissen Grad zu einer Verbesserung des Risikoprofils des betreffenden Kontos bei. Mit dieser Methode kann allerdings nur eine geringe Anzahl von Angriffsarten verhindert werden, da zahlreiche Tools und Techniken vorhanden sind, mit denen Angreifer feststellen können, bei welchem Konto es sich um das vordefinierte Administratorkonto handelt. Auch wenn es durchaus hilfreich sein kann, das Standardkonto umzubenennen, ist es tatsächlich effektiver, sekundäre Administratorkonten zu erstellen und anschließend die ursprünglichen vordefinierten Konten zu deaktivieren, so wie es später in diesem Dokument behandelt wird.
  
###### Erstellen von Köderadministratorkonten
  
Zusammen mit einem Eindringschutzmechanismus, der Warnmeldungen über bestimmte Kontoaktivitäten erkennen und senden kann, kann die Verwendung eines Köderadministratorkontos als zusätzliche Verteidigungsschicht gegen die auf ein Netzwerk ausgeführten Angriffsversuche dienen. Diese Technik allein kann schon einige Angreifer dadurch aufhalten, wenn diesem Konto mehr Kennworteingabeversuche gewährt werden, als dies normalerweise bei Konten der Fall ist, und sichere Kennwörter verwendet werden. Köderadministratorkonten sollten keine Mitglieder von mit Berechtigungen ausgestatteten Sicherheitsgruppen sein und sollten auf jegliche Aktivität überwacht werden. Jeder Versuch, ein derartiges Konto zu nutzen, sollte eine umgehende Untersuchung auslösen.
  
###### Erstellen von sekundären Administratorkonten und Deaktivieren von vordefinierten Konten
  
Auch wenn nicht jede Person, die über eine Administratorrolle verfügt, ein eigenes administratorähnliches Konto für die Ausführung von Verwaltungsaufgaben erhält – und selbst wenn die Terminaldienste nicht für die Serververwaltung genutzt werden –, gilt es dennoch als Best Practice, ein sekundäres Administratorkonto zu erstellen. Ein sekundäres Administratorkonto dient als Absicherung gegen eine Sicherheitsverletzung bei einem primären Administratorkonto und sollte erstellt werden, bevor das vordefinierte Administratorkonto deaktiviert wird.
  
**Hinweis:**    Es ist wichtig sicherzustellen, dass ein weiteres Konto mit den entsprechenden Administratorberechtigungen erstellt wurde, bevor das vordefinierte Administratorkonto deaktiviert wird. Wird das vordefinierte Administratorkonto deaktiviert, ohne dass ein weiteres entsprechendes Konto besteht, könnte dies zu Einbußen bei der Verwaltbarkeit der Domäne führen und eine Systemwiederherstellung bzw. eine Neuinstallation erforderlich machen, um das Problem zu beheben.
  
###### Aktivieren der Kontosperrung für Remoteadministratoranmeldungen
  
Auch wenn das vordefinierte Administratorkonto nicht gesperrt werden kann, so ist doch die Sperrung von Remoteanmeldungen möglich, die vom Administratorkonto ausgehen. Zu diesem Zweck bietet das Microsoft Windows 2000 Server Resource Kit ein Befehlszeilenprogramm namens Passprop.exe, über das die Kontosperrung für Remoteanmeldungen aktiviert werden kann. Wenn dieses Befehlszeilenprogramm mit der Option /ADMINLOCKOUT verwendet wird, gelten sowohl für die interaktive als auch für die Remoteanmeldung beim Administratorkonto die bestehenden Sperrrichtlinien von Windows 2000 Server.
  
**Hinweis:**    Das Verwenden von Passprop.exe /ADMINLOCKOUT unter Windows Server 2003 hat Auswirkungen auf die Remoteanmeldung und die interaktive Anmeldung beim Administratorkonto. Diese Funktion sollte mit Vorsicht eingesetzt werden, da es unmöglich ist, das Administratorkonto zur Serververwaltung einzusetzen, solange das Konto gesperrt ist.
  
###### Erstellen von sicheren Administratorkennwörtern
  
Eine weitere Best Practice-Methode besteht in der Verwendung eines sicheren Kennworts für Konten mit Administratorberechtigungen sowie für vordefinierte Administratorkonten. Sichere Kennwörter mindern die Wahrscheinlichkeit, dass ein Angreifer Brute-Force-Angriffe zur Erhöhung von Berechtigungen nutzt. Sichere Kennwörter weisen typischerweise die folgenden Merkmale auf:
  
-   Sie sind mindestens 15 Zeichen lang.
  
-   Sie enthalten niemals Kontonamen, echte Namen oder den Namen des Unternehmens in irgendeiner Form.
  
-   Sie enthalten niemals vollständige Wörter, umgangssprachliche Ausdrücke oder andere Begriffe, nach denen gesucht werden kann.
  
-   Sie unterscheiden sich wesentlich von vorher benutzten Kennwörtern und sind nicht inkrementell.
  
-   Sie weisen mindestens drei der folgenden Zeichenarten auf:
  
    -   Großbuchstaben (A, B, C...)
  
    -   Kleinbuchstaben (a, b, c...)
  
    -   Ziffern (0, 1, 2...)
  
    -   Nicht-alphanumerische Symbole (@, &, $...)
  
    -   Unicode-Zeichen (€, ƒ, ?...)
  
###### Automatisches Erkennen von unsicheren Kennwörtern
  
Es gibt zwei grundlegende Ansätze, die bei Tools zum Überprüfen von Kennwörtern eingesetzt werden, um nach unsicheren oder leeren Kennwörtern zu suchen. Hierbei handelt es sich um die folgenden Ansätze:
  
-   **Onlinescannen von Kennwörtern**: Beim Onlinescannen werden mehrere Versuche unternommen, sich mithilfe von verbreiteten Kennwortmängeln anzumelden. Ein Beispiel hierfür ist die Verwendung des Kennworts „Kennwort“ oder sogar eines leeren Kennworts. Das Tool Microsoft Baseline Security Analyzer (MBSA) funktioniert z. B. nach dieser Methode.
  
-   **Offlinescannen von Kennwörtern**: Das Offlinescannen beinhaltet eine Reihe von Mechanismen, bei denen zwischengespeicherte Anmeldeinformationen genutzt werden, um die Sicherheit von Kennwörtern für verschiedene Konten zu testen und sogar entsprechend einer Rangfolge zu ordnen. Tools, die nach dieser Methode funktionieren, weisen gegenüber der zuvor beschriebenen Methode einige Vorteile auf, erfordern jedoch Software von Drittanbietern.
  
Es sind zwar Tools von Drittanbietern erhältlich, mit denen nach unsicheren Kennwörtern gesucht werden kann, doch Microsoft Baseline Security Analyzer (MBSA) ist als kostenloser Download verfügbar. Mit MBSA werden alle deaktivierten oder gesperrten Konten angezeigt, die erkannt werden, während alle Benutzerkonten aufgelistet werden, um nach den folgenden Kennwortmängeln zu suchen.
  
-   Leere Kennwörter
  
-   Verwendung von Benutzernamen als Kennwort
  
-   Verwendung von Computernamen als Kennwort
  
-   Verwendung der Wörter „Kennwort“, „Admin“ oder „Administrator“ als Kennwort
  
Weitere Informationen hierzu finden Sie auf der Webseite [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa.mspx) unter www.microsoft.com/germany/technet/sicherheit/tools/mbsa.mspx.
  
###### Einschränken von Verwaltungsaufgaben auf vertrauenswürdige Computer
  
Administratoranmeldeinformationen stellen für Angreifer, die in das Netzwerk eindringen möchten, ein verlockendes Ziel dar. Die Methoden, über die sie versuchen, sich Zugriff auf diese Informationen zu verschaffen, können manchmal nur schwer erkannt werden. Um an diese vertraulichen Daten zu gelangen, werden typischerweise Tools eingesetzt, mit denen die Tastatureingaben aufgezeichnet oder die Bildschirminhalte eines Computers erfasst werden können, dessen Sicherheit bereits nicht mehr intakt ist. Malware in dieser Form kann sehr versteckt zum Einsatz kommen. Dadurch ist es außerordentlich schwierig, diese schädlichen Programme nach der Installation auf einem Computer aufzuspüren oder gar zu entfernen.
  
Deshalb gilt als Best Practice, dass administratorähnliche Konten in ihrer Verwendung auf so wenig Computer wie möglich beschränkt bleiben, damit die Sicherheitsanfälligkeit gegenüber derartigen Bedrohungen verringert wird. Bei Beschränkung der Ressourcen, auf denen Administratorkonten verwendet werden sollen, muss darüber hinaus sichergestellt werden, dass derartige Systeme vertrauenswürdig und gut geschützt sind. Es sind zahlreiche Techniken für den Schutz von sicherheitskritischen Ressourcen verfügbar, über die die Sicherheit bei bestimmten Geräten erhöht werden kann, ohne dabei die Verwendbarkeit des Netzwerks zu beeinträchtigen. Zu diesen Techniken gehört beispielsweise die Netzwerkisolation über IPSec.
  
Weitere Informationen zur Verwendung von IPSec zur Isolierung von Domänen und Servern finden Sie auf der Technology Center-Seite zur [Isolierung von Domänen und Servern](http://www.microsoft.com/technet/itsolutions/network/sdiso/default.mspx) (möglicherweise in Englisch) unter www.microsoft.com/technet/itsolutions/network/sdiso/default.mspx.
  
###### Überwachen von Konten und Kennwörtern
  
Die regelmäßige Überwachung von Konten trägt dazu bei, die Sicherheit der Domäne vor Angriffen zu gewährleisten, die mit der Erhöhung von Berechtigungen verbunden sind. Wenn es einem Angreifer gelingt, Zugriff auf ein Konto auf Administratorebene zu erhalten, kann er Schwachstellen erzeugen und Sicherheitsmaßnahmen umgehen. Angreifer, die Zugriff auf ein administratorähnliches Konto erlangen, können beispielsweise Proxybenutzerkonten erstellen, Kontomitgliedschaften ändern und sogar Ereignisprotokolle modifizieren, um ihre Spuren zu verwischen.
  
Alle administrativen Benutzer und Gruppen auf Domänenebene sowie sämtliche lokalen Administratorkonten und -gruppen auf sicherheitskritischen Servern sollten regelmäßig überwacht werden. Die Verwendung derartiger Administratoranmeldeinformationen muss überwacht werden, um zu gewährleisten, dass sie ausschließlich im Rahmen der internen Richtlinien und in Übereinstimmung mit festgelegten und gut dokumentierten internen Prozessen, z. B. Änderungssteuerungsverfahren, eingesetzt werden. Durch eine regelmäßige Überwachung von Konten wird sichergestellt, dass bei der Ausführung von Verwaltungsaufgaben adäquate Verfahrensweisen zur Anwendung kommen. Außerdem kann überprüft werden, ob die Richtlinien hinsichtlich der Kennwortsicherheit eingehalten werden.
  
Die Ereignisanzeige kann sich als nützliches Tool im Überwachungsprozess erweisen, wenn Maßnahmen ergriffen wurden, um die Manipulation von Ereignisprotokollen auszuschließen. Weitere Informationen zur Verwendung von Ereignisprotokollen zur Überwachung der Netzwerksicherheit sowie Informationen zur Sicherung von Ereignisprotokolldaten finden Sie im [*Planungshandbuch zur Überwachung der Sicherheit und Erkennung von Angriffen*](http://go.microsoft.com/fwlink/?linkid=41309) (möglicherweise in Englisch) unter http://go.microsoft.com/fwlink/?LinkId=41309.
  
###### Untersagen der Kontoübertragung
  
Delegierte Authentifizierung findet statt, wenn ein Netzwerkdienst die Anforderung eines Benutzers akzeptiert und die Identität dieses Benutzers annimmt, um eine neue Verbindung zu einem anderen Netzwerkdienst zu initiieren. Delegierte Authentifizierung ist sinnvoll für mehrstufige Anwendungen, die im Netzwerk Funktionalität für einmaliges Anmelden (SSO) verwenden. Bei Microsoft Outlook Web Access (OWA) wird dieser Mechanismus genutzt, um eine Schnittstelle zu Datenbanken auf anderen Computern bereitzustellen.
  
Administratorkonten sollten als „Konto kann nicht delegiert werden“ gekennzeichnet sein. Mithilfe dieser Methode können administratorähnliche Berechtigungen vor einer Identitätsübertragung durch Server geschützt werden, die als „Für Delegierungszwecke vertraut“ gekennzeichnet sind. Computerkonten in Active Directory, die Computern ohne physische Absicherung zugeordnet sind, sollte die Möglichkeit zur delegierten Authentifizierung nicht gewährt werden. Für Domänenadministratorkonten sollte die delegierte Authentifizierung ebenfalls ausgeschlossen werden, da über sie der Zugriff auf sicherheitskritische Informationen und Ressourcen im Netzwerk ermöglicht wird.
  
Weitere Informationen zur Kontoübertragung finden Sie im Artikel zum Thema [Aktivieren delegierter Authentifizierung](http://technet2.microsoft.com/windowsserver/germany/library/72612d01-622c-46b7-ab4a-69955d0687c81033.mspx?mfr=true) (möglicherweise in Englisch) unter http://technet2.microsoft.com/WindowsServer/germany/Library/72612d01-622c-46b7-ab4a-69955d0687c81033.mspx?mfr=true.
  
###### Erzwingen einer Mehrfaktor-Authentifizierung für Administratorkonten
  
Die Gruppen „Administratoren“, „Organisations-Admins“ und „Domänen-Admins“ enthalten die Konten mit den höchsten Berechtigungen in einem Unternehmensnetzwerk. Folglich sollten diese Konten auch am besten geschützt sein.
  
Mehrfaktor-Authentifizierungsmethoden tragen zur Sicherheit des Anmeldevorgangs bei, indem autorisierte Benutzer zu ihrer Identifikation zusätzliche Angaben machen müssen. Dadurch wird der Umfang von Informationen erhöht, die ein Angreifer erlangen müsste, um Zugriff auf ein Konto zu erhalten. Wie der Name schon sagt, werden bei einer Mehrfaktor-Authentifizierungsmethode mehrere zur Identifikation dienende Informationen benötigt. Diese Methode könnte typischerweise die folgenden Elemente erfordern:
  
-   Ein Gegenstand im Besitz des Benutzers, etwa eine Smartcard.
  
-   Eine Angabe, die dem Benutzer bekannt ist, etwa eine PIN-Nummer.
  
-   Ein Merkmal des Benutzers (normalerweise als biometrische Daten bezeichnet). Die Authentifizierung kann über etwas so einfaches wie einen Fingerabdruckscanner erfolgen.
  
Durch die Verwendung der Mehrfaktor-Authentifizierung werden die Sicherheitsanfälligkeiten vermieden, die mit Authentifizierungsmethoden verbunden sind, die auf Benutzernamen in Klartext und Kennwörtern basieren. Der Kontoinhaber kann hier durch einen auf Zufallsbasis erzeugten Code identifiziert werden, der auf einer Smartcard gespeichert ist. Jede Smartcard enthält einen eindeutigen privaten Schlüssel, durch den sichergestellt wird, dass die Authentifizierungsdaten nicht mehrmals vorhanden sind.
  
Eine Smartcard erfordert zusätzlich eine PIN-Nummer, bei der es sich um einen weiteren verschlüsselten Code handelt, den der Karteninhaber festlegt und auf der Karte speichert. Über diese PIN-Nummer wird die Benutzung des in der Smartcard enthaltenen privaten Schlüssels bei der Authentifizierung ermöglicht. Zu allen anderen Zeiten bleibt der Schlüssel verschlüsselt und kann nicht genutzt werden.
  
Weitere Informationen zu Mehrfaktor-Authentifizierungsmethoden sowie zu Smartcards finden Sie Artikel [*Planungshandbuch für sicheren Zugriff unter Verwendung von Smartcards*](http://go.microsoft.com/fwlink/?linkid=41313) unter http://go.microsoft.com/fwlink/?LinkID=41313.
  
#### Verwaltung von Dienst- und Anwendungskonten
  
Es stehen zudem verschiedene, auf Best Practices basierende Methoden zur Verfügung, mit denen die Sicherheit von Diensten und Dienstkonten erhöht werden kann. In diesem Abschnitt werden die Methoden dargestellt, über die sich die Sicherheit in realen Netzwerkumgebungen erwiesenermaßen steigern lässt. Auch wenn der kombinierte Einsatz all dieser Methoden die Sicherheit von Netzwerken mittelgroßer Unternehmen beträchtlich erhöhen kann, ist es am besten, jede einzelne Methode zu betrachten, um für jede individuelle Unternehmensumgebung die beste Kombination der Methoden zu bestimmen.
  
##### Überwachen von Diensten auf wichtige Eigenschaften
  
Wie bereits erwähnt, besteht der erste Schritt bei der Entwicklung eines Plans zur Sicherung von Diensten in einer Umgebung darin, diese Dienste zu kennen und zu erfassen, wo sie zur Anwendung kommen und warum sie ausgeführt werden. Dies klingt zwar nach einer relativ einfachen Aufgabe, doch es kann sich als überraschend schwierig erweisen, herauszufinden, welche Dienste auf den jeweiligen Computern ausgeführt werden und welches Ausmaß an Verwaltung diese Dienste erfordern.
  
Jeder Server in einer Umgebung sollte dokumentiert und überwacht werden, um sämtliche Dienste zu identifizieren, die auf dem Server ausgeführt werden, und zu ermitteln, welche Anmeldeinformationen von jedem Dienst zur Authentifizierung verwendet werden. Um Administratoren bei dieser Aufgabe zu unterstützen, stehen eine Reihe von Tools zur Verfügung. Im Folgenden sind einige Beispiele aufgelistet:
  
-   **Systeminformationen in Microsoft Windows Server 2003**: Die Systeminformationen bieten eine umfassende Liste von Einstellungen für sämtliche Dienste, die auf einem lokalen Computer ausgeführt werden. Allerdings ist dieses Tool nicht besonders effektiv, um eine große Anzahl von Servern zu überwachen.
  
-   **Diensteverwaltungskonsole**: In der Diensteverwaltungskonsole kann anhand der Registerkarte **Anmelden** auf der Seite **Eigenschaften** eines Dienstes festgestellt werden, welches Konto von einem Dienst zur Authentifizierung verwendet wird. Es kann auch mithilfe der Registerkarte **Abhängigkeiten** ermittelt werden, von welchen anderen Diensten der betreffende Dienst abhängt und welche Dienste wiederum von dem angezeigten Dienst abhängen. Leider ist auch diese Methode nicht besonders zur Überwachung einer großen Anzahl von Servern geeignet.
  
-   **Windows-Verwaltungsinstrumentation (Windows Management Instrumentation, WMI)**: Über WMI können Informationen über die Dienste abgerufen werden, die auf sämtlichen Servern in einem Netzwerk ausgeführt werden. Wenn WMI zusammen mit Skripts und anderen Programmiertools verwendet wird, ist es über WMI möglich, in weiten Bereichen die Konfigurationsdetails der Netzwerkcomputer zu ermitteln sowie Änderungen an diesen vorzunehmen.
  
-   **Windows-Verwaltungsinstrumentations-Befehlszeile (Windows Management Instrumentation Command Line, WMIC)**: WMIC bietet dieselbe Funktionalität wie WMI in Form eines Befehlszeilenprogramms, das mit bestehenden Shells und anderen Dienstprogrammbefehlen zusammenarbeiten kann, die durch Skripts und anderen Anwendungen erweitert werden können.
  
    Über den WMIC-Dienst kann eine Reihe von Informationen über die in einem Netzwerk ausgeführten Dienste ermittelt werden. Im Folgenden finden sich einige Beispiele dafür:
  
    -   Beschreibung
  
    -   DisplayName
  
    -   ErrorControl
  
    -   InstallDate
  
    -   PathName
  
    -   ProcessID
  
    -   StartMode
  
    -   StartName
  
    -   Status
  
    -   Skripts
  
        Wie bereits erwähnt, kann WMIC genutzt werden, um die Verwaltung von Remotecomputern und lokalen Rechnern mithilfe von Skripts zu automatisieren.
  
-   **Weitere Unternehmensverwaltungstools**: Es sind einige weitere Verwaltungstools erhältlich, die für die Überwachung von Serverdiensten eingesetzt werden können. Im Folgenden sind einige Beispiele aufgeführt:
  
    -   Microsoft Systems Management Server (SMS)
  
    -   IBM Tivoli
  
    -   HP OpenView
  
    -   Lieberman Software Service Account Manager
  
##### Feststellen, welche Dienste notwendig sind
  
Bei der Erstinstallation von Windows Server 2003 werden einige standardmäßige Dienste erstellt und für die Ausführung beim Systemstart konfiguriert. Diese standardmäßigen Dienste sorgen für Anwendungskompatibilität und Clientkompatibilität oder vereinfachen die Systemverwaltung. Allerdings ist es nicht in jeder Umgebung erforderlich, dass all diese Dienste eingesetzt werden müssen. Sämtliche Dienste sollten dahingehend übergeprüft werden, ob einige davon deaktiviert werden können, wodurch sich die Sicherheitsanfälligkeit der Server verringern lässt, auf denen die Dienste ausgeführt werden.
  
Es kann sehr kompliziert sein zu bestimmen, welche Dienste benötigt werden und welche deaktiviert werden können. Bei manchen Diensten ist die Antwort offensichtlich, doch bei anderen sind die Optionen keineswegs so klar definiert. Welche Dienste deaktiviert werden können, kann dabei anhand von zwei Hauptkriterien bestimmt werden:
  
-   Wenn kein Grund zur Verwendung eines bestimmten Dienstes vorliegt, kann er deaktiviert werden.
  
-   Wenn zum gegenwärtigen Zeitpunkt keine Notwendigkeit zur Verwendung eines Dienstes besteht, dies aber in der Zukunft der Fall sein könnte, kann der betreffende Dienst bis zum Bedarfsfall deaktiviert werden.
  
Die Dienste, die auf einem bestimmten Server benötigt werden, hängen in erster Linie von der Rolle dieses Servers ab. So sollte IIS (Internet Information Services, Internetinformationsdienste) nur auf einem Webserver oder einem Anwendungsserver ausgeführt werden, für den ein webbasierter Verteilungsmechanismus genutzt wird. Wenn auf diesem Server keine Telnet- oder Remotezugriffsdienste eingesetzt werden, sollten diese auf dem betreffenden Server deaktiviert werden.
  
Dienste können auch Bestandteil von Software sein, die auf einem Server installiert ist. So wird bei Microsoft Systems Management Services der Dienst Wuser32 Remote Control Agent installiert, um die Remoteclientfunktionalität für Softwareupdates oder die Remoteverwaltung bereitzustellen. Um bestimmen zu können, welche Dienste deaktiviert werden sollten, muss bekannt sein, welche Dienste bei einem Softwarepaket möglicherweise installiert werden bzw. welche Dienste für die Funktionsfähigkeit der Software erforderlich sind.
  
##### Verwenden des Sicherheitskonfigurations-Assistenten
  
Der Sicherheitskonfigurations-Assistent (Security Configuration Wizard, SCW) ist ein Bestandteil von Windows Server 2003 Service Pack 1 (SP1) und kann verwendet werden, um eine schnelle Konfiguration von Servern vorzunehmen, die auf funktionellen Anforderungen beruhen, z. B. Webserver oder Domänencontroller. Administratoren können gleichzeitig Sicherheitsrichtlinien festlegen, um Sicherheitsanfälligkeiten zu minimieren. Über den Sicherheitskonfigurations-Assistenten kann ermittelt werden, welche Dienste auf den Servern innerhalb eines Netzwerks ausgeführt werden und welche Abhängigkeiten bei diesen Diensten besteht.
  
**So installieren Sie den Sicherheitskonfigurations-Assistenten auf einem Server mit Windows Server 2003**
  
1.  Öffnen Sie die Systemsteuerung.
  
2.  Doppelklicken Sie auf **Software**.
  
3.  Klicken Sie auf **Windows-Komponenten hinzufügen/entfernen**.
  
4.  Aktivieren Sie auf der Anzeige für **Windows-Komponenten** unter **Komponenten** das Kontrollkästchen **Sicherheitskonfigurations-Assistent**.
  
5.  Klicken Sie auf **Weiter**.
  
6.  Klicken Sie auf **Beenden**, wenn der Installationsvorgang abgeschlossen ist.
  
Mithilfe des Sicherheitskonfigurations-Assistenten lässt sich die Angriffsfläche von Computern unter Windows Server 2003 mit SP1 verringern. Administratoren werden von dem Assistenten durch den Prozess zur Erstellung von Sicherheitsrichtlinien geführt, die auf den Rollen basieren, die jeweils von einem bestimmten Server ausgeführt werden. Der Begriff *Serverrolle* definiert die Hauptfunktion, die ein Computer innerhalb eines Netzwerks einnimmt. Die benötigten Dienste, eingehenden Ports und Einstellungen variieren in Abhängigkeit von der Rolle, die ein Server einnimmt. Nach der Erstellung von Richtlinien können diese entsprechend der Konfiguration auf Server angewendet werden.
  
##### Eliminieren der Verwendung von Domänenadministratorkonten für Dienste
  
Nach Abschluss einer Serverüberprüfung sollten genug Informationen zur Umgebung vorliegen, um alle infrage kommenden Domänenadministratorkonten zu identifizieren und zu entfernen, die zur Authentifizierung von Diensten verwendet werden. Die erneute Bereitstellung von Diensten sollte möglichst immer unter Verwendung der Konten „Lokaler Dienst“, „Netzwerkdienst“ oder „Lokales System“ erfolgen.
  
Der Versuch, korrigierend in die Verwendung von administratorähnlichen Konten durch Dienste einzugreifen, sollte vor allem in den folgenden Fällen unternommen werden:
  
-   Bei Benutzerkonten mit administratorähnlichen Berechtigungen, bei denen die Anmeldung als Dienst erfolgt.
  
-   Bei vordefinierten Administratorkonten, bei denen die Anmeldung als Dienst erfolgt.
  
-   Bei Domänenadministratorkonten, bei denen die Anmeldung als Dienst auf einen Computer mit niedrigem Sicherheitsniveau erfolgt.
  
##### Verwenden von Hierarchien der geringsten Rechte zur Bereitstellung von Diensten
  
Wie bereits in diesem Dokument erläutert wurde, sollte für Dienste stets ein Konto mit Berechtigungen verwendet werden, die zur Ausführung des betreffenden Dienstes gerade ausreichend sind. Jegliche Dienste, die über höhere Berechtigungen verfügen, als es zur Ausführung erforderlich wäre, sollten unter Verwendung von Konten mit geringeren Berechtigungen erneut bereitgestellt werden.
  
In einer Hierarchie der geringsten Rechte wären die von Diensten verwendeten Konten wie folgt geordnet. Die Rangordnung verläuft dabei von der besten zur schlechtesten Variante:
  
-   Lokaler Dienst
  
-   Netzwerkdienst
  
-   Einzelnes lokales Benutzerkonto
  
-   Einzelnes Domänenbenutzerkonto
  
-   Lokales System
  
-   Lokales Administratorkonto
  
-   Domänenadministratorkonto
  
##### Erstellen von Hochsicherheits-Servergruppen für Ausnahmefälle
  
Bei Hochsicherheitsservern handelt es sich – einfach ausgedrückt – um Server, auf denen Ressourcen oder Dienste bereitgestellt werden, auf die das Unternehmen angewiesen ist oder mit denen ein erhöhtes Sicherheitsrisiko verbunden ist. Folgende Server erfüllen im Allgemeinen diese Kriterien:
  
-   Domänencontroller
  
-   Server, auf denen Dienste verwendet werden, für deren Ausführung eine Authentifizierung über ein Domänenadministratorkonto erfolgen muss
  
-   Server, die in einer Gesamtstruktur als vertrauenswürdig für Delegierungszwecke angesehen werden
  
-   Server, die von sicherheitskritischen Unternehmensgruppen verwendet werden oder auf denen kritische Unternehmensdaten gespeichert sind, etwa ein Server der Personalabteilung, auf dem Angaben zu Gehältern gespeichert sind.
  
-   Server, auf denen Dienste ausgeführt werden, die innerhalb einer Gesamtstruktur als „Für Delegierungszwecke vertraut“ eingestuft wurden und auf denen eine eingeschränkte Delegierung unter Windows Server 2003 verwendet wird.
  
Die Erstellung einer Hochsicherheits-Servergruppe beinhaltet im Allgemeinen die folgenden Aktivitäten:
  
1.  Es werden Server identifiziert, die als Hochsicherheitsserver gekennzeichnet werden sollten.
  
2.  In jeder Gesamtstruktur wird eine universelle Sicherheitsgruppe für die Hochsicherheitsserver erstellt.
  
3.  Die Computerkonten der ausgewählten Server werden in die neuen universellen Gruppen aufgenommen.
  
4.  In jeder Domäne wird eine lokale Gruppe für Domänenadministratorkonten erstellt.
  
5.  Die domänenadministratorähnlichen Benutzerkonten werden der neuen lokalen Gruppe zugewiesen.
  
6.  In jeder Domäne wird ein Gruppenrichtlinienobjekt erstellt, das die Verwendung von Administratorkonten auf Domänenebene für Dienste auf sämtlichen Computern beschränkt, indem die Benutzerrechte **Anmelden als Dienst verweigern** und **Anmelden als Batchauftrag verweigern** zugewiesen werden. Darüber hinaus werden die Berechtigungen **Lesezugriff zulassen** und **Anwenden zulassen** auf das Gruppenrichtlinienobjekt in der zuvor erstellten lokalen Gruppe für Domänenadministratorkonten angewendet.
  
7.  Auf jedes Gruppenrichtlinienobjekt werden Gruppenrichtlinienfilter für die Hochsicherheits-Servergruppe angewendet, so dass die Mitglieder dieser Gruppe auch weiterhin Domänenadministratorkonten für Dienste verwenden können. Diese Funktionalität wird über die Zuweisung der Berechtigungen **Lesezugriff zulassen** und **Anwenden verweigern** zum Gruppenrichtlinienobjekt für die betreffende Hochsicherheits-Servergruppe erreicht.
  
Die Verwaltung der Mitgliedschaft in der Hochsicherheits-Servergruppe sollte über einen internen Workflowprozess erfolgen, über den Anträge zur Aufnahme neuer Server bewertet werden. Dieser Prozess sollte Schritte zur Prüfung der Anträge sowie zur Einschätzung der Sicherheitsrisiken für den Fall beinhalten, dass ein Server in die Gruppe aufgenommen wird. Dieser Prozess kann dabei entweder auf einer ganz einfachen Grundlage beruhen, etwa auf E-Mail-Anforderungen an ein bestimmtes Konto, oder auf einem detaillierten automatisierten Prozess aufgebaut sein, für den mehrere Provisioningtools, z. B. Zero Touch Provisioning (ZTP), verwendet werden.
  
ZTP geht über den Rahmen dieses Dokuments hinaus, da es sich hierbei um ein Tool handelt, das auf die Erfordernisse der Umgebungen von Großunternehmen abgestimmt ist. Weitere Informationen zu ZTP und anderen vergleichbaren Tools finden Sie auf der Microsoft-Website [Desktop Deployment Center](http://www.microsoft.com/technet/desktopdeployment/default.mspx) (möglicherweise in Englisch) unter www.microsoft.com/technet/desktopdeployment/default.mspx.
  
##### Verwalten der Kennwortänderungen bei Dienstkonten
  
Wenn Konten einem Dienst zugeordnet sind, benötigt der Dienststeuerungs-Manager (Service Control Manager, SCM) das richtige Kennwort für das betreffende Konto, bevor die Zuweisung erfolgen kann. Bei Eingabe eines falschen Kennworts wird die Zuweisung vom Dienststeuerungs-Manager verweigert. Wenn Dienste so konfiguriert werden, dass sie lokale Systemkonten, lokalen Dienstkonten oder Netzwerkdienstkonten verwenden, besteht keine Notwendigkeit, Kennwörter für Konten zu verwalten, da die Kennwortverwaltung in diesem Fall über das Betriebssystem erfolgt.
  
Für andere Dienstkonten werden die Kennwörter vom Dienststeuerungs-Manager in der Datenbank für Dienste gespeichert. Nach der Zuweisung eines Kennworts überprüft der Dienststeuerungs-Manager die in dieser Datenbank gespeicherten Kennwörter nicht. Das Kennwort, das einem Benutzerkonto in Active Directory zugewiesen wurde, wird weiterhin akzeptiert. Dies kann in einer Situation wie der Folgenden zu Problemen führen:
  
1.  Ein Dienst ist so konfiguriert, dass er ein bestimmtes Benutzerkonto verwendet.
  
2.  Der Dienst wird durch die Verwendung des betreffenden Kontos mit dem aktuellen Kennwort gestartet.
  
3.  Das Kennwort für das betreffende Benutzerkonto wird geändert, während der Dienst weiterhin ausgeführt wird.
  
4.  Der Dienst wird solange weiter ausgeführt, bis er angehalten wird. Nachdem der Dienst angehalten wurde, ist es nicht möglich, den Dienst erneut zu starten, da der Dienststeuerungs-Manager weiterhin versucht, das alte Kennwort zu verwenden. In Active Directory geänderte Kennwörter werden nicht mit den Kennwörtern synchronisiert, die in der Datenbank für Dienste gespeichert sind.
  
Jeder Dienst, für den ein Standarddomänenkonto oder ein lokales Standardbenutzerkonto verwendet wird, muss jedes Mal mit neuen Authentifizierungsdaten aktualisiert werden, wenn das Kennwort für ein Benutzerkonto geändert wird. Dies kann sehr mühevoll und zeitraubend sein, wenn Dienste und die von ihnen verwendeten Konten nicht angemessen dokumentiert sind.
  
Natürlich stellt es ein ganz eigenes Sicherheitsrisiko dar, wenn in einem Dokument die Kontodaten für sämtliche Dienste gespeichert sind, die auf allen Servern ausgeführt werden. Deshalb sollten Maßnahmen zum Schutz eines solchen Dokuments ergriffen werden. Bei größeren Unternehmen kann die Aufzeichnung derartiger Informationen in einer verschlüsselten Datei erfolgen, die offline an einem sicheren Ort gespeichert wird. Kleinere Unternehmen könnten solche Daten möglicherweise einfach in einem Hefter notieren und diesen in einem Tresor oder an einem anderen gesicherten Ort aufbewahren.
  
Bei einigen Anwendungen werden möglicherweise auch Kennwörter für Dienstkonten verwendet, etwa bei Exchange Server oder SQL Server™. Deshalb sollte darauf geachtet werden, dass die relevanten Kennwörter in diesen Fällen an der Anwendungsschnittstelle geändert werden.
  
Informationen zum Erstellen von Tools zur Automatisierung des Prozesses zur Änderung von Kennwörtern für Dienstkonten finden Sie im Artikel über das [Ändern von Kennwörtern für das Benutzerkonto eines Dienstes](http://msdn.microsoft.com/library/default.asp?url=/library/en-us/ad/ad/changing_the_password_on_a_serviceampaposs_user_account.asp) (möglicherweise in Englisch) unter http://msdn.microsoft.com/library/default.asp?url=/library/en-us/ad/ad/changing\_the\_password\_on\_a\_serviceampaposs\_user\_account.asp.
  
##### Durchsetzen der Verwendung von sicheren Kennwörtern
  
Wie im entsprechenden Abschnitt über Administratorkonten bereits erwähnt wurde, sollte es strikt durchgesetzt werden, dass für administratorähnliche Konten sowie für sämtliche Dienstkonten Richtlinien für sichere Kennwörter befolgt werden. Zur Durchsetzung solcher Regeln können Gruppenrichtlinien genutzt werden, um ein Ablaufdatum für Kennwörter, eine Mindestlängenbeschränkung sowie andere Regeln für sichere Kennwörter durchzusetzen.
  
Weitere Informationen zu Richtlinien für sichere Kennwörter finden Sie im Whitepaper über [Kontenkennwörter und Richtlinien](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/technologies/security/bpactlck.mspx) (möglicherweise in Englisch) unter http://www.microsoft.com/technet/prodtechnol/windowsserver2003/technologies/security/bpactlck.mspx 
  
Weitere Informationen zur Durchsetzung der Verwendung von sicheren Kennwörtern finden Sie im [*Windows Server 2003-Sicherheitshandbuch*](http://go.microsoft.com/fwlink/?linkid=14845) unter http://go.microsoft.com/fwlink/?linkid=14845.
  
Unsichere Kennwörter stellen eine der häufigsten Sicherheitsschwachstellen in einem Netzwerk dar. Ihre Verwendung bei administratorähnlichen Konten macht es einem Angreifer leicht, Zugriff auf Netzwerkressourcen zu erhalten. Automatisierte Testtools zur Identifizierung von administratorähnlichen Konten mit unsicheren Kennwörtern sollten regelmäßig von den Personen eingesetzt werden, die für die Sicherheit oder Verwaltung eines Netzwerks verantwortlich sind.
  
Um dies zu erreichen, kann das Tool Microsoft Baseline Security Analyzer (MBSA) jeden Computer innerhalb des Netzwerks scannen und nach unsicheren Kennwörtern suchen. Mithilfe von MBSA können sämtliche Benutzerkonten aufgelistet und auf die folgenden Kennwortmängel hin überprüft werden:
  
-   Leere Kennwörter
  
-   Kennwörter, die mit dem Namen eines Benutzerkontos übereinstimmen
  
-   Kennwörter, die mit einem Computernamen übereinstimmen
  
-   Kennwörter, in denen die Wörter „Kennwort“, „Admin“ oder „Administrator“ enthalten sind
  
Beim Einsatz von MBSA wird auf der Grundlage der aufgelisteten Mängel ein neues Kennwort vorgeschlagen. Wenn ein unsicheres Kennwort gefunden wird, wird es nicht einfach geändert, sondern MBSA meldet, dass dieses Kennwort ein Sicherheitsrisiko darstellt. Mit MBSA werden zudem deaktivierte oder gesperrte Konten gemeldet.
  
Über MBSA lassen sich zwar die gängigsten Praktiken hinsichtlich mangelhafter Kennwortwahl identifizieren, doch verfügt das Tool nicht über umfassende Funktionen zur Kennwortüberwachung. Für diese Zwecke sind verschiedene Tools von Drittanbietern für das Offlinescannen von Kennwörtern verfügbar.
  
Unter www.microsoft.com/technet/security/tools/mbsahome.mspx können Sie auf der Webseite [Microsoft Baseline Security Analyzer](http://www.microsoft.com/technet/security/tools/mbsahome.mspx) mehr über MBSA erfahren oder das Tool herunterladen (möglicherweise in Englisch).
  
**Hinweis:**    Bei MBSA werden auf einem Computer festgestellte Kontensperrrichtlinien zurückgesetzt, um zu verhindern, dass Konten während des Scannens gesperrt werden. Außerdem werden mit MBSA keine Kennwörter auf Computern gescannt, die als Domänencontroller gekennzeichnet sind.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
Selbstverständlich kann eine ganze Reihe von Maßnahmen ergriffen werden, um die Sicherheit von kritischen Konten und Dienstkonten in Netzwerken mittelgroßer Unternehmen zu erhöhen. Im Grunde beruht jeder dieser Ansätze auf einigen wenigen Schlüsselkonzepten, etwa auf der Einrichtung gut dokumentierter Prozesse oder auf der Orientierung am Prinzip der geringsten Rechte. Es reicht bereits aus, diese wenigen Schlüsselkonzepte zu verstehen und als Grundlage für die Kontoverwaltung anzuwenden, um die Sicherheit eines Netzwerks beträchtlich zu erhöhen.
  
In der Umgebung eines mittelgroßen Unternehmens kann eine beliebige Anzahl der auf Best Practices basierenden Methoden, die in diesem Dokument beschrieben werden, eingesetzt werden, sofern sie als für die Unternehmensanforderungen geeignet eingestuft werden. Auch wenn sich mit einer Kombination aus allen beschriebenen Methoden zweifellos die Sicherheit eines jeden Netzwerks erhöhen ließe, ist es empfehlenswert, zunächst die potenziellen Auswirkungen zu analysieren, die jede dieser Methoden auf ein Unternehmensnetzwerk haben könnte. Auf diese Weise lässt sich die für das jeweilige Netzwerk geeignete Kombination von Verfahrensweisen ermitteln.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Anhang A: Gängige Dienste
  
In der folgenden Tabelle werden die gängigen Dienste unter Windows Server 2003 und Windows XP in alphabetischer Reihenfolge aufgeführt und beschrieben. Auch wenn diese Liste sowohl Standarddienste als auch Dienste beinhaltet, die auf einem Computer hinzugefügt werden können, handelt es sich nicht um eine vollständige Liste aller möglichen Dienste, die auf einem Computer installiert werden können, da keine Dienste enthalten sind, die als Bestandteil von Softwarepaketen von Drittanbietern installiert werden könnten.
  
**Tabelle A.1 Beschreibung von Diensten unter Windows XP und Windows Server 2003**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Dienst</p></th>
<th><p>Dienstname</p></th>
<th><p>Anmelden als</p></th>
<th><p>Beschreibung</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>IP6-zu-IP4</p></td>
<td style="border:1px solid black;"><p>IPv6-Hilfsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht IPv6-Konnektivität über IPv4-Netzwerke</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>AELookupSvc</p></td>
<td style="border:1px solid black;"><p>Anwendungskompatibilitäts-Suchdienst</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Verarbeitet Suchanfragen zur Anwendungskompatibilität für Anwendungen, wenn diese gestartet werden. Muss für Anwendungskompatibilitäts-Softwareupdates aktiviert sein.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Alerter</p></td>
<td style="border:1px solid black;"><p>Warndienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Dieser Dienst benachrichtigt ausgewählte Benutzer und Computer über administrative Warnungen und ist für die Zustellung vom Nachrichtendienst auf Clientcomputern abhängig.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ALG</p></td>
<td style="border:1px solid black;"><p>Gatewaydienst auf Anwendungsebene</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Unterstützt im Hintergrund von ICS arbeitende Plug-Ins, über die Netzwerkprotokolle die Firewall passieren können.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>AppMgmt</p></td>
<td style="border:1px solid black;"><p>Anwendungsverwaltung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Softwareinstallationsdienste wie Zuweisung, Veröffentlichung und Deinstallation. Im Falle der Deaktivierung ist es nicht möglich, Anwendungen über Active Directory-Dienste wie IntelliMirror® zu installieren.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>AppMgr</p></td>
<td style="border:1px solid black;"><p>Remoteserver-Manager</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Funktioniert als WMI-Instanzenanbieter für Warnobjekte bei der Remoteverwaltung und als WMI-Methodenanbieter für Remoteverwaltungsaufgaben.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>aspnet_state</p></td>
<td style="border:1px solid black;"><p>ASP.NET-Statusdienst</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Stellt die Unterstützung für Out-of-Process-Sitzungszustände von ASP.NET bereit.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>AudioSrv</p></td>
<td style="border:1px solid black;"><p>Windows-Audio</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet Audiogeräte für Windows-basierte Programme.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>BINLSVC</p></td>
<td style="border:1px solid black;"><p>Remoteinstallation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Dies ist die Hauptkomponente des Remoteinstallationsservers (Remote Installation Server, RIS) zur Beantwortung von PXE-Anfragen für remotestartfähige Computer.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>BITS</p></td>
<td style="border:1px solid black;"><p>Intelligenter Hintergrundübertragungsdienst</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Stellt einen Mechanismus für im Hintergrund ablaufende Dateiübertragungen für Warteschlangen-Manager bereit. Wenn dieser Dienst angehalten wird, können auf dem Computer keine automatischen Updatefunktionen verwendet werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Browser</p></td>
<td style="border:1px solid black;"><p>Computerbrowser</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Führt eine aktuelle Liste der Computer im Netzwerk.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertSvc</p></td>
<td style="border:1px solid black;"><p>Zertifikatdienste</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bestandteil des Betriebssystemkerns, der digitale Zertifikate ausstellt und verwaltet.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>cisvc</p></td>
<td style="border:1px solid black;"><p>Indexdienstleistung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet über eine Abfragesprache schnellen Zugriff auf Dateien durch die Indizierung der Dateiinhalte und -eigenschaften.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ClipSrv</p></td>
<td style="border:1px solid black;"><p>Ablagemappe</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht der Ablagemappe das Erstellen und Freigeben von Datenseiten für die Überprüfung durch Remotebenutzer.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>ClusSvc</p></td>
<td style="border:1px solid black;"><p>Clusterdienste</p></td>
<td style="border:1px solid black;"><p>Domänenkonto</p></td>
<td style="border:1px solid black;"><p>Steuert Clustervorgänge von Servern und verwaltet die Clusterdatenbank.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>COMSysApp</p></td>
<td style="border:1px solid black;"><p>COM+-Systemanwendung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Konfiguration und Verfolgung von COM+-basierten Komponenten. COM+-Komponenten funktionieren nicht ordnungsgemäß, wenn dieser Dienst deaktiviert wird.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CORRTSvc</p></td>
<td style="border:1px solid black;"><p>.NET Framework-Support Service</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Benachrichtigt Abonnentenclients, wenn bestimmte Prozesse den Clientlaufzeitdienst initialisieren.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CryptSvc</p></td>
<td style="border:1px solid black;"><p>Kryptografiedienste</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet kryptografische Schlüsselverwaltungsdienste für Windows-basierte Computer.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DcomLaunch</p></td>
<td style="border:1px solid black;"><p>DCOM-Serverprozess-Startprogramm</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet einen Teil der RPC-Dienste, die in der Kombination mit dem RPCSS-Dienst Berechtigungen für „Lokales System“ erfordern.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DFS</p></td>
<td style="border:1px solid black;"><p>Verteiltes Dateisystem (Distributed File System, DFS)</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Integriert unterschiedliche Dateifreigaben innerhalb des Netzwerks in einen einzigen logischen Namenspace. Dieses System wird für die Meldung der SYSVOL-Freigabe benötigt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DFSR</p></td>
<td style="border:1px solid black;"><p>DFS-Replikation</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Kopiert automatisch Updates in Dateien und Ordner von Computern, die Bestandteil einer gemeinsamen Replikationsgruppe sind (in Windows Server 2003 R2 hinzugefügt).</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Dhcp</p></td>
<td style="border:1px solid black;"><p>DHCP-Client</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Verwaltet Konfigurationsdaten von DHCP-Netzwerken durch das Registrieren und Aktualisieren von IP-Adressen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DHCPServer</p></td>
<td style="border:1px solid black;"><p>DHCP-Server</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Dieser Dienst verwaltet DHCP und weist Clientcomputern IP-Adressen zu.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dmadmin</p></td>
<td style="border:1px solid black;"><p>Dienst für die Verwaltung logischer Datenträger</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Führt administrative Dienste für Datenträgerverwaltungsanforderungen aus und konfiguriert Datenträger. Dieser Dienst wird ausschließlich im Rahmen solcher Konfigurationsprozesse ausgeführt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dmserver</p></td>
<td style="border:1px solid black;"><p>Logischer Diskettenmanager</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Erkennt und überwacht neue Laufwerke und sendet Datenträgerinformationen an den dmadmin-Dienst. Dieser Dienst darf nicht deaktiviert werden, wenn dynamische Datenträger verwendet werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DNS</p></td>
<td style="border:1px solid black;"><p>DNS-Server</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die DNS-Namensauflösung durch die Beantwortung von Abfragen und Updateanforderungen für DNS-Namen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Dnscache</p></td>
<td style="border:1px solid black;"><p>DNS-Client</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Ist für das Auflösen und Zwischenspeichern von DNS-Namen zuständig und muss auf jedem Computer ausgeführt werden, auf dem die DNS-Namensauflösung durchgeführt wird.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ERSvc</p></td>
<td style="border:1px solid black;"><p>Fehlerberichterstattungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Sammelt, speichert und meldet Fälle, in denen unerwartete Anwendungsfehler auftreten oder Anwendungen unerwartet beendet werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Eventlog</p></td>
<td style="border:1px solid black;"><p>Ereignisprotokoll</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Zeichnet Ereignisse, die von Programmen, Diensten sowie vom Betriebssystem gesendet werden, in Ereignisprotokollen auf.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>EventSystem</p></td>
<td style="border:1px solid black;"><p>COM+-Ereignissystem</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verteilt Ereignisse automatisch an abonnierte COM-Komponenten.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>FastUser Switching Compatibility</p></td>
<td style="border:1px solid black;"><p>Kompatibilität für schnelle Benutzerumschaltung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet Anwendungen, die Unterstützung in mehreren Benutzerumgebungen erfordern.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Fax</p></td>
<td style="border:1px solid black;"><p>Faxdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet TAPI-kompatible Faxfunktionen an.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Groveler</p></td>
<td style="border:1px solid black;"><p>SIS-Groveler</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Integraler Bestandteil des Remoteinstallationsdienstes (RIS), der Dateiduplikate ermittelt und das Original in SIS (Single Instance Storage) kopiert.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>helpsvc</p></td>
<td style="border:1px solid black;"><p>Hilfe und Support</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Zugriff auf Speicher und Dienste, in denen Metadaten und Informationen über Hilfethemen für die Hilfe- und Supportcenteranwendung enthalten sind.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>HidServ</p></td>
<td style="border:1px solid black;"><p>Eingabegerätzugriff</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht allgemeinen Eingabezugriff auf USB-Geräte wie Tastaturen und Mäuse.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>HTTPFilter</p></td>
<td style="border:1px solid black;"><p>HTTP-SSL</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht IIS die Ausführung von SSL-Funktionen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>IAS</p></td>
<td style="border:1px solid black;"><p>Internetauthentifizierungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet zentralisierte Authentifizierungs-, Autorisierungs-, Überwachungs- und Kontoführungsdienste für Benutzer, die eine Verbindung zu einem Netzwerk herstellen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>IASJet</p></td>
<td style="border:1px solid black;"><p>IAS-Jet-Datenbankzugriff</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Authentifizierungs-, Autorisierungs- und Kontoführungsdienste über das RADIUS-Protokoll.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>IISADMIN</p></td>
<td style="border:1px solid black;"><p>IIS-Verwaltungsdienst</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Verwaltung von IIS-Komponenten wie FTP und Webdiensterweiterungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ImapiService</p></td>
<td style="border:1px solid black;"><p>COM-Dienst für IMAPI-CD-Brennen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet das Erstellen von CDs über die IMAPI COM-Schnittstelle und führt auf Anforderung CD-R-Schreibvorgänge durch.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Irmon</p></td>
<td style="border:1px solid black;"><p>Infrarotüberwachung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Dateifreigabe über Infrarotverbindungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>IsmServ</p></td>
<td style="border:1px solid black;"><p>Standortübergreifender Messagingdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht den Austausch von Nachrichten zwischen Computern unter Windows Server.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>kdc</p></td>
<td style="border:1px solid black;"><p>Kerberos-Schlüsselverteilungscenter</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Benutzern die Anmeldung über das Kerberos-Authentifizierungsprotokoll. Wenn dieser Dienst angehalten wird, können Clients sich nicht mehr bei einer Domäne anmelden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>lanmanserver</p></td>
<td style="border:1px solid black;"><p>Server</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet RPC-Unterstützung und ermöglicht Datei-, Drucker- und Named-Piped-Freigabe über das Netzwerk.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>lanman-workstation</p></td>
<td style="border:1px solid black;"><p>Arbeitsstation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Netzwerkverbindungen und Kommunikation für Clientdienste.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>LicenseService</p></td>
<td style="border:1px solid black;"><p>Lizenzprotokollierung</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Wurde ursprünglich entwickelt, um die mit Windows NT® Server 3.51 eingeführten CALs zu verwalten. Der Dienst sollte nur von Benutzern aktiviert werden, die Microsoft Small Business Server verwenden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>LMHosts</p></td>
<td style="border:1px solid black;"><p>TCP/IP-NetBIOS-Hilfsprogramm</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Bietet NetBIOS-über-TCP/IP-Unterstützung sowie NetBIOS-Namensauflösung für Clients.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>LPDSVC</p></td>
<td style="border:1px solid black;"><p>TCP/IP-Druckserver</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht TCP/IP-basiertes Drucken durch Verwenden des LPD-Protokolls zum Empfang von Dokumenten von LPD-Dienstprogrammen auf UNIX-basierten Plattformen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>LSASS</p></td>
<td style="border:1px solid black;"><p>Lokale Sicherheitsautorität</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet eine Schnittstelle zur Verwaltung der lokalen Sicherheit, der Domänenauthentifizierung sowie von Active Directory-Prozessen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MacFile</p></td>
<td style="border:1px solid black;"><p>Dateiserver für Macintosh</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Macintosh-Benutzern, Dateien unter Windows Server 2003 zu speichern und darauf zuzugreifen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MacPrint</p></td>
<td style="border:1px solid black;"><p>Druckserver für Macintosh</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Macintosh-Benutzern die Verwendung von Windows Server 2003-Druckdiensten.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MDM</p></td>
<td style="border:1px solid black;"><p>Machine Debug Manager</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Verwaltet das lokales Debuggen sowie Remotedebuggen von Anwendungen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Messenger</p></td>
<td style="border:1px solid black;"><p>Nachrichtendienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Sendet Nachrichten an den Warndienst oder empfängt Nachrichten von diesem. Dieser Nachrichtendienst besitzt keine Beziehung zu Windows Messenger. Im Falle seiner Deaktivierung ist es nicht möglich, die Befehle „net send“ und „net name“ zu verwenden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>mnmsrvc</p></td>
<td style="border:1px solid black;"><p>NetMeeting-Remotedesktopfreigabe</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht autorisierten Benutzern über Windows NetMeeting®-Dienste den Remotezugriff auf den Windows-Desktop von anderen Computern aus.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>mqds</p></td>
<td style="border:1px solid black;"><p>Message Queuing Down Level Clients</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Active Directory-Zugriff für ältere Versionen von Windows, die den Message Queuing-Dienst verwenden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Mqtgsvc</p></td>
<td style="border:1px solid black;"><p>Message Queuing-Trigger</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet ein regelbasiertes System zur Überwachung von Nachrichten, die über eine Warteschlange des Message Queuing-Dienstes eingehen, und ruft Nachrichtenverarbeitungsdienste auf.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MSDTC</p></td>
<td style="border:1px solid black;"><p>Distributed Transaction Coordinator</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Koordiniert Transaktionen, die über mehrere Computer, Datenbanken, Dateisysteme, Nachrichtenwarteschlangen und andere transaktionsgeschützte Ressourcenmanager verteilt sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MSExchange MTA</p></td>
<td style="border:1px solid black;"><p>Microsoft Exchange MTA-Stacks</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Bietet einen abwärtskompatiblen Nachrichtenübertragungsdienst in einer Umgebung im gemischten Modus.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MSFTPSVC</p></td>
<td style="border:1px solid black;"><p>FTP-Publishingdienst</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Bietet FTP-Konnektivität und Verwaltung über das IIS-Snap-In.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MSIServer</p></td>
<td style="border:1px solid black;"><p>Windows Installer</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Installation und Deinstallation von Anwendungen durch die Anwendung einer Reihe von zentral definierten Setupregeln während des Installationsvorgangs.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>msmq</p></td>
<td style="border:1px solid black;"><p>Message Queuing</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Fungiert als Messaginginfrastruktur und Entwicklungstool zum Erstellen verteilter Messaginganwendungen für Windows-Programme.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MSSQL$UDDI</p></td>
<td style="border:1px solid black;"><p>MSSQL$UDDI</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Bietet UDDI-Dienste (Universal Description, Discovery, and Integration) für das SQL Server-Datenbankmodul.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MSSQL SERVER</p></td>
<td style="border:1px solid black;"><p>MS SQL-Server</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Bietet konfigurierbare MS SQL Server-Dienste.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MSSQLServer ADHelper</p></td>
<td style="border:1px solid black;"><p>MS SQL Server AD Helper</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht SQL Server und SQL Server Analysis Services das Veröffentlichen von Informationen in Active Directory.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>NetDDE</p></td>
<td style="border:1px solid black;"><p>Netzwerk-DDE</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Netzwerktransport und Sicherheit für DDE bei Programmen, die auf demselben Computer oder auf verschiedenen Computern ausgeführt werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>NetDDEdsdm</p></td>
<td style="border:1px solid black;"><p>Netzwerk-DDE-Serverdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet DDE-Netzwerkfreigaben.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Netlogon</p></td>
<td style="border:1px solid black;"><p>Netlogon</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Erhält einen Sicherheitskanal zwischen Clientcomputern und Domänencontrollern für die Authentifizierung von Diensten und Benutzern aufrecht.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Netman</p></td>
<td style="border:1px solid black;"><p>Netzwerkverbindungen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet Objekte im Ordner „Netzwerkverbindungen“.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Network Connections</p></td>
<td style="border:1px solid black;"><p>Netzwerkverbindungen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet Objekte im Order „Netzwerk- und DFÜ-Verbindungen“, über den Netzwerk- und Remoteverbindungen angezeigt werden können.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>NLA</p></td>
<td style="border:1px solid black;"><p>Dienst für Netzwerkadressinformationen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Sammelt und speichert Netzwerkkonfigurationsdaten und verarbeitet Informationen über Netzwerkadressenänderungen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>NntpSvc</p></td>
<td style="border:1px solid black;"><p>Network News Transfer-Protokoll</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Verwendung von Computern als NNTP-Newsserver.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>NtFrs</p></td>
<td style="border:1px solid black;"><p>Dateireplikation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Kopiert automatisch Updates in Dateien und Ordner von Computern, die einen gemeinsamen Replikatsatz des Dateireplikationsdienstes nutzen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>NtLmSsp</p></td>
<td style="border:1px solid black;"><p>NTLM Security Support Provider</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verantwortlich für Authentifizierung und Verwaltung von lokalen Sicherheitsrichtlinienobjekten.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>NWC Workstation</p></td>
<td style="border:1px solid black;"><p>Client Service für NetWare</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Bietet Zugriff auf NetWare-Datei- und -Druckressourcen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>nwsapagent</p></td>
<td style="border:1px solid black;"><p>SAP-Agent</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Meldet Netzwerkdienste in IPX-Netzwerken, die das IPX SAP-Protokoll verwenden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>One Point</p></td>
<td style="border:1px solid black;"><p>Microsoft Operations Manager 2000-Agent</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>MOM 2000-Agent (Microsoft Operations Manager)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PlugPlay</p></td>
<td style="border:1px solid black;"><p>Plug-and-Play</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Erkennung von Hardwareänderungen ohne Benutzereingaben.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PolicyAgent</p></td>
<td style="border:1px solid black;"><p>IPsec-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet IPsec-Richtlinien, startet IKE und koordiniert die Einstellungen für IPsec-Richtlinien im IPsec-Treiber.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>POP3SVC</p></td>
<td style="border:1px solid black;"><p>Microsoft Pop3-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Bietet Dienste für E-Mail-Transfer- und -abruf.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Protected-Storage</p></td>
<td style="border:1px solid black;"><p>Geschützter Speicher</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Stellt einen geschützten Speicher für vertrauliche Daten bereit.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RasAuto</p></td>
<td style="border:1px solid black;"><p>Verwaltung für automatische RAS-Verbindung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Erstellt jedes Mal Verbindungen zu Remotecomputern, wenn Programme auf DNS- oder NetBIOS-Remotenamen oder -adressen verweisen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RasMan</p></td>
<td style="border:1px solid black;"><p>RAS-Verbindungsverwaltung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet DFÜ- und VPN-Verbindungen zu Remotenetzwerken.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RDSessMgr</p></td>
<td style="border:1px solid black;"><p>Sitzungs-Manager für Remotedesktophilfe</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet und steuert die Funktion „Remoteunterstützung“ innerhalb der Hilfe- und Supportcenteranwendung.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Remote_</p>
<p>Storage_Server</p></td>
<td style="border:1px solid black;"><p>Remotespeicherserver</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verschieben und Abrufen von Dateien aus sekundären Speichermedien</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Remote_</p>
<p>Storage_User_</p>
<p>Link</p></td>
<td style="border:1px solid black;"><p>Remotespeicherbenachrichtigung</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Der Remote_Storage_User_Link-Dienst benachrichtigt Benutzer, wenn diese versuchen, Dateien zu lesen oder zu schreiben, die nur auf sekundären Speichermedien verfügbar sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RemoteAccess</p></td>
<td style="border:1px solid black;"><p>Routing und Remotezugriff</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Multiprotokoll-Routingdienste sowie DFÜ- und VPN-Remotezugriffsdienste.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RemoteRegistry</p></td>
<td style="border:1px solid black;"><p>Remoteregistrierungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Remotebenutzern mit den entsprechenden Berechtigungen das Ändern von Registrierungseinstellungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RpcLocator</p></td>
<td style="border:1px solid black;"><p>Remote Procedure Call Locator</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Verwaltet die RPC-Namensdienstdatenbank, um RPC-Clients das Auffinden von RPC-Servern zu ermöglichen. Standardmäßig deaktiviert</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RpcSs</p></td>
<td style="border:1px solid black;"><p>Remoteprozeduraufruf</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Dient als RPC-Endpunktzuweisungs- und COM-Dienst (Component Object Model).</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RSoPProv</p></td>
<td style="border:1px solid black;"><p>Richtlinienergebnissatz-Provider</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Verbindungen zu Windows-Domänencontrollern sowie den Zugriff auf die WMI-Datenbank und simuliert den Richtlinienergebnissatz für Gruppenrichtlinieneinstellungen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RSVP</p></td>
<td style="border:1px solid black;"><p>QoS RSVP</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Verwendung allgemeiner API-Dienstqualitätsanforderungen von Anwendungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Sacsvr</p></td>
<td style="border:1px solid black;"><p>Hilfsprogramm für spezielle Verwaltungskonsole</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Führt Remoteverwaltungsaufgaben aus, wenn ein Betriebssystem der Windows Server-Familie aufgrund von STOP-Fehlermeldungen nicht mehr funktioniert.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SamSs</p></td>
<td style="border:1px solid black;"><p>Sicherheitskontenverwaltung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Daten von Benutzer- und Gruppenkonten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SCardSvr</p></td>
<td style="border:1px solid black;"><p>Smartcard</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Verwaltet und steuert den Zugriff auf Smartcards, wenn diese in ein entsprechendes Lesegerät am Computer eingeführt werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Schedule</p></td>
<td style="border:1px solid black;"><p>Taskplaner</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Ausführung von automatisierten Aufgaben.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>seclogon</p></td>
<td style="border:1px solid black;"><p>Sekundärer Anmeldedienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Erstellung von Prozessen im Kontext verschiedener Sicherheitsprinzipale.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SENS</p></td>
<td style="border:1px solid black;"><p>Systemereignisbenachrichtigung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verfolgt Ereignisse im Zusammenhang mit dem System und der Stromversorgung und benachrichtigt COM+-Ereignissystem-Abonnenten von diesen Ereignissen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SharedAccess</p></td>
<td style="border:1px solid black;"><p>Windows-Verbindungsfirewall/Gemeinsame Nutzung der Internetverbindung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet NAT-, Adressen- und Namenauflösungsdienste für sämtliche Computer in einem Netzwerk, wenn die gemeinsame Nutzung der Internetverbindung aktiviert ist.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>ShellHW</p>
<p>Detection</p></td>
<td style="border:1px solid black;"><p>Shellhardwareerkennung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Benachrichtigt über AutoPlay-Hardwareereignisse.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SimpTcp</p></td>
<td style="border:1px solid black;"><p>Einfache TCP/IP-Dienste</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Bietet einfache TCP/IP-Dienste wie Echo, Discard, Daytime, Zeichengenerator und Zitat des Tages.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SMTPSVC</p></td>
<td style="border:1px solid black;"><p>Simple Mail Transport Protocol</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Fungiert als SMTP-Übermittlungs- und Relay-Agent, indem E-Mails, die von Remotezielen eingehen oder dorthin gesendet, angenommen und in Warteschlangen eingereiht werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SNMP</p></td>
<td style="border:1px solid black;"><p>SNMP-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht, dass eingehende SNMP-Anforderungen vom lokalen Computer bedient werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SNMPTRAP</p></td>
<td style="border:1px solid black;"><p>SNMP-Trap-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Empfängt SNMP-Trap-Nachrichten, die von lokalen oder von Remote-SNMP-Agenten erstellt wurden, und leitet diese Nachrichten an SNMP-Verwaltungsserver weiter.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Spooler</p></td>
<td style="border:1px solid black;"><p>Druckerspooler</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet alle lokalen und Netzwerkdruckwarteschlangen und steuert sämtliche Druckaufträge.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SQLAgent$</p>
<p>WEBDB</p></td>
<td style="border:1px solid black;"><p>SQL Agent$ UDDI oder WebDB</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p> </p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SrvcSurg</p></td>
<td style="border:1px solid black;"><p>Remoteverwaltungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verantwortlich für die Ausführung von Remoteverwaltungsaufgaben beim Serverstart. Dazu zählt auch die Bootcount-Inkrementierung des Servers sowie die Ausgabe von Warnmeldungen, wenn Datum und Uhrzeit des Servers nicht eingestellt wurden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>StiSvc</p></td>
<td style="border:1px solid black;"><p>Windows-Bilderfassung</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Bietet Bilderfassungsdienste für Scanner und Kameras.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>srservice</p></td>
<td style="border:1px solid black;"><p>Systemwiederherstellungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Überwacht Systemveränderungen sowie Anwendungsdateien und erstellt anschließend leicht identifizierbare Wiederherstellungspunkte.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SSDPSRV</p></td>
<td style="border:1px solid black;"><p>SSDP-Suchdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Verwaltet Meldungen über vorhandene Geräte, Cacheupdates sowie SSDP-Benachrichtigungen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>StiSvc</p></td>
<td style="border:1px solid black;"><p>Windows-Bilderfassung (Windows Image Acquisition, WIA)</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die stabile Kommunikation zwischen Anwendungen und Bilderfassungsgeräten für die effiziente Übertragung von Bildern an den Computer.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SwPrv</p></td>
<td style="border:1px solid black;"><p>Microsoft Software Shadow Copy Provider</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Software-basierten Schattenkopien des Volumeschattenkopie-Dienstes.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SysmonLog</p></td>
<td style="border:1px solid black;"><p>Leistungsprotokolle und Warnungen</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Sammelt Daten zu Leistungsprotokollen und Warnungen. Wird nur ausgeführt, wenn mindestens ein Leistungsdatensammelereignis geplant ist.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TapiSrv</p></td>
<td style="border:1px solid black;"><p>Telefonie</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet TAPI-Unterstützung für Programme, die Telefoniegeräte und IP-basierte Sprachverbindungen steuern.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TermService</p></td>
<td style="border:1px solid black;"><p>Terminaldienste</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht mehreren Clients den Zugriff auf virtuelle Windows-Desktopsitzungen, die auf dem Server ausgeführt werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TermServ</p>
<p>Licensing</p></td>
<td style="border:1px solid black;"><p>Terminaldienstelizenzierung</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Gewährt registrierten Clients Lizenzen, wenn sie eine Verbindung zu einem Terminalserver herstellen, und verfolgt diese Lizenzen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>tftpd</p></td>
<td style="border:1px solid black;"><p>Daemon für „Trivial FTP“</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Registriert und antwortet auf TFTP-Anforderungen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Design</p></td>
<td style="border:1px solid black;"><p>Design</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Renderingunterstützung für die grafische Benutzeroberfläche von Windows XP.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TlntSvr</p></td>
<td style="border:1px solid black;"><p>Telnet</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet Windows-Benutzern Telnet-Dienste und unterstützt Terminalsitzungen vom Typ ANSI, VT-100, VT52 und VTNT.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TrkSvr</p></td>
<td style="border:1px solid black;"><p>Server für die Überwachung verteilter Verknüpfungen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Speichert Informationen, so dass Dateien, die zwischen Volumes verschoben werden, zu jedem Volume innerhalb der Domäne verfolgt werden können. Dieser Dienst wird auf jedem Domänencontroller ausgeführt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TrkWks</p></td>
<td style="border:1px solid black;"><p>Client für die Überwachung verteilter Verknüpfungen</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verantwortlich für die Aufrechterhaltung von Verknüpfungen zwischen den NTFS-Dateisystemdateien auf dem Computer oder im Netzwerk. Stellt sicher, dass Verknüpfungen und OLE-Verknüpfungen funktionieren, nachdem Zieldateien verschoben oder umbenannt wurden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Tssdis</p></td>
<td style="border:1px solid black;"><p>Terminaldienste-Sitzungsverzeichnis</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verfolgt unterbrochene Terminaldienstesitzungen in einem Cluster, um sicherzustellen, dass für die Benutzer die Verbindung zu diesen Sitzungen wiederhergestellt wird.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Uploadmgr</p></td>
<td style="border:1px solid black;"><p>Upload-Manager</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet synchrone und asynchrone Dateiübertragungen zwischen Clients und Servern im Netzwerk.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>upnphost</p></td>
<td style="border:1px solid black;"><p>Universeller Plug &amp; Play-Gerätehost</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Implementiert sämtliche Komponenten, die zur Geräteregistrierung, Steuerung und Reaktion auf Ereignisse für Hostgeräte erforderlich sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>UPS</p></td>
<td style="border:1px solid black;"><p>Unterbrechungsfreie Stromversorgung</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Verwaltet die Kommunikation mit einer unterbrechungsfreien Stromversorgung (Uninterruptible Power Supply, UPS), die über einen seriellen Anschluss mit den Computer verbunden ist.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VDS</p></td>
<td style="border:1px solid black;"><p>Virtueller Datenträgerdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Bietet eine einzige Schnittstelle zur Verwaltung der Block-Storage-Virtualisierung, unabhängig davon, ob dafür Betriebssystemsoftware, RAID-Speicher oder andere Virtualisierungsmodule verwendet werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VSS</p></td>
<td style="border:1px solid black;"><p>Volumeschattenkopie</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verwaltet Volumesnapshots, die von Sicherungsanwendungen verwendet werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>W32Time</p></td>
<td style="border:1px solid black;"><p>Windows-Zeitgeber</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Verantwortlich für die Datums- und Zeitsynchronisierung mit NTP.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>W3SVC</p></td>
<td style="border:1px solid black;"><p>WWW-Publishingdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Enthält einen Prozess- und Konfigurationsmanager zur Bereitstellung von WWW-Publishingdiensten.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WebClient</p></td>
<td style="border:1px solid black;"><p>WebClient</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Ermöglicht Win32-Anwendungen den Zugriff auf Dokumente aus dem Internet.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WindowsSystem</p>
<p>Resource</p>
<p>Manager</p></td>
<td style="border:1px solid black;"><p>Windows-Verwaltungsinstrumentation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die richtlinienbasierte Verwaltung des CPU- und Speicherbedarfs für Prozesse, die über eine einzige Betriebssysteminstanz ausgeführt werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WinHttpAutoSvc</p></td>
<td style="border:1px solid black;"><p>WinHTTP-Web Proxy Auto-Discovery-Dienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Implementiert die Proxykonfigurationsermittlung für WinHttp-Clients.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>winmgmt</p></td>
<td style="border:1px solid black;"><p>Windows-Verwaltungsinstrumentation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Stellt Systemverwaltungsinformationen über mehrere Schnittstellen bereit.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WINS</p></td>
<td style="border:1px solid black;"><p>WINS-Dienst (Windows Internet Naming Service)</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die NetBIOS-Namensauflösung sowie die WINS-Replikation.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WmdmPmSN</p></td>
<td style="border:1px solid black;"><p>Seriennummer der tragbaren Medien</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht, dass WMDM die Seriennummern von tragbaren Musikgeräten abrufen kann, die an den Computer angeschlossen sind.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Wmi</p></td>
<td style="border:1px solid black;"><p>Treibererweiterungen für Windows-Verwaltungsinstrumentation</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Überwacht sämtliche Treiber und Ereignisablaufverfolgungsanbieter, die für die Veröffentlichung von WMI-Daten oder Ereignisablaufverfolgungsdaten konfiguriert sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WmiApSrv</p></td>
<td style="border:1px solid black;"><p>WMI-Leistungsadapter</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Wandelt von WMI-Anbietern bereitgestellte Leistungsindikatoren in Indikatoren um, die über die Reverse Adapter Performance Library von PDH verarbeitet werden können.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WMServer</p></td>
<td style="border:1px solid black;"><p>Windows Media-Dienste</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die Bereitstellung von Windows Media-Diensten.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>wscsvc</p></td>
<td style="border:1px solid black;"><p>Sicherheitscenter</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Überwacht Sicherheitseinstellungen und Konfigurationsdaten des Systems.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>wuauserv</p></td>
<td style="border:1px solid black;"><p>Automatische Updates</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht das Herunterladen von Updates auf der Windows Update-Website von Microsoft.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Wuser32</p></td>
<td style="border:1px solid black;"><p>SMS Remote Control Agent</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Stellt Remotecomputerverwaltungsdienste bereit, beispielsweise Remotesteuerungs- und Remotedateiübertragungsdienste für SMS 2003.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WZCSVC</p></td>
<td style="border:1px solid black;"><p>Konfigurationsfreie drahtlose Verbindung</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht die automatische Konfiguration für drahtlose Adapter vom Typ IEEE 802.11 für die drahtlose Kommunikation.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>xmlprov</p></td>
<td style="border:1px solid black;"><p>Netzwerkbereitstellungsdienst</p></td>
<td style="border:1px solid black;"><p>Lokales System</p></td>
<td style="border:1px solid black;"><p>Ermöglicht das Herunterladen und Verwalten von XML-Konfigurationsdateien aus Netzwerkbereitstellungsdiensten wie Wireless Provisioning Service (WPS) von Microsoft.</p></td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
**Download**
  
[Leitfaden „Sichern von kritischen Konten und Dienstkonten“ herunterladen](http://go.microsoft.com/fwlink/?linkid=73609)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
