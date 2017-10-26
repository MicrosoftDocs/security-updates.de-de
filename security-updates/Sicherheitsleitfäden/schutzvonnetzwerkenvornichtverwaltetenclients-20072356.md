---
Title: Schutz von Netzwerken vor nicht verwalteten Clients
TOCTitle: Schutz von Netzwerken vor nicht verwalteten Clients
ms:assetid: 9a90dd07-0efb-4151-bf99-629448130645
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Cc875843(v=TechNet.10)
ms:contentKeyID: 20072356
---


# Schutz von Netzwerken vor nicht verwalteten Clients

Veröffentlicht: 29. Aug 2006

#### Auf dieser Seite

[Einführung](#efaa)  
[Definition](#eeaa)  
[Herausforderungen](#edaa)  
[Lösungen](#ecaa)  
[Zusammenfassung](#ebaa)  
[Anhang A: Netzwerkzugriffsschutz](#eaaa)  



### Einführung

Willkommen bei diesem Dokument aus der Reihe der Sicherheitsleitfäden für mittelgroße Unternehmen. Microsoft hofft, dass Sie die folgenden Informationen beim Erstellen einer IT-Umgebung mit erhöhter Sicherheit und Produktivität unterstützen.


#### Kurzzusammenfassung

In der heutigen sicherheitsbewussten Computerwelt ist ein fundiertes Konzept zum Schutz des Netzwerks eines mittelgroßen Unternehmens und der darin gespeicherten Daten eine sehr komplexe Angelegenheit. Zum Schutz von Netzwerkressourcen und vertraulichen Informationen reicht es nicht mehr aus, sich nur auf Umkreisverteidigung und Antivirensuites zu verlassen. Sicherheitsorganisationen und Fachleute verstehen heute, dass interne Netzwerkrisiken, egal, ob mutwillig herbeigeführt oder unbeabsichtigt, unter Umständen noch vernichtender sein können als externe Bedrohungen.

Um den unzähligen Sicherheitsanfälligkeiten Herr zu werden, die eine Bedrohung für mittelgroße Unternehmen darstellen, wurden in die Bereiche Patchverwaltung, Antimalwarelösungen und Identitätsverwaltungsinitiativen Zeit und Ressourcen in erheblichem Umfang investiert. Um sicherzustellen, dass diese Investitionen innerhalb des Unternehmens universell und möglichst effizient eingesetzt werden, muss das Unternehmen Möglichkeiten finden, Sicherheitsrichtlinien wirksam umzusetzen.

Nicht autorisierte Computer (Rogue-Computer) sind Systeme, die nicht als substanzielle Risiken gelten, da sich nicht feststellen lässt, ob sie den geltenden Sicherheitsrichtlinien entsprechen. Rogue-Computer können für Systemadministratoren ebenso wie für Sicherheitsexperten ein Problem darstellen. Nichtkonforme Systeme bergen zahlreiche Risiken, von ihrer Anfälligkeit für Malwarebefall bis zu der Tatsache, dass sie potenzielle Plattformen für Angriffe sein können. Im Allgemeinen ist es schwierig, sie in den Griff zu bekommen und mit den Sicherheitsrichtlinien in Einklang zu bringen.

Im vorliegenden Dokument werden einige wirksame Methoden beschrieben, mit denen sich die Konformität mit den Sicherheitsrichtlinien leichter durchsetzen lässt. Dieses Konzept ermöglicht eine Maximierung der Vorteile von Risikomanagement-Anstrengungen und fügt dem Netzwerk eines mittelgroßen Unternehmens eine zusätzliche Sicherheitsebene hinzu, die zur Verringerung der Risiken durch nicht vertrauenswürdige und nicht verwaltete Computer beiträgt.


#### Übersicht

Dieses Dokument gliedert sich in vier Hauptabschnitte, die sich mit Details befassen, mit denen ein Leser die Konzepte und Prinzipien zum Schutz eines mittelgroßes Unternehmens vor nicht verwalteten Computern leichter versteht. Diese vier Hauptabschnitte lassen sich folgendermaßen zusammenfassen:

Einführung

Dieser Abschnitt enthält eine Kurzzusammenfassung des Dokuments und eine Übersicht über die Struktur des Dokuments sowie einige Informationen zu seiner Zielgruppe.

Definition

Dieser Abschnitt enthält einige Details und Definitionen, die zum besseren Verständnis der in diesem Dokument vorgestellten Lösungen beitragen.

Herausforderungen

In diesem Abschnitt wird auf einige typische Probleme eingegangen, mit denen mittelgroße Unternehmen oftmals konfrontiert sind, wenn es zu entscheiden gilt, wie ein Schutz vor nicht verwalteten und nicht vertrauenswürdigen Computern gewährleistet werden kann. Diese Informationen dienen als allgemeiner Hintergrund zum Verständnis der in diesem Dokument behandelten Fragen.

Lösungen

In diesem Abschnitt werden Lösungen erörtert, mit denen die Herausforderungen durch nicht verwaltete Computer bewältigt werden können. Hierzu werden die möglichen Herangehensweisen ermittelt und Fragen bezüglich der Planung von Lösungen für das Problem diskutiert. Zudem finden Sie hier einige Informationen zu Bereitstellungs- und Verwaltungsmethoden.


#### Zielgruppe dieses Leitfadens

Dieses Fachdokument soll IT-Experten und Technikmanagern helfen, das Netzwerk eines mittelgroßen Unternehmens vor den Gefahren durch nicht verwaltete Geräte zu schützen und diesbezüglich möglichst fundierte Entscheidungen zu treffen. Wenngleich auch nicht fachkundige Leser anhand dieses Dokuments einen besseren Einblick in diese spezielle Sicherheitsproblematik erlangen können, ist es sinnvoll, über Grundkenntnisse in folgenden Bereichen zu verfügen, um die in diesem Dokument behandelten Lösungen verstehen und anwenden zu können.

Im Einzelnen werden vor allem folgende Technologien behandelt:
* IEEE 802.1X-Authentifizierung

* IPsec-Richtlinien

* Netzwerksicherheit

* Microsoft® Systems Management Server 2003

* Microsoft Windows Server™ 2003

* Active Directory®-Verzeichnisdienst

* Microsoft Operations Management Server

* Microsoft Internetauthentifizierungsdienst

* RADIUS-Authentifizierung

[Zum Seitenanfang](#mainsection)  



### Definition

In dieser Anleitung wird das Prozessmodell von Microsoft Operations Framework (MOF) zusätzlich zu den Dienstverwaltungsfunktionen (SMFs) von MOF Security Administration verwendet.

Im Besonderen wird bei den hierin vorgestellten Lösungen die Verwendung eines kontinuierlichen Prozesses anstelle eines linearen Bereitstellungsansatzes empfohlen, um die Netzwerksicherheit gegenüber Gefahren durch nicht verwaltete Computer zu erhöhen.

Die Anwendung dieser Lösungen sollte mit den in der folgenden Abbildung dargestellten Schritten einhergehen:

![](images/cc875843.pnfuc01(de-de,technet.10).gif)

**Abbildung 1. Anwenden von MOF**
 

Wie aus der Abbildung hervorgeht, sollten alle Antworten auf die Sicherheitsprobleme durch nicht verwaltete Systeme kontinuierliche Test- und Justierungsprozesse sein und sich nicht nur auf die Planung und Bereitstellung beschränken. Die Bedrohungen, denen das Netzwerk eines mittelgroßen Unternehmens ausgesetzt ist, ändern sich ständig, und die Systeme, die ein Unternehmensnetzwerk schützen, müssen fortlaufend an diese Bedrohungen angepasst werden.

Das Anwenden der in diesem Dokument behandelten Lösungen entspricht der Dienstverwaltungsfunktion „Sicherheitsverwaltung“, die aus folgenden Grundschritten besteht:
* Ermitteln Sie den Gefährdungsgrad des Unternehmens, und bestimmen Sie, welche Ressourcen gesichert werden müssen.

* Identifizieren Sie Möglichkeiten, wie das Risiko durch ungesicherte Geräte auf ein akzeptables Maß reduziert werden kann.

* Erstellen Sie einen Plan zur Minderung von Sicherheitsrisiken.

* Überwachen Sie die Effizienz von Sicherheitsmechanismen.

* Beurteilen Sie die Effektivität und die Sicherheitsanforderungen regelmäßig neu.


Näheres über MOF finden Sie auf der [Microsoft Operations Framework](http://www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx)-Website im Microsoft TechNet unter www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx.

Weitere Informationen über die Dienstverwaltungsfunktion „Sicherheitsverwaltung“ finden Sie auf der Seite [Sicherheitsverwaltungsfunktionen](http://go.microsoft.com/fwlink/?linkid=37696) (möglicherweise in englischer Sprache) unter http://go.Microsoft.com/fwlink/?LinkId=37696.

Das Risikomanagement umfasst das Ermitteln eines akzeptablen Risikopotenzials eines Unternehmens, das Beurteilen der aktuellen Risiken, das Entwickeln von Methoden zum Erreichen des akzeptablen Risikopotenzials sowie das Verwalten des Risikos. Wenngleich in diesem Dokument einige Risikomanagementkonzepte genannt werden, ist eine eingehende Behandlung des Risikomanagements ein Thema für sich und verdient somit spezielle Aufmerksamkeit. Weitere Informationen über Risikoanalyse und -beurteilung finden Sie im [*Leitfaden zum Sicherheitsrisikomanagement*](http://go.microsoft.com/fwlink/?linkid=30794) unter http://go.Microsoft.com/fwlink/?LinkId=30794.

[Zum Seitenanfang](#mainsection)  



### Herausforderungen

Einige Herausforderungen in Zusammenhang mit dem Schutz vor nicht verwalteten Computern:
* Wie lässt sich verhindern, dass nicht verwaltete Computer auf Netzwerkressourcen zugreifen?

* Wie kann bewirkt werden, dass Roaming-Computer immer die neuesten Updates erhalten und den aktuellen Richtlinien entsprechen?

* Wie lassen sich geltende Sicherheitsrichtlinien auf Computern durchsetzen, die über Remoteverbindungen auf das Netzwerk zugreifen?

* Wie lässt sich ein Netzwerk vor drahtlosen Rogue-Geräten schützen?

* Wie können nicht verwaltete Systeme wie etwa die Laptops von Zulieferern oder persönliche Geräte erkannt werden, wenn sie eine Verbindung zum Netzwerk herstellen?

* Welchen Schutz gibt es vor anderen Mobilgeräten wie Palmtops oder Handheld-PCs?

[Zum Seitenanfang](#mainsection)  



### Lösungen

Im Abschnitt „Herausforderungen“ wurden verschiedene Faktoren genannt, die es zu berücksichtigen gilt, wenn es um Vorkehrungen zum Schutz vor den Gefahren geht, die Rogue-Computer für ein Netzwerk darstellen. Neben der Absicherung des traditionellen, drahtgebundenen Netzwerks muss auch für den Schutz des drahtlosen Netzwerks sowie von etwaigen Remotezugriffspfaden gesorgt werden. Um alle möglichen Kanäle abzudecken, über die sich ein Rogue-Gerät mit einem Netzwerk verbinden kann, muss die Lösung möglichst umfassend sein.

Im nachstehenden Abschnitt werden die folgenden Konzepte als Antwort auf die genannten Herausforderungen behandelt:
* IPsec-Domänen- und -Serverisolation zur Verhinderung, dass nicht verwaltete Computer auf Netzwerkressourcen zugreifen

* VPN-Quarantäne zur Durchsetzung geltender Sicherheitsrichtlinien auf Computern, die über Remoteverbindungen auf das Netzwerk zugreifen

* 802.1X-Authentifizierung zum Schutz vor nicht vertrauenswürdigen drahtlosen Geräten

* SMS zur Erkennung des Zugriffs nicht verwalteter Computer auf das Netzwerk


**Hinweis**   In diesem Dokument wird vorausgesetzt, dass der Leser bereits Prozesse implementiert hat, die dafür sorgen, dass Mitgliedscomputer in den Domänenstrukturen mittelgroßer Unternehmen den geltenden Sicherheits- und Patchinganforderungen entsprechen, und dass er aktiv nach Methoden sucht, mit denen sich die Konformität und der Schutz vor nichtkonformen Geräten gewährleisten lassen. Leider kann im Rahmen dieses Dokuments nicht darauf eingegangen werden, wie die Richtlinienkonformität von Computern erzielt werden kann oder wie automatische Sicherheitsaktualisierungsmethoden wie WSUS oder die Patchverwaltungsfunktionen von SMS genutzt werden können.


#### Leistungsnachweise

In diesem Abschnitt werden einige potenzielle Lösungen vorgestellt, mit denen sich die Probleme durch nicht verwaltete Computer in mittelgroßen Unternehmen vermeiden lassen. Überdies wird auf verschiedene Entscheidungen hingewiesen, die es vor der Umsetzung einer dieser Lösungen zu treffen gilt. Jede einzelne der behandelten Lösungen würde zur Erhöhung der Netzwerksicherheit im Netzwerk eines mittelgroßen Unternehmens beitragen. Im Rahmen eines umfassenden, tief greifenden Schutzkonzepts bildet jedoch die Kombination dieser Lösungen eine noch effizientere Antwort auf die oben genannten Herausforderungen.

Isolieren von Domänen und Servern mittels IPsec

Das physische Isolieren von Computern und Netzwerken ist kein neues Konzept. Es wurde im Lauf der Jahre in verschiedensten Formen praktiziert, insbesondere dort, wo es Entwicklungs- und Testnetzwerke zu schützen galt. Die älteren Methoden der physischen Isolation sind jedoch nicht besonders hilfreich, wenn es darum geht, verwaltete Systeme vor potenziell bedrohlichen, nicht verwalteten Geräten zu schützen. Dies gilt besonders in modernen Unternehmensnetzwerkumgebungen, wo die mobile Computernutzung im Vormarsch ist und die Nachfrage nach automatisierten und flexiblen Lösungen steigt. Die folgende Tabelle bietet einen Überblick über früher gängige Methoden der physischen Isolation sowie über die Schwierigkeiten, die sie im vorliegenden Fall mit sich bringen.

**Tabelle 1. Methoden der Netzwerkisolation**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

OSI-Schicht

</th>

<th style="border:1px solid black;">

Methode

</th>

<th style="border:1px solid black;">

Probleme

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Schicht 1

</td>

<td style="border:1px solid black;">


Separate Verkabelung für Segmente verwenden, die vom vertrauenswürdigen Netzwerk isoliert sein müssen

</td>

<td style="border:1px solid black;">

&#x2022; Kostenaufwand für das Verlegen neuer Kabel für jede neue Verbindung<br/>

&#x2022; Höherer Verwaltungsaufwand für jeweils neue Kabelanschlüsse bei räumlicher Verlagerung von Benutzern<br/>

&#x2022; Mangelnde Flexibilität und schwierige Handhabung bei Expansion des Unternehmens<br/>

&#x2022; Erhöhte Wahrscheinlichkeit versehentlicher Fehler aufgrund des höheren Verwaltungsaufwands


</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schicht 2

</td>

<td style="border:1px solid black;">


Mithilfe von VLANs logische Subnetze erstellen, die vom vertrauenswürdigen Netzwerk isoliert sind

</td>

<td style="border:1px solid black;">

&#x2022; Zusätzliche Kosten in Zusammenhang mit der Aktualisierung der Switchstruktur zur Unterstützung der VLANs<br/>

&#x2022; Höherer Verwaltungsaufwand für Netzwerkänderungen, räumliche Verlagerung von Benutzern und Beantwortung von Gastverbindungsanforderungen<br/>

&#x2022; Anfälligkeit für versehentliche Fehler bei räumlicher Verlagerung mehrerer Benutzer oder bei Verwendung mobiler Geräte


</td>

</tr>

</table>


Wie diese Tabelle verdeutlicht, benötigt ein modernes Unternehmensnetzwerk eine flexiblere Lösung zur Gewährleistung der Konformität mit Sicherheitsstandards, die vor den Gefahren durch nicht verwaltete Systeme schützen. Einige Lösungen für dieses Problem sind bei Drittanbietern erhältlich. Diese Lösungen müssen jedoch jeweils clientseitig auf allen verwalteten Arbeitsstationen installiert werden und fügen dem Netzwerk eine zusätzliche Komplexitätsebene hinzu. Glücklicherweise sind aktuelle Versionen von Microsoft Windows bereits mit einer Funktionalität ausgestattet, mit der sich das Problem ohne Installation zusätzlicher Software und ohne administrativen Lernaufwand lösen lässt.

Mithilfe der Microsoft-Server- und Domänenisolation sind IT-Administratoren in der Lage, die TCP/IP-Kommunikation einzuschränken, indem sie die integrierte Active Directory-Gruppenrichtlinie und IPsec verwenden. Dies hat folgende Vorteile:
* Verwendung der Netzwerkschicht des OSI-Modells über Switch- und Routergrenzen hinweg

* Unabhängigkeit von der Switchstruktur und den physischen Begrenzungen des Netzwerks

* Kosteneinsparung durch Nutzung der integrierten Authentifizierungsfunktionen von Windows-basierten Computern

* Automatisiert, erfordert keine ständige Wartung bei Netzwerkänderungen und räumlichen Verlagerungen von Benutzern

* Ermöglicht nicht nur die Authentifizierung vertrauenswürdiger Computer, sondern auch die Kommunikation zwischen vertrauenswürdigen Systemen

* Sicherheitsrichtlinien werden durchgesetzt, indem Verbindungen von nicht verwalteten Geräten abgelehnt werden

* Verbesserte Überwachung und Ressourcenverwaltung

* Möglichkeit, spezifische Ressourcen bei Angriffen rasch zu isolieren


Die typischen Unzulänglichkeiten der Verwendung von IPsec zum Sichern der Kommunikation wurden durch entsprechende Weiterentwicklungen weitgehend behoben. So ist vor allem die Netzwerkadressübersetzung (NAT) dank der NAT-Traversalfunktionen aktueller Microsoft Windows-Versionen, wie Windows Server 2003 und Microsoft Windows XP mit Service Pack 2 (SP2), kein Problem mehr. Zudem ist Unterstützung für nicht IPsec-fähige Plattformen über konfigurierbare Ausnahmelisten und/oder Fallbackausnahmen möglich, die eine Klartextkommunikation mit diesen Systemen gestatten.

Die in diesem Dokument vorgestellten Domänen- und Serverisolationslösungen verwendet sogar Microsoft selbst in seinem internen Netzwerk. Microsoft empfiehlt diese Lösungen nicht nur seinen Kunden, sondern verlässt sich selbst auf die zusätzliche Sicherheitsschicht, die diese Lösung bietet, und beabsichtigt, diese Methode für hohe Sicherheit und leichte Verwaltbarkeit einer vertrauenswürdigen Computerumgebung auch langfristig zu unterstützen.

Domänen- und Serverisolation

Einfach ausgedrückt müssen zur Schaffung eines isolierten Netzwerks die verschiedenen Computertypen in einem Unternehmensnetzwerk nach ihren jeweiligen Zugriffsarten voneinander getrennt werden. Im konkreten Fall handelt es sich um folgende zwei Computertypen: verwaltete und nicht verwaltete Computer. Für eine brauchbare Netzwerkisolation müssen zwei Grundbedingungen erfüllt sein, nämlich:
* Die Computer, die sich im isolierten Netzwerk befinden, können eine Kommunikation mit allen Computern im gesamten Netzwerk initiieren, darunter auch mit denen, die sich außerhalb des vertrauenswürdigen Netzwerks befinden.

* Die Computer, die sich außerhalb des isolierten Netzwerks befinden, können nur mit anderen Computern außerhalb des vertrauenswürdigen Netzwerks eine Kommunikation initiieren, nicht jedoch mit Computern innerhalb des vertrauenswürdigen Netzwerks.


Bei der IPsec-Domänen- und -Serverisolation werden bestehende Domänenstrukturen mittels Gruppenrichtlinieneinstellungen genutzt. Alles, was für die Erstellung eines isolierten Netzwerks benötigt wird, ist auf Computern mit Windows XP, Windows 2000 Server und Windows Server 2003 bereits vorhanden. Wenn die notwendigen Gruppenrichtlinieneinstellungen konfiguriert wurden, muss ein neuer Computer, der in ein isoliertes Netwerk eingebunden werden soll, lediglich der jeweiligen Domäne hinzugefügt werden.

![](images/cc875843.pnfuc02(de-de,technet.10).gif)

**Abbildung 2. Netzwerkisolation mittels Active Directory-Domänen**
 

Wie in der obigen Abbildung dargestellt, gilt jeder Computer, der der Domäne nicht angehört, als nicht vertrauenswürdig und befindet sich deshalb außerhalb des isolierten Netzwerks. Ein System, das sich außerhalb des isolierten Netzwerks befindet, kann keine IPsec-Kommunikation initiieren und somit keine Verbindung zu einem System innerhalb der isolierten Domäne herstellen. Mitglieder der isolierten Domäne können hingegen Klartextkommunikation mit Geräten außerhalb des isolierten Netzwerks durchführen.

Viele Unternehmen besitzen natürlich Computer und Server, die zwar verwaltet und vertrauenswürdig sind, aber keiner Active Directory-Domäne angehören oder aus verschiedenen Gründen nicht IPsec-fähig sind, aber dennoch in der Lage sein müssen, mit Systemen innerhalb des isolierten Netzwerks zu kommunizieren. Zur Lösung dieses Dilemmas kann mithilfe von Ausnahmelisten eine weitere isolierte Gruppe (eine so genannte Grenzgruppe) eingerichtet werden, wie aus der folgenden Abbildung hervorgeht.

![](images/cc875843.pnfuc03(de-de,technet.10).gif)

**Abbildung 3. Netzwerkisolation und Grenzgruppen**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875843.pnfuc03_big(de-de,technet.10).gif)
 

Mit einem solchen Netzwerkisolationsmodell lässt sich der Sicherheitsaufwand eines Unternehmensnetzwerks verringern. Diese Lösung allein kann jedoch nicht garantieren, dass vertrauenswürdige Systeme auch künftig den Standards entsprechen, die sie vertrauenswürdig machen. Diese Lösung allein stellt noch keine umfassende Netzwerksicherheitslösung dar. Sie ist vielmehr Teil eines größeren, umfassenden Sicherheitsprozesses, der in Verbindung mit anderen Lösungen zur Minderung von Risiken beitragen kann, denen moderne Netzwerke mittelgroßer Unternehmen ausgesetzt sind. Insbesondere bei Verwendung mit anderen Sicherheitslösungen wie WSUS, SMS oder MOM kann diese Isolationsmethode für die Durchsetzung der Sicherheitsrichtlinien innerhalb des isolierten Netzwerks sorgen.

Andere auf Active Directory basierende Sicherheitslösungen ermöglichen eine Automatisierung von Aufgaben, die eine dauerhafte Konformität mit den Sicherheitsrichtlinien innerhalb des vertrauenswürdigen isolierten Netzwerks gewährleisten. Bei einer Grenzgruppe muss jedoch mit anderen Methoden sichergestellt werden, dass die ihr angehörenden Computer nicht zu Schwachstellen innerhalb der Netzwerkisolationslösung werden. Solche Computer müssen als richtlinienkonform erkannt werden, bevor sie der Grenzgruppe hinzugefügt werden. Zudem müssen für diese Computer spezifische Richtlinien und Methoden gelten, die eine dauerhafte Konformität mit den Sicherheitsrichtlinien vertrauenswürdiger Systeme garantieren.

IPsec

IPsec ist ein Internetprotokoll-Sicherheitsstandard, der eine allgemeine Sicherheitsmethode mit einer auf Richtlinien basierenden IP-Schicht bietet, die sich ideal für eine Host-für-Host-Authentifizierung eignet. IPsec-Richtlinien verfügen definitionsgemäß über Sicherheitsregeln und -einstellungen, die bei einem Hostsystem den eingehenden und ausgehenden Datenfluss steuern. Diese Richtlinien werden in Active Directory mithilfe von Gruppenrichtlinienobjekten (GPOs) für Richtlinienzuweisungen zu Domänenmitgliedern zentral verwaltet. Sie bieten die Möglichkeit, eine sichere Kommunikation zwischen Domänenmitgliedern herzustellen. Diese sichere Kommunikation ist das Grundprinzip der hier vorgestellten Lösung.

Bei IPsec werden mithilfe des IKE-Aushandlungsprotokolls (IKE = Internet Key Exchange) die Optionen zwischen Hosts ausgehandelt, nach denen die sichere IPsec-Kommunikation erfolgen soll. Die Vereinbarungen zwischen zwei Hosts und die verschiedenen Parameter, die diese Aushandlungsmethode definieren, werden als Sicherheitszuordnungen (SAs) bezeichnet. Microsoft Windows kann folgende IKE-Methoden verwenden:
* Kerberos-Authentifizierungsprotokoll, Version 5

* Digitale X.509-Zertifikate mit entsprechenden RSA-Schlüsselpaaren

* Vorinstallierte Schlüssel unter Verwendung von Passphrasen


**Hinweis**   Wenngleich auch PKI als Authentifizierungsmethode verwendet werden kann, ist PKI aufgrund der Integration der Windows 2000-Domänenauthentifizierung (Kerberos) in das IKE-Verhandlungsprotokoll nicht zu empfehlen.

Die Windows-IKE-Verhandlung kann so konfiguriert werden, dass eine Kommunikation mit Computern erlaubt wird, die nicht auf die IKE-Verhandlungsanforderung reagieren. Diese Funktionalität wird als Fallback auf Klartext bezeichnet. Sie ist nicht nur während eines Rollouts unabdingbar, sondern ist in diesem Kontext auch dadurch nützlich, dass sie den Systemen in der Grenzgruppe die Kommunikation mit Mitgliedern des isolierten Netzwerks gestattet. Jede Kommunikation, die IPsec nicht schützen kann, wird als schwache Sicherheitszuordnung (soft security association) bezeichnet und im Sicherheitsprotokoll nicht als positives Überprüfungsergebnis aufgezeichnet.

IPsec erfüllt neben der Authentifizierung noch andere nützliche Funktionen. Beispielsweise sorgt es mithilfe von Authentifizierungsheadern (AHs) und Encapsulating Security Payload-Optionen (ESP-Optionen) für die Integrität und die Verschlüsselung von Netzwerkdatenverkehr. Obwohl AHs sicherstellen können, dass ein Paket während der Übertragung nicht modifiziert wurde, bewirkt die Verwendung von Headern in dieser Funktion eine Inkompatibilität mit der Netzwerkadressübersetzung (NAT). ESP, das normalerweise zum Verschlüsseln von Datenverkehr verwendet wird, kann auch im Null-Verschlüsselungsmodus (ESP/null) verwendet werden, wodurch eine NAT-kompatible Datenintegritätsprüfung möglich ist.

IPsec kann ebenfalls in zwei verschiedenen Modi, nämlich im Transport- und im Tunnelmodus betrieben werden. Der IPsec-Transportmodus ist die empfohlene Methode zum Sichern des Datenverkehrs zwischen zwei Hosts. Hierbei wird einfach nach dem Original-IP-Header ein weiterer Header eingefügt und dann der Rest des Pakets mit AH oder ESP verschlüsselt. Der Tunnelmodus wird normalerweise für VPN-Tunnel zwischen zwei Gateways verwendet. Hierbei werden die Originalpakete und -IP-Header vollständig eingekapselt, und der Original-IP-Header wird durch einen neuen IPsec-Header ersetzt.

Weitere Informationen hierzu finden Sie auf der Microsoft-Seite [Server und Domänenisolation](http://www.microsoft.com/technet/itsolutions/network/sdiso/default.mspx) (möglicherweise in englischer Sprache) unter www.microsoft.com/technet/itsolutions/network/sdiso/default.mspx.

Tief greifende Verteidigung

![](images/cc875843.pnfuc04(de-de,technet.10).gif)

**Abbildung 4. Das Modell der tief greifenden Verteidigung mit logischer Isolation**

Die obige Abbildung verdeutlicht, wie sich die logische Isolation in das Modell der tief greifenden Verteidigung einfügt. Obwohl die Domänen- und Serverisolation – ebenso wie eine hostbasierte Firewall – vornehmlich auf das Sichern des Hostcomputers ausgerichtet ist, setzt sie unter Verwendung von IPsec im Bereich der Netzwerkkommunikation an. Wenngleich diese Lösung die Lücke zwischen Host und internem Netzwerk schließt, befindet sie sich weder gänzlich in der einen noch in der anderen Sphäre, da es sich um eine auf „logischer Isolation“ basierende Lösung handelt. Somit sind folgende Funktionen nicht in ihrem Leistungsumfang enthalten:
* Die logische Isolation kann keine Netzwerkgeräte wie etwa Router sichern.

* Die logische Isolation kann keine Netzwerkverbindungen sichern und ist somit nicht vergleichbar mit dem, was beispielsweise 802.11i WPA für die drahtlose Verschlüsselung und 802.1x EAP-TLS für die drahtlose Zugriffssteuerung bewirken.

* Die logische Isolation kann keine Sicherheit für alle Hosts im Netzwerk bieten, da sie nur für Systeme mit vertrauenswürdigen Computeranmeldeinformationen und domänenbasierter IPsec-Richtlinie gilt.

* Die logische Isolation verfügt über keine automatisch konfigurierbare Methode für die Sicherung von Pfaden auf Anwendungsebene, wie dies zum Beispiel bei HTTPS und SSL in Bezug auf Webanwendungen der Fall ist.


Es ist wichtig, sich bewusst zu machen, welche Rolle die logische Isolation in einer umfassenden, tief greifenden Verteidigung spielt. Von sich aus kann diese Lösung nicht alle Aspekte der Infrastruktur eines mittelgroßen Unternehmens sichern. Bei Verwendung im Rahmen einer umfassenden Lösung kann die logische Isolation jedoch eine wichtige Rolle spielen.

##### VPN-Quarantänedienste zum Schutz vor nicht verwalteten Remotecomputern

Remotesysteme, die VPN-Lösungen für den Zugriff auf ein Unternehmensnetzwerk verwenden, stellen in Hinblick auf Sicherheitsrichtlinie ein besonderes Problem dar. Die meisten Remotezugriffslösungen überprüfen nur die Anmeldeinformationen eines Remotebenutzers, überprüfen aber nicht, ob der Remotecomputer den Sicherheitsrichtlinien entspricht. Diese begrenzte Überprüfung ist insofern problematisch, als Bemühungen um den Schutz eines Netzwerks vor Bedrohungen wie veralteten Antimalware-Signaturdateien, veralteten Sicherheitsupdates, falschen Routingeinstellungen und mangelndem Firewallschutz ignoriert werden.

Die auf Microsoft Windows Server 2003 basierende Quarantänesteuerung für IAS-Netzwerkzugriff trägt zur Lösung dieses Problems bei, indem sie den Remotezugriff auf ein VPN so lange verzögert, bis eindeutig festgestellt werden kann, dass der Konfigurationszustand des verbindenden Computers den aktuellen Sicherheitsrichtlinien entspricht.

VPN-Quarantänedienste

Die Quarantänesteuerung für IAS-Netzwerkzugriff ist eine Funktion der Windows Server 2003-Familie, die normale Remotezugriffsdienste so lange verzögert, bis die verbindenden Remotecomputer durch ein vom Administrator konfiguriertes Skript untersucht und überprüft wurden. Beim Initiieren einer Remotesitzung wird im Normalfall der Benutzer authentifiziert und der Remotecomputer mit einer IP-Adresse versehen. An diesem Punkt wird jedoch die Verbindung in den Quarantänemodus versetzt, wodurch der Netzwerkzugriff so lange eingeschränkt bleibt, bis das vom Administrator bereitgestellte Skript auf dem Remotecomputer ausgeführt wird. Nachdem das Skript ausgeführt und dem RAS-Server mitgeteilt wurde, dass der Remotecomputer den festgelegten Netzwerkrichtlinien entspricht, wird der Quarantänemodus aufgehoben, und der Remotecomputer erhält Zugriff auf das Netzwerk.

Für eine Remoteverbindung im Quarantänemodus können folgende Einschränkungen festgelegt werden:
* Durch eine Gruppe von Quarantänepaketfiltern kann die Art des Datenverkehrs eingeschränkt werden, den der Client initiieren oder empfangen kann.

* Durch einen Quarantänesitzungstimer kann die Dauer der Verbindung eines Clients im Quarantänemodus eingeschränkt werden.


Die Quarantänesteuerung für IAS-Netzwerkzugriff kann als Teil einer umfassenden Sicherheitslösung verwendet werden, die die Durchsetzung von Sicherheitsrichtlinien unterstützt und verhindern hilft, dass nicht vertrauenswürdige Systeme eine Verbindung zu einem vertrauenswürdigen Netzwerk herstellen. Die Quarantänesteuerung für IAS-Netzwerkzugriff ist für sich genommen jedoch keine Sicherheitslösung und kann keine Verbindungen von böswilligen Benutzern verhindern, die an gültige Anmeldeinformationen gelangt sind.

**Hinweis**   Die Quarantänesteuerung für IAS-Netzwerkzugriff ist nicht dasselbe wie Netzwerkzugriffsschutz (NAP), eine Plattform zur Richtliniendurchsetzung, die im Funktionsumfang der Betriebssystemfamilie Windows Server Longhorn enthalten sein wird. Weitere Information über NAP finden Sie in „Anhang A: Netzwerkzugriffsschutz“ am Ende dieses Dokuments.

Komponenten der Quarantänesteuerung für IAS-Netzwerkzugriff

![](images/cc875843.pnfuc05(de-de,technet.10).gif)

**Abbildung 5. Komponenten der Windows-Quarantänesteuerung für IAS-Netzwerkzugriff**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875843.pnfuc05_big(de-de,technet.10).gif)
 

In der obigen Abbildung sind die typischen Komponenten einer Windows-Remotezugriffslösung dargestellt, bei der die Quarantänesteuerung für IAS-Netzwerkzugriff verwendet wird. Hierzu gehören folgende Komponenten:
* **Quarantänekompatibler RAS-Client.**   Diese Komponente besteht aus einem Computer mit einer Windows-Version, die mit dem Verbindungs-Manager-Verwaltungskit erstellte CM-Profile unterstützt. Das Verbindungs-Manager-Verwaltungskit ist Teil von Windows Server 2003. Windows Betriebssysteme ab Windows 98 Second Edition unterstützen diese Profile. Auf solchen Clientcomputern müssen eine Benachrichtigungskomponente und ein Netzwerkrichtlinien-Anforderungsskript vorhanden sein. Außerdem müssen sie so konfiguriert sein, dass das Skript als Nachverbindungsaktion ausgeführt wird.

* **Quarantänekompatibler RAS-Server.**   Diese Komponente besteht aus einem Computer mit Windows Server 2003, auf dem Routing und Remotezugriff (RAS) ausgeführt werden. Diese Funktion unterstützt die Verwendung einer Listenerkomponente und der anbieterspezifischen RADIUS-Attribute „MS-Quarantine-IPFilter“ und „MS-Quarantine-Session-Timeout“ zusammen mit einer installierten Listenerkomponente.

* **Quarantänekompatibler RADIUS-Server.**   Dies ist eine optionale Komponente. Sie kommt zum Einsatz, wenn die RADIUS-Authentifizierung auf dem RAS-Server mit Windows Server 2003 und IAS konfiguriert ist, so dass die anbieterspezifischen RADIUS-Attribute „MS-Quarantine-IPFilter“ und „MS-Quarantine-Session-Timeout“ unterstützt werden.

* **Quarantäneressourcen.**   Diese Komponenten sind die Server und Dienste, auf die der Remoteclient im Quarantänemodus Zugriff hat. Normalerweise bestehen sie aus den Servern, die DNS-Dienste, CM-Profile oder Sicherheitsupdate-Anbieter bereitstellen, um Clients richtlinienkonform zu machen.

* **Kontendatenbank.**   Normalerweise ist diese Komponente die Active Directory-Domäne, in der das Konto des Remotebenutzers und die DFÜ-Eigenschaften gespeichert sind.

* **Quarantäne-RAS-Richtlinie.**   Diese Richtlinie ist notwendig, um die erforderlichen Verbindungen für Remotezugriffsverbindungen bereitzustellen und die Attribute „MS-Quarantine-IPFilter“ oder „MS-Quarantine-Session-Timeout“ festzulegen.


Tief greifende Verteidigung

![](images/cc875843.pnfuc06(de-de,technet.10).gif)

**Abbildung 6. Tief greifende Verteidigung und Quarantänesteuerung für IAS-Netzwerkzugriff**

Wie diese Anpassung des Modells der tief greifenden Verteidigung von Microsoft zeigt, erstreckt sich die VPN-Quarantäne über drei Ebenen des Modells: Host, internes Netzwerk und Umkreis. Wenngleich diese Lösung den Client nicht direkt sichert, trägt sie zur Sicherung von Servern gegenüber Bedrohungen bei, die von nicht richtlinienkonformen Remoteclients ausgehen. Indirekt sichert diese Lösung auch die Remoteclients, indem sie dafür sorgt, dass diese die Richtlinien erfüllen, um effektiv zu funktionieren. Dadurch wird ein Anreiz geschaffen, die jeweils aktuellen Updates zu verwenden.

Überdies verbessert diese Lösung den Schutz des Netzwerks selbst vor Unterbrechungen, die durch falsch konfigurierte Rogue-Remotecomputer hervorgerufen werden können, u. a. auch durch Remotecomputer, die Malware verbreiten, was eine vernichtende Wirkung auf die Netzwerkleistung haben kann. Obwohl der Umkreis keine Bedeutung zu haben scheint, da diese Lösung Brute-Force-Angriffe auf das VPN (das sich am Umkreis befindet) nicht direkt verhindert, bietet er eine weitere Sicherheitsschicht, die ein Angreifer durchdringen müsste, um direkten Zugriff auf Ressourcen im internen Netzwerk zu erlangen, auch wenn er in den Besitz gültiger Anmeldeinformationen gelangt wäre.

802.1X-Authentifizierung zum Schutz vor nicht verwalteten drahtlosen Geräten

Die Verwendung des Standards IEEE (Institute of Electrical and Electronic Engineers) 802.1X ist eine gute Möglichkeit, drahtlose Netzwerke vor Missbrauch durch Unbefugte zu schützen. Dabei wird, einfach ausgedrückt, jedem Computer die Kommunikation im Netzwerk versagt, sofern er nicht als autorisierter Computer konfiguriert wurde. Wenngleich diese Lösung in drahtlosen Netzwerken gut funktioniert, ist sie in drahtgebundenen Netzwerken weniger effektiv, auch wenn dieser Standard grundsätzlich auch für solche Netzwerke verwendet werden kann. Seine begrenzte Effektivität ist der Grund, weshalb in diesem präskriptiven Dokument eine kombinierte Lösung zur Sicherung von Netzwerken in mittelgroßen Unternehmen empfohlen wird. Durch eine Kombination der wirksamsten Konzepte zur Sicherung der einzelnen Aspekte eines typischen Unternehmensnetzwerks kann eine robuste Lösung zur tief greifenden Verteidigung erzielt werden.

IEEE 802.1X-Authentifizierung

Die IEEE 802.1X-Authentifizierung ist eine portbasierte Zugriffssteuerungsmethode, die sich so konfigurieren lässt, dass sie eine gegenseitige Authentifizierung zwischen den Clients und dem Netzwerk verlangt. Dadurch kann kein Gerät, das sich nicht authentifizieren lässt, an einer Kommunikation mit dem jeweiligen Netzwerk teilnehmen.

802.1X unterstützt EAP (Extensible Authentication Protocol). Dieses Protokoll existiert in verschiedenen Varianten. Drei davon werden von den aktuellen Versionen von Microsoft Windows serienmäßig unterstützt:
* **EAP-MD5.**   Mit MD5 sendet ein Authentifizierungsserver eine In-Frage-Stellung an einen Client (Bittsteller), und dieser Bittsteller kombiniert die Anforderung der In-Frage-Stellung mit seinem eigenen Bezeichner und eigener Passphrase. Diese Antwort wird in einen MD5-Hash ungewandelt und an den Authentifizierungsserver zurückgesendet, der die Antwort entschlüsselt und mit der ursprünglichen In-Frage-Stellung vergleicht. Wenn die Antwort übereinstimmt, erfolgt die Authentifizierung. Dieses Methode ist in den meisten Implementierungen nicht wirklich sicher, da das Kennwort selbst gesendet wird und somit von Dritten abgefangen und entschlüsselt werden kann.

* **Geschütztes EAP.**   Beim geschützten EAP (PEAP) werden vom Client stammende serverseitige Zertifikats- und Authentifizierungsinformationen (z. B. Benutzernamen und Kennwörter) verwendet, um die gegenseitige Authentifizierung durchzuführen. Die Microsoft-Implementierung dieses Standards verwendet MS-CHAP, Version 2, wobei die Authentifizierung mit herkömmlichen Domänenkonto- und Kennwortinformationen und einem RADIUS-Server erfolgt. Diese Methode gilt im Allgemeinen als ausreichend sicher für kleinere Umgebungen, bei denen der zusätzliche Infrastruktur- und Verwaltungsaufwand der EAP-TLS-Methode aus Kostengründen nicht in Frage kommt.

* **EAP-TLS.**   Mit dieser Methode richtet ein Authentifizierungsserver eine TLS-Sitzung (Transport Layer Security) für den Bittsteller ein, bei der dem Client ein digitales Zertifikat zugesendet wird. Der Bittsteller überprüft dieses Zertifikat bei dessen Empfang und sendet daraufhin sein eigenes Zertifikat, das wiederum vom Authentifizierungsserver überprüft wird. Sofern beide Seiten das Zertifikat der jeweils anderen Seite akzeptieren, findet die Authentifizierung statt. Diese Methode eignet sich am besten für Netzwerke, die eine PKI-Infrastruktur sowie RADIUS-Authentifizierungsserver unterstützen. Sie ist auch die sicherste verfügbare Option für drahtlose Netzwerke, insbesondere in Kombination mit dem Standard 802.11i WPA2.


Bevor ein Client eine Authentifizierung durchführen kann, muss er auf den Authentifikator (einen Drahtloszugriffspunkt oder Netzwerkswitch) zugreifen, bis er selbst durch den authentifizierenden Server authentifiziert ist. Deshalb wird während des anfänglichen Authentifizierungshandshakes die gesamte Kommunikation durch den Authentifikator zwischen dem Bittsteller und dem Authentifizierungsserver weitergeleitet. Wenn die Authentifizierung abgeschlossen ist, kann der Bittsteller direkt auf das Netzwerk zugreifen.

Weshalb 802.1X für drahtgebundene Netzwerke wenig bringt

Wenngleich 802.1X im Allgemeinen zur Erhöhung der Sicherheit von drahtlosen Netzwerken beiträgt, bringt diese Methode hinsichtlich der Sicherung von drahtgebundenen Netzwerken einige Probleme mit sich. Das erste Problem ist Folgendes: Obwohl 802.1X über einige Active Directory-Gruppenrichtlinienobjekte verfügt, die seine Implementierung in drahtlosen Netzwerken unterstützen, unterstützt es in drahtgebundenen Netzwerken keine 802.1X-Authentifizierung. Deshalb würde 802.1X bei einer solchen Implementierung ein beträchtliches Maß an Verwaltungsaufwand erfordern. Zudem unterstützen viele Switches, Netzwerkdruckgeräte und andere drahtgebundene Netzwerkinfrastrukturgeräte den Standard 802.1X nicht. Somit ist bei den meisten Netzwerken mittelgroßer Unternehmen die Wahrscheinlichkeit groß, dass kostspielige Aktualisierungen installiert werden müssten, um diese Implementierung zu unterstützen.

Neben den Verwaltungs- und Infrastrukturkosten einer solchen Implementierung ergeben sich auch einige Sicherheitsprobleme, wenn dieser für drahtlose Netzwerke konzipierte Standard für drahtgebundene Netzwerke verwendet wird. Da die 802.1X-Authentifizierung beispielsweise nur stattfindet, wenn eine Verbindung hergestellt wird und Hubs für 802.1X nicht erkennbar sind, müsste ein Angreifer lediglich einen Hub sowie einen authentifizierten Computer und einen „Schattencomputer“, mit dem der Angriff ausgeführt würde, an das interne Netzwerk anschließen.

**Hinweis**   Drahtlose Netzwerke sind von diesen spezifischen Nachteilen und Anfälligkeiten nicht betroffen. Diese Probleme in Verbindung mit der 802.1X-Sicherheit ergeben sich nur in Zusammenhang mit drahtgebundenen Netzwerken.

Sie sind der Grund, weshalb für die Domänen- und Serverisolation IPsec statt 802.1X empfohlen wird. Diese Empfehlung bedeutet jedoch nicht, dass in Netzwerken mittelgroßer Unternehmen kein Platz für 802.1X ist. Wie bereits erwähnt, ist 802.1X ein wertvolles Hilfsmittel, das zur Steigerung der Sicherheit im Drahtlosbereich dient und durch das Hinzufügen einer IPsec-basierten Netzwerkisolationslösung nur noch sicherer werden kann.

Tief greifende Verteidigung

![](images/cc875843.pnfuc07(de-de,technet.10).gif)

**Abbildung 7. Tief greifende Verteidigung mit 802.1X-Sicherheit für drahtlose Netzwerke**

Wie die obige Abbildung verdeutlicht, setzt die Sicherheitslösung mithilfe der 802.1X-Authentifizierung für drahtlose Umgebungen an der Netzwerkschicht des Modells zur tief greifenden Verteidigung an. Wenngleich es so scheinen mag, dass sich die Drahtlossicherheit auch auf den Umkreis erstreckt, sind drahtlose Netzwerke eigentlich ein Teil eines lokalen Netzwerks, während der Umkreis eher mit externen Netzwerken wie dem Internet zu tun hat. Einige Teilbereiche der Drahtlossicherheit verfügen über Hostkomponenten, doch die Drahtlossicherheit ist nicht für den direkten Schutz des Hosts vorgesehen.

SMS zum Erkennen und Absichern nicht verwalteter Systeme

Microsoft Systems Management Server (SMS) 2003 wird häufig zu folgenden Zwecken eingesetzt: Verwalten von Computern in einem Netzwerk, Handhaben von Inventarinformationen und Bereitstellen von Software und Updates zur Wahrung der Konformität mit Sicherheitsrichtlinien sowie zur Instandhaltung der Gesamtinstallation von Plattform und Software. Die Netzwerkermittlungs- und Bestandsaufnahmefunktionen von SMS 2003 gehören zum Themenbereich dieses Dokuments, da sie eine Methode bereitstellen, mit der nicht vertrauenswürdige Systeme beim Herstellen einer Verbindung zum Netzwerk besser erkannt werden können. Diese Funktionen tragen auch zu einer Absicherung dieser Systeme bei, wobei es darauf ankommt, welche Richtlinien als Antwort auf die Verwendung nicht verwalteter Computer implementiert werden.

In diesem Dokument wird davon ausgegangen, dass der Leser bereits SMS und andere Methoden nutzt, um Domänenmitgliedscomputer in Übereinstimmung mit den Sicherheitsrichtlinien zu bringen. Dies bedeutet, dass auch alle aktuellen Sicherheitsupdates installiert sein müssen. Deshalb wird auf die verschiedenen Aspekte der Patchverwaltung mittels SMS 2003 und anderer Tools im Rahmen dieses Dokuments nicht weiter eingegangen. Mehr zu diesen Themen sowie weitere SMS-bezogene Informationen finden Sie auf der Solution Accelerator-Seite [Microsoft Systems Management Server](http://www.microsoft.com/technet/itsolutions/cits/mo/swdist/pmsms/2003/pmsms031.mspx">Patchverwaltung mit Systems Management Server 2003 (möglicherweise in englischer Sprache) unter www.microsoft.com/technet/itsolutions/cits/mo/swdist/pmsms/2003/pmsms031.mspx oder auf der 

Ermitteln und Dokumentieren vorhandener Ressourcen

In Unternehmen, die bereits SMS implementiert haben, ist die Dokumentation der vorhandenen Ressourcen wahrscheinlich bereits abgeschlossen, und die Bestandsliste verwalteter und nicht verwalteter Systeme ist komplett. Eine solche Bestandsliste sollte auch Informationen über die erforderlichen Sicherheitsupdates und Verfahren für Computer enthalten, die nicht durch SMS verwaltet werden, sei es aufgrund ihrer Bauart oder weil sie keine funktionierenden Agents für den jeweiligen Clienttyp sind. Zu solchen nicht verwalteten Computern können auch Geräte in einem Sicherheitsumkreis (auch DMZ, Demilitarized Zone und überwachtes Subnetz genannt) sowie Testcomputer oder Einzelplatzgeräte zählen.

Es ist wichtig, die Geräte, die nicht durch SMS verwaltet werden, sorgsam in einer Liste zu dokumentieren, und zwar nicht nur aus Gründen der Sicherheit, sondern auch, weil eine solche Liste für Vergleiche mit neuen Bestandsinformation erforderlich ist, so dass festgestellt werden kann, ob neu erkannte Systeme autorisiert oder unbekannt sind. Um solche Listen aktuell zu halten, muss ein Verfahren für die Hinzufügung neuer nicht verwaltbarer Systeme zum Unternehmensnetzwerk definiert sein, mit dem die Informationen nicht nur erfasst werden, sondern mit dem auch die Sicherheit solcher Systeme sowie Eigentumszuweisungen verwaltet werden können.

Wenngleich SMS über solche nicht verwaltete Systeme unter Umständen nicht sehr viel mehr Informationen als die IP-Adresse und einen Namen erfassen kann, reichen diese Informationen oftmals schon aus, um festzustellen, ob das jeweilige Netzwerkgerät autorisiert ist oder nicht.


#### Entwicklung

Im Abschnitt „Leistungsnachweise“ wurde gezeigt, dass sich eine Mischung verschiedener Lösungen, die spezifische Funktionen im Netzwerk eines mittelgroßen Unternehmens durchführen, als umfassendste Methode zum Schutz dieses Netzwerks erweist. Die Domänen- und Serverisolation schützt das drahtgebundene Netzwerk, indem sie nur bekannten und verwalteten Computern den Zugriff auf vertrauenswürdige Ressourcen gestattet. Die VPN-Quarantäne gewährleistet, dass Remotesysteme, die nur gelegentlich Verbindungen zum Netzwerk herstellen, dauerhaft den Sicherheitsrichtlinien entsprechen. Die 802.1X-Authentifizierung sichert das drahtlose Netzwerk dadurch, dass sie nur autorisierte Computer Verbindungen herstellen lässt. SMS trägt seinerseits dazu bei, dass vertrauenswürdige Computer den Richtlinien entsprechen und nicht vertrauenswürdige Rogue-Computer erkannt werden, wenn sie eine Verbindung zum Netzwerk herstellen. Durch die Kombination all dieser Lösungen lässt sich ein Netzwerk wirksam vor nicht autorisierten Verbindungen und Rogue-Computern schützen.

Neben den Anforderungen an eine Implementierung dieser Lösungen werden in diesem Abschnitt auch einige potenzielle Probleme behandelt, die es zu vermeiden gilt, damit die einzelnen Lösungen in der jeweiligen Unternehmensumgebung möglichst effektiv funktionieren.

Isolieren von Domänen und Servern mittels IPsec

Beim Entwickeln eines Plans zur Implementierung der IPsec-basierten Domänen- und Serverisolation muss unter anderem entschieden werden, ob diese Lösung in der jeweiligen Netzwerkumgebung umsetzbar ist; ferner müssen die nötigen Voraussetzungen zur Entwicklung eines Implementierungsplans ermittelt werden. Das Konzept der IPsec-Netzwerkisolation wurde im Abschnitt „Leistungsnachweise“ dieses Dokuments vorgestellt. Nun, da die Vorteile dieses Konzepts bekannt sind, können sie den möglichen Problemen gegenübergestellt werden, die die Implementierung einer IPsec-Netzwerkisolation mit sich bringt. Diese Probleme sowie die Anforderungen an eine solche Implementierung werden in diesem Abschnitt als Entscheidungshilfe erörtert.

Identifizieren der Netzwerkarchitektur

Da IPsec im Internetprotokoll selbst angesiedelt ist, ist ein detailliertes Verständnis der aktuellen Netzwerkinfrastruktur und des Datenverkehrsflusses für eine erfolgreiche Bereitstellung dieser Lösung unabdingbar. Während Informationen bezüglich IP-Adressierungsschemata, Subnetzlayouts und Netzwerkdatenverkehrsmustern wichtige Komponenten sind, die es zu identifizieren gilt, ist eine detaillierte Dokumentation der Netzwerksegmentierung und ein aktuelles Modell des Datenverkehrsflusses im Netzwerk absolut erforderlich, damit ein effektiver Netzwerkisolationsplan entwickelt und bereitgestellt werden kann.

**Hinweis**   Auf das Dokumentieren der Netzwerkumgebung kann im Rahmen dieses Dokuments nicht detailliert eingegangen werden. Das Erstellen einer solcher Dokumentation ist für den Erfolg umfassender Netzwerksicherheitsinitiativen von entscheidender Bedeutung, darunter auch für die hier vorgestellte Lösung. Fehlt eine solche Dokumentation, so ist die Umsetzung einer derartigen Lösung mit unkalkulierbaren Risiken behaftet.

In der Dokumentation der Netzwerkarchitektur sollten die folgenden Informationen detailliert erfasst sein:
* Detail- und Ortsangaben zu Firewalls und Lastenausgleichsfunktionen

* Informationen zu Netzwerkgeräten, einschließlich Speichergröße, Hersteller/Modell und MTU-Einstellungen

* Berichte über Netzwerkdatenverkehr und Netzwerkauslastung

* NAT-Nutzung

* VLAN-Segmentierung

* Gerätenetzwerkverbindungen

* Angaben zu Einbruchserkennungssystemen (IDS)


Identifizieren des Netzwerk-Datenverkehrsflusses

Neben Informationen über Geräte und Konfigurationen, die für die IPsec-basierte Netzwerkisolation von Bedeutung sein können, ist es wichtig, innerhalb des Netzwerks herrschende Datenverkehrsmuster zu untersuchen. Beim Erfassen dieser Informationen ist unter anderem zu bedenken, wie Nicht-Windows-Geräte (z. B. Linux-Computer) oder Geräte, auf denen ältere Windows-Versionen als Windows 2000 SP4 verwendet werden, mit anderen Windows-basierten Systemen kommunizieren. Darüber hinaus sind folgende Überlegungen anzustellen:
* Sind Subnetze für bestimmte Arten von Datenverkehr vorhanden, etwa für die Kommunikation mit Mainframes?

* Muss der Datenverkehr zwischen bestimmten Standorten getrennt werden?

* Gibt es Arten von Datenverkehr, die besonders hohe Sicherheit durch Verschlüsselung erfordern, etwa die Kommunikation mit einer Personaldatenbank?

* Sind Sicherheitsgeräte oder Firewallregeln vorhanden, die sich auf die Implementierung auswirken können, etwa die Blockierung von UDP-Port 500?

* Wie erfolgt die Kommunikation von Anwendungen? Verwenden die Anwendungen zum Beispiel Remoteprozeduraufrufe (RPCs), die zusätzlich berücksichtigt werden müssen?

* Wie kommunizieren Hosts und Server miteinander? Verwenden sie Verbindungen auf Port-/Protokollebene, oder stellen sie mehrere Sitzungen über viele verschiedene Protokolle her?


Identifizieren der Active Directory-Struktur

Um festzustellen, welche mögliche Auswirkung die IPsec-Implementierung auf eine Active Directory-Struktur hat, ist es wichtig, neben den oben genannten Informationen auch Informationen über die Active Directory-Gesamtstruktur, das Domänenlayout, das Organisationseinheitendesign und die Standorttopologie zu sammeln. Im Einzelnen geht es dabei um folgende Angaben:
* Anzahl der Gesamtstrukturen

* Anzahl und Namen der Domänen

* Anzahl und Arten der Beziehungen

* Anzahl und Namen der Standorte

* Organisationseinheiten- und Gruppenrichtlinienstruktur

* Eventuell vorhandene Informationen zu IPsec-Richtlinien (sofern IPsec aktuell verwendet wird)


Identifizieren von Hosts

Bezüglich Hosts müssen unter anderem folgende Informationen erfasst werden:
* Computernamen

* IP-Adressen, insbesondere statische Adressen

* MAC-Adressen

* Betriebssystemversion, einschließlich Service Pack- und Hotfix-Versionsnummern

* Domänenmitgliedschaft

* Physischer Standort

* Typ und Aufgabe der Hardware


Identifizieren von Aspekten der IPsec-Kapazität

Beim Entwickeln eines IPsec-Implementierungsplans sind auch einige Aspekte der Kapazitätsplanung zu berücksichtigen, insbesondere, wenn die Verwendung der IPsec-Verschlüsselung in Frage kommt, da diese ein bestimmtes Maß an Hostauslastungs- und Netzwerkreserven erfordert. Zu berücksichtigen sind unter anderem folgende Aspekte:
* **Speicherauslastung des Servers.**   Jede Sitzung kann bis zu 5 KB an Arbeitsspeicher benötigen.

* **CPU-Auslastung des Servers****,****der Arbeitsstationen****,****und der Infrastrukturgeräte.**   Diese Information ist vor allem für Server von Bedeutung. Vergewissern Sie sich, dass keines der Geräte bereits überlastet ist.

* **Latenz und Auslastung des Netzwerks.**   Durch die Verwendung von IPsec erhöht sich die Latenz. Als Microsoft bei sich IPsec einführte, stieg die Netzwerkauslastung um 1 bis 3 Prozent.

* **Verwendung von NAT und Verschlüsselungstyp.**   Die AH-Kommunikation kann NATs nicht traversieren. Deshalb müsste die Kommunikation stattdessen mit ESP verschlüsselt werden. ESP überlastet den Server stärker als die AH-Verschlüsselung (Ausnahme: ESP-Null-Verschlüsselung).

* **Auswirkung von Gruppenrichtlinien.**   IPsec-Gruppenrichtlinienobjekte haben eine Auswirkung darauf, wie lange der Computerstart und verschiedene Anmeldevorgänge dauern. Durch entsprechende Testimplementierungen sollten diese Zeiten im Vergleich zur Situation ohne Implementierung ermittelt werden.


Identifizieren von Vertrauensstufen

Ein weiterer wichtiger Aspekt ist es, festzustellen, welche Hosts an dieser Lösung in welcher Kapazität beteiligt sind. Um dies festzustellen, muss zunächst klar definiert sein, welche Bedingungen erfüllt werden müssen, um vertrauenswürdig zu sein, und welche möglichen Vertrauensstufen vorhanden sind. Die folgenden Informationen können hierbei als Hilfestellung dienen. Sie bieten einige klare Definitionen der Vertrauenswürdigkeit, der zu erfüllenden Kriterien für verschiedene Stufen der potenziellen Vertrauenswürdigkeit sowie der Art, wie diese Kriterien den Planungsprozess beeinflussen.

Ein Host kann die folgenden vier Stufen der Vertrauenswürdigkeit aufweisen (von höchster bis niedrigster Vertrauenswürdigkeit):
* **Vertrauenswürdig.**   Der Status „vertrauenswürdig“ bedeutet, dass die Sicherheitsrisiken des Hosts bereits verwaltet werden und andere vertrauenswürdige Hosts keinen böswilligen Angriff von ihm zu befürchten haben. Wenngleich dieser Status nicht unbedingt bedeutet, dass der jeweilige Host vollkommen sicher ist, signalisiert er, dass die Vertrauenswürdigkeit dieses Hosts der Verantwortung einer IT-Abteilung unterliegt und durch einen bestimmten automatischen oder dokumentierten Prozess verwaltet wird.

Da dieser Host vertrauenswürdig ist, sollte die Kommunikation zwischen ihm und anderen vertrauenswürdigen Hosts nicht durch die Netzwerkinfrastruktur behindert werden. Da man sicher annehmen kann, dass von diesem Host kein böswilliger Angriff ausgeht, besteht keine Notwendigkeit, den von ihm stammenden Datenverkehr durch Firewalls oder ähnliche Vorkehrungen zu blockieren.

* **Potenziell vertrauenswürdig.**   Der Status „potenziell vertrauenswürdig“ bedeutet, dass der Computer, obwohl er prinzipiell zu einem vertrauenswürdigen Gerät werden kann, immer noch einige zusätzliche Konfigurationsänderungen oder bestimmte Aktualisierungen erfordert, um als vertrauenswürdig zertifiziert werden zu können. Das Identifizieren solcher Computer ist vor allem während der Entwurfsphase äußerst wichtig, da es gewisse Rückschlüsse auf den Arbeits- und Kostenaufwand erlaubt, der zum Aufbau eines isolierten Netzwerks erforderlich ist.

* **Bekannt****,****nicht vertrauenswürdig.**   Es gibt verschiedene Gründe, weshalb ein bekannter Computer möglicherweise nicht in der Lage ist, zu einer vertrauenswürdigen Ressource zu werden, beispielsweise finanzielle Beschränkungen, geschäftliche Erfordernisse oder sogar funktionelle Anforderungen. So ist möglicherweise das Projektbudget zu gering, um alle Computer entsprechend zu aktualisieren, einige Unternehmensbereiche besitzen möglicherweise eigene Domänen, oder eine ältere Anwendung ist eventuell nicht mit den aktuell unterstützten Betriebssystemen kompatibel und kann deshalb auf einem gesicherten Computer nicht ausgeführt werden.

Welcher Grund auch immer vorliegt: Mit dem Eigentümer des bekannten, aber nicht vertrauenswürdigen Computers sollte geklärt werden, ob es möglich ist, den Computer richtlinienkonform zu machen, und wie die Situation unter Wahrung eines akzeptablen Risikoprofils gehandhabt werden kann.

* **Unbekannt****,****nicht vertrauenswürdig.**   Der Status „unbekannt, nicht vertrauenswürdig“ sollte der Standardstatus aller Hosts sein. Hosts mit diesem Status sind nicht verwaltet, und ihre Konfigurationen sind unbekannt. Deshalb kann ihnen kein anderer Vertrauensstatus verliehen werden. Es sollte davon ausgegangen werden, dass diese Hosts manipuliert und als Plattform für böswillige Aktivitäten genutzt werden können, so dass sie für das Unternehmen ein nicht akzeptables Risiko darstellen. Mit der genannten Lösung lässt sich das Gefahrenpotenzial solcher Systeme verringern.


Verwenden der erfassten Informationen

Wenn alle relevanten Informationen erfasst wurden, kann ein Implementierungsplan erstellt und festgestellt werden, ob die IPsec-basierte Netzwerkisolation für die derzeitige Netzwerkumgebung eine geeignete Lösung ist. Die Entscheidung für oder gegen eine Implementierung dieser Lösung kann unter anderem durch folgende Aspekte beeinflusst werden:
* Kosten für benötigte Aktualisierungen, um Hosts in den vertrauenswürdigen Status zu bringen und mit den IPsec-Anforderungen kompatibel zu machen

* Kosten für Aktualisierungen oder Ersatz der Infrastruktur, wenn IPsec von den aktuellen Netzwerkgeräten nicht unterstützt wird

* Ausgleich des möglichen Verlusts an routerbasierter QOS (Dienstqualität) und der Sicherheitsvorteile der Netzwerkisolation, da die portbasierte Priorisierung nicht funktioniert, wenn zwar IPsec implementiert ist, aber die IP-Adressen-basierte QOS weiterhin aktiv ist

* Netzwerküberwachungssysteme und IDS-Geräte können ausfallen, wenn IPsec implementiert wird, insbesondere bei Verwendung der ESP-Verschlüsselung. Mithilfe von Parsern lässt sich das Problem lösen, sofern für das Gerät ein IPsec-Parser verfügbar ist.

* Für die Implementierung von IPsec sind aufgrund des höheren Aufwands und der Anforderungen an CPU und Arbeitsspeicher bei Servern und Netzwerkgeräten möglicherweise Hardwareaktualisierungen erforderlich.

* Erwartungsmanagement kann ein entscheidender Aspekt sein, da die Netzwerklatenz unter Umständen ansteigt.

* Auch das Zulieferer- und Gastbenutzermanagement kann einen übermäßigen Aufwand erzeugen, da es sich hierbei um Benutzer mit nicht vertrauenswürdigen Geräten handelt, die möglicherweise aus geschäftlichen Gründen Zugriff auf Netzwerkressourcen im isolierten Netzwerk benötigen. Solche Ausnahmen sind mit steigender Zahl und Häufigkeit eventuell schwierig zu handhaben. Die Gefahren lassen sich jedoch mithilfe einer Grenzzone zwischen vertrauenswürdigen und nicht vertrauenswürdigen Netzwerken abmildern.


Diese Probleme verdeutlichen, weshalb sorgfältiges Planen und Testen notwendig ist, bevor Änderungen implementiert werden, die das gesamte Netzwerk betreffen, beispielsweise die Implementierung von IPsec und Netzwerkisolation. All diese Punkte sollten sorgfältig durchdacht werden, um nicht nur zur klären, wie die Lösung implementiert werden kann, sondern auch, ob die Implementierung angesichts des aktuellen Netzwerkzustands und der finanziellen und unternehmenspolitischen Kosten für die Absicherung des Netzwerks überhaupt machbar ist. Darüber hinaus sollten begrenzte oder schrittweise Bereitstellungen, die nur bestimmte Zielressourcen isolieren, als mögliche alternative Gefahrenabmilderungsstrategien in Erwägung gezogen werden.

Auch hierbei ist die IPsec-basierte Netzwerkisolation nur ein Teil einer umfassenden Lösung. Jede in dieser Anleitung vorgestellte Lösung ist ein Beitrag zum Schutz vor nicht vertrauenswürdigen Geräten, die Verbindungen zum Netzwerk herstellen können, doch auch jeder Bestandteil der jeweiligen Lösung erhöht bereits die Sicherheit eines beliebigen Netzwerks. Selbst wenn also die IPsec-Domänen- und Serverisolation momentan keine annehmbare Lösung ist, kann es sinnvoll sein, die anderen hier genannten Lösungen zu implementieren und vielleicht auf die Netzwerkisolation zurückzukommen, wenn das betreffende Netzwerk weiter ausgereift und mit den in diesem Dokument genannten Anforderungen kompatibel ist.

VPN-Quarantänedienste zum Schutz vor nicht verwalteten Remotecomputern

Bei einer standardmäßigen Windows-basierten RAS-Server-Sitzung führt der Server die folgenden Aktionen aus, wenn ein RAS-Client eine Sitzung initiiert:
1. Der RAS-Server überprüft den RAS-Client auf Einhaltung der konfigurierten RAS-Richtlinien und lässt die Verbindung zu.

2. Der Server überprüft die Remotezugriffsberechtigungen des Benutzers.

3. Anschließend authentifiziert der Server die Anmeldeinformationen des Benutzers mittels Active Directory oder eines anderen Authentifizierungsdiensts.

4. Der Server weist dem Remoteclient eine IP-Adresse zu.


Ab diesem Zeitpunkt hat der Remoteclient vollen Zugriff auf das Netzwerk, wobei noch keine Überprüfungen bezüglich Updateversionen, Vorhandensein oder Aktualisierungsstatus von Antivirensoftware oder sonstigen Informationen in Zusammenhang mit Sicherheitsrichtlinien vorgenommen wurden. Diese Funktionalität ist nicht optimal, da sie mitunter dazu führt, dass Updates, Konfigurationsänderungen oder Patches auf Remote- oder Roaming-Computer nicht angewendet werden.

Eine VPN-Quarantäneverbindung unterscheidet sich hiervon grundlegend, wie aus der folgenden Abbildung und der nummerierten Liste hervorgeht:

![](images/cc875843.pnfuc08(de-de,technet.10).gif)

**Abbildung 8. VPN-Quarantäneprozess**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875843.pnfuc08_big(de-de,technet.10).gif)
 
1. Der Remoteclient führt ein Verbindungs-Manager-Vorverbindungsskript aus, das die wichtigsten Verbindungsvoraussetzungen überprüft (z. B. Sicherheitsupdateversion und Datum der Virensignaturdatei) und das Ergebnis speichert. Nachdem dieses Skript ausgeführt wurde, stellt der Client eine Remotezugriffssitzung über einen VPN-Tunnel her.

2. Der RAS-Server authentifiziert die Benutzeranmeldeinformationen mittels RADIUS. Dabei werden die Anmeldeinformationen mithilfe von Active Directory überprüft.

3. Nachdem der Benutzer durch Active Directory authentifiziert wurde, stellt der RAS-Server den Client unter Quarantäne, indem er die RAS-Richtlinie anwendet. Während des Verweilens im Quarantänezustand beschränkt sich der Netzwerkzugriff auf die in der Quarantänerichtlinie definierten Bereiche. Dieser eingeschränkte Zugriff lässt sich durch einen IP-Filter erzielen, der den Zugriff auf bestimmte Ressourcen beschränkt, durch die der Client in Einklang mit den Richtlinien gebracht werden kann, oder durch ein Zeitlimit, nach dessen Überschreitung die Verbindung zum Client getrennt wird.

4. Ein Nachverbindungsskript informiert den RAS-Server darüber, ob der Client den festgelegten Anforderungen entspricht. Wenn die Verbindung innerhalb eines bestimmten Zeitlimits nicht den Anforderungen entspricht, wird dies dem Benutzer mitgeteilt, und die Verbindung wird abgebrochen.

5. Wenn das Nachverbindungsskript meldet, dass der Client die festgelegten Anforderungen erfüllt, befreit der RAS-Server den Client aus dem Quarantänemodus, indem er die IP-Filterbeschränkungen aufhebt, und gewährt dem Client dadurch Zugriff auf die in der RAS-Richtlinie definierten Netzwerkressourcen.


Ein RAS-Client kann nur auf Ressourcen zugreifen, die sich innerhalb des festgelegten Quarantänenetzwerks befinden, egal, ob dieses Netzwerk ein separates Subnetz oder eine definierte Gruppe von Internet-orientierten Servern ist. Ein Quarantänenetzwerk sollte die Ressourcen bereitstellen, mit denen ein Remoteclient die nötigen Aktivitäten ausführen kann, um einen Remotecomputer mit den Sicherheitsstandards in Einklang zu bringen. Im Allgemeinen zählen dazu folgende Ressourcen: die Zugriffsmöglichkeit auf einen DNS-Server für die Namensauflösung, ein Dateiserver, von dem Updates abgerufen werden können sowie eventuell ein Webserver für Anweisungen oder webbasierte Updates.

Die Verwendung eines Quarantänesubnetzes in diesem Prozess würde längere Sitzungszeitlimits erfordern, um zu gewährleisten, dass für das Herunterladen und Installieren von Updates auf den Remoteclientcomputer genügend Zeit zur Verfügung steht. Um dieses Problem zu umgehen, könnte der Clientcomputer angewiesen werden, andere Quellen oder Internet-orientierte Updateserver außerhalb der VPN-Sitzung zu verwenden, wenngleich hierzu ein komplexeres Skript erforderlich wäre und andere Sicherheitsprobleme entstehen könnten. In beiden Fällen ist es das Skript, das das Quarantäneverhalten bestimmt, nicht das Quarantänenetzwerk selbst.

**Hinweis**   IPsec-Richtlinien können als Skript erstellt werden, wenn in der Quarantänelösung auch Systeme berücksichtigt werden müssen, die nicht der Domäne angehören. In diesen Fällen können mit „netsh“ oder „lpseccmd.exe“ einfache Richtlinien mit Zertifikaten zum Unterstützen der IPsec-Authentifizierung angewendet werden. IPsec kann auch für der Domäne angehörende Systeme in VPN-Quarantänekonfigurationen sowie in mehrschichtigen Lösungen eingesetzt werden.

Komponenten des VPN-Quarantäneclients

Wie im vorangehenden Abschnitt erwähnt, beginnt der VPN-Quarantäneprozess immer mit dem Client, genauer gesagt, mit dem Verbindungs-Manager-Vorverbindungsskript. Verbindungs-Manager ist Teil des Verbindungs-Manager-Verwaltungskits (CMAK), das die Herstellung und Verwaltung von Netzwerkverbindungen zentralisiert und automatisiert. Zudem unterstützt das CMAK folgende wichtige Bereiche der VPN-Quarantänekonfiguration:
* Vorverbindungssicherheitsprüfungen zur automatischen Verwaltung von Clientcomputerkonfigurationen

* Nachverbindungssicherheitsprüfungen und Anmeldungsüberprüfungen


Mit dem Verbindungs-Manager können Administratoren über Profile individuelle Aktionen definieren, die dann an zahlreiche Computer verteilt werden können. Diese Möglichkeit vereinfacht den Verbindungsprozess für Remotebenutzer, da sie die Anzahl der Einstellungen begrenzt, die geändert werden können. Zu den Einstellungen, die sich ändern lassen, gehören folgende:
* Festlegen von Telefonlisten, die für DFÜ-Verbindungen verwendet werden können

* Ändern von Grafiken, Symbolen, Nachrichten und Hilfetext

* Ausführen von benutzerdefinierten Vor- und Nachverbindungsaktionen, zum Beispiel Zurücksetzen des Dialerprofils oder Konfigurieren der Paketfilterregeln für die Windows-Firewall


Eine weitere CMAK-Komponente ist der Client-Agent (RQC.exe), der über TCP-Port 7250 mit dem Remotezugriffsquarantänedienst (RQS.exe) auf dem RAS-Server kommuniziert. Wenn eine Quarantäneverbindung hergestellt wird, sendet der RQS dem RQC einen geheimen gemeinsamen Schlüssel. Wenn der Client die notwendigen Bedingungen erfüllt, sendet der RQC den gemeinsamen Schlüssel, um den Client aus der Quarantäne zu befreien.

Die Verbindungs-Manager-Profile sind selbstextrahierende, benutzerdefinierte Client-Dialerpakete für den Verbindungs-Manager, die mithilfe von CMAK erstellt und konfiguriert werden können. Der CMAK-Assistent führt den Administrator durch den Prozess der Konfiguration des Profils, das dann mit verschiedenen Methoden – von Gruppenrichtlinien bis Microsoft Systems Management Server (SMS) 2003-Softwareverteilung – verteilt werden kann. Wenn die erstellte ausführbare Datei auf dem Clientcomputer ausgeführt wird, erstellt sie das Profil auf dem lokalen Computer, zusammen mit den notwendigen Einstellungen zum Herstellen der Kommunikation mit RAS-Servern. Nach Abschluss der Installation braucht der Benutzer nur den Profilnamen im Windows XP-Menü **Verbinden mit** zu initiieren, um eine Verbindung herzustellen.

Weitere Information über das CMAK finden Sie auf der Seite [Verbindungs-Manager-Verwaltungskit](http://technet2.microsoft.com/windowsserver/en/library/be5c1c37-109e-49bc-943e-6595832d57611033.mspx?mfr=true) im Microsoft TechNet unter http://technet2.microsoft.com/WindowsServer/en/library/be5c1c37-109e-49bc-943e-6595832d57611033.mspx?mfr=true.

Komponenten des VPN-Quarantäneservers

Der VPN-RAS-Server ist der zentrale Bestandteil dieser Lösung. Er erfüllt folgende Funktionen:
* Er führt den RAS-Quarantänedienst (RQS.exe) aus.

* Er wendet RAS-Richtlinien auf Quarantänezugriffseinstellungen an.

* Er handelt die Kommunikation mit dem Client-Agent aus.

* Er empfängt Informationen zur Richtlinienkonformität vom Client-Agent.

* Er wendet RAS-Richtlinien an, um Zugriffsberechtigungen für Netzwerkressourcen zu ermitteln.


Der RAS-Quarantänedienst ist eine optionale Komponente von Windows Server 2003 mit Service Pack 1. Er unterstützt die APIs, die notwendig sind, um Remoteclientcomputer unter Quarantäne zu stellen, und befreit die Computer wieder aus dem Quarantänemodus, sobald der Client-Agent meldet, dass die Richtlinien erfüllt sind. Dieser Dienst (RQS.exe) überwacht TCP-Port 7250 auf etwaige Benachrichtigungen von der clientseitigen Komponente (RQC.exe) darüber, dass der Clientcomputer die Anforderungen der Richtlinie erfüllt. Diese Funktionalität bedeutet, dass alle vorhandenen Firewalls, darunter auch hostbasierte Firewalls, den Datenverkehr an TCP-Port 7250 zulassen müssen, damit diese Lösung funktioniert.

Komponenten des VPN-Quarantänenetzwerks

Im Folgenden sind sowohl erforderliche als auch optionale Netzwerkkomponenten aufgeführt, die, wie oben erwähnt, Teil der VPN-Quarantänenetzwerklösung sein können.
* **IAS-RADIUS-Server (empfohlen).**   Obwohl IAS-Server (Internetauthentifizierungsdienst-Server) nur benötigt werden, wenn RADIUS als Authentifizierungsanbieter verwendet wird, bieten sie einige überzeugende Vorteile gegenüber anderen Authentifizierungslösungen, beispielsweise Unterstützung von EAP (Extensible Authentifizierung Protocol) für die Zweifaktorauthentifizierung mittels Zertifikat und Smartcard. Wenn RADIUS verwendet wird, empfiehlt sich die Verwendung von IAS (im Lieferumfang von Windows Server 2003 enthalten) als RADIUS-Anbieter, da IAS die anbieterspezifischen Attribute „MS-Quarantine Session Timeout“ und „MS-Quarantine-IPFilter“ unterstützt, was bei anderen RADIUS-Servern möglicherweise nicht der Fall ist.

* **Active Directory (empfohlen).**   Active Directory dient als Datenbank für die Benutzerkontenauthentifizierung mit RADIUS und lässt sich in IAS und andere Dienste integrieren. In Kombination mit IAS kann Active Directory die Zweifaktorauthentifizierung mit Zertifikaten und anderen Methoden unterstützen.

* **DHCP-Server (empfohlen).**   DHCP-Server dienen der Bereitstellung von IP-Adressen für Remoteclients.

* **DNS-Server (empfohlen).**   Ein DNS-Server stellt die erforderlichen Namensauflösungsdienste bereit, so dass Clients im Quarantänenetzwerk gegebenenfalls Verbindungen zu anderen Servern herstellen können, die ihrerseits dazu beitragen, dass die Remoteclientcomputer die Richtlinien einhalten.

* **WSUS-Server (optional).**   WSUS-Server (Windows Software Update Service-Server) stellen die Sicherheitsupdates und Hotfixes bereit, mit denen Remotecomputer die nötigen Voraussetzungen erfüllen können, um aus dem Quarantänezustand entlassen zu werden. Andere Methoden, wie SMS 2003 oder standardmäßige Windows-Updatedienste, könnten ebenfalls verwendet werden, wenn die Computer ersatzweise an externe Quellen weitergeleitet werden sollen.

* **Dateiserver (optional).**   Mithilfe von Dateiservern können Freigaben bereitgestellt werden, in denen unter Quarantäne gestellte Computer auf Softwareupdates und Antiviren-Signaturdateien zugreifen können, um die vorgegebenen Richtlinien zu erfüllen.

* **Webserver (optional).**   Webserver können bei Quarantäne dafür sorgen, dass die Benutzer die Anweisungen erhalten, die sie benötigen, um ihren Computer aus dem Quarantänezustand zu befreien. Einige Updatepakete verwenden auch Webkomponenten, etwa bestimmte Antivirenprodukte, für die Übermittlung.


802.1X-Authentifizierung zum Schutz vor nicht verwalteten drahtlosen Geräten

Im vorangehenden Abschnitt wurde die 802.1X-Authentifizierung als die derzeit wirksamste Option zum Sichern von drahtlosen Netzwerken gegenüber nicht vertrauenswürdigen Computern vorgestellt. Dabei wurden die verschiedenen 802.1X-Methoden beschrieben, die in einigen aktuellen Versionen von Microsoft Windows nativ unterstützt werden, und es wurde erläutert, weshalb die 802.1X-Authentifizierung für drahtgebundene Netzwerke weniger effektiv ist (obwohl sie für drahtlose Netzwerke sehr effektiv ist). Mit diesem Hintergrundwissen ist es nun möglich, die Unterschiede zwischen den unterstützten Methoden aufzuzeigen und zu bestimmen, welche Methode sich für die verschiedenen Netzwerktypen mittelgroßer Unternehmen am besten eignet.

802.1X-Methoden im Vergleich

Wie erwähnt, unterstützen aktuelle Microsoft Windows-Versionen drei verschiedene 802.1X-Methoden, nämlich:
* EAP-MD5

* Geschütztes EAP (PEAP)

* EAP-TLS


Von diesen drei Methoden gilt die erste (EAP-MD5) als die unsicherste, da hierbei Passphrasen per Funk übertragen und somit abgefangen werden könnten. Die anderen beiden Methoden (PEAP und EAP-TLS) kommen für den Einsatz im Netzwerk eines mittelgroßen Unternehmens in Frage.

Die Microsoft-Implementierung von PEAP verwendet das Microsoft Challenge Handshake Authentication Protocol, Version 2 (MS-CHAP 2), das ursprünglich als DFÜ-VPN-Authentifizierungsmethode konzipiert wurde, aber auch gut für PEAP geeignet ist, da es die Richtlinien für sichere Kennwörter unterstützt, die über Active Directory bereitstehen. Dieses Konzept lässt sich leichter als EAP-TLS implementieren und erfordert weniger Ressourcen und Anfangsinvestitionen, da hierfür weniger zusätzliche Server und Dienste notwendig sind. Obwohl diese Lösung Zertifikate für die Authentifizierungsserver erfordert, könnten diese Zertifikate von entsprechenden Drittanbietern generiert werden, da sie für die Implementierung nur in kleiner Zahl benötigt werden.

EAP-TLS gilt jedoch als die sicherste verfügbare 802.1X-Authentifizierung, da hierbei sowohl auf dem Client als auch auf dem Authentifizierungsserver Zertifikate für eine gegenseitige Authentifizierung verlangt werden. Weil für eine solche Implementierung sehr viele Zertifikate nötig wären, ist es sinnvoller, zu ihrer Unterstützung eine Public Key-Infrastruktur zu implementieren, sofern noch keine vorhanden ist. Somit gilt EAP-TLS hinsichtlich der Implementierungs- und Supportkosten im Vergleich zu PEAP mit MS-CHAP 2 als teurere Lösung.

Der Entscheidungsprozess für 802.1X

Damit Sie leichter entscheiden können, welche Implementierung von 802.1X sich für Ihre jeweilige Netzwerkumgebung am besten eignet, hat Microsoft den folgenden Entscheidungsbaum für die 802.1X-Authentifizierung entwickelt.

![](images/cc875843.pnfuc09(de-de,technet.10).gif)

**Abbildung 9. Der Entscheidungsbaum für 802.1X**

Dieses Flussdiagramm ist insofern etwas verwirrend, als darin von „großen Unternehmen“ die Rede ist. Hiermit sind im Allgemeinen Unternehmen gemeint, die über mindestens 500 Mitarbeiter und eine IT-Abteilung mit mindestens 5 Technologieexperten verfügen. Damit ist klar, dass sich beide Lösungen auch für Unternehmen mittlerer Größe eignen. Somit richtet sich der Entscheidungsprozess eher nach der Risikobereitschaft und der Kosteneffizienz.

Der Hauptunterschied zwischen PEAP und EAP-TLS besteht in der Notwendigkeit einer Zertifikatinfrastruktur. Deshalb wird EAP-TLS eher den Anforderungen größerer Unternehmen gerecht, während PEAP im Allgemeinen für kleinere Unternehmen ausreicht, sofern keine speziellen Vorschriften einen strengeren Sicherheitsstandard erfordern. Abgesehen von den finanziellen Aspekten besteht bei manchen Unternehmen zusätzlicher Bedarf an einer Zertifikatinfrastruktur, wodurch eine Investition in PKI noch stärker gerechtfertigt ist. Denn wenn zahlreiche Zertifikate für sicheren Webinhalt oder für Codesignierungszwecke benötigt werden, ist es nur vernünftig, auch eine Infrastrukturinvestition in die Implementierung der sichersten Form der 802.1X-Authentifizierung zu tätigen.

Voraussetzungen für 802.1X PEAP

Ein Microsoft-basiertes PEAP mit MS-CHAP 2-Implementierung würde mindestens zwei IAS RADIUS-Server erfordern, damit ein Authentifizierungsserver den drahtlosen Client anhand einer Active Directory-Kontendatenbank authentifizieren könnte. Die Anzahl der RADIUS-Server muss eventuell neu angepasst werden, um der Anzahl der Remotesites gerecht zu werden bzw. um mehr Benutzerauthentifizierungsversuche berücksichtigen zu können.

Das Vorhandensein von Remotestandorten erfordert nicht automatisch zusätzliche IAS RADIUS-Server. Wenn jedoch Remotestandorte keine redundanten Verbindungen mit hoher Bandbreite aufweisen oder bereits über eigene Domänencontroller und andere lokale Ressourcen verfügen, sollten für solche Sites zusätzliche Authentifizierungsserver hinzugefügt werden.

Voraussetzungen für 802.1X EAP-TLS

Wie bereits oben erwähnt, erfordert EAP-TLS aufgrund der zusätzlich benötigten Zertifikate mehr Ressourcen als PEAP-Implementierungen. Es ist natürlich möglich, Drittanbieter die notwendigen Zertifikate für alle drahtlosen Clients und Authentifizierungsserver ausstellen zu lassen, doch dieser Ansatz ist kostspieliger als die Implementierung einer Zertifikatinfrastruktur, es sei denn, die Anzahl der drahtlosen Clients beschränkt sich wirklich nur auf einige wenige Benutzer.

Insgesamt erfordert eine einfache EAP-TLS-Implementierung mindestens vier Server, gegebenenfalls mehr für größere Unternehmen oder für geografisch verteilte Netzwerke. Zwei der vier Server fungieren als IAS RADIUS-Server, die anderen zwei als Zertifikatinfrastruktur. Einer der beiden Zertifikatsserver (der Stammzertifikatsserver) sollte außerhalb des Netzwerks eingerichtet werden und normalerweise nicht mit dem Netzwerk verbunden sein. Auf diese Weise kann unter bestimmten Umständen ein Server eingespart werden.

WEP oder WPA

Hinsichtlich der Sicherheit in drahtlosen Netzwerken stellt sich auch die Frage, ob Verschlüsselung verwendet werden soll, und wenn ja, nach welchem Standard. Auf die Verschlüsselung des drahtlosen Datenverkehrs zu verzichten, kann für ein Unternehmen mittlerer Größe höchstens dann in Frage kommen, wenn aus geschäftlichen Gründen öffentlich zugängliche Internetverbindungen bereitgestellt werden müssen. Ansonsten ist für die Sicherheit eines drahtlosen Netzwerks nicht nur die 802.1X-basierte Authentifizierung notwendig, sondern auch die Verschlüsselung des Datenverkehrs in irgendeiner Form.

Die Verschlüsselung des drahtlosen Datenverkehrs erfolgt in zwei Hauptformen sowie in einer zusätzlichen Variante:
* **WEP.**   Der Standard WEP (Wired Equivalent Privacy) war Teil des ursprünglichen Standards IEEE 802.11, bei dem die drahtlose Kommunikation mit 64-Bit- oder 128-Bit-RC4-Verschlüsselung gesichert wird. Bei dieser Technik wurden einige ernste Mängel erkannt, die diese Verschlüsselungsmethode äußerst anfällig gegenüber passiven Abhörangriffen machen. Inzwischen sind verschiedene Tools frei erhältlich, mit denen sich WEP-Übertragungen in relativ kurzer Zeit, mitunter binnen weniger Minuten, dekodieren lassen. Generell ist WEP somit nicht für Unternehmensumgebungen zu empfehlen. Es kann jedoch mit verschiedenen Methoden, etwa mit 802.1X-Authentifizierung, ein wenig sicherer gestaltet werden.

* **WPA.**   Als Antwort auf die Schwächen des WEP-Standards entwickelte ein Konsortium aus führenden Organisationen der Branche, darunter auch Microsoft und das Wi-Fi Institute, den Standard WPA (Wi-Fi Protected Access) als partielle Implementierung des Standards 802.11i, der sich damals noch im Entwicklungsstadium befand. Dieser Standard ermöglicht eine viel sicherere Verschlüsselung mithilfe des TKIP (Temporal Key Integrity Protocol), die dem mängelbehafteten Standard WEP weit überlegen ist. Die meisten heute erhältlichen Drahtloszugriffspunkte (WAPs) unterstützen den Standard WPA, ebenso wie alle aktuellen Versionen des Betriebssystems Microsoft Windows.

* **WPA2.**   Der Standard WPA2 (Wireless Protected Access 2) wurde im September 2004 von der Wi-Fi Alliance eingeführt. Dieser Standard ist als vollwertige Implementierung der im Juni 2004 ratifizierten Spezifikation IEEE 802.11i zertifiziert. Er unterstützt 802.1X-basierte EAP-Authentifizierungsmethoden bzw. die PSK-Technologie (mitunter auch „WPA im persönlichen Modus“ genannt), verfügt jedoch über die weiterentwickelte Verschlüsselungsmethode AES (Advanced Encryption Standard), für die CCMP (Counter-Mode/CBC-MAC Protocol) genutzt wird. Diese Implementierung der drahtlosen Verschlüsselung ist äußerst sicher. Die meisten Anbieter unterstützen WPA2 in irgendeiner Form, so auch die aktuellen Versionen des Betriebssystems Microsoft Windows.


WPA2 oder WPA sollte zur Absicherung drahtlos übertragener Daten verwendet werden, wo immer dies möglich ist. Diese Möglichkeit besteht unter Umständen nicht, wenn bereits beträchtliche Investitionen in eine Drahtlostechnologie getätigt wurden, die diese neuen Standards nicht unterstützt. Wie bereits erwähnt, kann die Sicherheitsstufe, die WEP bietet, dadurch erhöht werden, dass die 802.1X-Authentifizierung und häufige Änderungen der Schlüsselpaare konfiguriert werden. Dennoch sollte sich die Verwendung von WEP auf drahtlose Netzwerke beschränken, die sich im Übergangsstadium auf den Standard WPA oder WPA2 befinden.

SMS zum Erkennen nicht verwalteter Systeme

Microsoft Systems Management Server (SMS) 2003 ist in einem Microsoft-Netzwerk ein sehr vielseitiges Verwaltungstool. Mit SMS lassen sich mehrere Verwaltungsfunktionen zentralisieren, darunter die Softwarebereitstellung, die Bereitstellung von Sicherheitsaktualisierungen und die Systemüberprüfung. Das zentrale Element dieser Funktionen ist die Möglichkeit, den Systembestand automatisch und zentral zu erfassen, von dem aus diese überaus nützlichen Tools bereitgestellt werden können. Hierbei kommt die Erkennung der nicht verwalteten Systeme ins Spiel.

SMS 2003 bietet verschiedene Ermittlungsmethoden, mit denen Administratoren die Computersammlungsdatenbank aufbauen können, in der Informationen über jeden Computer im Netzwerk gespeichert werden. Diese Ermittlungsmethoden reichen von der Active Directory-basierten Ermittlung (bei der die Sammlung mit Details aus der Active Directory-Computerkontenliste aktualisiert wird) bis zur Netzwerkerkennung (bei der das Netzwerk aktiv auf angeschlossene Geräte abgesucht wird). Diese Ermittlungsmethoden lassen sich so konfigurieren, dass sie in vorgegebenen Intervallen stattfinden und anschließend die Sammlungsdatenbanken aktualisieren.

Um dem Erfordernis gerecht zu werden, nicht verwaltete Systeme zu erkennen, wenn diese eine Verbindung zum Netzwerk herstellen, kann die Netzwerkermittlung so konfiguriert werden, dass sie häufiger stattfindet und die Ergebnisse anschließend in regelmäßigen Zeitabständen ausgewertet werden, um festzustellen, wann ein neues System mit dem Netzwerk verbunden wurde. Wenn solche Systemverbindungen stattfinden, können sie mit einer festgelegten Liste neuer Computerversionen oder Netzwerkverbindungsanforderungen verglichen werden, um zu bestätigen, dass das neue System für die Verwendung des Netzwerks autorisiert ist.

Netzwerkermittlungsprozess

Einer der Nachteile dieses Ansatzes zur Ermittlung nicht verwalteter Systeme ist die Tatsache, dass SMS unter Umständen nicht die Details von Computern erkennt, die andere Betriebssysteme als Microsoft Windows verwenden. Tatsächlich lassen sich selbst Vorgängerversionen von Microsoft Windows 98 SE nicht unbedingt mit den SMS 2003-Ermittlungsmethoden aufspüren, da sie die WMI-Implementierungen (Windows Management Interface) nicht unterstützen. Deshalb ist es notwendig, diesem Lösungsprozess Skripts hinzuzufügen, so dass jedes neue Gerät erkannt wird, sobald es an das Netzwerk angeschlossen wird. Die folgende Abbildung verdeutlicht, wie ein solcher Prozess abläuft.

![](images/cc875843.pnfuc10(de-de,technet.10).gif)

**Abbildung 10. Ermittlung nicht verwalteter Computer mittels SMS**

Diese Abbildung zeigt die Ermittlungsmethoden, mit denen verschiedene Computertypen in die SMS-Sammlungsdatenbank aufgenommen werden können. Dabei müssen drei verschiedene Arten von Computern berücksichtigt werden:
* **Für SMS zugängliche verwaltete Systeme.**   Diese Computer können von SMS verwaltet werden und sind bereits der Verwaltung durch SMS unterstellt. Sie sind bereits in der SMS-Sammlungsdatenbank gespeichert und sollten für die automatische Verwaltung konfiguriert sein. Sie würden wahrscheinlich als Bestandteil des vertrauenswürdigen Netzwerks betrachtet werden und erfordern keine weitere Aufmerksamkeit.

* **Für SMS zugängliche nicht verwaltete Systeme.**   Diese Computer lassen sich von SMS verwalten, sind aber noch nicht der Verwaltung durch SMS unterstellt. Ob sie von SMS erkannt werden, hängt davon ab, an welcher Stelle des Netzwerks sie sich befinden (z. B. vor oder hinter einer Firewall), und es kann sich dabei auch um Computer handeln, die auf andere Art verwaltet werden. Diese Computer sollten in einer gesonderten Liste verzeichnet sein, zusammen mit Details zur ihrer Verwaltung. Ist dies nicht der Fall, sollten sie als nicht vertrauenswürdig betrachtet und eventuell näher untersucht werden. Sie können von SMS erkannt werden, wobei jedes Netzwerkgerät ausgesperrt wird, das eine solche Aktivität blockiert.

* **Für SMS nicht zugängliche, nicht verwaltete Systeme.**   Diese Computer lassen sich nicht von SMS verwalten und sind nicht der Verwaltung durch SMS unterstellt. Hierzu können auch bekannte Systeme gehören, die auf andere Art verwaltet werden. Diese Computer sollten in einer gesonderten Liste verzeichnet sein, die auch Details zur Verwaltung erhält. Ist dies nicht der Fall, sollten sie als unbekannt und nicht vertrauenswürdig betrachtet und näher untersucht werden. Diese Computer können nur mit anderen Prozessen als der SMS-Ermittlung erkannt werden, beispielsweise mit benutzerdefinierten Ermittlungsskripts.


An diese Stelle sollte klar sein, dass die Ermittlung nicht verwalteter Systeme im Netzwerk von der Festlegung von Prozessen abhängt, die die Details jeder autorisierten Computerverbindung im Netzwerk dokumentieren. In einer solchen Dokumentation sollten auch Detailangaben zum Computer sowie Informationen darüber vorhanden sein, ob der Computer durch automatisierte Methoden (wie SMS) verwaltet wird, und wenn nicht, durch welchen Prozess die Konformität des Computers mit den gegebenenfalls festgelegten Sicherheitsrichtlinien gewährleistet wird. Natürlich könnte ein autorisierter Computer in einem Netzwerk vorhanden sein, ohne dass er die Sicherheitsstandards erfüllen muss. Solche Computer sollten jedoch zwangsweise in einem nicht vertrauenswürdigen Netzwerksegment verbleiben, der vom vertrauenswürdigen Netzwerk isoliert ist.

Wenn ein dokumentierter Computerhinzufügungsprozess eingerichtet ist, der alle Computer dokumentiert, von denen bekannt ist, dass sie in autorisierter Form im Netzwerk vorhanden sind, kann anhand dieser Informationen bestimmt werden, was autorisiert ist und was nicht. Alle im Netzwerk erkannten Computer, die nicht auf dieser Liste stehen, sollten als verdächtig angesehen und sofort näher untersucht werden.


#### Bereitstellung und Verwaltung

Im Abschnitt „Entwicklung“ wurde erläutert, welche Details zum Erstellen von Bereitstellungsplänen erforderlich sind. Der vorliegende Abschnitt behandelt nun ausführlich einige wichtige Aspekte und Prozesse der Bereitstellung und bietet dadurch Technikern eine Hilfestellung bei der Implementierung dieser Lösungen und Entscheidungsträgern einen besseren Einblick in ihre Besonderheiten, so dass sie eine fundierte Entscheidung darüber treffen können, ob diese Lösungen für eine bestimmte Umgebung geeignet sind.

Isolieren von Domänen und Servern mittels IPsec

Aufgrund der Komplexität in Zusammenhang mit der IPsec-basierten Netzwerkisolation empfiehlt es sich, die Bereitstellung dieser Lösung in einem Produktionsnetzwerk in mehreren Phasen durchzuführen. Die phasenweise Bereitstellung kann auf mehrere Arten durchgeführt werden, je nachdem, wie die IPsec-Richtlinien bereitgestellt werden: nach Gruppen oder nach Richtlinien.

Egal, welche Methode verwendet wird: Es ist wichtig, während der Anfangsphasen der Bereitstellung Pilotbeispiele aus jeder Gruppe zu verwenden und die Auswirkung dieser Lösung in einer Testumgebung zu überprüfen, sofern dies möglich ist. Der Bereitstellung von IPsec sollte ein formeller Anforderungsprozess zur Änderungssteuerung vorausgehen, in dem Rollbackpläne sowie das informierte Einverständnis von Technologie- und betroffenen Unternehmensprozesseigentümern ausführlich dargelegt sind.

Bereitstellen von IPsec nach Gruppe

Zum Bereitstellen der IPsec-Netzwerkisolation nach Gruppe werden vollständig definierte IPsec-Richtlinien verwendet, wobei die Implementierung jedoch über ACLs an den Gruppenrichtlinienobjekten (GPOs) gesteuert wird, die die Richtlinien bereitstellen. Alle IPsec-Richtlinien verfügen über Ausnahmen und sichere Subnetze, die zusammen mit allen zugehörigen, vor der Bereitstellung aktivierten Filteraktionen vollständig definiert sind.

Nach erfolgter Konfiguration erstellen die Administratoren GPOs für jede IPsec-Richtlinie sowie Computergruppen zum Verwalten dieser GPOs. Anschließend werden den GPOs die entsprechenden IPsec-Richtlinien zugewiesen, und die GPOs werden mit den entsprechenden Objekten in Active Directory verknüpft. Keine der Richtlinien sollte an diesem Punkt des Prozesses übermittelt werden, da die ACLs, die die GPO-Zuweisung steuern, leer sind.

Wenn Pilotcomputer identifiziert wurden, können die jeweiligen Computerkonten in den entsprechenden Computergruppen platziert werden, und die IPsec-Richtlinie wird angewendet, nachdem das nächste GPO-Abfrageintervall verstrichen ist. Bei der phasenweisen Erweiterung der Bereitstellungsliste um zusätzliche Computer können deren jeweilige Konten in den entsprechenden Gruppen für die Richtlinienübermittlung platziert werden.

Diese Methode erfordert sorgfältige Planung, um sicherzustellen, dass die Kommunikation nicht unterbrochen wird. Würde beispielsweise ein Server, der als Host für eine Anwendung diente, die von allen Hosts verwendet wurde, in einer sicheren Gruppe platziert, für die IPsec-verschlüsselte Kommunikation erforderlich wäre, so würde die Kommunikation mit Computern, die noch nicht zu Gruppen hinzugefügt wurden, sowie mit allen Hosts, die die IPsec-Verschlüsselung nicht verwenden können, unterbrochen.

Bereitstellen von IPsec nach Richtlinie

Bei dieser Bereitstellungsmethode werden die IPsec-Richtlinien erst während der Bereitstellung und nicht bereits vor der tatsächlichen Produktionsbereitstellung erstellt. Dabei enthalten die anfänglichen IPsec-Richtlinien nur Ausnahmelisten ohne festgelegte Regeln für Computer, um die Sicherheit auszuhandeln. Nach dem Übermitteln der anfänglichen Richtlinie können Administratoren eine Sicherheitsregel mit einem Filter erstellen, der nur ein einziges Subnetz betrifft. Mit fortschreitender Bereitstellung können der sicheren Regel weitere Subnetze hinzugefügt werden, bis die Richtlinie den Bereitstellungsendzustand erreicht.

Der Vorteil dieser phasenweisen Bereitstellung besteht darin, dass IPsec nur für einen kleinen Teil des gesamten TCP/IP-Datenverkehrs und nicht für alle Subnetze ausgehandelt wird, wie dies bei einem gruppenweisen Vorgehen der Fall wäre. Zudem bietet diese Methode die Möglichkeit, alle Netzwerkpfade von einem einzelnen Subnetz zu testen, so dass bei etwaigen Problemen weniger Clients betroffen sind. Der Nachteil dieser Methode ist, dass sie auf alle Computer der Isolationsdomäne oder -gruppe angewendet wird und nicht, wie beim gruppenweisen Vorgehen, auf spezifische Computer. Außerdem müssen alle Computer mit der dreisekündigen Verzögerung für das Fallback auf Klartext zurechtkommen, wenn Verbindungen mit den jeweiligen Subnetzen hergestellt werden.

Diese Methode eignet sich gut für komplexe Netzwerke mit mehreren Subnetzen, ist jedoch für kleinere Netzwerke mit relativ wenigen Subnetzen nur bedingt attraktiv.

Ausnahmelisten

Auch ein noch so gut aufgebautes Netzwerkisolationsmodell unterliegt einigen Einschränkungen, wenn es in einer Produktionsumgebung implementiert werden soll. In der Regel bringen wichtige Komponenten einer Netzwerkumgebung, wie DNS-Server und Domänencontroller, einige Herausforderungen mit sich, die es zu bewältigen gilt. Solche Systeme müssen einerseits gesichert werden, aber andererseits auch für alle Systeme im Netzwerk verfügbar sein. Deshalb müssen sie für eingehende Verbindungsanforderungen offen sein. Probleme können sich auch ergeben, wenn es um die Umsetzung des Plans in der Produktionsumgebung geht. Für solche Probleme gibt es jedoch eine Lösungsmöglichkeit: Ausnahmelisten.

Eine Ausnahmeliste ist eine Liste der Computer, die nicht mit IPsec gesichert werden können und daher in jeder IPsec-Richtlinie implementiert werden müssen. Da IPsec nur eine statische Filterung unterstützt, lässt jeder Host, der einer Ausnahmeliste hinzugefügt wird, ausgehenden wie eingehenden Datenverkehr von allen Teilen des Netzwerks zu, egal, ob diese vertrauenswürdig sind oder nicht. Aus diesem Grund sollte die Ausnahmeliste so kurz wie möglich gehalten werden, da die jeweiligen Hosts zusätzlichen Schutz durch Serverabsicherung und hostbasierte statusbehaftete Firewallfilterung benötigen, um die Risiken zu mindern, die von nicht verwalteten Geräten ausgehen. Unter Umständen kann es auch sinnvoll sein, die Hosts der Ausnahmeliste zur leichteren Verwaltung in einem einzelnen Subnetz oder VLAN zu platzieren oder Serverfunktionen zusammenzufassen, um die Anzahl der Ausnahmehosts zu verringern.

Zu den Hosts, die wahrscheinlich einer Ausnahmeliste hinzugefügt werden müssen, gehören folgende:
* Domänencontroller, da sie die IPsec-Kommunikation mit Domänenmitgliedern nicht unterstützen, obwohl sie IPsec-Richtlinien für Domänenmitglieder bereitstellen und die Kerberos-Authentifizierung durchführen, auf der die Netzwerkisolation basiert

* Hosts, deren Leistung in inakzeptablem Maß beeinflusst wird, beispielsweise Hosts, die tausende Clients gleichzeitig verwalten müssen, oder Hosts, auf die sich die dreisekündige Fallback-auf-Klartext-Verzögerung auswirkt, etwa DHCP-Server

* Hosts, die über keine kompatible IPsec-Implementierung verfügen oder Dienste für vertrauenswürdige und nicht vertrauenswürdige Computer bereitstellen, aber IPsec nicht verwenden


Ebenso wie für die Grenzgruppe sollte für Hosts, die in die Ausnahmelisten aufgenommen werden müssen, ein formeller Genehmigungsprozess vorhanden sein.

**Hinweis**   Für Microsoft Windows XP und Windows Server 2003 steht das Hotfix „Simple Policy“ (einfache Richtlinie) zur Verfügung, das Ausnahmelisten überflüssig macht. Weitere Informationen hierzu finden Sie im Knowledge Base-Artikel [914841](http://support.microsoft.com/?kbid=914841) unter http://support.microsoft.com/?kbid=914841 und im Knowledge Base-Artikel [914842](http://support.microsoft.com/?kbid=914842) unter http://support.microsoft.com/?kbid=914842 (möglicherweise in englischer Sprache).

Aspekte der IPsec-Verwaltung

Sobald IPsec-Richtlinien implementiert sind, wirken sie sich auf die Kommunikation zwischen vielen Hosts im Netzwerk aus. Deshalb können sich Änderungen, die nach der Bereitstellung erfolgen, für viele Benutzer deutlich bemerkbar machen. Aus diesem Grund sollten alle Änderungen, die an einem IPsec-basierten Isolationsnetzwerk vorgenommen werden, nach einem standardisierten MOF-Änderungsmanagementprozess erfolgen, der folgende Schritte umfasst:
* Änderungsanforderung (RFC)

* Änderungsklassifizierung

* Änderungsautorisierung

* Änderungsentwicklungsplan

* Änderungsfreigabeplan

* Änderungsüberprüfung


Microsoft empfiehlt die Verwendung von Windows Server 2003 als IPsec-Verwaltungsplattform. Zur Erleichterung von Verwaltungsaufgaben können Administratoren entweder das IP-Sicherheitsrichtlinien-Snap-In für MMC oder das Befehlszeilentool Netsh in der Konsole von Windows Server 2003 verwenden. Ansonsten ist die Verwaltung von IPsec-Richtlinien eine recht unkomplizierte Angelegenheit, da sie mithilfe der Gruppenrichtlinie übermittelt wird. Somit lässt sich das Hinzufügen neuer Computer zum vertrauenswürdigen Netzwerk automatisieren, sofern ein festgelegter „Computerhinzufügungsprozess“ verwendet wird.

Einige Dinge müssen jedoch berücksichtigt werden, wenn Änderungen in Erwägung gezogen werden:
* Alle Änderungen an einer Filteraktion, die für eine IPsec-SA verwendet wurde, bewirken, dass festgelegte SAs unter diesen Richtlinieneinstellungen gelöscht werden. Diese Funktionalität erstellt einen neuen Schnellmodusversuch, wenn Datenverkehr unterwegs ist, was zu Ausfällen des Netzwerkverkehrs führen kann.

* Eine Änderung der Authentifizierungsmethode oder der Hauptmodus-Sicherheitsmethode führt dazu, dass IKE vorhandene Hauptmodi löscht. Unter bestimmten Umständen kann diese Funktionalität bewirken, dass serverseitige IKE-Hauptmodusverhandlungen mit Clients fehlschlagen.

* Wenn IPsec-Richtlinien in einem GPO geändert werden, finden bestimmte Verzögerungen statt (darunter die Active Directory-Replikationsverzögerung und die GPO-Abfrageverzögerung), die – je nach Umfang und Komplexität der Umgebung – einige Minuten bis Stunden anhalten können.


Ein weiterer Aspekt der Verwaltung ist die Frage, wie verdächtige Computer bei Infizierungen isoliert werden sollen. Es gibt verschiedene Möglichkeiten, mit böswilligen Aktivitäten umzugehen:
* **Isolieren der Isolationsdomäne.**   Indem Sie den IPsec-Filter „Sicherer Anforderungsmodus“ so ändern, dass unsichere Kommunikation deaktiviert wird, kann das isolierte Netzwerk vollständig vom nicht vertrauenswürdigen Netzwerk getrennt werden, wenn ein nicht vertrauenswürdiges Gerät in Verdacht steht, eine Plattform für böswillige Aktivitäten zu sein.

* **Blockieren verdächtiger Ports.**   Indem Sie Filterlisten mit zwei unidirektionalen Filtern erstellen, können Sie Datenverkehr an spezifischen Ports blockieren. Diese Methode sollte mit Vorsicht verwendet werden, da auch notwendiger Datenverkehr wie etwa DNS blockiert werden kann, wodurch sich weitere IPsec-Änderungen oder -Rollbacks schwierig gestalten würden.

* **Isolation in untergeordneten Domänen.**   Indem Sie die Richtlinien für eine Domäne so ändern, dass ein vordefinierter Schlüssel statt des Kerberos-Protokolls für die IPsec-Authentifizierung verwendet wird, können Sie eine Domäne von anderen Domänen einer Gesamtstruktur isolieren.

* **Isolation in vordefinierten Gruppen.**   Indem Sie statt des Kerberos-Protokolls vordefinierte Schlüssel oder Zertifikate für die IPsec-Authentifizierung verwenden, können Sie Isolationsgruppen erstellen, bei denen mit verschiedenen Schlüsseln oder Zertifikaten dieselbe Art von Isolationsfunktionalität erzielt wird.

VPN-Quarantänedienste zum Schutz vor nicht verwalteten Remotecomputern

Die eigentliche Bereitstellung der VPN-Quarantänesteuerung erfordert sechs Schritte zusätzlich zu allen anderen Anforderungsprozessen des Änderungsmanagements und Testprozessen vor der Bereitstellung, die in einem Unternehmen vorhanden sein können. Dabei handelt es sich um die folgenden sechs Schritte:

1. Erstellen von Quarantäneressourcen

2. Erstellen von Skripts zum Überprüfen der Clientkonfigurationen

3. Installieren der Listenerkomponente Rqs.exe auf RAS-Servern

4. Erstellen von Verbindungs-Manager-Profilen (CM-Profilen) für die Quarantäne mit Windows Server 2003 CMAK

5. Verteilen der CM-Profile an RAS-Clientcomputer

6. Konfigurieren der Quarantäne-RAS-Richtlinie

1. Erstellen von Quarantäneressourcen

Wenn unter Quarantäne gestellte Clients interne Ressourcen verwenden sollen, um sich in einen Zustand zu bringen, der den geltenden Sicherheitsrichtlinien entspricht, muss eine Gruppe von zugänglichen Ressourcen vorhanden sein, mit denen die Clients die nötigen Updates und andere Software installieren können, die für die Sicherheit benötigt werden. Wie im vorangegangen Abschnitt ausführlich beschrieben, gehören zu diesen Ressourcen normalerweise ein Namensserver sowie Dateiserver und mitunter auch Webserver. Das Festlegen dieser Quarantäneressourcen kann auf verschiedene Art erfolgen, beispielsweise durch das Festlegen vorhandener Server, die sich im internen Netzwerk befinden, oder durch Platzieren der erforderlichen Ressourcen in einem eigenen separaten Subnetz.

Mit der ersten Methode, dem Festlegen einzelner Server, lassen sich eventuell die Kosten für die Anschaffung von Servern zur Bereitstellung von Updates einsparen, da ja bereits vorhandene Server verwendet werden. Allerdings sind für diese Methode komplexe Paketfilter erforderlich, da jede Ressource eine eigene Gruppe von Filtern im Attribut „MS-Quarantine-IPFilter“ der Quarantäne-RAS-Richtlinie benötigt.

Für die andere Methode, das Platzieren sämtlicher Quarantäneressourcen in einem eigenen Subnetz für Quarantänedienste, müssen der Netzwerkumgebung möglicherweise zusätzliche Server hinzugefügt werden, allerdings wird hierbei nur ein einziger Eingangs- und Ausgangsfilter für alle Quarantäneressourcen benötigt.

2. Erstellen von Überprüfungsskripts

Quarantäneskripts führen eine Reihe von Tests durch, um sicherzustellen, dass RAS-Computer den Sicherheitsrichtlinien entsprechen. Nach Abschluss dieser Tests muss das Skript entweder die Clientkomponente RQC.exe starten (bei positivem Testergebnis) oder den Clientcomputer an entsprechende Ressourcen weiterleiten, um ihn in Einklang mit den Richtlinien zu bringen. Natürlich könnte das Skript auch einfach ein Netzwerkzeitlimit anwenden und eine Fehlermeldung anzeigen, wenn die Netzwerkrichtlinien diese Vorgehensweise diktieren. Diese Skripts können einfache Befehlszeilen-Batchdateien oder komplexe ausführbare Dateien sein.

Einige Beispielsskripts können von der Seite* *[VPN-Quarantäne-Beispielskripts](http://www.microsoft.com/downloads/details.aspx?familyid=a290f2ee-0b55-491e-bc4c-8161671b2462&amp;displaylang=en) (möglicherweise in englischer Sprache) im Microsoft Download Center unter www.microsoft.com/downloads/details.aspx?FamilyID=a290f2ee-0b55-491e-bc4c-8161671b2462&amp;displaylang=en heruntergeladen werden.

3. Installieren von RQS.exe auf RAS-Servern

Das Installieren des Diensts RAS-Quarantäne-Agent (Rqs.exe) auf einem Microsoft Windows Server 2003 unterscheidet sich je nachdem, ob Service Pack 1 (SP1) installiert ist oder nicht. In diesem Abschnitt wird um der Kürze willen nur die Installation von Windows Server 2003 mit SP1 beschrieben, da davon auszugehen ist, dass alle Systeme mit sämtlichen aktuellen Service Packs und Sicherheitsupdates ausgestattet sind.

**So installieren Sie Rqs.exe auf einem Server mit Windows Server 2003 und SP1**
1. Klicken Sie auf **Start** und dann auf **Systemsteuerung.**  

2. Klicken Sie auf **Software.**  

3. Klicken Sie auf **Windows-Komponenten hinzufügen/entfernen.**  

4. Wählen Sie **Komponenten** aus, und klicken Sie dann auf **Netzwerkdienste.**  

5. Klicken Sie auf **Details.**  

6. Wählen Sie **Unterkomponenten von „Netzwerkdienste“**, klicken Sie auf **RAS-Quarantänedienst** und anschließend auf **OK.**  


Mit diesem Prozess wird der Quarantänedienst installiert, aber nicht gestartet. Er muss manuell von einem Administrator gestartet werden, nachdem die Lösung komplett konfiguriert und die Umgebung für die Implementierung vorbereitet wurde.

Ein weiterer Schritt beim Installationsprozess besteht darin, die Skriptversionszeichenfolgen so zu ändern, dass sie mit der Zeichenfolge übereinstimmen, die für Rqc.exe im Quarantäneskript konfiguriert wurde. Rqs.exe kann so konfiguriert werden, dass mehrere Skriptversionszeichenfolgen akzeptiert werden, die ihrerseits in die Registrierung des RAS-Servers unter **HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\rqs\AllowedSet** geschrieben werden. Dort müssen die Einstellungen mithilfe eines REG_MULTI_SZ-Werttyps angewendet werden. Normalerweise ist der Wert **Allowed Set** (zulässiger Satz) auf **RASQuarantineConfigPassed** gesetzt, es können jedoch weitere Zeichenfolgenwerte hinzugefügt werden.

4. Erstellen von Quarantäne-CM-Profilen

    Ein Quarantäne-CM-Profil ist eigentlich nur ein typisches Remotezugriffs-CM-Profil mit folgenden Zusätzen:
    * Eine Nachverbindungsaktion, die das Skript ausführt, um die Netzwerkrichtlinienkonformität und das Skript als solches zu überprüfen. Dies erfolgt über die Seite „Benutzerdefinierte Aktionen“ des CMAK-Assistenten.

    * Eine Benachrichtungskomponente muss dem Profil ebenfalls hinzugefügt werden, wie dies auch über den Bildschirm **Zusätzliche Dateien** des CMAK-Assistenten getan wird.


5. Verteilen von CM-Profilen

Die neu erstellten Quarantäne-CM-Profile müssen an alle RAS-Clientcomputer verteilt und dort installiert werden. Ein Profil wird in Form einer ausführbaren Datei bereitgestellt, die auf jedem RAS-Client-Computer ausgeführt wird, um das Profil zu installieren und die Quarantänenetzwerkverbindung zu konfigurieren.

Die Verteilung dieser Profile kann manuell erfolgen, wobei diese Profile beispielsweise als Anhänge zusammen mit Anweisungen an den Benutzer gesendet werden. Die Verteilung kann aber auch automatisiert werden, etwa mit der Softwareverteilungsfunktion von SMS 2003. Es stehen also verschiedene Methoden zur Auswahl. Welche Methode die beste ist, hängt ganz von der jeweiligen Umgebung ab.

6. Konfigurieren einer Quarantäne-RAS-Richtlinie

Das zum Konfigurieren einer Quarantäne-RAS-Richtlinie anzuwendende Verfahren unterscheidet sich je nachdem, ob die Konfiguration auf einem IAS-Server oder einem anderen Authentifizierungsanbieter erfolgt:

* Für die Konfiguration auf einem IAS RADIUS-Server ist das IAS-Snap-In (Internet Authentication Service) zu verwenden.

* Für die Konfiguration auf einem Windows-Authentifizierungsanbieter ist das Routing- und Remotezugriffs-Snap-In zu verwenden.


Beim Erstellen einer Richtlinie sollte zuerst eine Normalmodus-RAS-Richtlinie definiert werden. Anschließend sollten über die Registerkarte **Erweitert** der RAS-Richtlinien-Profileigenschaften die Attribute „MS-Quarantine-Session-Timeout“ und „MS-Quarantine-IPFilter“ hinzugefügt werden.

Wenn RADIUS verwendet wird, muss die Quarantäne-RAS-Richtlinie auf den anderen RADIUS-Servern repliziert werden – entweder durch Kopieren der Konfiguration oder durch manuelles Erstellen auf jedem einzelnen Server.

802.1X-Authentifizierung zum Schutz vor nicht verwalteten drahtlosen Geräten

Wie in den vorangegangenen Abschnitten bereits erwähnt, werden von Microsoft folgende Optionen für die Sicherung von drahtlosen Netzwerken in mittelgroßen Unternehmen empfohlen (von der sichersten bis zur unsichersten Option):
* WPA2/AES und EAP-TLS

* WPA2/AES und PEAP-MS-CHAP, Version 2

* WPA/TKIP und EAP-TLS

* WPA/TKIP und PEAP-MS-CHAP, Version 2


Obwohl WEP durch EAP-TLS oder PEAP-MS-CHAP, Version 2, sicherer gemacht werden kann, ist WEP als Teil einer dieser Lösungen lediglich für den Übergang auf die sichereren Standards WPA oder WPA2 zu empfehlen.

Die Prozesse der Implementierung von EAP-TLS und PEAP-MS-CHAP 2 weisen einige Gemeinsamkeiten auf. Beide Prozesse erfordern den Einsatz von Microsoft IAS RADIUS-Servern als Bestandteil der Lösung, und beide benötigen Zertifikate, wobei jedoch bei EAP-TLS die Zertifikate sowohl auf dem Clientcomputer als auch auf dem Server vorliegen müssen, während sie bei PEAP-MS-CHAP 2 nur auf den Authentifizierungsservern erforderlich sind. Aus diesem Grund ist für die Implementierung von EAP-TLS eine Zertifikatinfrastruktur dringend zu empfehlen, da sich die Kosten für den Kauf von Zertifikaten von Drittanbietern für sämtliche Clients als unannehmbar erweisen könnten.

Authentifizierung von drahtlosen Geräten mit EAP-TLS und PEAP-MS-CHAP 2

Bei der Implementierung für EAP-TLS und PEAP-MS-CHAP, Version 2, sind zahlreiche Details zu beachten, auf die im Rahmen dieses Dokuments nicht näher eingegangen werden kann. Inzwischen stehen jedoch einige hervorragende Ressourcen zur Verfügung, mit denen sich Lösungen zum Sichern von drahtlosen Netzwerke entwerfen und implementieren lassen, beispielsweise folgende:
* Die Seite [Bereitstellung von sicheren 802.11-Netzwerken mit Microsoft Windows](http://www.microsoft.com/technet/prodtechnol/winxppro/deploy/ed80211.mspx) (möglicherweise in englischer Sprache) im Microsoft TechNet mit Informationen zur Implementierung beider IEEE 802.1X-Authentifizierungsmethoden finden Sie unter www.microsoft.com/technet/prodtechnol/winxppro/deploy/ed80211.mspx.

* Die Downloadseite [Sichern von drahtlosen LANs mit Zertifikatsdiensten](http://go.microsoft.com/fwlink/?linkid=14844) (möglicherweise in englischer Sprache) unter http://go.Microsoft.com/fwlink/?LinkId=14844 bietet Ressourcen und ausführliche Informationen zum Implementieren von EAP-TLS in Microsoft-Netzwerken.

* Die Downloadseite [Sichern von drahtlosen LANs mit PEAP und Kennwörtern](http://go.microsoft.com/fwlink/?linkid=23481) (möglicherweise in englischer Sprache) unter http://go.Microsoft.com/fwlink/?LinkId=23481 bietet detaillierte Informationen zum Implementieren von PEAP-MS-CHAP 2 in Microsoft-Netzwerken.

* Das [WPA2-/WPS IE-Update für Windows XP mit SP2](http://support.microsoft.com/default.aspx?scid=kb;en-us;893357) unter http://support.microsoft.com/default.aspx?scid=kb;en-us;893357 wird benötigt, damit Microsoft Windows XP mit SP2 den Standard WPA2 unterstützt.


SMS zum Erkennen und Absichern nicht verwalteter Systeme

Wie bereits im Abschnitt „Entwicklung“ festgestellt wurde, ist der SMS-Ermittlungsprozess sehr nützlich, um neu angeschlossene Computer im Netzwerk zu finden, wenn diese durch SMS verwaltet werden können. Dabei wurde auch darauf hingewiesen, dass SMS einige nicht verwaltbare Systeme im Rahmen des Ermittlungsprozesses nicht erkennen kann, so dass dieser Mangel mit einer anderen Methode ausgeglichen werden muss.

Es kann mehrere Gründe geben, weshalb an ein Netzwerk angeschlossene Computer von SMS nicht erkannt werden, beispielsweise folgende:
* Der Computer ist zwar angeschlossen, doch er ist zum Zeitpunkt der Ermittlung nicht eingeschaltet und hat kein Computerkonto in der Domäne.

* Der Computer ist an ein Subnetz angeschlossen, in dem eine Firewall oder ein anderes Netzwerkgerät die Kommunikation zwischen dem SMS-Server und dem Subnetz verhindert.

* Der Computer ist zwar an ein zugängliches Netzwerk angeschlossen, aber er verwendet ein Betriebssystem, das SMS nicht erkennen kann.


Um für solche Fälle gerüstet zu sein, ist eine benutzerdefinierte Lösung erforderlich, die die Vorteile von SMS mit Skripts kombiniert, mit denen die Lücken von SMS kompensiert werden. Mit benutzerdefinierten Skripts kann das Netzwerk mit einem Planerprozess in regelmäßigen Abständen überprüft werden. Dabei können auch Geräte ermittelt werden, die möglicherweise nur für kurze Zeit eingeschaltet sind. Solche Skripts können auch von Arbeitsstationen oder Servern ausgeführt werden, die sich in ansonsten isolierten Subnetzen befinden. Damit kann erkannt werden, wann nicht verwaltete Systeme eine Verbindung zu diesen ansonsten nicht überwachten Netzwerksegmenten herstellen. Solche Skripts versuchen nicht, WMI-basierte Ermittlungsprozesse durchzuführen, so dass es für sie ohne Bedeutung ist, welches Betriebssystem auf den nicht verwalteten Clients verwendet wird.

Weitere Informationen darüber, wie Sie SMS zum Ermitteln von Geräten im Netzwerk verwenden können, finden Sie auf der Solution Accelerator-Seite [Patchverwaltung mit Systems Management Server 2003](https://www.microsoft.com/technet/itsolutions/cits/mo/swdist/pmsms/2003/pmsms031.mspx) (möglicherweise in englischer Sprache) unter www.microsoft.com/technet/itsolutions/cits/mo/swdist/pmsms/2003/pmsms031.mspx oder auf der [Microsoft Systems Management Server](https://www.microsoft.com/smserver/default.mspx)-Homepage unter www.microsoft.com/smserver/default.mspx. Dort finden Sie weitere Links, unter anderem zu Ressourcen für SMS-Skripterstellungslösungen. 

[Zum Seitenanfang](#mainsection)  

### Zusammenfassung

In diesem Dokument wurde gezeigt, dass umfassende Methoden zur Verfügung stehen, mit denen sich die Probleme in Zusammenhang mit nicht verwalteten Systemen lösen lassen. Mithilfe der IPsec-Netzwerkisolation wird weitgehend verhindert, dass nicht verwaltete Systeme Zugriff auf vertrauenswürdige Netzwerkressourcen erhalten, und zur Durchsetzung der Konformität beigetragen, indem nicht konformen Computern der Dienst verweigert wird. Die VPN-Quarantänedienste tragen zur Durchsetzung der Konformität bei mobilen Computern bei, die eine Remotezugriffslösung verwenden, aber selten Verbindungen zum lokalen Netzwerk herstellen. IEEE 802.1X und WPA/WPA2 tragen zum Schutz vor Rogue-Geräten in drahtlosen LANs bei. Mit SMS und Erkennungsskripts lassen sich nicht verwaltete Systeme erkennen und verwaltete Computer mit den jeweils aktuellen Patches und Sicherheitsupdates versorgen.

Wenngleich diese technischen Lösungen zur Beseitigung vieler Probleme mit nicht verwalteten Geräten und Rogue-Geräten beitragen, lassen sie sich nur dann optimal einsetzen, wenn auch sinnvolle Sicherheitsrichtlinien erstellt und strenge Änderungsmanagementprozesse festgelegt werden. Die Kombination all dieser Lösungen, Richtlinien und Prozesse ergibt eine handhabbare Infrastruktur für mittelgroße Unternehmen, die eine Senkung von Verwaltungskosten und eine Reduzierung der Sicherheitsrisiken auf ein akzeptables Maß ermöglichen kann.

[Zum Seitenanfang](#mainsection)  

### Anhang A: Netzwerkzugriffsschutz

Der Netzwerkzugriffsschutz (NAP) ist eine neue Funktion, die in der nächsten Generation von Windows (Microsoft Windows Server Longhorn und Windows Vista™) serienmäßig enthalten sein wird. NAP ermöglicht die Konformität mit Richtlinien zur Computerintegrität. Mit NAP können Administratoren Schwellenwerte für Integritätsüberprüfungsrichtlinien festlegen. Hierzu wird eine Anwendungsprogrammierschnittstelle (API) verwendet, die den Netzwerkzugriff für Computer einschränkt, die die Integritätsanforderungen nicht erfüllen, wenn sie Verbindungen zum Netzwerk herstellen.

Die Flexibilität von NAP gibt Administratoren die Möglichkeit, individuelle Lösungen für die Erfordernisse ihrer Umgebung zu konfigurieren, egal, ob es darum geht, den Integritätszustand von Computern zu protokollieren, die Verbindungen zum Netzwerk herstellen, Softwareupdates automatisch bereitzustellen oder die Konnektivität von Systemen einzuschränken, die die Integritätsanforderungen nicht erfüllen. Darüber hinaus ist NAP flexibel genug, um in Anwendungen und Programmlösungen von Drittherstellern integriert zu werden, damit die Computerintegritätsrichtlinien umfassend durchgesetzt werden können. NAP wird ebenfalls eine umfassende Lösung sein. Seine Durchsetzungskomponenten werden Administratoren in die Lage versetzen, die Konformität mit Integritätsrichtlinien mittels DHCP, VPN und drahtlosen 802.1X-Netzwerken zu erzwingen. Zudem ist NAP kompatibel mit IPsec.

Weitere Informationen über NAP finden Sie auf der Hompage zum Thema [Netzwerkzugriffsschutz](http://www.microsoft.com/technet/itsolutions/network/nap/default.mspx) unter www.microsoft.com/technet/itsolutions/network/nap/default.mspx.
 

**Download**  


[Dokument „Schutz von Netzwerken vor nicht verwalteten Clients“ herunterladen](http://go.microsoft.com/fwlink/?linkid=71713)
 
[Zum Seitenanfang](#mainsection)