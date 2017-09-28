---
TOCTitle: Sicherheitsüberwachung und Angriffsermittlung
Title: Sicherheitsüberwachung und Angriffsermittlung
ms:assetid: 'a30af90e-ce18-47fc-a947-11f332ee4731'
ms:contentKeyID: 20072339
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc875806(v=TechNet.10)'
---

Sicherheitsüberwachung und Angriffsermittlung
=============================================

Veröffentlicht: 29. Aug 2006

##### Auf dieser Seite

[](#egaa)[Einführung](#egaa)
[](#efaa)[Definition](#efaa)
[](#eeaa)[Die Herausforderung für mittelgroße Unternehmen](#eeaa)
[](#edaa)[Lösungen](#edaa)
[](#ecaa)[Zusammenfassung](#ecaa)
[](#ebaa)[Anhang A: Ausschließen unnötiger Ereignisse](#ebaa)
[](#eaaa)[Anhang B: Implementieren von Gruppenrichtlinieneinstellungen](#eaaa)

### Einführung

Willkommen bei diesem Dokument aus der Reihe der Sicherheitsleitfäden für mittelgroße Unternehmen. Microsoft hofft, dass Ihnen die folgenden Informationen beim Erstellen einer sichereren und produktiveren Computerumgebung helfen werden.

#### Kurzzusammenfassung

Die Anzahl spektakulärer Fälle von Bedrohungen und Vorfällen im Zusammenhang mit bösartiger Software, die die Berichterstattung in den Medien schon seit Jahren dominieren, hat zu einem gesteigerten Bewusstsein geführt und die meisten Unternehmen dazu veranlasst, Zeit und Ressourcen in den Schutz vor diesem anhaltenden Sicherheitsproblem zu investieren. Die größte Bedrohung für die Infrastruktur eines Unternehmens stellt allerdings nicht unbedingt ein Angriff von außen dar, wie etwa durch einen Virus, sondern kann durchaus aus dem internen Netzwerk selbst kommen.

Angriffe, die aus einem Unternehmensnetzwerk erfolgen, weisen ein sehr hohes Schadenspotenzial auf, insbesondere wenn sie von Mitarbeitern in vertrauensvollen Positionen und mit Zugriff auf alle Netzwerkressourcen in einem Unternehmen ausgeführt werden. Nach genauer Untersuchung der Risiken durch externe und interne Bedrohungen halten viele Unternehmen nach geeigneten Systemen zur Netzwerküberwachung und zur Ermittlung von Angriffen jeglichen Ursprungs Ausschau.

Sicherheitsüberwachungspraktiken sind dabei für Unternehmen, die gesetzlichen Vorschriften unterliegen, keine Option, sondern eine Notwendigkeit. Solche Vorschriften können auch die Dauer und die Art der Aufbewahrung und Archivierung von Sicherheitsüberwachungsprotokollen regeln. Gesetzliche Vorschriften unterliegen kontinuierlichen Veränderungen, und für regulierte Unternehmen gelten immer größere Anforderungen hinsichtlich der Netzwerksicherung, der Identifizierung von Personen, die auf Ressourcen zugreifen, und des Datenschutzes. Damit sind Unternehmen auf der ganzen Welt immer stärker gefordert, effektive Sicherheitsüberwachungslösungen zu implementieren.

Es gibt mehrere Gründe dafür, dass sich auch mittelgroße Unternehmen, die keinen gesetzlichen Vorschriften unterliegen, mit der Sicherheitsüberwachung und Angriffsermittlung beschäftigen sollten. Einer dieser Gründe sind die Folgen, die ein erfolgreicher Angriff auf die Infrastruktur eines Unternehmens für das betroffene Unternehmen haben kann. Dies könnte zu Betriebsunterbrechung und damit zu Produktivitätseinbußen und sogar finanziellen Verlusten führen. Außerdem könnte der gute Ruf eines Unternehmens leiden – und der lässt sich oftmals nur sehr viel schwieriger wiederherstellen als andere Verluste infolge eines Angriffs.

Die in Microsoft® Windows® vorhandenen Sicherheitsprotokollfunktionen können als Ausgangspunkt für eine Sicherheitsüberwachungslösung dienen. Sicherheitsprotokolle allein bieten jedoch nicht genügend Daten, um geeignete Vorfallsreaktionen zu planen. Sie lassen sich allerdings mit anderen Technologien zur Sammlung und Abfrage solcher Daten kombinieren und können so den zentralen Teil einer umfassenden Sicherheitsüberwachungs- und Angriffsermittlungslösung bilden.

Das Hauptziel eines Systems zur Sicherheitsüberwachung und Angriffsermittlung besteht in der Erkennung verdächtiger Ereignisse in einem Netzwerk, die auf bösartige Aktivitäten oder Verfahrensfehler hinweisen könnten. In diesem Dokument wird die Vorgehensweise zur Ausarbeitung eines Plans beschrieben, der der Notwendigkeit eines solchen Systems auf Windows-basierten Netzwerken Rechnung trägt. Es enthält außerdem Anleitungen zur Implementierung, Verwaltung und Überprüfung solcher Systeme.

#### Übersicht

Dieses Dokument besteht aus vier Hauptabschnitten, die sich mit grundlegenden Begriffen und Aspekten bezüglich des Entwurfs und der Implementierung einer wirksamen Sicherheitsüberwachungs- und Angriffsermittlungslösung befassen. Der erste Abschnitt ist die Einführung, die Sie gerade lesen. Die anderen Abschnitte sind folgende:

##### Definition

Dieser Abschnitt enthält Informationen, die für das Verständnis der mit der Erstellung und Anwendung der in diesem Dokument beschriebenen Lösung hilfreich sind.

##### Die Herausforderung für mittelgroße Unternehmen

In diesem Abschnitt werden einige der häufigen Herausforderungen beschrieben, denen sich mittelgroße Unternehmen in Bezug auf Sicherheitsüberwachungs- und Angriffsermittlungssystemen gegenübersehen.

##### Lösungen

Dieser Abschnitt enthält detaillierte Informationen zur Entwicklung, Implementierung, Verwaltung und Überprüfung der in diesem Dokument vorgestellten Lösung. Er ist in zwei Unterabschnitte aufgeteilt. „Entwickeln der Lösung“ befasst sich mit Vorabmaßnahmen und Planungsschritten. „Bereitstellen und Verwalten der Lösung“ enthält Informationen, die Ihnen bei der Bereitstellung, Verwaltung und Überprüfung eines Sicherheitsüberwachungs- und Angriffsermittlungssystems behilflich sind.

#### Zielgruppe dieses Dokuments

Dieses Dokument befasst sich mit Datenschutz- und Sicherheitsaspekten für mittelgroße Unternehmen, insbesondere für solche, die aufgrund von gesetzlichen Vorgaben Identitätsschutz und Kontrolle über den Datenzugriff gewährleisten müssen. Dementsprechend richtet sich dieses Dokument an Technikmanager und Entscheidungsträger ebenso wie an IT-Experten und Techniker, die für die Planung, Bereitstellung, den Betrieb oder speziell für die Sicherheit eines Unternehmensnetzwerks zuständig sind.

Teile dieses Dokuments enthalten Informationen, die für die meisten technischen Entscheidungsträger hilfreich sind. Zur Umsetzung aller in diesem Dokument vorgestellten Informationen sollten Leser jedoch mit Sicherheits- und Risikoaspekten in der eigenen Netzwerkumgebung sowie mit den Konzepten der Ereignisprotokollierungsdienste in Windows vertraut sein.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Definition

In diesem Dokument findet das Prozessmodell von Microsoft Operations Framework (MOF) zusätzlich zu den Dienstverwaltungsfunktionen (SMFs) von MOF für die Sicherheit und das Vorfallsmanagement Anwendung.

Für die hier vorgestellte Lösung wird insbesondere die Verwendung eines Ansatzes mit kontinuierlichen Prozessen statt eines Ansatzes der linearen Bereitstellung für die Sicherheitsüberwachung und Angriffsermittlung empfohlen. Konkret sollten die in der folgenden Abbildung dargestellten Schritte für diese Lösung berücksichtigt werden:

![](images/Cc875806.SMAAD1(de-de,TechNet.10).gif)

**Abbildung 1. Anwenden von MOF**

Eine Sicherheitsüberwachungslösung besteht im Grunde genommen aus einem kontinuierlichen Prozess der Planung, Implementierung, Verwaltung und Überprüfung, denn dies macht das Wesen der Sicherheitsüberwachung aus. Weil sich die Bedrohungen für Unternehmensnetzwerke ständig verändern, muss das System zur Sicherheitsüberwachung in einem Unternehmensnetzwerk dies ebenfalls tun.

Die Anwendung dieses Prozesses auf die Sicherheitsüberwachung entspricht der Dienstverwaltungsfunktion „Sicherheitsverwaltung“, die die folgenden Aufgaben verfolgt:

-   Ermitteln des Gefährdungsgrads des Unternehmens und Festlegen, welche Anlagen gesichert werden müssen.

-   Identifizieren der Möglichkeiten zur Reduzierung des Risikos auf ein akzeptables Maß.

-   Erstellen eines Plans zur Minderung von Sicherheitsrisiken.

-   Überwachen der Effizienz von Sicherheitsmechanismen.

-   Regelmäßiges Neubeurteilen der Effektivität und Sicherheitsanforderungen.

Weitere Informationen zu MOF finden Sie auf der [Microsoft Operations Framework](http://www.microsoft.com/mof)-Website unter www.microsoft.com/mof. Weitere Informationen zur [Dienstverwaltungsfunktion „Sicherheitsverwaltung“](http://www.microsoft.com/technet/itsolutions/cits/mo/smf/mofsmsmf.mspx) finden Sie unter www.microsoft.com/technet/itsolutions/cits/mo/smf/mofsmsmf.mspx.

Das Risikomanagement umfasst die Ermittlung eines akzeptablen Risikopotenzials für ein Unternehmen, die Bewertung der aktuellen Risiken, die Entwicklung von Methoden zum Erreichen des akzeptablen Risikopotenzials sowie die Verwaltung dieses Risikos. Wenngleich in diesem Dokument einige Risikomanagementkonzepte sowie einige Schritte zur Risikoabschätzung genannt werden, ist eine eingehende Behandlung des Risikomanagements ein Thema für sich und verdient somit spezielle Aufmerksamkeit. Weitere Informationen zur Risikoanalyse und -beurteilung finden Sie im [*Leitfaden zum Sicherheitsrisikomanagement*](http://go.microsoft.com/fwlink/?linkid=30794) unter http://go.microsoft.com/fwlink/?linkid=30794.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Die Herausforderung für mittelgroße Unternehmen

Mittelgroße Unternehmen sind bei der Ausarbeitung eines wirksamen Sicherheitsüberwachungssystems und unterstützender Richtlinien mit vielfältigen Herausforderungen konfrontiert. Zu diesen Herausforderungen gehören:

-   Das Verständnis der Notwendigkeit und der Vorteile des Schutzes der gesamten Netzwerkumgebung vor internen und externen Bedrohungen.

-   Der Entwurf eines wirksamen Sicherheitsüberwachungs- und Angriffsermittlungssystems, das Methoden zur Erkennung von Versuchen der Umgehung vorhandener Richtlinien und zu deren Vorbeugung umfasst.

-   Die Implementierung umfassender und effektiver Überwachungsrichtlinien, die nicht nur Angriffe erkennen, sondern auch ein Gesamtbild der Sicherheitsstufe einer Umgebung zu Zwecken der Fehlerbehebung zeichnen können.

-   Die Verwaltung von Richtlinien und Prozessen, die Sicherheitsberichte effizient mit vorhandenen Richtlinien korrelieren, um so den Verwaltungsaufwand bei der Erkennung verdächtiger Aktivitäten gering zu halten.

-   Die Implementierung und Umsetzung effizienter Geschäftspraktiken und -richtlinien, die die Sicherheitsüberwachung unter Berücksichtigung des Geschäftsbedarfs unterstützen.

-   Das Ermitteln akzeptabler Risikoschwellen zur Abwägung zwischen Verwendbarkeit und Risikominderung.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Lösungen

Wie bereits erwähnt hilft ein umfassender Sicherheitsüberwachungsprozess nicht nur bei der forensischen Analyse, sondern kann außerdem eine proaktive Sicherheitsmaßnahme darstellen, durch die Informationen vor, während und nach einem Angriff bereitgestellt werden. Durch Einrichtung einer zentralisierten Datenbank für Sicherheitsberichte können Angriffe während der Suchphase, während ihrer Durchführung oder unmittelbar danach erkannt werden. Auf diese Weise erhalten die zuständigen Personen die nötigen Informationen für eine effektive Reaktion auf die Angriffe, so dass sich die Auswirkungen eines Einbruchsversuchs in Grenzen halten lassen.

Es ist wichtig, sich während der Entwicklungsphase über die vielfältigen Vorteile der Implementierung einer Sicherheitsüberwachungslösung bewusst zu sein, damit all diese Vorteile für den Entwurf und die Richtlinien genutzt werden können. Die Sicherheitsüberwachung bietet z. B. folgende Vorteile:

-   Identifizierung von und Abhilfe bei Systemen, die nicht den Sicherheits- oder Updaterichtlinien zur Reduzierung des Sicherheitsanfälligkeitsprofils eines mittelgroßen Unternehmens entsprechen.

-   Bereitstellung von Informationen, die durch Erkennung ungewöhnlicher Aktivitäten vor Einbruchsversuchen warnen, bevor ein Angriff tatsächlich erfolgt.

-   Erstellung und Schutz von Sicherheitsüberwachungsdaten zur Verbesserung forensischer Analysen, was nicht nur gesetzlichen Vorschriften entspricht, sondern auch die Auswirkungen von Angriffen begrenzen kann.

-   Hilfestellung bei der Sicherheitsstufenanalyse zur Erhöhung der Sicherheit insgesamt.

-   Erkennen von sowohl mutwilligen als auch nicht beabsichtigten Aktivitäten, die außerhalb vorhandener Geschäftsprozesse erfolgen.

-   Hilfestellung bei der Identifizierung nicht verwalteter Systeme in einem Netzwerk bzw. Fehlerbehebung bei gefährdeten Geräten.

#### Entwickeln der Lösung

Sicherheit ist für viele Unternehmen ein wichtiger Aspekt. Zwar setzen die meisten Unternehmen im angemessenen Umfang Ressourcen für die physische Sicherheit ein, indem sie Maßnahmen von einfachen Türschlössern bis hin zu komplexen kartenbasierten Zugangskontrollsystemen treffen, doch kümmern sich viele Unternehmen nicht genug um die Sicherheit von Daten, die für sie von zunehmender Bedeutung sind.

Werden Datensicherheits- und Überwachungsaspekte berücksichtigt, konzentrieren Unternehmen ihre Datensicherheitsmaßnahmen häufig auf den Umkreis mit Firewalls. Durch diesen Ansatz allein bleiben andere Angriffspunkte jedoch in hohem Maße gefährdet. Laut [2004 E-Crime Watch Survey](http://www.cert.org/archive/pdf/2004ecrimewatchsummary.pdf), einem vom United States Secret Service und dem CERT Coordination Center unter www.cert.org/archive/pdf/2004eCrimeWatchSummary.pdf veröffentlichten Dokument, kommen 29 Prozent aller identifizierten Angreifer aus internen Quellen und schließen beispielsweise aktuelle und ehemalige Mitarbeiter sowie Subunternehmer ein. Bei Betrachtung dieser Angaben wird klar, dass ein mehrschichtiger Sicherheitsansatz zum Schutz vor internen Bedrohungen neben dem vor externen Quellen erforderlich ist.

Eine Methode, bei der sowohl interne als auch externe Bedrohungen von einer reaktiven Sicherheitsperspektive aus berücksichtigt werden, besteht in der Implementierung eines Protokollierungsprozesses für Sicherheitsüberwachungen. In allen Versionen von Microsoft Windows von Microsoft Windows NT® 3.1 bis zu den aktuellen Versionen wird ein integriertes Sicherheitsereignisprotokoll zur Aufzeichnung von Sicherheitsereignissen verwendet. Auch wenn diese integrierte Funktion allein bei der Durchführung forensischer Analysen als Reaktion auf einen bereits erfolgten Angriff hilfreich sein kann, wäre die proaktive Verwendung von ausschließlich dieser Funktion zur Identifizierung von Aktivitäten zu bevorstehenden Angriffen oder zur Benachrichtigung des zuständigen Personals über Einbruchsversuche während ihres Auftretens nur schwer möglich.

Wie bereits erwähnt, werden Sicherheitsprotokolle häufig reaktiv bei forensischen Analysen von bereits eingetretenen Sicherheitsvorfällen verwendet. Das Dokument [2005 Insider Threat Study](http://www.cert.org/archive/pdf/insidercross051105.pdf), das vom United States Secret Service und vom CERT unter www.cert.org/archive/pdf/insidercross051105.pdf veröffentlicht wurde, enthält jedoch eine Analyse wichtiger Ergebnisse, laut der Sicherheitsprotokolle und Überwachungen durchaus für die proaktive Erkennung statt für rein reaktive, forensische Zwecke geeignet sind. Darüber hinaus versuchen die meisten Angreifer, seien es interne oder externe, ihre Spuren durch Manipulation von Protokollen zu verwischen. Daher sollten Maßnahmen zum Schutz von Systemprotokollen ergriffen werden. Wie sich erwiesen hat, können Sicherheitsprotokolle und andere Methoden zur Überwachung und Angriffsermittlung wichtige Hilfsmittel im Bereich der Netzwerksicherheit darstellen, sofern sie korrekt verwendet und gesichert werden.

Systemsicherheitsprotokollen gilt zwar das Hauptaugenmerk dieses Dokuments, doch bilden sie lediglich das Kernstück der Sicherheitsüberwachungs- und Angriffsermittlungsmethodik. Weitere zu berücksichtigende Aspekte schließen die Art der Identifizierung und Abhilfe hinsichtlich Systemen ein, die vorhandenen Sicherheitsrichtlinien nicht entsprechen oder auf denen empfohlene Patches gegen Sicherheitslücken nicht implementiert wurden. Die interne Netzwerkinfrastruktur sollte ebenfalls überwacht werden, was idealerweise Sicherheitsberichte zu Switchports (um zu verhindern, dass nicht verwaltete Systeme Zugriff auf das Netzwerk erhalten) und zur drahtlosen Sicherheitsüberwachung (um nicht autorisierte Verbindungen oder das Mitlesen des Datenverkehrs zu verhindern) einschließt. Viele dieser Überwachungsthemen gehen über den Rahmen dieses Dokuments hinaus, sollten aber in jeder ausgereiften Sicherheitsüberwachungslösung berücksichtigt werden.

##### Implementieren der Sicherheitsüberwachung

Die folgenden Unterabschnitte enthalten Informationen zu verschiedenen Implementierungsgesichtspunkten hinsichtlich eines Sicherheitsüberwachungssystems.

###### Windows-Sicherheitsereignisprotokollierung

In allen Versionen von Microsoft Windows (Microsoft Windows NT® 3.1 und höher) können Sicherheitsereignisse anhand von integrierten Protokolldateifunktionen aufgezeichnet werden. In einer Microsoft Windows-basierten Umgebung bildet diese Funktion die Basis für die Sicherheitsüberwachung. Ohne zusätzliche Dienstprogramme oder Hilfsmittel zur Korrelation dieser Informationen gestaltet sich die proaktive Verwendung jedoch schwierig, da die Informationen verstreut sind.

![](images/Cc875806.SMAAD2(de-de,TechNet.10).gif)

**Abbildung 2. Sicherheitsprotokoll in der Ereignisanzeige**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875806.smaad2_big(de-de,technet.10).gif)
Für das Sicherheitsereignisprotokoll (siehe Abbildung oben) wird ein benutzerdefiniertes Dateiformat zur Aufzeichnung von Sicherheitsüberwachungsdaten verwendet. Teile dieser Aufzeichnungen können zwar in einem Textbearbeitungsprogramm gelesen werden, doch ist ein geeignetes Programm wie die Ereignisanzeige notwendig, um alle in diesen Protokollen enthaltenen Informationen anzuzeigen. Die Sicherheitsereignisprotokolldatei (SecEvent.evt) befindet sich im Verzeichnis %systemroot%\\System32\\config. Der Zugriff auf die Ereignisprotokolle erfolgt stets über den Ereignisprotokolldienst, der Zugriffskontrolle für jedes Protokoll bietet.  Die Standardberechtigungen im Sicherheitsprotokoll sind im Vergleich zu anderen Protokollen im System sehr strikt. Standardmäßig können nur Administratoren auf das Sicherheitsprotokoll zugreifen.

Es werden zwei Ereignistypen im Sicherheitsereignisprotokoll aufgezeichnet: Erfolgsüberwachungen und Fehlerüberwachungen. Erfolgsüberwachungsereignisse kennzeichnen von einem Benutzer, Dienst oder Programm erfolgreich durchgeführte Vorgänge. Fehlerüberwachungsereignisse betreffen Vorgänge, die nicht erfolgreich abgeschlossen wurden. Eine fehlgeschlagene Benutzeranmeldung ist ein Beispiel für ein Fehlerüberwachungsereignis und würde im Sicherheitsereignisprotokoll aufgezeichnet werden, sofern Anmeldungsüberwachungen aktiviert sind.

Mit den Gruppenrichtlinieneinstellungen für Überwachungsrichtlinien unter Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien wird festgelegt, welche Ereignisse zu Einträgen in den Sicherheitsprotokollen führen. Überwachungsrichtlinieneinstellungen können entweder über die Konsole „Lokale Sicherheitseinstellungen“ oder auf Site-, Domänen- oder Organisationseinheitsebene anhand der Gruppenrichtlinien mit Active Directory konfiguriert werden.

###### Interpretieren von Überwachungsereignissen

Im gesamten Dokument wird genauer auf Überwachungsereignisse eingegangen, daher sind grundlegende Kenntnisse der Überwachungsereignisstruktur und der in Überwachungsereignissen enthaltenen Informationen wichtig.

![](images/Cc875806.SMAAD3(de-de,TechNet.10).gif)

**Abbildung 3. Fenster „Ereigniseigenschaften“**

Ereignisse weisen drei Bestandteile auf: den Ereignis-Header, die Ereignisbeschreibung und einen Abschnitt mit Binärdaten.

Ereignis-Header umfassen die folgenden Felder:

**Tabelle 1. Der Ereignis-Header**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Feld</p></th>
<th><p>Definition</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Datum</p></td>
<td style="border:1px solid black;"><p>Das Datum, an dem das Ereignis eintrat</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Uhrzeit</p></td>
<td style="border:1px solid black;"><p>Die örtliche Uhrzeit, zu der das Ereignis eintrat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Typ</p></td>
<td style="border:1px solid black;"><p>Eine Klassifizierung des Schweregrads oder Typs des Ereignisses. Bei Sicherheitsüberwachungsereignissen finden die Typen „Erfolgsüberwachung“ und „Fehlerüberwachung“ Anwendung.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Quelle</p></td>
<td style="border:1px solid black;"><p>Die Anwendung, die das Ereignis protokolliert hat. Dies kann beispielsweise ein echtes Programm wie SQL Server, ein Treibername oder eine Systemkomponente wie die Sicherheitskomponente sein.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Kategorie</p></td>
<td style="border:1px solid black;"><p>Die Ereignisquellenklassifizierung des Ereignisses. Die Ereignisquellenklassifizierung ist in Sicherheitsüberwachungsprotokollen von Relevanz, da sie sich auf Ereignistypen bezieht, die in der Gruppenrichtlinie konfiguriert werden können.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Ereignis-ID</p></td>
<td style="border:1px solid black;"><p>Dieser Code dient der Identifizierung des spezifischen Ereignistyps. Die Abbildung oben weist die Ereignis-ID 680 auf. Dies bedeutet, dass Anmeldeinformationen von einem lokalen Prozess, einem Remoteprozess oder einem Benutzer an das Authentifizierungssystem übergeben wurden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Benutzer</p></td>
<td style="border:1px solid black;"><p>Der Benutzername, unter dem das Ereignis auftrat. Dieser Name entspricht der Client-ID, falls das Ereignis von einem Prozess verursacht wurde, bzw. der Primär-ID, falls kein Identitätswechsel erfolgt. Bei Sicherheitsereignissen werden sowohl die Primär- als auch die Identitätswechselinformationen angezeigt, sofern dies möglich und sinnvoll ist.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Computer</p></td>
<td style="border:1px solid black;"><p>Der Name des Computers, auf dem das Ereignis eintrat.</p></td>
</tr>
</tbody>
</table>
  
Das Ereignisbeschreibungsfeld enthält verschiedene Informationen, die sich von Ereignis zu Ereignis unterscheiden können. Im in der obigen Abbildung verwendeten Beispiel mit Ereignis 680 enthält das Feld **Fehlercode:** den Wert **0xC000006A**, was auf ein inkorrektes Kennwort hinweist. Für jeden Ereignistyp werden in diesem Feld ereignisspezifische Informationen angezeigt.
  
Bei Windows-Sicherheitsereignisprotokollereignissen findet der Abschnitt mit den Binärdaten im Ereigniseintrag keine Anwendung.
  
###### Technische Aspekte
  
Bei der Implementierung eines Sicherheitsüberwachungs- und Angriffsermittlungssystems auf Basis der Windows-Sicherheitsereignisprotokollierung sind die folgenden Aspekte zu berücksichtigen:
  
-   **Bewältigung von hohen Sicherheitsereignisaufkommen**. Um die hohe Anzahl an generierten Sicherheitsereignissen zu bewältigen, muss genau überlegt werden, welche konkreten Sicherheitsüberwachungsereignisse zu verfolgen sind. Diese Erwägungen sind besonders bei der Überwachung des Datei- und Objektzugriffs wichtig, da bei beiden sehr umfangreiche Datenmengen erzeugt werden können.
  
-   **Speicherung und Verwaltung von Ereignisdaten in einer zentralen Datenbank**. Die Speicherung von Ereignisdaten kann je nach Konfiguration des Überwachungssystems mit Terabytes von Daten einhergehen. Dies ist der wichtigste Gesichtspunkt bei der Erwägung des Bedarfs für forensische Analysen. Im entsprechenden Abschnitt wird dies detailliert beschrieben.
  
-   **Identifizierung von und Reaktion auf Angriffssignaturen**. Um Muster von Aktivitäten zu erkennen, die auf einen Angriff hinweisen, muss die zuständige Person bzw. eine konfigurierte Abfrage in der Lage sein, die mit den Aktivitäten verbundenen Ereignisse, die in den Informationen enthalten sind, zu identifizieren. Es sollte ein Mechanismus vorhanden sein, der eine rechtzeitige und geeignete Reaktion auslöst, sobald eine verdächtige Aktivität erkannt wird.
  
-   **Unterbindung der Umgehung von Sicherheitsüberwachungskontrollen durch Mitarbeiter**. Mitarbeiter – und besonders Administratoren – mit umfassenden Berechtigungen in einem Netzwerk sollten zur Einschränkung des Zugriffs auf Überwachungsdaten so aufgeteilt werden, dass nur Sicherheitsexperten für die Verwaltung von Überwachungssystemen zuständig sind.
  
###### Lösungsplanung
  
Die folgenden Aktionen sollten vor der Implementierung eines Sicherheitsüberwachungs- und Angriffsermittlungssystems durchgeführt werden:
  
-   Überprüfen der aktuellen Sicherheitsüberwachungseinstellungen.
  
-   Bewerten der Administratorrollen und Aufgaben für normale Benutzer.
  
-   Überprüfen von Unternehmensrichtlinien und -verfahren.
  
-   Identifizieren von gefährdeten Systemen.
  
-   Auflisten von hochwertigen Anlagen.
  
-   Identifizieren vertraulicher oder verdächtiger Konten.
  
-   Auflisten genehmigter Programme.
  
Informationen zu Speicherungsanforderungen finden Sie im Abschnitt „Implementieren forensischer Analysen“ weiter unten.
  
###### Überprüfen der aktuellen Sicherheitsüberwachungseinstellungen
  
Unternehmen sollten ihre vorhandenen Sicherheitsüberwachungs- und Sicherheitsprotokolldateieinstellungen überprüfen, um eine Basis für in diesem Dokument empfohlene Änderungen zu schaffen. Derartige Überprüfungen sollten regelmäßig nach Implementierung einer Lösung durchgeführt werden und Aufschluss über Folgendes geben:
  
-   Aktuell vorhandene Sicherheitsüberwachungseinstellungen.
  
-   Die Ebene, für die diese Einstellungen gelten (lokaler Computer, Site, Domäne oder Organisationseinheit).
  
-   Aktuelle Protokolldateieinstellungen (Größenbeschränkungen und Verhalten bei Erreichen des Maximums).
  
-   Zusätzliche Sicherheitsüberwachungseinstellungen, die relevant sein könnten (z. B. Überwachung der Verwendung von Sicherungs- und Wiederherstellungsberechtigungen).
  
Die Informationen in „Anhang B: Implementieren von Gruppenrichtlinieneinstellungen“ am Ende dieses Dokuments können bei der Festlegung der aufzuzeichnenden Einstellungen behilflich sein. Weitere Informationen zu Sicherheitsüberwachungseinstellungen finden Sie im [*Windows Server 2003-Sicherheitshandbuch*](http://www.microsoft.com/germany/technet/datenbank/articles/900117.mspx) unter http://go.microsoft.com/fwlink/?LinkId=14845.
  
###### Bewerten der Administratorrollen und Aufgaben für normale Benutzer
  
Ein Schlüsselelement bei der Implementierung einer wirksamen Sicherheitsüberwachungslösung ist die Sicherstellung, dass Inhaber von Administratorkonten sowie deren Rollen und Zuständigkeiten bekannt sind. In den meisten Unternehmen sind z. B. Administratoren Mitglieder der Gruppe der Domänenadministratoren, damit sie neue Benutzerkonten in der Domäne einrichten können. Es kann jedoch in Unternehmensrichtlinien festgelegt sein, dass neue Konten nur über ein installiertes Bereitstellungssystem eingerichtet werden dürfen. In einer solchen Situation würde auf ein von einem Administratorkonto initiiertes Konteneinrichtungsereignis umgehend eine Untersuchung folgen.
  
Eine Bewertung von Benutzerkontoaufgaben ist normalerweise einfacher, da solche Konten typischerweise über erheblich weniger Zugriff auf Netzwerkressourcen verfügen als Administratorkonten. Da normale Benutzer beispielsweise üblicherweise keinen Zugriff auf das Dateisystem auf Computern im Netzwerkumkreis benötigen, ist die Überwachung der Aktivitäten dieser Benutzer auf solchen Servern kaum erforderlich.
  
###### Überprüfen von Unternehmensrichtlinien und -verfahren
  
Eine Überprüfung der Geschäftsprozesse und -verfahren ähnelt einer Bewertung der Administratorrollen und -zuständigkeiten, ist jedoch nicht darauf beschränkt. Wichtige Komponenten für eine derartige Überprüfung können z. B. die Untersuchung des Benutzereinrichtungsvorgangs und des Änderungssteuerungsprozesses sein. Die Untersuchung der Mechanismen für Genehmigungsprozesse und Überwachungspfade für alle Ereignisse in einem Netzwerk ist wichtig, um eine Korrelation zwischen genehmigten Überwachungsereignissen und möglichen Einbruchsversuchen herzustellen.
  
###### Identifizieren von gefährdeten Systemen
  
Gefährdete Systeme sind jene Computer und Geräte in einem Netzwerk, die mit der größten Wahrscheinlichkeit das Ziel von Angriffen und Zugriffsversuchen darstellen, bevor externe Angreifer eine andere Taktik ausprobieren. Typischerweise befinden sich solche Computer im Netzwerkumkreis, doch können auch interne Geräte angriffsgefährdet sein und sollten daher nicht völlig unbeachtet bleiben.
  
Anhand einer umfassenden Überprüfung gefährdeter Systeme sollte Folgendes sichergestellt werden:
  
-   Alle relevanten Sicherheitsupdates und Service Packs wurden angewendet.
  
-   Nicht benötigte Dienste und Benutzerkonten wurden deaktiviert.
  
-   Dienste sind so konfiguriert, dass sie nach Möglichkeit unter den Konten „Lokaler Dienst“ oder „Netzwerkdienst“ ausgeführt werden.
  
-   Die Notwendigkeit der Zugriffsebene für Dienste, für die eine Benutzerkontoanmeldung erforderlich ist, wird überprüft, besonders wenn solche Konten Administratorberechtigungen aufweisen.
  
-   Es wurden Richtlinienvorlagen für hohe Sicherheit angewendet.
  
**Hinweis**   Dieser Überprüfungsvorgang sollte nicht auf gefährdete Computer im Umkreis begrenzt werden. Es empfiehlt sich, alle Computer in einem Netzwerk in diese Überprüfungen einzuschließen.
  
Weitere Informationen über die Konfiguration zur sicheren Ausführung von Diensten finden Sie im [*Planungshandbuch für die Sicherheit von Diensten und Dienstkonten*](http://go.microsoft.com/fwlink/?linkid=41311) unter http://go.microsoft.com/fwlink/?LinkId=41311.
  
###### Auflisten von hochwertigen Anlagen
  
Die meisten Unternehmen haben wahrscheinlich bereits die hochwertigen Anlagen in ihren Netzwerken identifiziert, diese Informationen jedoch noch nicht durch Dokumentation und Angabe der vorhandenen Schutzeinrichtungen für jede Anlage formal in eine Unternehmensrichtlinie aufgenommen. So kann ein Unternehmen z. B. Access Control Lists (ACLs) und Verschlüsselung zur sicheren Speicherung vertraulicher Finanzdaten auf NTFS-Dateisystempartitionen nutzen. Eine Unternehmensrichtlinie sollte jedoch derartige Daten als geschützte Dateien kenntlich machen, auf die nicht autorisierte Benutzer und Administratoren nicht zugreifen dürfen, so dass sich die Administratoren und Benutzer über diese Einschränkung im Klaren sind.
  
Jegliche Änderungen an einer ACL, die zum Schutz solcher Dateien verwendet wird, sollten untersucht werden, besonders wenn Eigentumsänderungen auftreten, da solche Ereignisse auf unerlaubte Dateizugriffsversuche ohne entsprechende Autorisierung hinweisen können. Derartige Eigentumsänderungen treten eher selten auf, daher sollten sie nach erfolgter Identifizierung und Dokumentation hochwertiger Anlagen leicht zu erkennen sein.
  
###### Identifizieren vertraulicher oder verdächtiger Konten
  
Alle vertraulichen Konten sollten überprüft werden, um festzustellen, für welche Konten eine höhere Überwachungsstufe erforderlich ist. Solche Konten umfassen das standardmäßige Administratorenkonto, jegliche Mitglieder der Unternehmens-, Schema- oder Domänenadministratorengruppe sowie jegliche Konten, die von Diensten genutzt werden.
  
Neben vertraulichen Konten ist die Anpassung von Sicherheitsüberwachungsstufen für Konten von Einzelpersonen wichtig, die als Risiko gelten oder vermutlich an verdächtigen Aktivitäten teilnehmen. Weitere Informationen zur Anpassung der Überwachungsstufen für Einzelbenutzerkonten finden Sie im Abschnitt „Richtlinienverletzungen und Schwellen“ weiter unten in diesem Dokument.
  
###### Auflisten genehmigter Programme
  
Um Informationen über ein Netzwerk zu erlangen, muss ein Angreifer Programme auf Systemen ausführen, die sich innerhalb dieses Netzwerks befinden. Durch Einschränkung der Programme, die in einem Netzwerk ausgeführt werden dürfen, kann ein Unternehmen die Bedrohung durch externe Angriffe erheblich reduzieren. Um eine Liste der genehmigten Programme zu erstellen, sollte eine Überwachung aller Programme durchgeführt werden, die zurzeit genehmigt oder als in einer Netzwerkumgebung notwendig identifiziert worden sind. Jegliche bei dieser Überwachung entdeckten unbekannten Programme sind als verdächtig einzustufen und umgehend zu untersuchen. Microsoft Systems Management Server 2003 kann bei Softwareüberwachungen hilfreich sein, ist aber nicht erforderlich.
  
**Hinweis**   Es können einige Ausnahmen für bestimmte Computer wie z. B. Arbeitsstationen für Entwickler erforderlich sein, auf denen sich ausführbare Dateien in der Entwicklungsphase befinden können, die nicht auf der Liste der genehmigten Programme vorhanden sind. Ein sichererer Ansatz bestünde darin, dass Entwicklungs- und Testarbeiten ausschließlich in einer virtuellen Computerumgebung oder nur in einer isolierten Netzwerkdomäne stattfinden dürften.
  
##### Erkennen von Richtlinienverletzungen und Schwellen
  
Richtlinienverletzungen stellen die größte Kategorie von Sicherheitsproblemen dar, für die in einem Unternehmen Vorkehrungen getroffen werden müssen. Diese Vorfallsarten umfassen Folgendes:
  
-   Einrichtung von Benutzerkonten außerhalb des etablierten Prozesses
  
-   Unsachgemäße oder ungenehmigte Verwendung von Administratorberechtigungen
  
-   Verwendung von Dienstkonten für interaktive Anmeldungen
  
-   Versuche des Dateizugriffs über nicht autorisierte Benutzerkonten
  
-   Löschen von Dateien, auf die Benutzerkonten zugreifen dürfen
  
-   Installation und Ausführung von ungenehmigter Software
  
Die häufigste Art der Richtlinienverletzung besteht in unbeabsichtigten Benutzerzugriffsversuchen, z. B. Navigation zu eingeschränkten Verzeichnissen. Derartige Verletzungen sind normalerweise unerheblich, da dieses Problem durch Zugriffsbeschränkungen und geeignete Berechtigungsrichtlinien abgedeckt wird. Verwaltungsrichtlinienverletzungen stellen aufgrund des Wesens von Verwaltungsrechten den folgenschwersten Ereignistyp dar, egal, ob sie absichtlich oder unbeabsichtigt erfolgen.
  
Einzelpersonen, die zur Durchführung ihrer Aufgaben Administratorkontoberechtigungen benötigen und erhalten, verfügen über Systemzugriff in erheblichem Umfang. Solche Berechtigungen implizieren allerdings nicht deren Verwendbarkeit außerhalb des genehmigten Umfangs oder Prozesses. Die Möglichkeit, mit Administratorkonten Benutzerkonten einzurichten bzw. zu ändern, vertrauliche Daten einzusehen und Datenzugriffsrechte zu ändern, macht genaue Erwägungen hinsichtlich der Minderung des mit solchen umfassenden Funktionen verbundenen Risikos erforderlich.
  
###### Erstellen von Bedrohungsmodellen
  
Einige Bedrohungen lassen sich nachweislich durch Überwachungen mindern, andere wiederum nicht, und einige können durch Überwachungen gemindert werden, ohne dass dies eigentlich die Mühe wert wäre. Es ist wichtig zu verstehen, dass nicht jede Sicherheitsanfälligkeit auch eine Bedrohung für ein Netzwerk darstellt. Um festzustellen, welche Sicherheitsanfälligkeiten behoben werden können oder müssen, kann die Umsetzung der Bedrohungsmodellierungsprinzipien von Nutzen sein.
  
Die Bedrohungsmodellierung ist ein technisches Verfahren, mit dem Bedrohungen und Sicherheitsanfälligkeiten erkannt und wirksamere Gegenmaßnahmen im Kontext einer konkreten Umgebung ergriffen werden können. Dieses Verfahren umfasst im Allgemeinen drei grundlegende Schritte:
  
-   Hineinversetzen in die Sicht des Angreifers
  
-   Identifizieren des Sicherheitsprofils des Systems
  
-   Ermitteln und Einstufen der relevanten Bedrohungen
  
Die Untersuchung einer Netzwerkumgebung aus der Sicht eines Angreifers umfasst die Ermittlung, welche Ziele am aussichtsreichsten für jemanden sind, der Zugriff auf ein Netzwerk erhalten möchte, und welche Bedingungen für einen erfolgreichen Angriff auf solche Ziele erfüllt sein müssen. Wenn potenziell anfällige Ziele erkannt wurden, kann die Umgebung hinsichtlich der Auswirkung von vorhandenen Schutzeinrichtungen auf die Angriffsbedingungen untersucht werden. Dieser Vorgang gibt Aufschluss über relevante Bedrohungen, die sich daraufhin entsprechend ihrem Risikopotenzial, den wirksamsten Abhilfemaßnahmen für die jeweilige Bedrohung sowie dem Maß der möglichen positiven oder negativen Auswirkungen auf andere Bereiche, die Einfluss auf den Wert der Abhilfemaßnahme haben könnten, einstufen lassen.
  
Dementsprechend gibt es einige konkrete Schritte für eine erfolgreiche Netzwerkbedrohungsmodellierung, die auf diesen Anforderungen basieren:
  
1.  **Identifizieren wichtiger Anlagen**. Zur Ermittlung des geeignetsten Einsatzes von Sicherheitsressourcen gehört auch die Auflistung der Anlagen, die für den Geschäftsbetrieb von grundlegender Bedeutung sind. Dieser Vorgang sollte sowohl die Zuständigen für den Unternehmensprozess als auch für die Technologie einschließen, da beide Parteien relevante Ansichten darüber haben, welche Anlagen dem Unternehmen bei Kompromittierung Schaden zufügen könnten.
  
2.  **Erkennen möglicher Angriffspunkte**. Diese Erkennungsphase umfasst ebenfalls zwei unterschiedliche Perspektiven. Erstens ist es erforderlich, die Arten der Grenzen zu klassifizieren, innerhalb derer sich Daten im Netzwerk befinden können. Diese Grenzen gelten je nach dem potenziellen Schaden, der durch Offenlegung der entsprechenden Daten für den kritischen, vertraulichen oder öffentlichen Bereich entstehen könnte. Zweitens werden aus Technologieperspektive die Angriffspunkte anhand von Vektoren sowie Schwachpunkte, durch die Zugang zu kritischen und vertraulichen Anlagen ermöglicht werden könnte, untersucht. Die Kombination dieser Informationen kann dazu beitragen, Sicherheitsmaßnahmen auf solche Schwachpunkte zu konzentrieren, durch die auf kritische Daten zugegriffen werden könnte.
  
3.  **Erkennen tatsächlicher Bedrohungen**. Nachdem die kritischen Anlagen und potenziellen Zugriffspunkte erkannt wurden, kann eine Liste mit denkbaren schädlichen Angreiferaktionen angefertigt werden. Anhand dieser Liste lassen sich die Anstrengungen auf tatsächliche, konkrete Bedrohungen konzentrieren.
  
    Es können verschiedene Methoden zur Identifizierung tatsächlicher Bedrohungen verwendet werden. Das STRIDE-Modell ist eine Methode, mit der Bedrohungen auf Basis der verwendbaren Angriffsarten untersucht werden (Spoofing, unerlaubte Änderungen, Zurückweisung, Offenlegung von Informationen, DoS und Erhöhung von Berechtigungen). Es gibt noch weitere Varianten, etwa das Unterteilen von Bedrohungen nach logischen Ebenen (z. B. Netzwerk, Host und Anwendung). Jedes Unternehmen muss selbst entscheiden, welcher Ansatz in einer konkreten Umgebung am sinnvollsten ist.
  
4.  **Kategorisieren und Einstufen von Bedrohungen**. In diesem Schritt finden allgemeine Risikoabschätzungs- und Managementprinzipien Anwendung, anhand derer Bedrohungen auf Basis ihrer Verwendungswahrscheinlichkeit und ihrer potenziellen Auswirkungen auf ein Unternehmen eingestuft werden. Die verwendete Standardformel lautet:
  
    Risiko = Verwendungswahrscheinlichkeit x potenzielle Auswirkungen auf ein Unternehmen
  
    Für diesen Prozess stehen mehrere Methoden sowie verschiedene Hilfsmittel zur Verfügung, die die Risikoabschätzung unterstützen. Auf sie genauer einzugehen würde jedoch den Rahmen dieses Dokuments sprengen. Weitere Informationen zum Risikomanagement sowie zu diesen Methoden finden Sie im [*Leitfaden zum Sicherheitsrisikomanagement*](http://go.microsoft.com/fwlink/?linkid=30794) unter http://go.microsoft.com/fwlink/?linkid=30794.
  
5.  **Abhilfe und Neubewertung**. Nach Durchführung der bisherigen Schritte lässt sich eine Liste der tatsächlichen Bedrohungen erstellen, die sich auf das Unternehmen auswirken könnten, und diese Bedrohungen können entsprechend ihren Risiken für das Unternehmen eingestuft werden. Anhand solch einer Liste sind gezielte Abhilfemaßnahmen möglich, die wiederum hinsichtlich ihres Kosten-Nutzen-Verhältnisses bewertet werden sollten. Es können sich mehrere unterschiedliche Arten der Risikominderung als geeignet erweisen, von denen einige möglicherweise weitere Sicherheitsanfälligkeiten berücksichtigen, was dann zu einer weiteren Erhöhung der Effizienz derartiger Sicherheitsmaßnahmen führt.
  
Auch nach Umsetzung eines Abhilfeplans bleibt die Methode der Bedrohungsmodellierung ein iterativer Prozess, der in regelmäßigen Abständen und unter kontinuierlicher Neubewertung durchgeführt werden sollte, um sicherzustellen, dass Sicherheitsmaßnahmen so effektiv und umfassend wie möglich sind.
  
###### Hintergrunduntersuchungen und -überprüfungen
  
Die meisten Unternehmen überprüfen bereits in der einen oder anderen Form den Hintergrund potenzieller Mitarbeiter als Einstellungsvoraussetzung, nicht jedoch nach erfolgter Einstellung. Regelmäßige Hintergrundüberprüfungen während der Einstellung sollten in Betracht gezogen werden, insbesondere für wichtige Positionen, die mit Zugriff auf vertrauliche Daten einhergehen.
  
###### Richtlinienvereinbarungen zur Computernutzung
  
Computer- oder Netzwerknutzungsvereinbarungen informieren Mitarbeiter nicht nur über die zulässige Nutzung von Unternehmensanlagen, sondern auch über Richtlinien zur Überwachung von Netzwerkaktivitäten und Computernutzungen sowie über mögliche Folgen von Richtlinienverletzungen.
  
Die Vorgaben in Nutzungsrichtlinien stellen außerdem juristische Dokumente dar, sofern sie diese Aspekte explizit definieren und die Unterschrift eines Mitarbeiters als Bestätigung des Einverständnisses erfordern. Ohne den Beweis, dass sich ein Mitarbeiter über die internen Sicherheitsüberwachungsrichtlinien sowie die Erwartungen hinsichtlich der akzeptablen Nutzung von Unternehmensanlagen voll bewusst war, gestaltet sich die strafrechtliche Verfolgung von Missbrauch als schwierig.
  
Wichtig ist auch eine Warnung vor dem Zugriff und der ungenehmigten Nutzung an jedem Zugriffspunkt im Unternehmensnetzwerk, die jeden Benutzer beim Zugriffsversuch darüber informiert, dass es sich um ein privates Netzwerk handelt und alle nicht autorisierten Zugriffe verboten sind und strafrechtlich verfolgt werden. So kann in Windows-Betriebssystemen beispielsweise bei einem Anmeldungsversuch eine Warnung ausgegeben werden, die Benutzer darüber informiert, dass sie versuchen, Zugriff auf eine geschützte Unternehmensressource zu erlangen, und dass nicht autorisierte Zugriffe untersagt sind.
  
Die juristischen Aspekte hinsichtlich der genauen Formulierung und Verwendung solcher Dokumente sind zwar nicht Bestandteil dieses Dokuments, es ist jedoch wichtig, auf die Existenz derartiger Dokumente und Richtlinien hinzuweisen. Im Internet sind viele Beispiele für solche Nutzungs- und Zugriffsvorgaben vorhanden, diese Materialien sollten jedoch ausschließlich unter Einbeziehung qualifizierter Rechtsberater vorbereitet werden, da eine Vielzahl lokaler und internationaler rechtlicher Aspekte zu berücksichtigen sind.
  
###### Aufgabentrennung
  
So wie verschiedene Funktionalitäten für Systeme zu Zwecken der Sicherheit, Leistung und Verfügbarkeit über ein Netzwerk verteilt sind, ist auch eine Duplizierung und Trennung von Aufgaben bei der Ausarbeitung des Personalbedarfs für eine IT-Sicherheitsabteilung wichtig.
  
Wichtige Rollen, für die Zugriff auf oder Kontrolle über vertrauliche Daten und Systeme erforderlich ist, sollten redundant sein, wann immer dies möglich und sinnvoll ist. Dies dient nicht nur zur Vermeidung von Wissenslücken im Fall von Mitarbeiterausfall, sondern auch zur Bereitstellung einer Sicherheitsfunktion im Fall von interner Sabotage. Wenn z. B. nur ein Mitarbeiter die Administratorkennwörter kennt und dieser Mitarbeiter das Unternehmen verlässt, ohne die Kennwörter bekannt zu geben, ließe sich dieses Problem nur sehr schwer lösen.
  
Neben der Rollenredundanz ist auch die Trennung von kritischen Rollen besonders für die Sicherheitsüberwachung wichtig. Netzwerkverwalter sollten nicht gleichzeitig für die Überprüfung der Sicherheitsüberwachungsdaten zuständig sein, und das Sicherheitspersonal sollte über keine Berechtigungen verfügen, die mit denen der Administratoren übereinstimmen. Mitunter ist es zur weiteren Aufgabentrennung außerdem erforderlich, Administrationspersonal den Zugriff auf Abteilungsdaten zu verweigern. Einige Unternehmen verfügen beispielsweise über Organisationseinheiten mit eigenen Systemen oder Administratorkonten zum Schutz vertraulicher Daten wie Finanz- oder Personaldaten.
  
**Hinweis**   Es lässt sich mitunter nicht verhindern, dass Inhaber von Administratorkonten Möglichkeiten zur Umgehung der Aufgabentrennung finden, doch ist es wichtig, zumindest konkrete Richtlinien für die zulässige Verwendung für Administratoren unter Berücksichtigung der Aufgabentrennung aufzustellen.
  
###### Überprüfen der Sicherheitsüberwachungsfunktionalität
  
Das regelmäßige Testen einer Sicherheitsüberwachungslösung sollte bereits vor der Implementierung eines solchen Programms genau geplant werden. Zwar ist ein Anfangstest zur Überprüfung einer Sicherheitsüberwachungslösung wichtig, doch sollte darüber hinaus angesichts der sich ständig verändernden Sicherheitsumgebung ein Plan für regelmäßige Tests vorliegen.
  
Tests können Einbruchsversuche und die Verwendung von Administratorberechtigungen zur Überprüfung der Wirksamkeit der Erkennung solcher Aktivitäten umfassen. Es ist jedoch auch wichtig, Neuerungen bei Sicherheitsverfahren und Angriffsprofilen zu untersuchen, um den Änderungsbedarf zu ermitteln. Die Bedrohungen für Unternehmensnetzwerke unterliegen mit der Anpassung von Angreifern an Sicherheitseinrichtungen konstanten Veränderungen, so dass Schutzmechanismen und Überwachungsverfahren zur Wahrung ihrer Wirksamkeit ständig weiterentwickelt werden müssen.
  
###### Aufstellen von Prozessen
  
Um autorisierte Ereignisse von nicht autorisierten Sicherheitsereignissen zu trennen, muss ein Plan für eine etablierte und verbindliche Änderungssteuerung und für Problemverwaltungsprozesse aufgestellt werden. Durch solch einen Plan kann ein detaillierter Dokumentpfad bereitgestellt werden, der sich mit Sicherheitsprotokolldaten abgleichen lässt. Die Problemverfolgung ist in den meisten Unternehmen in Form von Helpdesk-Tickets oder Vorgängen üblich, doch wird die Änderungssteuerung häufig vernachlässigt. Sie stellt einen erforderlichen Mechanismus dar und lässt sich nicht nur zur Trendermittlung bei der Erkennung von problematischen Systemen oder Anwendungen, sondern auch als wichtiges Sicherheitsinstrument nutzen.
  
Änderungssteuerungsprozesse sollten als proaktives Verfahren gestaltet sein, während reaktive Änderungen auf die Verwendung eines Problemverwaltungsprozesses begrenzt werden sollten. Ein Änderungssteuerungsprozess sollte Einreich- und Genehmigungsvorgänge vor allen Änderungen vorsehen und folgende Angaben enthalten:
  
-   Name des Genehmigenden
  
-   Name des Implementierenden
  
-   Zeitrahmen für die Änderung
  
-   Gründe für die Änderung
  
-   Vorzunehmende Änderungen
  
-   Von der Änderung betroffene Systeme
  
-   Auswirkungen auf das Unternehmen
  
-   Tatsächliche Ergebnisse der Änderung
  
Weiterhin empfohlen wird ein Bereitstellungsprozess für Benutzer mit Verfahren zum Hinzufügen, Ändern und Löschen von Benutzern, anhand dessen außerdem ein Überwachungspfad zum Schutz gegen nicht autorisierte Kontoänderungen eingerichtet werden kann. Vor der Aufstellung eines solchen Prozesses ist es wichtig, eine Sicherheitsüberwachung der aktuellen Benutzerkonten durchzuführen, um deren Gültigkeit sowie in regelmäßigen Abständen die sich ändernde Liste zu überprüfen.
  
Die Verwendung von automatischen Benutzerbereitstellungs- und Identitätsverwaltungslösungen, z. B. Microsoft Identity Integration Server (MIIS) 2003, kann durch Automatisierung von Kontoänderungen und der mit solchen Aktivitäten verbundenen Prozesse ebenfalls nützlich sein. Bei Verwendung solcher Lösungen muss bedacht werden, dass Administratorkonten nach wie vor die Möglichkeit zur Erstellung neuer Konten bieten, dies jedoch nicht notwendig ist, da neue Konten durch etablierte Prozesse erstellt werden. Daher sollten alle mit der Kontoerstellung verbundenen Ereignisse, z. B. Ereignis 624, nur mit MIIS 2003 oder einem anderen etablierten Dienstkonto für die automatische Bereitstellung in Zusammenhang stehen.
  
Zwar wird in den Medien permanent über externe Bedrohungen für Unternehmensnetzwerke berichtet, doch lehrt die Erfahrung, dass Netzwerke und Unternehmensdaten viel häufiger durch Verlust oder infolge inkorrekter Konfigurationen bzw. Verfahrensfehler gefährdet werden. Ein Schutz ist sowohl vor externen als auch vor internen Bedrohungen erforderlich, und es gibt viele Anbieter, die Ihrem Unternehmen bei dieser Aufgabe helfen können. Niemand kann jedoch ein Paket anbieten, das die Fehler der für das Netzwerk und die Sicherheit zuständigen Personen verhindert. Die beste Art der Risikominderung besteht in der Implementierung und Umsetzung geeigneter Prozesse und Verfahren zu Änderungen, die im Netzwerk auftreten.
  
###### Definieren von sicherheitsrelevanten Reaktionen
  
Um den Schaden infolge einer Sicherheitsverletzung zu begrenzen, müssen ein definierter, geeigneter Schutzplan sowie Prozesse für die Reaktion auf Vorfälle ausgearbeitet werden. Vorfallsberichte, die Aufstellung eines Notfallteams und ein Protokoll für die Reaktion auf Notfälle sind gute Beispiele hierfür. Schnelle und wirksame Vorfallsreaktionen verbessern das Sicherheitsprofil eines Unternehmens und halten den tatsächlichen und den vermuteten Schaden eines Einbruchsversuchs in Grenzen.
  
Die Ausarbeitung eines etablierten Prozesses für sicherheitsrelevante Reaktionen hilft nicht nur bei der Schadensbegrenzung nach einem Vorfall, sondern dient auch durch die Benachrichtigung von Mitarbeitern und anderen Personen darüber, dass Sicherheitsverletzungen koordinierte und umgehende Reaktionen zur Folge haben werden, als Abschreckung.
  
###### Mitarbeiter
  
Viele Angriffe von internen Quellen ließen sich laut Untersuchungen vom CERT und des U.S. Secret Service verhindern, wenn Unternehmen ein größeres Bewusstsein hinsichtlich Verhaltensänderungen oder Drohungen von Mitarbeitern sowie Maßnahmen als Reaktion darauf aufweisen würden. Die wertvollsten Sicherheitsressourcen in einem Unternehmen sind die Mitarbeiter selbst, denn sie bemerken Verstimmungen bei Kollegen oder verdächtige Verhaltensweisen von Besuchern und können dies den zuständigen Stellen melden. Einer der ersten Schritte, die ein externer Dienst für die Sicherheitsüberwachung normalerweise durchführt, besteht dementsprechend darin, sich nach niedergeschriebenen Kennwörtern und ungesicherten Geräten umzusehen oder durch direktes Verbinden mit dem internen Netzwerk Einbruchsversuche zu unternehmen.
  
Das Personal eines Unternehmens kann eine wichtige „Schutzschicht“ gegen interne und externe Bedrohungen bilden. Richtlinien, die zum Melden von beunruhigenden Verhaltensweisen von Kollegen ermutigen, sowie die Sensibilisierung des Supportpersonals, alle Meldungen über ungewöhnliche Computeraktivitäten von Mitarbeitern ernst zu nehmen, können in erheblichem Maß zur Minderung von Einbruchsversuchen oder Malwarevorfällen beitragen. Internes Training stellt ebenfalls eine wichtige Methode zur Unterrichtung von Mitarbeitern über die Erkennung jener Arten von Computerverhalten dar, die gemeldet werden sollten. Training dient außerdem als eine Vorbeugungsmaßnahme gegen Social-Engineering-Angriffe.
  
##### Korrelieren von Sicherheitsrichtlinienverletzungen mit Überwachungsereignissen
  
Die Korrelation von Sicherheitsereignisdaten umfasst das Erfassen von Sicherheitsereignissen aus mehreren Systemen und die Aufbewahrung dieser Daten an sicherer zentraler Stelle. Nach der Korrelation von Sicherheitsdaten kann das zuständige Personal diese zentrale Datenbank analysieren, um Sicherheitsverletzungen oder externe Angriffe zu erkennen. Die Datenbank spielt nicht nur für forensische Analysen eine wichtige Rolle, sie ist auch ein Hilfsmittel zum Erkennen von Angriffen und Sicherheitsanfälligkeiten. Es gibt für diesen Zweck verschiedene Lösungen von Drittanbietern. Die folgenden Produkte und Tools von Microsoft unterstützen diese Notwendigkeit durch Korrelation von Sicherheitsereignisprotokollen und anderen Sicherheitsüberwachungsdaten in einer zentralen Datenbank.
  
###### EventCombMT
  
EventCombMT (Multithread) ist eine Komponente des [*Windows Server 2003-Sicherheitshandbuchs*](http://www.microsoft.com/germany/technet/datenbank/articles/900117.mspx), das unter http://go.microsoft.com/fwlink/?LinkId=14845 zur Verfügung steht. Mit diesem Tool können Ereignisse aus Ereignisprotokollen auf mehreren Computern analysiert und erfasst werden. Es wird als Multithread-Anwendung ausgeführt und erlaubt es dem Benutzer, beim Durchsuchen von Ereignisprotokollen beliebig viele Parameter festzulegen, beispielsweise:
  
-   Ereignis-IDs (einzeln oder mehrfach)
  
-   Ereignis-ID-Bereiche
  
-   Ereignisquellen
  
-   Konkreter Ereignistext
  
-   Ereignisalter in Minuten, Stunden oder Tagen
  
![](images/Cc875806.SMAAD4(de-de,TechNet.10).gif)
  
**Abbildung 4. EventCombMT**
  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875806.smaad4_big(de-de,technet.10).gif)  
Bestimmte Suchkategorien sind in EventCombMT integriert, z. B. Kontensperrungen (siehe Abbildung oben), wodurch Suchfunktionalität für die folgenden Ereignisse gegeben ist:
  
-   **529**. Anmeldefehler (Benutzername oder Kennwort ungültig)
  
-   **644**. Ein Benutzerkonto wurde automatisch gesperrt
  
-   **675**. Vorauthentifizierung auf einem Domänencontroller fehlgeschlagen (falsches Kennwort)
  
-   **676**. Fehlgeschlagene Anfrage für Authentifizierungsticket
  
-   **681**. Anmeldefehler
  
Ein sicherheitsrelevantes Ereignis, das nicht in der Sicherheitsprotokolldatei vorhanden ist, ist Ereignis 12294 aus der Systemprotokolldatei. Es ist wichtig, dieses Ereignis zu jeder Suche hinzuzufügen, da es zur Ermittlung von Angriffsversuchen verwendet werden kann, die gegen das Administratorkonto gerichtet sind. Es weist keine Sperrschwelle auf und stellt daher ein gefährdetes und interessantes Ziel für potenzielle Angreifer dar.
  
**Hinweis**   Ereignis 12294 wird in der Sicherheitskontenverwaltung (SAM) des Systemprotokolls, nicht jedoch im Sicherheitsprotokoll geführt.
  
EventCombMT kann Ereignisse in einer Microsoft SQL Server™-Datenbanktabelle speichern, was langfristige Speicherungen und Analysen ermöglicht. Nach der Speicherung in einer SQL Server-Datenbank kann auf die Daten der Ereignisprotokolle durch eine Vielzahl verschiedener Programme zugegriffen werden, z. B. SQL Query Analyzer, Microsoft Visual Studio® .NET und einige Dienstprogramme von Drittanbietern.
  
###### Log Parser 2.2
  
Log Parser ist ein kostenloses Tool von Microsoft, das für die Suche nach Daten in einem Protokoll, zum Hochladen von Protokollen in eine SQL-Datenbank oder CSV-Datei und zur Berichterstellung aus den Ereignisprotokollen, CSV-Dateien und anderen Protokollformaten (einschließlich IIS-Protokolle, für die das Tool ursprünglich konzipiert wurde) verwendet werden kann.
  
Dieses befehlszeilenbasierte Scripting-Tool kann als eine Ressource zur Korrelation von Ereignisprotokolldaten an zentraler Stelle, zur Analyse von bestimmten Ereignissen sowie zur Berichterstellung verwendet werden. Für die Scripting- und Befehlszeilenschnittstelle sind jedoch Detailinformationen erforderlich, die über den Rahmen dieses Dokuments hinausgehen. Weitere Informationen zu Log Parser, seiner Verwendung und zu Scripting-Ressourcen sind auf der Seite [Log Parser 2.2](http://www.microsoft.com/technet/scriptcenter/tools/logparser/default.mspx) unter www.microsoft.com/technet/scriptcenter/tools/logparser/default.mspx sowie im Artikel [How Log Parser 2.2 Works](http://www.microsoft.com/technet/community/columns/profwin/pw0505.mspx) (Funktionsweise von Log Parser 2.2; in englischer Sprache) unter www.microsoft.com/technet/community/columns/profwin/pw0505.mspx erhältlich.
  
###### EventQuery.vbs
  
EventQuery.vbs ist ein Tool, das mit Windows XP veröffentlicht wurde. Es kann zur Auflistung von Ereignissen und Ereigniseigenschaften aus einem oder mehreren Ereignisprotokollen verwendet werden. Zur Nutzung dieses Skripts muss der befehlsbasierte Skripthost (CScript.exe) ausgeführt werden. Wurde der standardmäßige Windows Script Host nicht auf CScript eingestellt, können Sie dies durch Ausführen des folgenden Befehls tun:
  
    Cscript //h:cscript //s //nologo
  
Dieses befehlszeilenbasierte Skriptdienstprogramm ist äußerst flexibel und kann eine Vielzahl verschiedener Parameter zur Anpassung der Filterung und des Formats für die Ausgabe verarbeiten. Weitere Informationen zur Verwendung dieses Tools und zu den verfügbaren Parametern finden Sie auf der Seite [Managing event logs from the Command Line](http://www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/event_commandline.mspx?mfr=true) (Ereignisprotokollverwaltung in der Befehlszeile; in englischer Sprache) in der Windows XP Professional-Produktdokumentation unter www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/event\_commandline.mspx?mfr=true.
  
###### Internetinformationsdienst-Protokollierung
  
Die in den Internetinformationsdiensten (IIS) verfügbaren zusätzlichen Protokollierungsfunktionen ermöglichen Berichte zur Identität, zu den Zugriffszielen sowie den Zugriffszeitpunkten von Website-Besuchern. IIS-Protokolle zeichnen erfolgreiche und fehlgeschlagene Zugriffsversuche auf Sites, virtuelle Ordner und Dateien auf und können zur selektiven Überwachung von Daten konfiguriert werden, um den Speicherbedarf zu minimieren und die Aufzeichnung unnötiger Daten zu vermeiden.
  
Die Speicherung dieser Protokolle erfolgt entweder im nativen Format als Datei, die daraufhin anhand einer der oben genannten Analyse- und Sortierungstools gefiltert werden kann, oder über die ODBC-Datenbankprotokollierung direkt an zentraler Stelle, wobei die Daten in einer SQL-Datenbank oder einer anderen ODBC-kompatiblen Datenbank gespeichert werden können.
  
Bestimmte Aktivitäten und Ereignisabfolgen wie die folgenden sollten genau beobachtet werden:
  
-   Mehrmals fehlgeschlagene Befehle zum Ausführen von ausführbaren Dateien oder Skripts.
  
-   Übermäßig viele fehlgeschlagene Anmeldeversuche über die gleiche IP-Adresse oder den gleichen IP-Adressbereich, was auf den Versuch eines DoS-Angriffs oder der Erhöhung von Berechtigungen hinweisen kann.
  
-   Fehlgeschlagene Zugriffs- oder Änderungsversuche bei .bat- oder .cmd-Dateien.
  
-   Nicht autorisierte Versuche, Dateien in einen Ordner hochzuladen, der ausführbare Dateien enthält.
  
Ab Windows Server 2003 weist IIS neue Überwachungsfunktionen auf, die entweder zusammen mit den neuen, direkt in der Ereignisanzeige integrierten Protokollierungsfunktionen in IIS verwendet werden können, oder auf die für angepasste Lösungen über ASP-Seiten zugegriffen werden kann. Weitere Informationen zu diesen Funktionen und deren Implementierung finden Sie in der IIS-Dokumentation.
  
###### Microsoft Internet Security & Acceleration Server
  
Microsoft Internet Security & Acceleration (ISA) Server ist ein erweitertes statusbehaftetes Paket und eine Firewall auf Anwendungsschicht mit zusätzlichen Funktionen wie VPN- und Proxyzwischenspeicherung.
  
Neben dem Dienstprogramm für aktiven Schutz bietet ISA eine Sicherheitsüberwachungsfunktion, die durch die Nutzbarkeit als zentralisiertes Protokollierungstool für die Überwachung aller im Umkreis eines Netzwerks auftretenden Aktivitäten gegeben ist. Die Protokollierungsfunktionen in ISA Server schließen die Möglichkeit ein, Firewallverkehr, Webproxyaktivitäten und SMTP-Nachrichtenüberwachungsprotokolle zu erfassen. Diese Protokolle können gefiltert, abgefragt und anhand der integrierten Protokollanzeige (siehe Abbildung unten) oder des Überwachungsdashboards in Echtzeit überwacht werden.
  
![](images/Cc875806.SMAAD5(de-de,TechNet.10).gif)
  
**Abbildung 5. Echtzeit-Protokollanzeige in Microsoft ISA Server 2004**
  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875806.smaad5_big(de-de,technet.10).gif)  
Neben der integrierten Protokollierungsfunktionalität verfügt ISA Server über eine Funktion, die Warnungen per E-Mail oder als Einträge im Ereignisprotokoll ausgeben und Dienste starten oder stoppen kann. Die Möglichkeit, verdächtige Aktivitäten in das Ereignisprotokoll aufzunehmen, ist in Hinblick auf das Thema dieses Dokuments besonders hilfreich. Mit ihr können Daten zu möglichen Angriffen aufgezeichnet und zusammen mit anderen Überwachungsereignisprotokolldaten an zentraler Stelle gespeichert werden.
  
Neben diesen Protokollierungs- und Warnfunktionalitäten steht ein integriertes Tool zur Einbruchserkennung zur Verfügung, das in ISA Server aktiviert werden kann. Diese grundlegenden Einbruchserkennungsdienste werden unter Lizenz von Internet Security Systems verwendet und umfassen mehrere Filter für IP-Pakete und DNS-Anwendungen sowie einen POP-Anwendungsfilter. Mit diesen Diensten lassen sich viele häufig auftretende Angriffe erkennen.
  
Die Einbruchserkennungsfunktionalität in ISA Server kann dafür verwendet werden, Ereignisse zu protokollieren und bei Erkennung potenzieller Angriffe Warnungen auszugeben. Sie kann außerdem Dienste oder verdächtige Verbindungen beenden. Zu den erkennbaren Angriffsprofilen gehören unter anderem:
  
-   WinNuke (Windows-Out-of-Band-Angriffe)
  
-   Land Attacks
  
-   IP-Half-Scan-Angriffe
  
-   UDP-Bombs
  
-   Portscans
  
-   DNS-Hostnamenüberlaufsangriffe
  
-   DNS-Zonentransfer von privilegierten oder hohen TCP/IP-Ports
  
Gleichgültig, ob ISA Server oder eine andere Firewall- und IDS-Lösung verwendet wird, ist es wichtig, das Umkreisnetzwerk (auch DMZ, Demilitarized Zone und überwachtes Subnetz genannt) beim Entwurf eines Sicherheitsüberwachungs- und Angriffsermittlungssystems zu berücksichtigen.
  
###### Microsoft Operations Manager 2005
  
Microsoft Operations Manager (MOM) überwacht mehrere Server in einer Unternehmensumgebung von zentraler Stelle aus. Der Microsoft Operations Manager-Agent erfasst Ereignisdaten aus den Ereignisprotokollen und überträgt sie an den MOM-Verwaltungsserver, der diese Ereignisdaten wiederum in die MOM-Datenbank aufnimmt. MOM 2005 und spätere Versionen können auch Ereignisdaten von Computern erfassen, auf denen keine MOM-Agents ausgeführt werden.
  
Die Management-Pack-Regeln von MOM werden zur Identifizierung von Problemen verwendet, die den wirksamen Serverbetrieb beeinträchtigen. Es können weitere Regeln zur Überwachung spezifischer Ereignisse eingerichtet werden, die bei Auftreten dieser Ereignisse Warnungen per E-Mail, Popupmeldung oder direkt auf Pagern ausgeben.
  
MOM enthält zwar eine Vielzahl nützlicher Funktionen für die Sicherheitsüberwachung und Angriffsermittlung, wurde aber ursprünglich nicht für diese Funktionalität konzipiert. Zukünftige Versionen von MOM werden verbesserte Sicherheitsprotokollierungsfunktionen aufweisen.
  
###### Microsoft Systems Management Server 2003
  
Mit Microsoft Systems Management Server (SMS) 2003 können Server und Arbeitsstationen in einem Netzwerk von zentraler Stelle aus überwacht und verwaltet werden. Es ist hauptsächlich für Verwaltungsaufgaben vorgesehen, kann aber auch wichtige sicherheitsrelevante Funktionen im Rahmen einer Sicherheitsüberwachungslösung bieten, da die Verteilung und Bekanntgabe von Sicherheitsupdates verwaltet bzw. alle nicht autorisierten Softwareinstallationen gemeldet werden können.
  
Die SMS-Bestandsaufnahmefunktionen können als zentralisierte Echtzeit-Bestandsverwaltungslösung dienen, was für jeden Sicherheitsüberwachungs- und Beobachtungsprozess wichtig ist, und dadurch eine Anforderung von Sicherheitsüberwachungslösungen erfüllen.
  
##### Implementieren forensischer Analysen
  
Die forensische Analyse ist ein eigenes Thema, dessen Umfang über den Rahmen dieses Dokuments hinausgeht. In diesem Dokument wird insbesondere der Versuch unterlassen, die Anforderungen für die Beweishandhabung bei forensischen Analysen oder forensische Daten, die nicht aus den Sicherheitsereignisprotokollen stammen, zu beschreiben.
  
Forensische Analysen eignen sich dazu, Zeitpunkt, Schweregrad und Folgen von Sicherheitsverletzungen zu erkennen und angegriffene Systeme zu identifizieren. Zur Gewährleistung der Nützlichkeit sind unter anderem die folgenden Informationen für forensische Analysen erforderlich:
  
-   Zeitpunkt eines Angriffs
  
-   Dauer eines Angriffs
  
-   Von einem Angriff betroffene Systeme
  
-   Während eines Angriffs erfolgte Änderungen
  
Aufgrund der schieren Anzahl an Detailinformationen, die nötig sind, um die Gesetzesgrundlagen für Beweisverfahren, die wichtigsten Datentypen für forensische Analysen, die für die Analyse erforderlichen Hilfsmittel, die Sammlung und Aufbewahrung von Beweisen und die forensischen Methoden zu verstehen, kann dieses Thema in diesem Dokument nicht behandelt werden. Auf diversen Websites, die Sicherheitsstudien gewidmet sind, stehen jedoch hervorragende Ressourcen zur Verfügung, z. B. das englischsprachige Dokument [First Responders Guide to Computer Forensics](http://www.cert.org/archive/pdf/frgcf_v1.3.pdf) von CERT unter www.cert.org/archive/pdf/FRGCF\_v1.3.pdf.
  
###### Geschäftliche Aspekte
  
Die Einplanung der Verwendung von forensischen Analysen unterscheidet sich von Ansätzen für andere Lösungen, da sie die Untersuchung von Vorfällen nach deren Eintreten anstelle einer Echtzeitanalyse von Vorfällen einschließt. Daher ist eine längerfristige detaillierte Ereignishistorie aus mehreren Systemen erforderlich. Aufgrund dieser zusätzlichen Notwendigkeit sollte ein wirksames System für forensische Analysen zentralisiert sein und über erhebliche Speicherkapazitäten zur Speicherung einer großen Anzahl von Datensätzen in einer geeigneten Datenbankstruktur verfügen.
  
Eine der Entscheidungen, die ein Unternehmen zur Schadensbegrenzung treffen muss, betrifft die Dauer der Aufbewahrung von derartigen Datensätzen für forensische Analysen sowie die Art des zu verwendenden Aufbewahrungszyklus. Solche Faktoren können große Auswirkung auf den Speicher- und Ausrüstungsbedarf eines Plans für forensische Analysen haben. Die folgende Tabelle zeigt Aufbewahrungszeiträume auf, die häufig in Unternehmen mit etablierten Plänen für forensische Analysen gelten.
  
**Tabelle 2. Speichergrenzen für forensische Analysen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Speicherungsfaktoren</p></th>
<th><p>Speichergrenzen</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Onlinespeicherung (Datenbank)</p></td>
<td style="border:1px solid black;"><p>21 Tage</p></td>
<td style="border:1px solid black;"><p>Bietet schnellen Zugriff auf Ereignisdetails</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Offlinespeicherung (Sicherung)</p></td>
<td style="border:1px solid black;"><p>180 Tage</p></td>
<td style="border:1px solid black;"><p>Sinnvolle Archivierungsdauer für die meisten Unternehmen</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Regulierte Umgebung</p></td>
<td style="border:1px solid black;"><p>7 Jahre</p></td>
<td style="border:1px solid black;"><p>Erforderliche Archivierungsdauer für regulierte Unternehmen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Geheimdienste</p></td>
<td style="border:1px solid black;"><p>Permanent</p></td>
<td style="border:1px solid black;"><p>Vorschrift für Geheimdienst- und Verteidigungseinrichtungen</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   In einigen regulierten Branchen (beispielsweise in Unternehmen, die medizinische Akten verwahren) werden zeitliche Einschränkungen eher als maximale Aufbewahrungsdauer statt als fester Zeitpunkt ausgedrückt.
  
Eine Option, die berücksichtigt werden kann, besteht in der Nutzung von Onlinedatenbanken zur Aufbewahrung forensischer Analysedaten und der Archivierung älterer Daten in einem besser komprimierbaren Format, z. B. als kommagetrennter Text (CSV-Datei), zur Offlinespeicherung. Bei Bedarf können CSV-Dateien zu Analysezwecken erneut in die Onlinedatenbank importiert werden.
  
Stellen Sie sicher, dass die gewählte Lösung den Unternehmensanforderungen einer umgehenden Untersuchbarkeit von Ereignissen einschließlich der zusätzlichen Möglichkeit der Wiederherstellbarkeit älterer Ereignisdaten für den Bedarfsfall gerecht wird. Eine Historie der Sicherheitsvorfälle in einem Unternehmen sowie eine Liste der verfügbaren Ressourcen dürften bei der Ausarbeitung eines Plans mit einer optimalen Abstimmung der Datenaufbewahrungsdauern für die Online- und Offlinespeicherung hilfreich sein. Testen Sie nach Möglichkeit das Ereignissammelsystem in einer relativ großen Datenbank anhand der gewünschten Berichte, und überprüfen Sie, ob die Berichte innerhalb eines sinnvollen Zeitrahmens ausgeführt werden und brauchbare Daten liefern.
  
Die Sicherheit der forensischen Analysedaten ist ebenfalls zu berücksichtigen, da der Zugriff auf diese Daten nur in seltenen Fällen erforderlich sein sollte. Ist der Zugriff erforderlich, sollte er ausschließlich einer geringen Anzahl vertrauenswürdiger Mitarbeiter des Sicherheitspersonals gewährt werden. Der Administratorzugriff auf diese Daten sollte im Rahmen eines etablierten Änderungssteuerungsprozesses, der zusätzliche Sicherheitsaufsicht bietet, streng geregelt werden. Es sollte keiner anderen Person möglich sein, auf diese Daten zuzugreifen, ihre Erfassung zu unterbinden oder sie zu ändern.
  
###### Technische Aspekte
  
Für die Planung einer Sicherheitsüberwachungslösung für forensische Analysen ist die Ermöglichung einer sicheren und zuverlässigen Erfassung und Speicherung einer sehr hohen Anzahl an Ereignissen erforderlich. Die Anforderungen für die Sicherheitsüberwachung ähneln denen anderer Lösungsszenarien, allerdings sind weitaus größere Ressourcen für die Datenbankspeicherung und für die effiziente Datenverwaltung erforderlich.
  
Im Folgenden finden Sie einige der technischen Herausforderungen, die zu berücksichtigen sind:
  
-   Zuverlässige und sichere Speicherung von Onlinedaten.
  
-   Bereitstellung von sehr hohen und leistungsstarken Datenträgerkapazitäten für die Onlinespeicherung.
  
-   Zuverlässige Sicherungssysteme für die Archivierung älterer Ereignisdaten.
  
-   Sichere Archivierungsverwaltungsprozesse.
  
-   Getestete Wiederherstellungsprozesse zum Datenabruf aus Sicherungen.
  
Diese Herausforderungen sollten nicht nur für die Sicherheitsüberwachung gelten, da Datenbankadministratoren ähnliche Bedürfnisse auch für andere Anwendungen haben, etwa für Onlinetransaktionsverarbeitungs- (OLTP-)Datenbanken. Im Gegensatz zu herkömmlichen Datenbankanwendungen wie OLTP muss eine Datenbank für forensische Analysen jedoch für sehr viel mehr Schreibvorgänge als Lesevorgänge geeignet sein.
  
###### Anforderungen
  
Zur Planung eines effektiven Programms für forensische Analysen müssen die folgenden Anforderungen berücksichtigt werden:
  
-   Korrekte Konfiguration der Sicherheitsprotokollierungseinstellungen.
  
-   Sichere Überprüfungsprozesse für Protokolleinträge liegen vor.
  
-   Es wurden ein sicherer und zentralisierter Sammelpunkt und ein Prozess für Sicherheitsprotokolle eingerichtet.
  
-   Zuverlässige Speicherung von Sicherheitsüberwachungsdaten.
  
-   Effektive Archivierungspläne und entsprechende Zeitpläne wurden ausgearbeitet.
  
Die Anforderungen, Möglichkeiten und gesetzlichen Vorschriften in einer Unternehmensumgebung sollten in jede Lösung für forensische Analysen einbezogen werden, da sich alle Unternehmen diesbezüglich unterscheiden.
  
#### Bereitstellen und Verwalten der Lösung
  
Das grundlegende Ziel jeder Sicherheitsüberwachungs- und Angriffsermittlungslösung besteht in der Identifizierung und Profilerstellung von Angriffen und einer geeigneten Reaktion auf sie. Daher befasst sich der größte Teil dieses Abschnitts mit einer detaillierten Beschreibung relevanter Ereignisse, deren Vorhandensein in einem Ereignisprotokoll auf momentan erfolgende Angriffe hinweisen könnte. In Anbetracht dieses Sachverhalts sollte ein Sicherheitsüberwachungs- und Angriffsermittlungsplan den folgenden Anforderungen genügen:
  
-   Erkennen von internen Richtlinienverletzungen
  
-   Erkennen von Angriffen aus externen Quellen
  
-   Ermöglichen effizienter und akkurater forensischer Analysen
  
Für die in diesem Dokument beschriebene Lösung werden ähnliche Komponenten für jede dieser drei Anforderungen verwendet. Die Implementierung von forensischen Analysefunktionen geht mit weiteren Anforderungen einher, die weiter unten beschrieben werden.
  
##### Sicherheitsüberwachung und Angriffsermittlung
  
Das Lösungskonzept für die Sicherheitsüberwachung und Angriffsermittlung erfordert die Planung geeigneter Sicherheitsüberwachungsstufen für die folgenden Aspekte:
  
-   Kontoverwaltung
  
-   Zugriff auf geschützte Dateien
  
-   Änderungen an Sicherheitsrichtlinien
  
-   Einrichten und Löschen von Vertrauensstellungen
  
-   Verwendung von Benutzerrechten
  
-   Systemneustarts und Zeitänderungen
  
-   Registrierungsänderungen
  
-   Ausführung unbekannter Programme
  
Das Sicherheitsüberwachungs- und Angriffsermittlungssystem erfasst Daten aus den Sicherheitsereignisprotokollen und sortiert sie an zentraler Stelle. Mit der Sicherheitsüberwachung betraute Personen können diese Daten daraufhin auf verdächtige Aktivitäten untersuchen. Darüber hinaus können diese Daten bei Bedarf für spätere forensische Analysen gespeichert und archiviert werden.
  
Ein wichtiger Bestandteil dieser Lösung ist die Möglichkeit, eine Funktion zur Überwachung einzelner Benutzer in Microsoft Windows 2003 mit Service Pack 1 (SP1) bzw. Microsoft Windows XP mit Service Pack 2 (SP2) zu konfigurieren. Diese Funktion ermöglicht die Festlegung unterschiedlicher Überwachungsstufen für bestimmte Benutzerkonten, wodurch sich strengere Überwachungen auf vertrauliche oder verdächtige Konten anwenden lassen.
  
###### Voraussetzungen für die Lösung
  
Für die Konfiguration dieser Sicherheitsüberwachungs- und Angriffsermittlungslösung gelten die folgenden Voraussetzungen:
  
-   Auf den Servern muss Windows Server 2003 SP1 oder höher ausgeführt werden, und sie müssen sich in einer Active Directory-Domäne befinden.
  
-   Auf Clientcomputern muss Windows XP SP2 oder höher ausgeführt werden, und sie müssen einer Active Directory-Domäne angehören.
  
**Hinweis**   Befinden sich die Computer im Unternehmensumkreis nicht in einer Domäne, können sie nicht anhand von Active Directory-Gruppenrichtlinieneinstellungen konfiguriert werden. Lokale Richtlinien und Vorlagen können jedoch für die Konfiguration solcher Systeme verwendet werden.
  
Schwerpunkt dieses Dokuments ist die Identifizierung charakteristischer Angriffssignaturen. Es spricht keine Empfehlungen für bestimmte Technologien zur Verwendung für die Sortierung von Sicherheitsereignissen aus. Es enthält dennoch eine Liste einiger möglicher Lösungen. Nachdem eine Entscheidung in Hinblick auf einen geeigneten Erfassungsmechanismus getroffen wurde, können die in diesem Dokument genannten Ereignisse und Ereignisabfolgen zum Entwurf von Abfragen und Warnungen zur Identifizierung von verdächtigem Verhalten genutzt werden.
  
##### Richtlinienverletzungen und Schwellen
  
Anhand neuer Funktionen, die in Microsoft Windows Server 2003 und Microsoft Windows XP mit SP2 verfügbar sind, können verschiedene Überwachungsstufen für einzelne Benutzerkonten angewendet werden. Überwachungsstufen können z. B. so eingestellt werden, dass ausschließlich Anmelde- und Abmeldeaktivitäten für alle Benutzer aufgezeichnet werden, während für einen bestimmten Benutzer sämtliche Aktivitäten überwacht werden. Die selektive Überwachung einzelner Benutzer lässt sich außerdem zur Reduzierung des Ereignisaufkommens im Sicherheitsprotokoll verwenden, indem einzelne Konten von der Überwachung bestimmter Aktivitäten ausgenommen werden. Mit dieser Funktion können nur Benutzerkonten überwacht werden, nicht jedoch Sicherheits- und Verteilungsgruppen. Konten der lokalen Administratorengruppe lassen sich nicht aus der selektiven Überwachungsmethode für einzelne Benutzer ausschließen.
  
Das zur Einstellung der Richtlinie zur selektiven Überwachung einzelner Benutzer unter Windows Server 2003 und Windows XP SP2 verwendete Befehlszeilendienstprogramm ist Auditusr.exe. Folgendes sind gültige selektive Überwachungskategorien:
  
-   Systemereignis
  
-   Anmeldung/Abmeldung
  
-   Objektzugriff
  
-   Rechteverwendung
  
-   Detaillierte Verfolgung
  
-   Richtlinienänderung
  
-   Kontoverwaltung
  
-   Verzeichnisdienstzugriff
  
-   Kontoanmeldung
  
Wird Auditusr.exe ohne Parameter auf der Befehlszeile ausgeführt, werden die aktuellen selektiven Überwachungseinstellungen angezeigt, die anfangs leer sind. Die Parameter können auf zwei Arten festgelegt werden: manuelle Eingabe von Befehlszeilenparametern für einzelne Benutzer oder Eingabe mehrerer Parameter durch Importieren einer entsprechenden Überwachungseinstellungsdatei.
  
Audituser.exe wird folgendermaßen verwendet:
  
    Audituser.exe /parameter useraccount:”kategorie”
  
(oder eine durch Kommata getrennte Liste von Kategorien).
  
Um beispielsweise die Fehlerüberwachung bei Systemereignissen und Anmelde-/Abmeldeereignissen des Kontos „LocalUser“ zu aktivieren, ist die folgende Befehlszeileneingabe erforderlich:
  
    Audituser /if LocalUser:”Systemereignis”,”An-/Abmeldung”
  
Die folgenden Parameter können in der Befehlszeile verwendet werden:
  
-   **/is** – Eintrag zum Erfolgseinschluss hinzufügen oder ändern
  
-   **/if** – Eintrag zum Fehlereinschluss hinzufügen oder ändern
  
-   **/es** – Eintrag zum Erfolgsausschluss hinzufügen oder ändern
  
-   **/ef** – Eintrag zum Fehlerausschluss hinzufügen oder ändern
  
-   **/r** – alle Überwachungseinträge für einzelne Benutzer für ein bestimmtes Benutzerkonto entfernen
  
-   **/ra** – alle Überwachungseinträge für einzelne Benutzer für sämtliche Benutzerkonten entfernen
  
-   **/e** – Einstellungen in die Datei mit dem angegebenen Namen exportieren
  
-   **/i** – Einstellungen aus der Datei mit dem angegebenen Namen importieren
  
Bei einer Überwachungseinstellungsdatei für einzelne Benutzer handelt es sich um eine reine Textdatei, für die das in der folgenden Abbildung dargestellte Format verwendet wird.
  
![](images/Cc875806.SMAAD6(de-de,TechNet.10).gif)
  
**Abbildung 6. Beispiel für eine Importdatei für Auditusr.exe**
  
**Hinweis**   Für einen erfolgreichen Import muss die Importdatei wie abgebildet mit der Zeile „Auditusr 1.0“ beginnen.
  
Zum Importieren der in der Abbildung oben dargestellten Überwachungseinstellungsdatei wäre daher die folgende Befehlseingabe erforderlich:
  
    Audituser /i path\audit.txt
  
Sie können dieses Dienstprogramm beim Festlegen von Schwellwerten für Überwachungsprotokollierungsdaten nutzen, wodurch sich der Speicherbedarf reduzieren und die Erkennungswahrscheinlichkeit bei Einbruchsversuchen erhöhen lässt.
  
##### Korrelation zwischen Sicherheitsrichtlinienverletzungen und Überwachungsereignissen
  
In diesem Abschnitt wird zwar nicht zwischen Richtlinienverletzungen aus externen oder internen Quellen unterschieden, doch ist zu beachten, dass interne Richtlinienverletzungen für ein Unternehmen genauso schädlich sein können wie externe Angriffe. Wie weiter oben bereits erwähnt, erfolgt ein hoher Prozentsatz böswilliger Angriffe aus internen Quellen, wobei unbeabsichtigte Schäden infolge der unangemessenen Verwendung von erhöhten Berechtigungen außerhalb etablierter Verfahren hierbei noch nicht eingeschlossen sind.
  
Aufgrund des mit der unbeabsichtigten oder absichtlichen Verwendung von erhöhten Berechtigungen durch interne Quellen verbundenen Risikos ist es wichtig, Richtlinien und Verfahren hinsichtlich der angemessenen Verwendung solcher Berechtigungen sowie Überwachungspfade für die Abgleichung einzurichten. Nach der Implementierung eines Änderungsmanagementprozesses und einer Dokumentationsrichtlinie kann eine Korrelation zum Abgleich von Überwachungsdaten mit genehmigten und nicht genehmigten Ereignissen entwickelt werden, wodurch sich ungewöhnliches Verhalten in einem Unternehmen leichter erkennen lässt. Dieser Abschnitt gibt Hilfestellung bei der Korrelation durch Beschreibung der unterschiedlichen Ereignistypen, die verfolgt werden können, und von deren Anwendbarkeit auf Richtlinien und Verfahren.
  
###### Nicht autorisiertes Zugreifen auf Computer
  
Bei Verwaltungs- und Supportpersonal nimmt die Verwendung von Remoteverwaltungseinrichtungen, z. B. Terminal Services, für die Verbindung mit und die Verwaltung von Remotesystemen kontinuierlich zu. Solche Systeme sollten auf interaktive Anmeldeversuche hin überwacht werden, und es sollte die Zulässigkeit jedes Verbindungsversuchs überprüft werden. Derartige Überprüfungen sollten die folgenden Vorgänge einschließen:
  
-   Identifizierung von Dienstkontoanmeldungen.
  
-   Aufzeichnung von Zugriffsversuchen durch nicht autorisierte Konten.
  
-   Untersuchung von Versuchen mit unerwartetem geografischen Ursprung.
  
-   Auflistung der Versuche aus externen IP-Adressbereichen.
  
Besondere Beachtung verdient hierbei die Überwachung hochwertiger Anlagen. Solche wichtigen Ressourcen sollten sich auf speziellen Servern befinden, die anhand strenger Überwachungs- und Zugriffskontrolleinstellungen konfiguriert wurden.
  
Die folgende Tabelle enthält eine Liste von Anmeldeüberwachungsereignissen, die bei Auftreten auf Systemen mit hochwertigen Anlagen mit Listen von autorisierten Konten verglichen werden sollte.
  
**Tabelle 3. Ereignisse im Zusammenhang mit nicht autorisierten Computerverwendungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>528</p></td>
<td style="border:1px solid black;"><p>Erfolgreiche Anmeldung</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie die Namen der Arbeitsstation und des Benutzerkontos. Vergewissern Sie sich, dass sich die Quellnetzwerkadresse innerhalb eines Netzwerks befindet.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>529</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – unbekannter Benutzername oder falsches Kennwort</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie, ob ein Anmeldungsversuch unternommen wurde, bei dem der Zielkontoname „Administrator“ lautet oder dem umbenannten standardmäßigen Administratorkonto entspricht. Überprüfen Sie außerdem, ob mehrere fehlgeschlagene Anmeldeversuche vorliegen, die unterhalb der Kontensperrungsschwelle liegen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>530</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Zeitbeschränkungen</p></td>
<td style="border:1px solid black;"><p>Dies weist auf einen Anmeldeversuch außerhalb des zulässigen Zeitrahmens hin. Überprüfen Sie den Namen des Benutzerkontos und der Arbeitsstation.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>531</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Das Konto ist zurzeit deaktiviert</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie den Namen des Zielkontos und der Arbeitsstation. Dieses Ereignis kann auf Einbruchsversuche von ehemaligen Benutzern hinweisen und sollte eine Untersuchung nach sich ziehen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>532</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Das angegebene Benutzerkonto ist abgelaufen</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie den Namen des Zielkontos und der Arbeitsstation. Dieses Ereignis kann auf Missbrauchsversuche von Mitarbeitern mit vertraglicher oder befristeter Anstellung hinweisen und sollte eine Untersuchung nach sich ziehen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>533</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Der Benutzer darf sich nicht an diesem Computer anmelden</p></td>
<td style="border:1px solid black;"><p>Dies weist darauf hin, dass ein Benutzer versucht, sich bei einer Arbeitsstation mit beschränktem Zugriff anzumelden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>534</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Anmeldetyp unzulässig</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie den Namen des Zielkontos und der Arbeitsstation sowie den Anmeldetyp. Dieses Ereignis weist auf einen fehlgeschlagenen Versuch einer interaktiven Anmeldung mit Dienstkontoberechtigungen hin, wenn Gruppenrichtlinieneinstellungen interaktive Anmeldungen bei solchen Kontos unterbinden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>535</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Das angegebene Kennwort des Kontos ist abgelaufen</p></td>
<td style="border:1px solid black;"><p>Dies weist darauf hin, dass ein Benutzer sich mit einem Konto anmelden möchte, dessen Kennwort abgelaufen ist. Eine Untersuchung kann erforderlich sein, wenn dies ohne entsprechende Kennwortänderung oder Supportanfrage wiederholt auftritt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>536</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Der Anmeldedienst ist nicht aktiv</p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass der NetLogon-Dienst aktiviert ist. Anderenfalls kann dieses Ereignis eine Untersuchung nach sich ziehen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>540</p></td>
<td style="border:1px solid black;"><p>Erfolgreiche Anmeldung</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis ist die Entsprechung von Ereignis 528 für Netzwerke.</p></td>
</tr>
</tbody>
</table>
  
###### Trojaner, Rootkits und Malware
  
Die Ereignis-ID 592 eignet sich besonders für die Erkennung von Trojanern, Rootkits und anderer Malware, da sie bei jedem Starten eines neuen Prozesses ausgegeben wird. Auf jedes Auftreten dieses Ereignisses sollte eine umgehende Untersuchung folgen, wenn der Bilddateiname keinem der Prozesse in einer Liste der genehmigten Programme entspricht.
  
Während Trojaner und Keylogger relativ leicht zu entdecken sind, sind Rootkits besonders gut verborgen. Sie können erkannt werden, indem nach unbekannten Programmen, die in schneller Abfolge gestartet und gestoppt werden, gesucht wird. Wenn ein Rootkit gestartet wird, kann das Betriebssystem es nicht entdecken und gibt daher auch keine weiteren Ereignisse aus.
  
Andere Malwareangriffe können in Form von E-Mail-Anhängen oder infizierten Websites erfolgen und mit dem Versuch einhergehen, Berechtigungen zu erhöhen, falls das ausführende Konto keine Berechtigung zum Starten neuer Programme aufweist. In solchen Fällen sollte die nicht autorisierte Software zu einem Fehlerereignis führen, das zu untersuchen ist, insbesondere bei Auftreten der folgenden Ereignisse:
  
-   **Prozesse werden als LocalSystem gestartet**. Prozesse, die als LocalSystem ausgeführt werden, sollten in einer Liste genehmigter Programme genau definiert sein. Sie können Prozesse wie Services.exe umfassen.
  
-   **Prozesse werden zu unerwarteten Zeitpunkten gestartet**. Werden auf dem überwachten System keine geplanten Batchprozesse verwendet, sollten bestimmte Aktivitäten (z. B. Sicherungen, CGI oder Skripts) bei Auftreten untersucht werden. In anderen Fällen sollte eine Untersuchung stattfinden, wenn die Ereignisse außerhalb der regelmäßig geplanten Batchzeitpunkte auftreten.
  
**Tabelle 4. Ereignis 592**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>592</p></td>
<td style="border:1px solid black;"><p>Ein neuer Prozess wird erstellt</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie die Einträge für den Bilddateinamen und den Benutzernamen darauf, ob ungenehmigte Prozesse oder unerwartete Startzeitpunkte vorliegen, oder ob unbekannte Programme in schneller Abfolge gestartet und gestoppt werden.</p></td>
</tr>
</tbody>
</table>
  
###### Zugreifen auf Ressourcen durch Änderung von Dateiberechtigungen
  
Mit Administratorberechtigungen kann auf Dateien zugegriffen werden, auf die der Zugriff normalerweise verweigert würde, wenn die Besitzrechte für die Daten geändert und dann die Konten zur Liste der Leseberechtigungen für die Daten hinzugefügt werden. Überdies ist es möglich, derartige Aktivitäten unter Windows Server 2003 zu verbergen, indem die Originaleinstellungen für die Besitzrechte und Berechtigungen wiederhergestellt werden.
  
Die Identifizierung von hochwertigen Anlagen und Daten ist diesbezüglich von Bedeutung, da die Implementierung von Objektzugriffsüberwachungen für jede Datei in einem üblichen Netzwerk von mittelgroßen Unternehmen aufgrund der schieren Anzahl der normalen, alltäglichen Zugriffsereignisse kontraproduktiv wäre. Die Objektzugriffsüberwachung sollte für vertrauliche Dateien und Ordner aktiviert werden. ACL-Einträge reichen für einen wirksamen Schutz vor nicht autorisierten Zugriffsversuchen nicht aus.
  
Zur effizienten Erkennung von unerlaubten Aktivitäten sollten die folgenden Fragen für alle hochwertigen Dateien einfach zu beantworten sein:
  
-   Welches Objekt war von einem Zugriffsversuch betroffen?
  
-   Welches Konto wurde zur Zugriffsanforderung verwendet?
  
-   Welches Konto hat den Zugriff autorisiert?
  
-   Welche Art von Zugriff wurde ausprobiert?
  
-   War das Ereignis erfolgreich, oder ist es fehlgeschlagen?
  
-   Welches System wurde für den Versuch verwendet?
  
Die integrierte Ereignisanzeige verfügt nicht über ausreichende Filtereinstellungen zur Klärung dieser Angaben. Daher ist EventCombMT oder ein anderer Mechanismus zur Durchführung dieser Analyse zu verwenden.
  
Die Objektzugriff-Überwachungsereignisse in der folgenden Tabelle betreffen derartige Versuche.
  
**Tabelle 5. Ereignisse in Verbindung mit Dateiberechtigungsänderungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>560</p></td>
<td style="border:1px solid black;"><p>Zugriff auf vorhandenes Objekt gewährt</p></td>
<td style="border:1px solid black;"><p>Weist auf eine erfolgreiche Zugriffsanforderung für ein Objekt hin. Überprüfen Sie die primäre Anmeldekennung, den Client-Benutzernamen und den Hauptbenutzernamen zur Ermittlung von nicht autorisiertem Zugriff. Überprüfen Sie im Feld für Zugriffe den Vorgangstyp. Mit diesem Ereignis werden nur Zugriffsanforderungen erkannt, nicht jedoch tatsächlich erfolgte Zugriffe.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>567</p></td>
<td style="border:1px solid black;"><p>Mit einem Handle verbundene Berechtigung verwendet</p></td>
<td style="border:1px solid black;"><p>Weist auf die erste Instanz einer Zugriffsart auf ein Objekt und die Änderung der Berechtigungen hin, falls das Zugriffsfeld „WRITE_DAC“ enthält. Korrelieren Sie dies durch Vergleich der Zielhandlefelder mit Ereignis 560.</p></td>
</tr>
</tbody>
</table>
  
###### Zugreifen auf Ressourcen durch Zurücksetzen von Kennwörtern
  
Kennwortänderungen sollten ausschließlich innerhalb eines genehmigten Rahmens etablierter Verfahren auftreten. Ordnungsgemäß konfigurierte Überwachungsstufen sollten die in der folgenden Tabelle aufgeführten Kontoverwaltungsereignisse aufzeichnen und diese mit aufgezeichneten Verfahren korrelieren, um Aktivitäten zu erkennen, die diesen Verfahren widersprechen.
  
**Tabelle 6. Ereignisse im Zusammenhang mit der Zurücksetzung von Kennwörtern**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>627</p></td>
<td style="border:1px solid black;"><p>Versuch, Kennwort zu ändern</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Kennwortänderungsanforderung hin, in der das Originalkennwort angegeben wurde. Vergleichen Sie den Hauptkontonamen mit dem Zielkontonamen, um festzustellen, ob es sich bei dem anfordernden Konto um das geänderte Konto handelt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>628</p></td>
<td style="border:1px solid black;"><p>Benutzerkontokennwort eingerichtet oder zurückgesetzt</p></td>
<td style="border:1px solid black;"><p>Weist auf die Zurücksetzung eines Kennworts über eine administrative Schnittstelle statt anhand eines Kennwortänderungsprozesses hin. Die Anforderung sollte von einem autorisierten Konto stammen, etwa einem Helpdesk-Konto oder einem Self-Service-Konto zum Zurücksetzen von Kennwörtern.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>698</p></td>
<td style="border:1px solid black;"><p>Kennwort für Wiederherstellungsmodus im Verzeichnisdienst geändert</p></td>
<td style="border:1px solid black;"><p>Weist auf einen Versuch hin, das Kennwort für den Wiederherstellungsmodus im Verzeichnisdienst auf einem Domänencontroller zu ändern. Überprüfen Sie die IP-Adresse der Arbeitsstation und den Kontonamen. Dieses Ereignis rechtfertigt eine umgehende Untersuchung.</p></td>
</tr>
</tbody>
</table>
  
###### Benutzerkontoänderung
  
Jede Kontoänderung, -hinzufügung und -löschung sollte in Einklang mit einem etablierten Prozess erfolgen, der einen Geschäftslogikprozess aus mehreren Schritten vorsieht und durch eine offizielle Anforderung von einem Mitarbeiter auf Managementebene initiiert wird. Alle Ereignisse in der folgenden Tabelle sollten einer offiziellen Kontoänderungsanforderung entsprechen oder eine umgehende Untersuchung nach sich ziehen.
  
**Tabelle 7. Ereignisse im Zusammenhang mit Benutzerkontoänderungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>624</p></td>
<td style="border:1px solid black;"><p>Benutzerkonto wird erstellt</p></td>
<td style="border:1px solid black;"><p>Weist auf die Einrichtung eines Netzwerkkontos hin.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>630</p></td>
<td style="border:1px solid black;"><p>Benutzerkonto wird gelöscht</p></td>
<td style="border:1px solid black;"><p>Weist auf die Löschung eines Netzwerkkontos hin.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>642</p></td>
<td style="border:1px solid black;"><p>Benutzerkonto wird geändert</p></td>
<td style="border:1px solid black;"><p>Weist auf sicherheitsrelevante Benutzerkontoänderungen hin, die nicht durch die Ereignisse 627 bis 630 abgedeckt sind.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>685</p></td>
<td style="border:1px solid black;"><p>Benutzerkontoname wird geändert</p></td>
<td style="border:1px solid black;"><p>Weist auf die Änderung eines Benutzerkontonamens hin.</p></td>
</tr>
</tbody>
</table>
  
Zur wirksamen Erkennung von Kontoverwaltungsproblemen sollten Abfragen für folgende Aufgaben konfiguriert werden:
  
-   Auffinden irregulärer oder ungewöhnlicher Kontoaktivitäten.
  
-   Identifizieren von Konten auf Administratorebene, mit denen Berechtigungen zum Einrichten und Ändern von Konten missbraucht werden.
  
-   Aufdecken von Mustern bei Kontoaktivitäten, die außerhalb der Sicherheitsrichtlinie des Unternehmens auftreten.
  
Die Bestätigung der Intervalle zwischen Kontoerstellung, erstmaliger Anmeldung und Kennwortänderung ist ebenfalls wichtig. Falls mit der Verwendung eines neuen Kontos nicht innerhalb eines festgelegten Zeitrahmens begonnen wird (üblicherweise wird der erwartete Verwendungsbeginn durch einen neuen Benutzer beim Kontoeinrichtungsprozess aufgezeichnet), sollte das Konto deaktiviert und eine Untersuchung hinsichtlich des Grunds für die Verzögerung eingeleitet werden.
  
###### Gruppenmitgliedschaftsänderungen
  
Merkmal einer guten Sicherheitspraxis ist die Berücksichtigung des Prinzips der geringsten Berechtigungen, d. h. der Gewährung der geringsten Zugriffsrechte, die für die ordnungsgemäße Durchführung der Funktionen eines Kontos benötigt werden. Bei Anwendung dieser Praxis gehören die meisten Konten zur standardmäßigen Gruppe der Domänenbenutzer mit zusätzlichen Mitgliedschaften in unternehmensspezifischen Sicherheitsgruppen.
  
Änderungen bei der Zugehörigkeit zu Sicherheitsgruppen sollten nur im Rahmen etablierter Richtlinien auftreten, besonders wenn Konten mit erhöhten Berechtigungen betroffen sind. Solche Änderungen sollten ausschließlich von etablierten, für die Kontoverwaltung verwendeten Konten durchgeführt werden, und die damit verbundenen Ereignisse sollten mit einem etablierten Prozess für derartige Änderungen korrelieren. Jegliche Änderungen, die außerhalb dieses Prozesses auftreten, sollten eine umgehende Untersuchung nach sich ziehen.
  
Die Kontoverwaltungsüberwachungsereignisse in der folgenden Tabelle beziehen sich auf Änderungen bei der Gruppenzugehörigkeit.
  
**Tabelle 8. Ereignisse im Zusammenhang mit Gruppenzugehörigkeitsänderungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>631, 632,<br />
633, 634</p></td>
<td style="border:1px solid black;"><p>Geänderte globale Gruppe mit aktivierter Sicherheit</p></td>
<td style="border:1px solid black;"><p>Stellen Sie im Feld mit dem Zielkontonamen fest, ob eine globale Gruppe geändert wurde oder die Gruppe über weit gefasste Zugriffsberechtigungen verfügt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>635, 636,<br />
637, 638</p></td>
<td style="border:1px solid black;"><p>Geänderte lokale Gruppe mit aktivierter Sicherheit</p></td>
<td style="border:1px solid black;"><p>Stellen Sie im Feld mit dem Zielkontonamen fest, ob die Gruppe der Administratoren, Server-Operatoren oder Sicherungs-Operatoren geändert wurde.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>639, 641,<br />
668</p></td>
<td style="border:1px solid black;"><p>Geänderte Gruppe mit aktivierter Sicherheit</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Änderung an einer Gruppe hin, bei der es sich nicht um eine Löschung, Erstellung oder Zugehörigkeitsänderung handelt. Stellen Sie anhand des Zielkontonamens sicher, dass keine Gruppe mit hohen Berechtigungen geändert wurde.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>659, 660, 661, 662</p></td>
<td style="border:1px solid black;"><p>Geänderte universelle Gruppe mit aktivierter Sicherheit</p></td>
<td style="border:1px solid black;"><p>Stellen Sie anhand des Zielkontonamens sicher, dass keine Gruppe mit hohen Berechtigungen, z. B. Organisations-Admins, geändert wurde.</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   Die Zugehörigkeit zu Verteilungsgruppen geht nicht mit dem Zugriff auf Netzwerkressourcen einher, da es sich hierbei nicht um Sicherheitsprinzipien handelt. Die Zugehörigkeit zu bestimmten Verteilungsgruppen kann jedoch je nach Gruppe zu Sicherheitsproblemen führen. Die Unterbringung von Benutzerkonten z. B. in einer verwaltenden oder ausführenden Verteilungsgruppe könnte etwa dazu führen, dass der Benutzer E-Mails erhält, die nicht für seine Position gedacht sind.
  
###### Nicht autorisierte Kontoverwendungsversuche
  
Durch die Heraufstufung des ersten Active Directory-Domänencontrollers in einer Gesamtstruktur wird ein Administratorkonto eingerichtet, das sowohl der Gruppe der Domänenadministratoren als auch der der Organisations-Admins angehört. Für dieses Konto ist besonderer Schutz erforderlich, da es das einzige Konto ist, das nicht von Kontensperreinstellungen betroffen ist. Daher bleibt dieses Konto auch bei vorhandener Kontensperrrichtlinie besonders anfällig für Wörterbuchangriffe.
  
Eine effektive Sicherheitsüberwachung sollte in der Lage sein, sämtliche Anmeldungsversuche mit einem Administratorkonto zu erkennen, selbst wenn es umbenannt wurde. Weitere Informationen zur Erhöhung der Sicherheit bei Administratorkonten finden Sie im [*Planungshandbuch für die Sicherheit von Administratorkonten*](http://www.microsoft.com/germany/technet/datenbank/articles/900353.mspx) unter http://go.microsoft.com/fwlink/?LinkId=41315.
  
Darüber hinaus können Anmeldungsversuche mit deaktivierten oder abgelaufenen Konten darauf hinweisen, dass ein ehemaliger oder befristet angestellter Mitarbeiter oder ein Subunternehmer ohne aktuell gültige Anmeldeinformationen versucht hat, auf das Netzwerk zuzugreifen. Solche Ereignisse sollten umgehende Untersuchungen nach sich ziehen.
  
Die folgende Tabelle bietet eine Übersicht über Ereignisse, die mit nicht autorisierter Kontoverwendung verbunden sind. Sie gehören zu den Kategorien der Kontoanmeldungen und der Anmeldeüberwachungen.
  
**Tabelle 9. Nicht autorisierte Anmeldeereignisse**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>528</p>
<p>540</p></td>
<td style="border:1px solid black;"><p>Anmeldungserfolg</p></td>
<td style="border:1px solid black;"><p>528 ist ein häufig auftretendes Ereignis. Das Ereignis 540 sollte hingegen eine Untersuchung des Zielkontonamens nach sich ziehen, um festzustellen, ob es vom standardmäßigen Administratorkonto ausgelöst wurde.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>529</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – unbekannter Benutzername oder unbekanntes Kennwort</p></td>
<td style="border:1px solid black;"><p>Es sind stets Untersuchungen durchzuführen, wenn der Zielkontoname „Administrator“ lautet oder dem umbenannten standardmäßigen Administratorkonto entspricht. Untersuchen Sie außerdem, ob Anmeldefehler knapp unterhalb der Sperrschwelle liegen. Des Weiteren ist zu überprüfen, ob für Versuche mit „Administrator“ oder „root“ als Zielkontoname und bei unbekanntem Domänennamen durchgeführt wurden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>531</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – deaktiviertes Konto</p></td>
<td style="border:1px solid black;"><p>Untersuchen Sie den Namen des Zielkontos und der Arbeitsstation zur Ermittlung der Quelle. Dieses Ereignis sollte eine Untersuchung hinsichtlich eines möglichen Einbruchsversuchs von ehemaligen Kontobenutzern nach sich ziehen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>532</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – abgelaufenes Konto</p></td>
<td style="border:1px solid black;"><p>Untersuchen Sie den Namen des Zielkontos und der Arbeitsstation zur Ermittlung der Quelle. Dieses Ereignis sollte eine Untersuchung hinsichtlich eines möglichen Einbruchsversuchs von ehemaligen Kontobenutzern nach sich ziehen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>576</p></td>
<td style="border:1px solid black;"><p>Besondere Rechte bei neuer Anmeldung</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Rechtezuweisung hin, mit der ein neues Konto Administratorberechtigungen oder die Möglichkeit zur Änderung des Überwachungspfads erhalten kann. Vergleichen Sie das Feld mit der Anmeldekennung mit Ereignis 528 oder 540, um auf einfache Art festzustellen, ob ein Konto Administratorberechtigungen erhalten hat.</p></td>
</tr>
</tbody>
</table>
  
Ein weiteres Sicherheitsproblem in Verbindung mit der nicht autorisierten Verwendung von Anmeldeinformationen entsteht aus der Anwendung vorhandener Kennwortrichtlinien, z. B. hinsichtlich sicherer Kennwörter und kürzerer Kennwortgültigkeitsdauern. Gelegentlich halten Benutzer ihre Kennwörter schriftlich oder auf andere Art fest, um sie nicht zu vergessen. Dieses Problem wird besonders in Umgebungen deutlich, die mehrere Identitätsspeicher ohne Identitätsverwaltungsdienste aufweisen und die Verwendung mehrerer Kennwörter und Konten erfordern.
  
**Hinweis**   Informationen zur Kennwortverwaltung in heterogenen Umgebungen erhalten Sie in der [Identitäts- und Zugriffsverwaltungsserie](http://go.microsoft.com/fwlink/?linkid=14841) unter http://go.Microsoft.com/fwlink/?LinkId=14841.
  
Unternehmen müssen Vorkehrungen dafür treffen, dass Benutzer ihre Kennwörter nicht aufzeichnen, vor allem nicht auf sichtbare Weise, da nicht autorisierte Personen sie einsehen und mit ihnen Angriffe durchführen könnten. Anhand der Informationen in der Tabelle weiter oben kann diese Einbruchsart überwacht werden, wobei allerdings ein Abgleich dieser Informationen mit einer Historie erfolgreicher Anmeldungen für das fragliche Benutzerkonto erforderlich ist, damit eine Liste der Arbeitsstationen mit häufigem Zugriff durch das Konto zu Vergleichszwecken erstellt werden kann.
  
**Hinweis**   Benutzerkonten können anhand integrierter Active Directory-Funktionalität auf bestimmte Arbeitsstationen beschränkt werden. Zur Nutzung dieser Funktionalität muss das Netzwerk jedoch NetBIOS-Namen unterstützen, die beispielsweise aus dem WINS- (Windows Internet Naming Service-)Dienst kommen.
  
###### Interaktive Anmeldung mit Dienstkontoberechtigungen
  
Beim Starten von Diensten müssen Anmeldeinformationen angegeben werden. Mitunter kann für bestimmte Dienste die Verwendung eines Domänenkontos erforderlich sein, um sie auszuführen oder Verbindungen zu Remotecomputern herzustellen. Für einige Dienste kann eine Administratoranmeldung notwendig sein, oder sie müssen auch mit dem Desktop interagieren.
  
Unter Windows Server 2003 und höher können einige Dienstkonten (z. B. der Warndienst) mit dem Switch **–LocalService** gestartet werden. Darüber hinaus kann für Dienste, für die Netzwerkkonnektivität benötigt wird, das Netzwerkdienstkonto NT AUTHORITY\\Network Service verwendet werden. Für alle Dienste, für die Benutzerkonten erforderlich sind, sollte sichergestellt werden, dass die verwendeten Konten durch sichere Kennwörter geschützt sind. Die Sicherheitsüberwachung sollte gewährleisten, dass Anmeldeereignisse mit solchen Konten nur beim Start von verbundenen Diensten auftreten. Weitere Informationen zur erhöhten Sicherheit für Dienstkonten finden Sie im [*The Services and Service Account Security Planning Guide*](http://go.microsoft.com/fwlink/?linkid=41311) (Planungshandbuch für die Sicherheit von Diensten und Dienstkonten; in englischer Sprache) unter http://go.Microsoft.com/fwlink/?LinkId=41311.
  
Das größte Sicherheitsrisiko im Zusammenhang mit Dienstkonten besteht, wenn Anmeldungen interaktiv statt als Dienst erfolgen. Solche Ereignisse treten nur auf, wenn ein Angreifer ein Dienstkonto manipuliert hat und sich über dieses Konto anmeldet. Sofern das kompromittierte Dienstkonto Administratorberechtigungen hat, hat der Angreifer umfangreichen Zugriff und kann normale Netzwerkdienste unterbrechen.
  
Alle Ressourcen, auf die dieses Dienstkonto zugreifen kann, müssen identifiziert werden und dürfen keine ungeklärten Berechtigungen für den Zugriff auf hochwertige Daten aufweisen. Für ein Dienstkonto kann beispielsweise gelegentlich Schreibzugriff auf ein Protokolldateiverzeichnis erforderlich sein, doch ist dies im Allgemeinen nicht der Fall. Dienstkonten, die mit dem Desktop interagieren können, verdienen ebenfalls besondere Beachtung, da sie Angreifern größere Möglichkeiten für Missbrauch bieten.
  
Die folgende Tabelle enthält Kontoanmeldungs- und Anmeldeüberwachungsereignisse, die auf nicht autorisierte Verwendungen von Dienstkontoanmeldeinformationen hinweisen.
  
**Tabelle 10. Ereignisse im Zusammenhang mit Anmeldungen anhand von Dienstkontoanmeldeinformationen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>528</p></td>
<td style="border:1px solid black;"><p>Anmeldungserfolg – Konsolenangriff oder Terminaldienste</p></td>
<td style="border:1px solid black;"><p>Weist auf einen erfolgenden Angriff hin, sofern das Ereignis mit Anmeldetyp 10, einem Dienstkonto oder dem lokalen Systemkonto verbunden ist. Auf dieses Ereignis sollte umgehend eine Untersuchung folgen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>534</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Anmeldetyp unzulässig</p></td>
<td style="border:1px solid black;"><p>Weist auf einen fehlgeschlagenen Versuch der interaktiven Anmeldung mit Dienstkontoanmeldeinformationen hin, wenn dies gemäß Gruppenrichtlinieneinstellungen untersagt ist. Überprüfen Sie bei Auftreten dieses Ereignisses den Namen des Zielkontos und der Arbeitsstation sowie den Anmeldetyp.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>600</p></td>
<td style="border:1px solid black;"><p>Prozess wurde ein primäres Token zugewiesen</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass ein Dienst ein benanntes Konto für die Anmeldung bei einem System verwendet, auf dem Windows XP oder später ausgeführt wird. Korrelieren Sie dies zur Untersuchung mit Informationen der Ereignisse 672, 673, 528 und 592.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>601</p></td>
<td style="border:1px solid black;"><p>Dienstinstallationsversuch durch Benutzer</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis sollte in einer Unternehmensumgebung mit klar definierter Richtlinie für akzeptable Anwendungen und einem Systemstandardisierungsprozess nur selten auftreten. Es sollte eine Untersuchung nach sich ziehen, wenn Änderungssteuerungsprozesse in solchen Umgebungen nicht korrelieren.</p></td>
</tr>
</tbody>
</table>
  
###### Nicht autorisierte Programmausführung
  
Mit Konten auf Administratorebene können Programme installiert und ausgeführt werden, weshalb sie normalerweise nur vertrauenswürdigen Mitarbeitern mit einem Bedarf an solchen erhöhten Berechtigungen zugewiesen werden. Aufgrund der mit ungetesteter Software verbundenen Risiken ist es wichtig, eine Liste mit genehmigter und lizenzierter Software zusammenzustellen und einen Prozess für die Anforderung, das Testen und die Genehmigung neuer Anwendungen einzurichten. Ungenehmigte Anwendungen sind auf eine isolierte Testumgebung zu begrenzen und sollten außerhalb eines etablierten Änderungssteuerungsprozesses nicht in einer Produktionsnetzwerkumgebung installiert werden. Sie sollten auf jeden Fall nur nach Aufnahme in eine Liste der genehmigten Software zugelassen werden.
  
Die folgende Tabelle enthält Prozessverfolgungsereignisse, mit denen die Verwendung nicht autorisierter Programme erkannt werden kann.
  
**Tabelle 11. Ereignisse im Zusammenhang mit der Ausführung nicht autorisierter Programme**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>592</p></td>
<td style="border:1px solid black;"><p>Ein neuer Prozess wird erstellt</p></td>
<td style="border:1px solid black;"><p>Weist auf die Erstellung eines neuen Prozesses hin. Untersuchen Sie die Felder für den Bilddateinamen und den Benutzernamen, und vergleichen Sie sie mit der Liste der genehmigten Programme, sofern eine etablierte Richtlinie für zulässige Programme im Unternehmen vorhanden ist. Suchen Sie außerdem nach Instanzen, bei denen eine Eingabeaufforderung mit LocalSystem aufgerufen wird, da dies eine geläufige Methode zur Umgehung eines Überwachungspfads darstellt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>602</p></td>
<td style="border:1px solid black;"><p>Eingeplanter Auftrag wird erstellt</p></td>
<td style="border:1px solid black;"><p>Untersuchen Sie den Zielnamen und den Zeitpunkt der Aufgabe, wenn solche Ereignisse zu unerwarteten Zeitpunkten auftreten.</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   Mit Sicherheitsüberwachungen zur Prozessverfolgung können nicht autorisierte Programme erkannt werden. Bei der Prozessverfolgung werden jedoch mehrere Sicherheitsprotokolleinträge erstellt, so dass darauf zu achten ist, dass die Anzahl der Ereignisse die Sicherheitserkennungsmechanismen nicht überfordert.
  
###### Nicht autorisierter Ressourcenzugriff
  
Die folgende Tabelle mit Objektzugriff-Überwachungsereignissen betrifft Zugriffsversuche auf Ressourcen, die ein Benutzer nicht verwenden darf.
  
**Tabelle 12. Ereignisse im Zusammenhang mit nicht autorisierten Ressourcenzugriffsversuchen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>560</p></td>
<td style="border:1px solid black;"><p>Zugriff auf vorhandenes Objekt verweigert</p></td>
<td style="border:1px solid black;"><p>Ermitteln Sie anhand des Objektnamenfelds, auf welche Ressource zugegriffen wurde, und korrelieren Sie die Felder für den Hauptbenutzernamen und die primäre Domäne oder die Felder für den Client-Benutzernamen und die Client-Domäne, um die Quelle zu ermitteln.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>568</p></td>
<td style="border:1px solid black;"><p>Versuch der Erstellung einer festen Verbindung zu einer überwachten Datei</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass ein Benutzer oder Programm versucht hat, eine feste Verbindung zu einer Datei oder einem Objekt herzustellen. Mit einer vorhandenen festen Verbindung kann ein Konto ohne Überwachungspfaderstellung eine Datei manipulieren, sofern das Konto über Rechte für das Objekt verfügt.</p></td>
</tr>
</tbody>
</table>
  
###### Verwendung nicht autorisierter Betriebssysteme
  
Die Verwendung nicht autorisierter Betriebssysteme kann zu erheblichen Problemen führen, die von reduziertem Schutz durch Ausnutzung von Sicherheitsanfälligkeiten bis zur gestiegenen Wahrscheinlichkeit der Datenbeschädigung auf Dateisystemen reichen können. Administratoren und Benutzer können nicht autorisierte Betriebssysteme folgendermaßen in ein Netzwerk einbringen:
  
-   Über PCs mit lokaler oder Remoteverbindung zum Netzwerk.
  
-   Durch Verwendung von über CD gestarteten Betriebssystemen.
  
-   Durch Neuinstallation eines Windows-Betriebssystems.
  
-   Durch Verwendung von Virtual PC-Images.
  
In Unternehmensrichtlinien kann festgelegt werden, wie Benutzer von Remotestandorten über ein VPN-Netzwerk oder den RAS-Dienst die Verbindung zu einem Netzwerk herstellen können. Dies kann Anforderungen für die Verbindung von Systemen, z. B. die Art des Betriebssystems, Updateversion und die Installation von Schutzeinrichtungen wie persönliche Firewalls und Antivirensoftware einschließen. Weitere Informationen zur Sicherstellung der Einhaltung von Unternehmenssicherheitsrichtlinien durch Remotesysteme finden Sie im Artikel [*Planungshandbuch zur Implementierung von Quarantänediensten mit Microsoft Virtual Private Network (VPN)*](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/quarantineservices/default.mspx) unter www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/quarantineservices/default.mspx.
  
Benutzer können auch Windows XP-Installations-CDs beim Neustarten ihrer Computer zur Installation eines nicht verwalteten Betriebssystems verwenden. Derartige Aktivitäten können erkannt werden, indem nach Anmeldeversuchen anhand eines Administratorkontos mit einem nicht identifizierten Arbeitsgruppennamen oder dem standardmäßigen Arbeitsgruppennamen gesucht wird.
  
**Hinweis**   Einige Open-Source-Distributionen können von CD gestartet werden, wodurch das Betriebssystem ohne Installation auf einem lokalen System verwendet werden kann. Da das Betriebssystem nicht tatsächlich auf dem lokalen Computer installiert wird, lassen sich solche Aktivitäten nur schwer erkennen. Anmeldeversuche über ein Benutzerkonto mit dem Namen „root“ in einer homogenen Netzwerkumgebung oder unter Verwendung unerwarteter Computernamen können jedoch auf das Vorhandensein eines nicht autorisierten Betriebssystems hinweisen. Derartige Aktivitäten lassen sich unterbinden, indem die Funktion zum CD-Start in den BIOS-Einstellungen eines Computers deaktiviert und die BIOS-Konfiguration danach kennwortgeschützt wird. Diese Vorgehensweise kann in einigen Umgebungen jedoch nicht praktikabel sein.
  
Virtual PC-Images bieten eine umfassende Emulation einer Computerumgebung auf einem Hostcomputer. Diese Emulation führt ein eigenes Betriebssystem mit eigenen Computernamen, Benutzerkonten, Verzeichnisdienststrukturen und Programmen in einer virtuellen Umgebung aus. Eine Virtual PC-Instanz kann darüber hinaus unabhängig vom Hostsystem gestartet, ausgeführt und gestoppt werden und wird daher wahrscheinlich keinerlei Überwachungsereignisse auf dem Hostcomputer erzeugen. Neben den Möglichkeiten eines virtuellen Computers der Verbindungsherstellung mit dem Netzwerk des Hosts, des IP-Adressabrufs und der Zuordnung zu freigegebenen Laufwerken stellen die oben genannten Fähigkeiten Sicherheitsrisiken dar, die von unsicherem Kennwortschutz bis zu erhöhter Sicherheitsanfälligkeit reichen können, da sie wahrscheinlich keinem auf dem Netzwerk vorhandenen Updateprozess unterliegen. Angesichts der Risiken in Verbindung mit virtuellen PCs ist es wichtig, die Verwendung von Software für virtuelle PCs auf autorisiertes Personal zu beschränken und Prozesse hinsichtlich der Erstellung und Verwendung von virtuellen PC-Instanzen zu dokumentieren.
  
Zur Ermittlung von nicht autorisierten Betriebssystemverwendungen muss es mit einer Sicherheitsüberwachungslösung möglich sein, Folgendes zu erkennen:
  
-   Unerkannte Benutzerkonten, Computernamen, Arbeitsgruppen oder Domänennamen.
  
-   Doppelte IP-Adressen oder solche außerhalb des zulässigen Bereichs.
  
-   Anmeldeversuche mit dem standardmäßigen Administratorkonto.
  
Die Prozessverfolgungsereignisse in der folgenden Tabelle können zur Ermittlung der Verwendung nicht autorisierter Betriebssysteme genutzt werden.
  
**Tabelle 13. Ereignisse im Zusammenhang mit der Verwendung nicht autorisierter Plattformen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>529</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – unbekannter Benutzername oder unbekanntes Kennwort</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie, ob Versuche mit „Administrator“ oder „root“ als Zielkontoname oder mit unbekanntem Domänennamen durchgeführt wurden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>533</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Benutzeranmeldung bei diesem Computer unzulässig</p></td>
<td style="border:1px solid black;"><p>Dies weist darauf hin, dass ein Benutzer versucht, sich bei einer Arbeitsstation mit beschränktem Zugriff anzumelden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>592</p></td>
<td style="border:1px solid black;"><p>Ein neuer Prozess wird erstellt</p></td>
<td style="border:1px solid black;"><p>Stellen Sie anhand der Felder für den Bilddateinamen und den Benutzernamen sicher, dass das Programm für die vorliegende Verwendung durch das fragliche Konto autorisiert ist.</p></td>
</tr>
</tbody>
</table>
  
###### Erstellen oder Aufheben von Vertrauensstellungen
  
Durch Vertrauensstellungen können Konten in einer Domäne auf Ressourcen in einer anderen Domäne zugreifen. Die Erstellung von Vertrauensstellungen ist sicherlich kein routinemäßiger Vorgang und sollte ausschließlich im Rahmen eines etablierten Änderungssteuerungsprozesses erfolgen. Auch das Aufheben von Vertrauensstellungen stellt eine Aktivität dar, die nur nach erfolgter Genehmigung im Rahmen eines Änderungssteuerungsprozesses und nach sorgfältiger Erwägung der Auswirkungen auf das Netzwerk erfolgen sollte.
  
Die Richtlinienänderung-Überwachungsereignisse in der folgenden Tabelle dienen zur Identifizierung von Vertrauensstellungsaktivitäten.
  
**Tabelle 14. Ereignisse im Zusammenhang mit der Änderung von Vertrauensstellungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>610<br />
611<br />
620</p></td>
<td style="border:1px solid black;"><p>Vertrauensstellung mit anderer Domäne wurde erstellt, aufgehoben oder geändert</p></td>
<td style="border:1px solid black;"><p>Diese Ereignisse werden auf dem Domänencontroller generiert, mit dem die Vertrauensstellung erstellt wurde. Dieses Ereignis sollte eine umgehende Untersuchung nach sich ziehen, sofern es nicht mit einem etablierten Anforderungsprozess zur Änderungssteuerung korreliert. Ermitteln Sie anhand des Felds für den Benutzernamen das anfordernde Konto.</p></td>
</tr>
</tbody>
</table>
  
###### Nicht autorisierte Sicherheitsrichtlinienänderungen
  
Änderungen an genehmigten Sicherheitsrichtlinieneinstellungen sollten ausschließlich im Rahmen eines etablierten Änderungssteuerungsprozesses erfolgen. Alle außerhalb dieses Genehmigungsprozesses erfolgenden Änderungen sollten eine sofortige Untersuchung nach sich ziehen.
  
Diese Art der Sicherheitsrichtlinienänderung umfasst Folgendes:
  
-   Gruppenrichtlinieneinstellungen
  
    -   Benutzerkontokennwortrichtlinie
  
    -   Benutzerkontensperrrichtlinie
  
    -   Überwachungsrichtlinie
  
    -   Ereignisprotokolleinstellungen, die für das Sicherheitsereignisprotokoll gelten
  
    -   IPsec-Richtlinie
  
    -   Richtlinien für drahtlose Netzwerke (IEEE 802.1x)
  
    -   Richtlinien für öffentliche Schlüssel und EFS (Encrypting File System)
  
    -   Richtlinien für Softwareeinschränkungen
  
-   Sicherheitseinstellungen
  
    -   Einstellungen für Benutzerrechte
  
    -   Benutzerkontokennwortrichtlinie
  
    -   Sicherheitsoptionen
  
Die vorstehende Liste weist lediglich Mindestanforderungen aus, da die meisten Unternehmen mit großer Wahrscheinlichkeit weitere Gruppenrichtlinieneinstellungen in ihrer Umgebung vornehmen. Anhand von Sicherheitsüberwachungen müssen sowohl erfolgreiche als auch fehlgeschlagene Einstellungsänderungsversuche erkannt werden können, da erfolgreiche Versuche von Konten vorgenommen werden sollten, die im Rahmen eines etablierten Prozesses zu solchen Änderungen berechtigt sind.
  
Die folgende Tabelle enthält Richtlinienänderung-Überwachungsereignisse, mit denen Änderungen an Gruppenrichtlinien und lokalen Systemrichtlinien erkannt werden können.
  
**Tabelle 15. Ereignisse im Zusammenhang mit Richtlinienänderungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>612</p></td>
<td style="border:1px solid black;"><p>Überwachungsrichtlinie wird geändert</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass eine Änderung an einer Überwachungsrichtlinie vorgenommen wurde. Diese Ereignisse sollten mit einer etablierten Änderungssteuerungsrichtlinie korreliert werden, um deren Legitimität zu ermitteln.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>613<br />
614<br />
615</p></td>
<td style="border:1px solid black;"><p>IPsec-Richtlinie wird geändert</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Änderung der IPsec-Richtlinie hin. Sollte untersucht werden, wenn dies nicht während eines Systemstarts auftritt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>618</p></td>
<td style="border:1px solid black;"><p>Richtlinie zur Wiederherstellung verschlüsselter Daten</p></td>
<td style="border:1px solid black;"><p>Diese Ereignisse treten bei Vorhandensein einer Richtlinie zur Wiederherstellung verschlüsselter Daten auf. Jedes Auftreten außerhalb festgelegter Richtlinien sollte eine Untersuchung nach sich ziehen.</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   Weitere Informationen zu Gruppenrichtlinieneinstellungen finden Sie im Abschnitt [Security Policy Settings](http://technet2.microsoft.com/windowsserver/en/library/bcd7ea4c-f989-4cee-969a-920f62f555111033.mspx?mfr=true) (Sicherheitsrichtlinieneinstellungen; in englischer Sprache) unter http://technet2.microsoft.com/WindowsServer/en/library/bcd7ea4c-f989-4cee-969a-920f62f555111033.mspx?mfr=true.
  
###### Versuchte Kompromittierung von Anmeldeinformationen
  
Um an Anmeldeinformationen von Benutzerkonten zu kommen, können Angreifer verschiedene Ansätze nutzen, die von Wörterbuchangriffen bis zu Social Engineering reichen. Die bekannteste Vorgehensweise sind Wörterbuchangriffe gegen einzelne Konten, während eine weitere geläufige Variante in der Anwendung einer Reihe von Kennwörtern auf alle Konten in einer Verzeichnisdienstdatenbank besteht. Im zweiten Fall ist es wahrscheinlich, dass der Angreifer entweder Zugriff auf die Verzeichnisdatenbank eines Unternehmens hat oder dass er Vermutungen zur Benutzernamensnomenklatur angestellt hat und über eine Liste der Mitarbeiter verfügt. Um derartige Angriffe zu erkennen, müssen mehrere Anmeldefehlschläge bei mehreren Konten nachgewiesen werden können, auch wenn keine Kontensperrungsschwellen überschritten werden.
  
Durch Zurücksetzen von Kennwörtern kann ebenfalls Zugriff auf Kontoanmeldeinformationen erlangt werden. Da das Zurücksetzen von Kennwörtern und Änderungsvorgänge sowohl bei Erfolg als auch bei einem Fehlschlag das gleiche Ereignis generieren, kann ein Angreifer unentdeckt bleiben, indem er die Kontensperrrichtlinie umgeht. Um dies zu vereiteln, muss eine Sicherheitsüberwachungslösung in der Lage sein, mehrfache Kennwortänderungen oder -rücksetzungen zu erkennen, insbesondere solche, die außerhalb etablierter Richtlinien und Geschäftsprozesse erfolgen.
  
Der Versuch eines Benutzers, Richtlinien zur erneuten Nutzung eines Kennworts anhand eines Skripts zu umgehen, das mehrere Kennwörter nacheinander zurücksetzt, bis das Originalkennwort erneut verwendet werden darf, stellt keinen Angriff dar, kann aber eine Beeinträchtigung der Sicherheitsvorkehrungen bedeuten. Während solcher Versuche entspricht die Anzahl der zurückgesetzten Kennwörter ungefähr der Kennwort-Neunutzungsschwelle und wird daher als eine schnelle Abfolge des Ereignisses 627 angezeigt. Durch die Implementierung von Richtlinien hinsichtlich der Mindestgültigkeitsdauer von Kennwörtern können derartige Versuche unterbunden werden.
  
Die folgende Tabelle enthält eine Auflistung von Ereignissen, die infolge von Angriffsversuchen auf Authentifizierungsinformationen auftreten können, wobei sie jedoch auch während des normalen Netzwerkbetriebs möglich sind, z. B. wenn zugelassene Benutzer ihre Kennwörter vergessen.
  
**Tabelle 16. Ereignisse im Zusammenhang mit Angriffen auf Authentifizierungsinformationen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>529</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – unbekannter Benutzername oder unbekanntes Kennwort</p></td>
<td style="border:1px solid black;"><p>Überprüfen Sie, ob Versuche mit dem Zielkontonamen „Administrator“ oder eines anderen Kontos auf Administratorebene vorliegen, die nicht zur Änderung von Kennwörtern berechtigt sind. Überprüfen Sie, ob mehrere fehlgeschlagene Anmeldeversuche vorliegen, die unterhalb der Sperrschwelle liegen. Korrelieren Sie Ereignis 529 mit Ereignis 539, um Muster kontinuierlicher Kontensperrungen zu erkennen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>534</p></td>
<td style="border:1px solid black;"><p>Anmeldung fehlgeschlagen – Anmeldetyp unzulässig</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass ein Benutzer sich mit einem nicht zugelassenen Kontotyp anmelden wollte, z. B. einem Netzwerk-, interaktiven, Batch- oder Dienstkonto. Überprüfen Sie die Felder für Zielkontonamen, Arbeitsstationsnamen und Anmeldetyp.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>539</p></td>
<td style="border:1px solid black;"><p>Konto gesperrt</p></td>
<td style="border:1px solid black;"><p>Weist auf einen Anmeldeversuch mit einem Konto hin, das gesperrt wurde. Korrelieren Sie dies mit Ereignis 529, um Muster kontinuierlicher Sperrungen zu erkennen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>553</p></td>
<td style="border:1px solid black;"><p>Wiedergabeangriff entdeckt</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass ein Authentifizierungspaket (normalerweise Kerberos) einen Anmeldeversuch durch Wiedergabe der Anmeldeinformationen eines Benutzers erkannt hat. Obwohl dieses Ereignis ein Zeichen für eine inkorrekte Netzwerkkonfiguration sein kann, sollte es eine umgehende Untersuchung nach sich ziehen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>627</p></td>
<td style="border:1px solid black;"><p>Versuch, Kennwort zu ändern</p></td>
<td style="border:1px solid black;"><p>Weist darauf hin, dass ein Kennwortänderungsversuch von jemandem durchgeführt wurde, der nicht der Inhaber des betroffenen Kontos ist, wenn das Feld für den Hauptkontonamen nicht mit dem Feld für den Namen des Zielkontos übereinstimmt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>628</p></td>
<td style="border:1px solid black;"><p>Benutzerkontokennwort eingerichtet oder zurückgesetzt</p></td>
<td style="border:1px solid black;"><p>Diese Aktivität sollte auf autorisierte Konten beschränkt sein, z. B. ein Helpdesk-Konto oder ein Self-Service-Benutzerkonto zum Zurücksetzen von Kennwörtern.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>644</p></td>
<td style="border:1px solid black;"><p>Benutzerkonto automatisch gesperrt</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Kontensperrung infolge der Anzahl aufeinander folgender, fehlgeschlagener Anmeldeversuche hin, die den Kontensperrgrenzwert überschritten hat. Korrelieren Sie dies mit den Ereignissen 529, 675, 681 und 676 (nur Windows 2000 Server). Siehe auch den Eintrag für Ereignis 12294 in dieser Tabelle.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>675</p></td>
<td style="border:1px solid black;"><p>Vorauthentifizierung fehlgeschlagen</p></td>
<td style="border:1px solid black;"><p>Weist auf ein mögliches Problem in Zusammenhang mit der zeitlichen Synchronisierung oder Computerkonten hin, die nicht korrekt mit der Domäne verbunden sind. Korrelieren Sie dies mit Ereignis 529, um den genauen Grund für die fehlgeschlagene Anmeldung zu ermitteln.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>12294</p></td>
<td style="border:1px solid black;"><p>Kontensperrungsversuch</p></td>
<td style="border:1px solid black;"><p>Weist auf einen möglichen Brute-Force-Angriff auf das standardmäßige Administratorkonto hin. Da Kontensperrrichtlinien nicht für dieses Konto gelten, wird dies als SAM-Ereignis 12294 im Systemereignisprotokoll aufgezeichnet. Jedes Vorkommen dieses Ereignisses sollte eine sofortige Untersuchung nach sich ziehen, da es auf die Verwendung eines nicht autorisierten Betriebssystems hindeuten kann. Überprüfen Sie das Feld für den Domänennamen auf unbekannte Domänen.</p></td>
</tr>
</tbody>
</table>
  
###### Ausnutzung von Sicherheitsanfälligkeiten
  
Sicherheitsanfälligkeiten sind das Hauptziel von Angreifern bei Einbruchsversuchen, da sie auf jedem Computer vorliegen können und da zu deren Behebung Zeit- und Arbeitsaufwand erforderlich ist. Die Dauer zwischen der Entdeckung von Sicherheitsanfälligkeiten und der Ausarbeitung einer Ausnutzungsmöglichkeit hat immer mehr abgenommen, was bedeutet, dass auch immer weniger Zeit zum Entwickeln, Testen und Verteilen von Patches für diese Sicherheitsanfälligkeiten zur Verfügung steht.
  
Die beste Verteidigung gegen die Ausnutzung von Sicherheitsanfälligkeiten ist nach wie vor ein wirksamer Patchverwaltungsprozess zum schnellen Testen und Verteilen von Sicherheitsupdates in einer Umgebung. Einige Dienste, die hierbei behilflich sein können, sind Microsoft Systems Management Server (SMS) 2003 und Windows Software Update Service (WSUS).
  
Die Sicherheitsüberwachung auf Umkreisnetzwerken ist diesbezüglich ebenfalls sehr wichtig, da Computer dort Angreifern die besten Angriffsmöglichkeiten bieten. Ohne vorhandene Mechanismen zur sofortigen Erkennung von Angriffen ist sich ein Unternehmen möglicherweise gar nicht über Missstände bewusst, bis das Netzwerk tatsächlich kompromittiert ist. Daher ist es äußerst wichtig, dass Computer im Umkreisnetzwerk hinsichtlich einer breiten Palette von Überwachungsereignissen sorgfältig beobachtet werden.
  
Zusätzlich zu den bereits erwähnten Ereignissen umfassen die beachtenswertesten Ereignisse im Abschnitt „Versuchte Kompromittierung von Anmeldeinformationen“ nicht autorisierte Zugriffsversuche und Berechtigungsidentitätsverwendungen. Die folgende Tabelle enthält einige Ereignisse zur Erkennung solcher Angriffe.
  
**Tabelle 17. Ereignisse im Zusammenhang mit der Ausnutzung von Sicherheitsanfälligkeiten zur Erhöhung der Berechtigungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>528</p>
<p>538</p></td>
<td style="border:1px solid black;"><p>Lokale An- und Abmeldung</p></td>
<td style="border:1px solid black;"><p>Korrelieren Sie das Feld für die Anmeldekennung, wenn derartige Ereignisse auf Umkreiscomputern auftreten. Dies sollte eine Untersuchung nach sich ziehen, wenn die Felder für Benutzerkontoname, Zeit oder Arbeitsstationsname unerwartete Werte aufweisen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>551</p></td>
<td style="border:1px solid black;"><p>Vom Benutzer initiierte Abmeldung</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis kann als gleichwertig mit Ereignis 538 betrachtet werden, da eine Tokenlücke zu einem Fehler beim Überwachungsereignis 538 führen kann und stattdessen Ereignis 551 ausgegeben wird.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>576</p></td>
<td style="border:1px solid black;"><p>Privilegierte Anmeldung</p></td>
<td style="border:1px solid black;"><p>Weist auf eine Administratorkontoanmeldung hin, d. h. eine Kontoanmeldung mit ausreichenden Berechtigungen zur Manipulation der Trusted Computing Base (TCP) oder zur Übernahme eines Computers unter Windows Server 2003 mit SP1 oder höher. Bei früheren Versionen von Windows verdient dieses Ereignis nur Beachtung, wenn es mit vertraulichen Berechtigungen wie „SeSecurityPrivilege“ oder „SeDebugPrivilege“ verbunden ist.</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   In Versionen von Windows vor Windows Server 2003 wird das Ereignis 576 in der Berechtigungenkategorie aufgelistet. Unter Windows Server 2003 oder höher wird dieses Ereignis außerdem in der Anmeldekategorie verzeichnet. Dieses Ereignis wird somit bei der Konfiguration von Überwachungseinstellungen für jede dieser Kategorien ausgegeben.
  
###### Versuche der Umgehung von Überwachungen
  
Genauso, wie es mehrere Methoden für Angriffe auf Unternehmensnetzwerke gibt, gibt es auch verschiedene Techniken, um diese Angriffe zu verbergen. Ein Angreifer kann z. B. die Sicherheitsrichtlinie auf einem kompromittierten System oder einer Domäne so ändern, dass Ereignisprotokolle die verdächtigen Aktivitäten nicht aufzeichnen, oder es kann ein Sicherheitsprotokoll mutwillig gelöscht werden, so dass sämtliche Überwachungsdaten verloren gehen.
  
Versuche, Sicherheitsüberwachungslösungen mit solchen Techniken auszutricksen, können zwar erkannt werden, dies stellt jedoch eine große Herausforderung dar, da es sich bei vielen Ereignissen, die während des Versuchs der Spurenvernichtung bei Einbruchsaktivitäten auftreten, um solche handelt, die auf typischen Unternehmensnetzwerken häufig vorkommen.
  
Die folgende Tabelle enthält mehrere Ereignistypen, mit denen Versuche der Überwachungsumgehung durch Angreifer, die die Spuren der Sicherheitsverletzung verbergen möchten, identifiziert werden können.
  
**Tabelle 18. Ereignisse im Zusammenhang mit der Umgehung von Ereignisüberwachungen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>512</p></td>
<td style="border:1px solid black;"><p>Starten von Windows</p></td>
<td style="border:1px solid black;"><p>Dies tritt normalerweise nach Ereignis 513 auf. Unerwartete Neustarts sollten untersucht werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>513</p></td>
<td style="border:1px solid black;"><p>Herunterfahren von Windows</p></td>
<td style="border:1px solid black;"><p>Dies tritt normalerweise vor Ereignis 512 auf. Hochwertige Computer sollten nur durch autorisiertes Personal neu gestartet werden, und selbst dann sollte dies nur in Übereinstimmung mit einem etablierten Änderungssteuerungs- oder einem anderen Verfahren erfolgen. Das Auftreten dieses Ereignisses auf einem beliebigen Server sollte eine umgehende Untersuchung nach sich ziehen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>516</p></td>
<td style="border:1px solid black;"><p>Überwachungsfehler</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis kann auftreten, wenn entweder die Anzahl der Ereignisse den Ereignisprotokollpuffer überfordert oder das Sicherheitsprotokoll nicht für Überschreibvorgänge eingerichtet ist. Diese Probleme lassen sich durch Einschränken der auf den meisten Computern überwachten Ereignistypen vermeiden, doch ist für die Sicherung hochwertiger oder besonders gefährdeter Computer eine detailliertere Überwachung erforderlich.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>517</p></td>
<td style="border:1px solid black;"><p>Löschen des Sicherheitsereignisprotokolls</p></td>
<td style="border:1px solid black;"><p>Sicherheitsereignisprotokolle sollten niemals ohne entsprechende Genehmigung gelöscht werden. Gleichen Sie die Felder für den Client-Benutzernamen und die Client-Domäne mit autorisiertem Personal und Datensätzen zu Verfahrensgenehmigungen ab.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>520</p></td>
<td style="border:1px solid black;"><p>Ändern der Systemuhrzeit</p></td>
<td style="border:1px solid black;"><p>Diese Aktivität kann mit dem Ziel durchgeführt werden, forensische Untersuchungen zu behindern oder Angreifern falsche Alibis zu verschaffen. Gleichen Sie die Felder für den Client-Benutzernamen und die Client-Domäne mit autorisiertem Personal ab und stellen Sie sicher, dass der Prozessname als %windir%\system32\svchost.exe aufgelistet ist.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>521</p></td>
<td style="border:1px solid black;"><p>Ereignisse können nicht protokolliert werden</p></td>
<td style="border:1px solid black;"><p>Dies tritt auf, wenn Windows Ereignisse nicht in das Ereignisprotokoll schreiben kann. Dieses Ereignis sollte untersucht werden, wenn es auf einem hochwertigen System auftritt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>608</p></td>
<td style="border:1px solid black;"><p>Es wurde eine Benutzerkontoberechtigung zugewiesen</p></td>
<td style="border:1px solid black;"><p>Dies tritt auf, wenn einem Benutzerkonto eine neue Berechtigung zugewiesen wird. Im Ereignisprotokoll wird dieser Vorgang zusammen mit der Sicherheits-ID (SID) des Benutzerkontos, nicht jedoch dem Benutzerkontonamen aufgezeichnet.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>609</p></td>
<td style="border:1px solid black;"><p>Es wurde eine Benutzerkontoberechtigung aufgehoben</p></td>
<td style="border:1px solid black;"><p>Dies tritt auf, wenn eine Berechtigung eines Benutzerkontos aufgehoben wurde. Im Ereignisprotokoll wird dieser Vorgang zusammen mit der SID des Benutzerkontos, nicht jedoch dem Benutzerkontonamen aufgezeichnet.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>612</p></td>
<td style="border:1px solid black;"><p>Überwachungsrichtlinie wird geändert</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis weist nicht unbedingt auf ein Problem hin, doch können Angreifer Überwachungsrichtlinien als Teil ihrer Angriffsstrategie ändern. Dieses Ereignis sollte auf hochwertigen Computern und Domänencontrollern untersucht werden.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>621</p></td>
<td style="border:1px solid black;"><p>Einem Konto wurde Systemzugriff gewährt</p></td>
<td style="border:1px solid black;"><p>Dies tritt auf, wenn einem Benutzer Zugriff auf ein System gewährt wurde. Die Felder für den Benutzernamen und das geänderte Konto sollten überprüft werden, wenn die Zugriffsberechtigung als interaktiv aufgelistet wurde.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>622</p></td>
<td style="border:1px solid black;"><p>Systemzugriff wurde aus einem System entfernt</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis kann auf den Versuch eines Angreifers hindeuten, Spuren im Zusammenhang mit Ereignis 621 zu löschen oder einem oder mehreren anderen Konten Dienste zu verweigern.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>643</p></td>
<td style="border:1px solid black;"><p>Domänensicherheitsrichtlinie wird geändert</p></td>
<td style="border:1px solid black;"><p>Dies tritt bei dem Versuch auf, die Einstellungen der Kennwortrichtlinie oder einer anderen Domänensicherheitsrichtlinie zu ändern. Korrelieren Sie den Benutzernamen mit allen vorhandenen Autorisierungsdatensätzen.</p></td>
</tr>
</tbody>
</table>
  
##### Forensische Analyse
  
Für forensische Analysen sind viele Elemente erforderlich, auf die in diesem Dokument eingegangen wurde, sie unterscheiden sich dennoch grundsätzlich von den anderen erwähnten Überwachungs- und Angriffsermittlungslösungen, da sie sich mit der Speicherung und Analyse von Sicherheitsdaten befassen und als Reaktion auf einen bereits erfolgten Angriff verwendet werden. Den Anfang der meisten forensischen Untersuchungen stellt eine Liste von Ereignissen dar, die mit einem bestimmten Benutzer oder System verbunden sind.
  
Die Sicherheitsüberwachung für forensische Analysen erfordert Folgendes:
  
-   Archivierung ausgewählter Ereignistypen.
  
-   Abschätzung der täglich zu erwartenden Ereignisanzahl.
  
-   Einrichtung von zeitlichen Grenzen für die Online-, Offline- und Archivierungsspeicherung.
  
-   Einrichtung von Datenbanken zur Bewältigung der erwarteten Ereignisanzahl.
  
-   Einrichtung der Sicherungssysteme zur Bewältigung des erwarteten täglichen Ereignisaufkommens.
  
-   Einrichten von Richtlinien zur Verwaltung des Archivierungssystems.
  
Es gibt drei Hauptfaktoren, nach denen der Speicherbedarf für ein Programm für forensische Analysen ermittelt werden kann:
  
-   Die Anzahl der aufzuzeichnenden Ereignisse
  
-   Die Generationsrate der Ereignisse durch Zielcomputer
  
-   Onlinespeicherungsdauer für die Verfügbarkeit
  
Ein Verständnis des Geschäftsbedarfs sowie die in den vorherigen Abschnitten enthaltenen Informationen dürften für die Bestimmung dieser drei Faktoren hilfreich sein, so dass ein angemessener Speicherbedarf ermittelt werden kann.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
In der heutigen Netzwerkumgebung stellt eine effektive und umfassende Sicherheitsüberwachungs- und Angriffsermittlungslösung keine Option, sondern eine Notwendigkeit für mittelgroße Unternehmen dar. Die Bedrohungen und Risiken, denen Unternehmensnetzwerke ausgesetzt sind, sind zahlreich und haben ihren Ursprung nicht nur außerhalb des Umkreises, sondern schließen auch absichtliche und unbeabsichtigte interne Bedrohungen ein. Sinnvolle Sicherheitsüberwachungssysteme berücksichtigen sämtliche Risiken und erfordern ein gründliches Verständnis dieser Risiken neben dem der aktuellen Architektur eines Unternehmensnetzwerks und der Anzeichen potenzieller Bedrohungen und Aktivitäten, die eine Gefährdung für die Daten auf den Systemen des Netzwerks darstellen könnten.
  
Microsoft nimmt die Sicherheit sehr ernst und bietet dementsprechend eine Vielzahl von Tools an, die für die Einrichtung eines wirksamen Sicherheitsüberwachungs- und Angriffsermittlungssystems verwendet werden können. Windows Server 2003 und andere Versionen des Windows-Betriebssystems tragen mit ihrer integrierten Protokollierungsfunktionalität zur Schaffung einer Basis für derartige Sicherheitsüberwachungslösungen bei. In Kombination mit anderen Komponenten wie beispielsweise Microsoft Operations Manager und EventCombMT sowie den erforderlichen Unternehmensrichtlinien und -verfahren lässt sich ein umfassendes Überwachungssystem entwickeln.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Anhang A: Ausschließen unnötiger Ereignisse
  
Die in der folgenden Tabelle enthaltenen Ereignisse werden normalerweise von Sicherheitsüberwachungsabfragen ausgenommen, weil sie sehr häufig auftreten und bei Einschluss in eine Sicherheitsüberwachungslösung für gewöhnlich keine nützlichen Ergebnisse liefern.
  
**Tabelle A1. Unnötige Ereignisse**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Ereignis-ID</p></th>
<th><p>Auftreten</p></th>
<th><p>Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>538</p></td>
<td style="border:1px solid black;"><p>Benutzerabmeldung</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis gibt nicht unbedingt die Uhrzeit an, zu der ein Benutzer aufgehört hat, das System zu verwenden. Falls ein Computer z. B. ausgeschaltet wird oder seine Netzwerkverbindung verliert, wird möglicherweise überhaupt kein Abmeldeereignis aufgezeichnet.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>562</p></td>
<td style="border:1px solid black;"><p>Handle für ein Objekt geschlossen</p></td>
<td style="border:1px solid black;"><p>Wird stets als erfolgreich aufgezeichnet.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>571</p></td>
<td style="border:1px solid black;"><p>Clientkontext durch Autorisierungs-Manager gelöscht</p></td>
<td style="border:1px solid black;"><p>Dies ist bei Verwendung des Autorisierungs-Managers ein erwartetes Ereignis.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>573</p></td>
<td style="border:1px solid black;"><p>Prozess generiert systemfremdes Überwachungsereignis mit AuthZ API (Authorization Application Programming Interface)</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>577<br />
578</p></td>
<td style="border:1px solid black;"><p>Privilegiendienst aufgerufen, Privilegiertes-Objekt-Vorgang</p></td>
<td style="border:1px solid black;"><p>Dies sind Ereignisse mit hohem Aufkommen, die normalerweise nicht genügend Informationen für Maßnahmen aufweisen, da sie den durchgeführten Vorgang nicht beschreiben.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>594</p></td>
<td style="border:1px solid black;"><p>Handle für ein Objekt dupliziert</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>595</p></td>
<td style="border:1px solid black;"><p>Indirekter Zugriff auf ein Objekt wurde erlangt</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>596</p></td>
<td style="border:1px solid black;"><p>Sicherung des Datensicherungs-Hauptschlüssels</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität. Dies tritt bei Standardeinstellungen alle 90 Tage auf.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>597</p></td>
<td style="border:1px solid black;"><p>Wiederherstellung des Datensicherungs-Hauptschlüssels</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>672</p></td>
<td style="border:1px solid black;"><p>Anfrage für Kerberos AS-Ticket</p></td>
<td style="border:1px solid black;"><p>Dies enthält keine weiteren Informationen, falls Überwachungsdetails von den Anmeldeereignissen 528 und 540 bereits erfasst wurden. Dieses Ereignis hält fest, dass ein Kerberos TGT gewährt wurde. Es erfolgt kein Zugriff, bis ein Dienstticket gewährt wird, was durch Ereignis 673 überwacht wird. Handelt es sich bei PATYPE um PKINIT, liegt eine Smartcard-Anmeldung vor.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>680</p></td>
<td style="border:1px solid black;"><p>Kontoanmeldung</p></td>
<td style="border:1px solid black;"><p>Aktivität bereits durch andere Ereignisse erfasst.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>697</p></td>
<td style="border:1px solid black;"><p>Kennwortüberprüfende API aufgerufen</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>768</p></td>
<td style="border:1px solid black;"><p>Gesamtstruktur-Namespace-Konflikt</p></td>
<td style="border:1px solid black;"><p>Dieses Ereignis betrifft nicht die Sicherheit.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>769<br />
770<br />
771</p></td>
<td style="border:1px solid black;"><p>Informationen zur vertrauten Gesamtstruktur hinzugefügt, gelöscht oder geändert</p></td>
<td style="border:1px solid black;"><p>Erwartete Aktivität. Diese Ereignisse sind nicht mit dem Hinzufügen, Ändern oder Löschen der Vertrauensstellung selbst zu verwechseln.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>832<br />
833<br />
834<br />
835<br />
836<br />
837<br />
838<br />
839<br />
840<br />
841</p></td>
<td style="border:1px solid black;"><p>Verschiedene Active Directory-Replikationsereignisse</p></td>
<td style="border:1px solid black;"><p>Diese Ereignisse betreffen nicht die Sicherheit.</p></td>
</tr>
</tbody>
</table>
  
**Hinweis**   Der Ausschluss von Informationen aus der Überwachung ist mit einigen Risiken verbunden, doch sollte dieses Risiko mit den Vorteilen verglichen werden, die die Auslastungsreduzierung für einen Analyse-Agent bringt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Anhang B: Implementieren von Gruppenrichtlinieneinstellungen
  
Dieser Anhang kann zur Überprüfung der aktuellen Einstellungen in einer Umgebung herangezogen werden. Er enthält zusätzliche Einstellungen, die sich auf die Sicherheitsüberwachung und Angriffsermittlung auswirken. Zur ordnungsgemäßen Konfiguration von Sicherheitsüberwachungsereignissen für Gruppenrichtlinien sind die Einstellungen in der folgenden Tabelle anzuwenden.
  
**Tabelle B1. Sicherheitsüberwachungseinstellungen für Gruppenrichtlinien**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Richtlinienpfad</p></th>
<th><p>Richtlinie</p></th>
<th><p>Richtlinieneinstellung und Anmerkungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Anmeldeversuche überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie die Überwachungserfolge für alle Computer, da dieses Ereignis aufzeichnet, wer auf Computer zugreift. Aktivieren Sie Überwachungsfehler nicht leichtfertig, da Angreifer mit Netzwerkzugriff, jedoch ohne Anmeldeinformationen einen DoS-Angriff durchführen könnten, indem ein Computer zum Ressourcenverbrauch bei der Aufzeichnung dieser Ereignisse gezwungen wird. Aktivieren Sie Überwachungserfolge ebenfalls nicht leichtfertig, da diese Einstellung zu DoS-Angriffen führen kann, wenn Computer zum Herunterfahren bei vollen Überwachungsprotokollen eingerichtet sind. Korrelieren Sie alle Administratoranmeldungen mit allen anderen verdächtigen Einträgen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Kontenverwaltung überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie sowohl erfolgreiche als auch fehlgeschlagene Ereignisse. Korrelieren Sie alle erfolgreichen Überwachungseinträge mit Administratorautorisierungen. Sämtliche Fehlschläge sollten als verdächtig eingestuft werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Verzeichnisdienstzugriff überwachen</p></td>
<td style="border:1px solid black;"><p>Durch die standardmäßige Gruppenrichtlinie für Domänencontroller wird diese Einstellung standardmäßig aktiviert. Konfigurieren Sie Überwachungseinstellungen für vertrauliche Verzeichnisobjekte anhand von Systemzugriff-Steuerungslisten (SACLs) in „Active Directory-Benutzer und -Computer“ oder „Active Directory-Schnittstellen-Editor“ (ADSI Edit). Planen Sie die SACL-Implementierung, und testen Sie die SACLs nach Möglichkeit in einer realistischen Laborumgebung, bevor Sie sie in einer Produktionsumgebung bereitstellen. Durch diese Vorgehensweise wird die Überlastung der Sicherheitsprotokolle infolge zu großer Datenmengen verhindert.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Anmeldeereignisse überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie die Überwachungserfolge für alle Computer, da dieses Ereignis aufzeichnet, wer auf Computer zugreift. Aktivieren Sie Überwachungsfehler nicht leichtfertig, da Angreifer mit Netzwerkzugriff, jedoch ohne Anmeldeinformationen eine DoS-Situation herbeiführen könnten, indem übermäßig viele Fehler generiert werden.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Objektzugriff überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie diese Einstellung mit Bedacht, da sie zu einem sehr hohen Überwachungsvolumen führen kann. Konfigurieren Sie Überwachungseinstellungen nur für hochwertige Ordner anhand von SACLs, und überprüfen Sie ausschließlich die konkreten Zugriffsarten, die von Interesse sind. Überprüfen Sie nach Möglichkeit nur Schreibzugriffsereignisse, nicht jedoch Lesezugriffsereignisse.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Richtlinienänderungen überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie Überwachungen sowohl von Erfolgen als auch von Fehlschlägen. Gleichen Sie alle Erfolgsereignisse mit Administratorautorisierungen ab.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Rechteverwendung überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie nicht die Überwachung der Rechteverwendung, da durch diese Konfiguration ein hohes Aufkommen an Ereignissen generiert werden würde.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Prozessverfolgung überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie diese Einstellung auf gefährdeten Computern, und untersuchen Sie umgehend unerwartete Anwendungsaktivitäten, indem Sie bei Bedarf das System isolieren. Aktivieren Sie diese Einstellung nicht auf CGI-Webservern (Common Gateway Interface, gemeinsame Gatewayschnittstelle), Testsystemen, Servern, auf denen Batchprozesse ausgeführt werden oder Arbeitsstationen von Entwicklern, da durch diese Einstellung Ereignisprotokolle schnell aufgefüllt werden können.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Überwachungsrichtlinie</p></td>
<td style="border:1px solid black;"><p>Systemereignisse überwachen</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie Überwachungen von Erfolgen und von Fehlschlägen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Zuweisen von Benutzerrechten</p></td>
<td style="border:1px solid black;"><p>Sicherheitsüberprüfung generieren</p></td>
<td style="border:1px solid black;"><p>Diese Einstellung wird standardmäßig dem lokalen System, lokalen Server und Netzwerkdienst zugewiesen. Dieses Recht sollte nur für Dienstkonten Anwendung finden. Ein Angreifer kann anhand dieser Einstellung falsche oder ungenaue Ereignisse im Sicherheitsprotokoll generieren.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Zuweisen von Benutzerrechten</p></td>
<td style="border:1px solid black;"><p>Überwachungs- und Sicherheitsprotokoll verwalten</p></td>
<td style="border:1px solid black;"><p>Schränken Sie mit dieser Einstellung die Möglichkeit von Administratoren ein, Änderungen an Überwachungseinstellungen in Dateien, Ordnern und der Registrierung vorzunehmen. Ziehen Sie in Erwägung, eine Sicherheitsgruppe für Administratoren einzurichten, die Änderungen an Überwachungseinstellungen vornehmen und die Administratorengruppe aus den Einstellungen für die lokale Sicherheitsrichtlinie entfernen dürfen. Es sollten ausschließlich Mitglieder einer Sicherheitsgruppe die Überwachung konfigurieren dürfen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Sicherheitsoptionen</p></td>
<td style="border:1px solid black;"><p>Überwachung: Zugriff auf globale Systemobjekte prüfen</p></td>
<td style="border:1px solid black;"><p>Mit dieser Einstellung werden SACLs zu benannten Systemobjekten wie Mutexen, Semaphoren und MS-DOS-Geräten hinzugefügt. Durch die Standardeinstellungen in Windows Server 2003 wird diese Option nicht aktiviert. Aktivieren Sie diese Einstellung nicht, da sie zu einem hohen Ereignisaufkommen führt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Sicherheitsoptionen</p></td>
<td style="border:1px solid black;"><p>Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen</p></td>
<td style="border:1px solid black;"><p>Sicherungs- und Wiederherstellungsvorgänge bieten die Gelegenheit zum Datendiebstahl durch Umgehung von ACLs. Aktivieren Sie diese Einstellung nicht, da sie zu einem sehr hohen Ereignisaufkommen führt.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lokale Richtlinien/Sicherheitsoptionen</p></td>
<td style="border:1px solid black;"><p>Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie diese Einstellung nur nach gründlicher Überlegung und ausschließlich auf hochwertigen Computern, da Angreifer anhand dieser Einstellung DoS-Angriffe einleiten können.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Ereignisprotokoll</p></td>
<td style="border:1px solid black;"><p>Maximale Größe des Sicherheitsprotokolls</p></td>
<td style="border:1px solid black;"><p>Die empfohlenen Einstellungen hängen vom erwarteten Ereignisaufkommen und von den Einstellungen für die Aufbewahrung von Sicherheitsprotokollen ab. Diese Einstellung kann nur in Schritten von 64 KB vorgenommen werden, wobei die durchschnittliche Ereignisgröße 0,5 KB beträgt. Für Umgebungen mit hohem Datenaufkommen kann die Einstellung auf bis zu 250 MB konfiguriert werden, die Gesamtgröße aller Ereignisprotokolle darf 300 MB jedoch nicht übersteigen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Ereignisprotokoll</p></td>
<td style="border:1px solid black;"><p>Lokalen Gastkontozugriff auf Systemprotokoll verhindern</p></td>
<td style="border:1px solid black;"><p>Windows Server 2003 aktiviert diese Einstellung standardmäßig. Ändern Sie dies nicht.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Ereignisprotokoll</p></td>
<td style="border:1px solid black;"><p>Sicherheitsprotokoll-Aufbewahrung</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie diese Einstellung nur, wenn „Ereignisse auf Tagen basierend überschreiben“ als Aufbewahrungsmethode ausgewählt wurde. Stellen Sie bei Verwendung eines Ereigniskorrelationssystems, das Ereignisse abruft, sicher, dass die Anzahl an Tagen mindestens dreimal so hoch wie die Abfragehäufigkeit ist, damit Abfragezyklusfehler berücksichtigt werden können.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Ereignisprotokoll</p></td>
<td style="border:1px solid black;"><p>Aufbewahrungsmethode des Sicherheitsprotokolls</p></td>
<td style="border:1px solid black;"><p>Aktivieren Sie in Hochsicherheitsumgebungen die Einstellung „Ereignisse nicht überschreiben“. Richten Sie in diesem Fall Verfahren zum regelmäßigen Leeren und Archivieren von Protokollen ein, besonders wenn die Einstellung zum umgehenden Herunterfahren des Systems bei nicht möglicher Protokollierung von Sicherheitsüberwachungen aktiviert ist.</p></td>
</tr>
</tbody>
</table>
  
**Download**
  
[Dokument „Sicherheitsüberwachung und Angriffsermittlung“ herunterladen](http://go.microsoft.com/fwlink/?linkid=71717)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
