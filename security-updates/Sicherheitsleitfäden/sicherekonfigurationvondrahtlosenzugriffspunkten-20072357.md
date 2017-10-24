---
Title: Sichere Konfiguration von drahtlosen Zugriffspunkten
TOCTitle: Sichere Konfiguration von drahtlosen Zugriffspunkten
ms:assetid: 57bb98c2-763f-468b-8eac-84910cfcca70
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Cc875845(v=TechNet.10)
ms:contentKeyID: 20072357
---


# Sichere Konfiguration von drahtlosen Zugriffspunkten

Veröffentlicht: 29. Aug 2006

Auf dieser Seite

[Einführung](#eeaa)  
[Definition](#edaa)  
[Herausforderungen](#ecaa)  
[Lösungen](#ebaa)  
[Zusammenfassung](#eaaa)  



### Einführung

Willkommen bei diesem Dokument aus der Reihe der Sicherheitsleitfäden für mittelgroße Unternehmen. Microsoft hofft, dass Ihnen die folgenden Informationen beim Erstellen einer sichereren und produktiveren Computerumgebung helfen werden.


#### Kurzzusammenfassung

Drahtlose lokale Netzwerke (WLANs) sind bei Unternehmen ein häufig diskutiertes Thema. Die meisten Unternehmen haben entweder ein WLAN bereitgestellt oder zumindest die Vorzüge und Nachteile der drahtlosen Technologie diskutiert. Unternehmen, die bereits drahtlose Netzwerke bereitgestellt haben, machen sich üblicherweise viele Gedanken über die Sicherheit ihrer Lösung. Andererseits haben Unternehmen, die sich noch nicht zum Einsatz drahtloser Technologie entschieden haben, die Befürchtung, dass sie mögliche Einsparpotenziale hinsichtlich Produktivität und Infrastruktur nicht nutzen.

Die meisten Entscheidungsträger im technischen Bereich machten sich früher zu Recht große Sorgen über die Sicherheit der drahtlosen Technologie. Selbst heute leidet die drahtlose Technologie noch unter dem Ruf, unsicher zu sein, da in der ersten Generation der WLAN-Sicherheitsprotokolle IEEE 802.11 Schwachstellen entdeckt und veröffentlicht wurden. Obwohl über die Jahre viele Problemumgehungen entwickelt wurden, waren die meisten Lösungen zum Beheben von drahtlosen Sicherheitsproblemen entweder zu kostspielig oder wiesen eigene Schwachstellen auf.

Viele Entwicklungen erfolgten, da drahtlose Netzwerke erst kurz zuvor eingeführt worden waren. In gleicher Weise, wie die Technologie ausreifte und höhere Geschwindigkeit und Zuverlässigkeit bot, verbesserten sich auch die Standards für das Sichern drahtloser Übertragungen. Die aktuellsten drahtlosen Sicherheitsprotokolle, WPA und WPA2, die beide auf dem Standard IEEE 802.11i beruhen, unterstützen die Bereitstellung eines verstärkten Schutzes für drahtlosen Datenverkehr. Die hierbei erreichte Sicherheit reicht selbst für Sicherheitsumgebungen mit besonders hohen Anforderungen aus. Diese aktuellen Standards bieten bei richtiger Konfiguration ein hohes Sicherheitsniveau und können mit gutem Gewissen in mittelgroßen Unternehmen eingesetzt werden.


#### Übersicht

Dieses Dokument besteht aus vier Hauptabschnitten, die sich mit den Details beim Entwickeln und Implementieren einer Lösung befassen, die zum Sichern von drahtlosen Netzwerken in mittelgroßen Unternehmen erforderlich ist. Dabei handelt es sich um folgende Abschnitte:
* **Einführung.**   Dieser Abschnitt stellt eine Kurzzusammenfassung dieses Dokuments zur Verfügung. Zudem enthält er eine Übersicht über den Aufbau des Dokuments sowie Informationen über die empfohlene Zielgruppe.

* **Definition.**   In diesem Abschnitt erhalten Sie einige Details und Definitionen, die zum Verstehen der Terminologie nützlich sind, die in diesem Dokument verwendet wird.

* **Herausforderungen.**   Dieser Abschnitt beschreibt einige der häufigen Probleme, die mittelgroße Unternehmen in Hinblick auf drahtlose Netzwerke berücksichtigen müssen. Darüber hinaus enthält der Abschnitt Hintergrundinformationen für die Lösung, die in diesem Dokument angesprochen wird.

* **Lösungen.**   In diesem Abschnitt erhalten Sie detaillierte schrittweise Anleitungen zum Planen, Entwickeln, Bereitstellen und Unterstützen einer sicheren drahtlosen Infrastruktur. Daher ist der Abschnitt mit den Lösungen in drei große Unterabschnitte unterteilt:
* **Bewerten der WLAN-Sicherheit.**   Dieser Abschnitt behandelt einführende Informationen und potenzielle Optionen zum Erarbeiten einer Grundlage, auf der eine spätere Lösung aufbaut.

* **Entwickeln einer sicheren WLAN-Lösung.**   Dieser Abschnitt verwendet die Informationen, die zuvor in der Bewertungsphase ermittelt wurden, um eine Entscheidung zu treffen und einen Plan zu erstellen. Danach wird die Grundlage der Lösung entwickelt.

* **Bereitstellung und Verwaltung.**   In diesem Abschnitt wird die tatsächliche schrittweise Lösung detailliert vorgestellt. Dazu zählen auch Informationen, die Sie beim Verwalten und Überprüfen der sicheren drahtlosen Netzwerklösung unterstützen, die in diesem Dokument beschrieben wird.




#### Zielgruppe dieses Dokuments

Dieses Dokument richtet sich an IT-Mitarbeiter in mittelgroßen Unternehmen und für die Implementierung zuständige Mitarbeiter und Führungskräfte im technischen Bereich, die die Verwendung von WPA (Wi-Fi Protected Access) oder WPA2 (Wi-Fi Protected Access 2) zum Sichern ihrer drahtlosen Infrastruktur in Betracht ziehen. In diesem Dokument wird davon ausgegangen, dass der Leser über allgemeine technische Kenntnisse in folgenden Bereichen verfügt: drahtlose Geräte, grundlegende Netzwerkkonzepte, Microsoft® Windows Server™ 2003, Internetauthentifizierungsdienst (IAS), Zertifikatsdienste, den Verzeichnisdienst Active Directory® sowie die Konfiguration und Anwendung einer Gruppenrichtlinie.
[Zum Seitenanfang](#mainsection)  



### Definition

Der Leser sollte mit den folgenden Themen und Konzepten vertraut sein, die in diesem Dokument verwendet werden:

**AES.**   Der erweiterte Verschlüsselungsstandard (Advanced Encryption Standard, AES) verwendet eine symmetrische Blockdaten-Verschlüsselungstechnik und ist Bestandteil von WPA2.

**EAP.**   Extensible Authentication-Protokoll (EAP) ist ein 802.1X-Standard, der Entwicklern das Übergeben von Authentifizierungsdaten zwischen RADIUS-Servern und drahtlosen Zugriffspunkten ermöglicht. EAP verfügt über eine Reihe von Varianten, darunter: EAP MD5, EAP-TLS, EAP-TTLS, LEAP und PEAP.

**EAP-TLS.**   EAP-TLS (EAP Transport Layer Security) wurde von Microsoft im Rahmen des Standards 802.1X entwickelt, um digitale Zertifikate für die Authentifizierung zu verwenden. Dabei handelt es sich derzeit um den Industriestandard für die 802.11i-Authentifizierung.

**IEEE 802.1X.**   IEEE 802.1X regelt den EAP-Kapselungsprozess, der zwischen Antragstellern (Clients), Echtheitsbestätigungen (drahtlose Zugriffspunkte) und Authentifizierungsservern (RADIUS) stattfindet.

**IEEE 802.11.**   Der Standard IEEE 802.11 regelt die drahtlose Netzwerkkommunikation und umfasst mehrere Spezifikationen, die vom Standard 802.11g für Datenverkehr mit einer Übertragungsrate von 20+ Mbit/s im 2,4-GHz-Band bis zum Standard 802.11i reichen, in der WPA2-Verschlüsselung und -Authentifizierung geregelt werden.

**IEEE 802.11i.**   Die Änderung IEEE 802.11i am Standard 802.11 gibt Sicherheitsmethoden (WPA2) an, welche eine AES-Blockchiffre zum Sichern der ursprünglichen Authentifizierungsprozesse (EAP) verwenden. Auf diese Weise werden Unzulänglichkeiten der Sicherheitsstandards und -spezifikationen für drahtlose Netzwerke berücksichtigt.

**MS-CHAP v2.**   Microsoft Challenge Handshake Authentication-Protokoll Version 2 (MS-CHAP v2) ist ein kennwortbasiertes gegenseitiges Authentifizierungsprotokoll auf der Grundlage von Abfrage/Rückmeldung, das MD4- und DES-Verschlüsselung verwendet. Es wird in Verbindung mit PEAP (PEAP-MS-CHAP v2) zum Sichern der drahtlosen Kommunikation verwendet.

**PEAP.**   Bei dem Protected Extensible Authentication-Protokoll (PEAP) handelt es sich um einen Typ der EAP-Kommunikation, bei dem Sicherheitsprobleme behoben werden, die durch EAP-Übertragungen im Klartext entstehen. Hierzu wird ein sicherer Kanal durch TLS verschlüsselt und geschützt.

**SSID.**   Service Set Identifier (SSID) ist der Name, der einem WLAN zugewiesen und vom Client verwendet wird, um die richtigen Einstellungen und Anmeldeinformationen zu identifizieren, die für den Zugriff auf ein WLAN erforderlich sind.

**TKIP.**   Temporal Key Integrity Protocol (TKIP) ist Bestandteil des WPA-Verschlüsselungsstandards für drahtlose Netzwerke. TKIP ist die nächste Generation von WEP, die eine paketweise Schlüsselmischung zur Verfügung stellt, um dadurch Fehler zu beheben, die im WEP-Standard entdeckt wurden.

**WEP.**   Wired Equivalent Privacy (WEP) ist Bestandteil des Standards IEEE 802.11 und verwendet eine RC4-Verschlüsselung mit 64 oder 128 Bit. Im Jahr 2001 wurden größere Fehler im WEP-Standard gefunden, die insbesondere auf die Länge des Initialisierungsvektors der RC4-Stromchiffre zurückzuführen waren. Dadurch war das passive Dekodieren des RC4-Schlüssels möglich.

**WLAN.**   Drahtloses lokales Netzwerk.

**WPA.**   Um die Schwächen zu beseitigen, die im WEP-Standard gefunden wurden, erfolgte die Einführung von Wi-Fi Protected Access (WPA) im Jahr 2003. Dabei handelt es sich um eine interoperable drahtlose Sicherheitsspezifikation, die eine Untergruppe des Standards IEEE 802.11 darstellt. Dieser Standard stellt Authentifizierungsfunktionen zur Verfügung und verwendet TKIP für die Datenverschlüsselung.

**WPA2.**   WPA2 wurde im September 2004 durch die Wi-Fi Alliance eingeführt und ist die zertifizierte interoperable Version der vollständigen Spezifikation IEEE 802.11i, die im Juni 2004 ratifiziert wurde. Wie der Vorgängerstandard unterstützt WPA2 die IEEE 802.1X/EAP-Authentifizierung oder PSK-Technologie, enthält jedoch auch einen neuen fortschrittlichen Verschlüsselungsmechanismus unter Verwendung des Counter-Mode/CBC-MAC-Protokolls (CCMP) mit der Bezeichnung Advanced Encryption Standard (AES).
[Zum Seitenanfang](#mainsection)  



### Herausforderungen

Viele Unternehmen sind sich über die Vorteile der drahtlosen Technologie zum Verbessern von Produktivität und Zusammenarbeit bewusst, zögern jedoch mit der Implementierung der Technologie. Der Grund hierfür sind die verständlichen Sorgen hinsichtlich der Sicherheitsanfälligkeiten, die drahtlose Netzwerke offensichtlich für Unternehmensumgebungen darstellen. Noch verwirrender sind die vielen vorgeschlagenen Methoden, die zum Sichern der drahtlosen Kommunikation verwendet werden, sowie die völlig unterschiedlichen Berichte über die Wirksamkeit dieser Maßnahmen.

Drahtlose Technologie stellt mittelgroße Unternehmen vor viele Herausforderungen, und dies nicht nur mit Blick auf das Sichern einer Bereitstellung, sondern auch hinsichtlich der Frage, ob eine solche Bereitstellung überhaupt erfolgen soll. Im Folgenden erhalten Sie eine Übersicht über einige der häufigsten Themen bei drahtlosen Netzwerken, die in diesem Dokument angesprochen werden.
* Entscheidung für oder gegen die Implementierung eines WLAN

* Informationen zu den Risiken drahtloser Lösungen und zur Risikoabwehr

* Ermitteln von Methoden zum Sichern einer WLAN-Umgebung

* Auswählen der richtigen WLAN-Sicherheitsoptionen

* Validieren der Sicherheitsstufe einer drahtlosen Netzwerkimplementierung

* Einbeziehen vorhandener Komponenten in eine drahtlose Sicherheitslösung

* Erkennen und Vermeiden von riskanten drahtlosen Geräteverbindungen

[Zum Seitenanfang](#mainsection)  



### Lösungen

Dieser Abschnitt beschreibt Entwurf, Entwicklung, Implementierung und Unterstützung von sicheren drahtlosen Lösungen, die in mittelgroßen Unternehmensumgebungen bereitgestellt werden können. Wie zuvor bereits erwähnt, gibt es viele Vorbehalte gegenüber der Verwendung drahtloser Technologie. Jeder dieser Punkte wird im Folgenden angesprochen, damit die Vorteile drahtloser Netzwerke so effizient und sicher wie möglich genutzt werden können.


#### Bewerten der WLAN-Sicherheit.

Obwohl drahtlose Technologie heute so ausgereift ist, dass sie für die Bereitstellung in einer mittelgroßen Unternehmensumgebung ausreichend schnell und sicher ist, müssen nach wie vor viele verschiedene Faktoren berücksichtigt und die richtigen Methoden ausgewählt werden, um ein drahtloses Netzwerk zu sichern. Dieser Abschnitt behandelt viele der üblichen Methoden, die zum Sichern drahtloser Netzwerke verwendet werden, bietet Unterstützung zum Ermitteln der besten Lösung für eine bestimmte Umgebung und stellt Argumente für und gegen jeden Ansatz zur Verfügung.

Vorteile drahtloser Netzwerke

Die Vorteile, die durch das Implementieren von WLAN-Technologie ermöglicht werden, können in zwei unterschiedliche Kategorien unterteilt werden: Wirtschaftliche Vorteile und Vorteile beim Betrieb. Zu den Vorteilen beim Betrieb zählen geringere Verwaltungskosten und verringerte Kapitalausgaben. Die wirtschaftlichen Vorteile umfassen neben verbesserter Produktivität und effizienteren Unternehmensprozessen auch ein erhöhtes Potenzial für das Erstellen neuer Unternehmensfunktionen.

Wirtschaftliche Vorteile

Die meisten zentralen wirtschaftlichen Vorteile bei der Verwendung von WLAN-Technologie sind auf eine Steigerung der Flexibilität und Mobilität der Mitarbeiter zurückzuführen. Bei der Verwendung drahtloser Netzwerke sind die Mitarbeiter nicht mehr an ihren Schreibtisch gebunden und können sich relativ problemlos frei im Büro bewegen. Durch diese zusätzliche Freiheit können die folgenden Vorteile genutzt werden:
* Die mobilen Mitarbeiter eines Unternehmens wie Vertriebsmitarbeiter können in verschiedenen Büros arbeiten oder nach einem Einsatz bei Kunden problemlos eine transparente Verbindung mit dem Unternehmensnetzwerk herstellen. Die Konnektivität steht sehr schnell zur Verfügung, und es nicht erforderlich, erst nach einem Netzwerkanschluss zu suchen oder Kabel zu entwirren. Auf diese Weise wird nicht nur viel Zeit gespart, sondern es werden auch die Probleme bei der Verwendung kabelgebundener Netzwerke vermieden.

* Die IT-Mitarbeiter können ständig in Kontakt mit den Systemen bleiben, die sie betreuen. Dabei spielt es keine Rolle, wo sie sich im Gebäude aufhalten, ob sie gerade an Besprechungen teilnehmen oder nicht am Schreibtisch sind. Durch die Verwendung tragbarer Geräte wie Laptops, Tablet PCs oder Handheld-Computer können die IT-Mitarbeiter eines Unternehmens sofort auf alle Anforderungen reagieren.

* Die Informationen stehen allen Benutzern stets zur Verfügung. Besprechungen müssen nicht mehr verschoben werden, da jemand Kopien anfertigen oder Berichte von seinem Schreibtisch holen muss. Präsentationen werden auf dem Computer gemeinsam genutzt und nicht mehr auf einem verschwommenen Overhead-Display angezeigt. Für Besprechungen können interaktive Technologien zum Zusammenarbeiten mit entfernt gelegenen Niederlassungen und Telearbeitern verwendet werden.

* Die Flexibilität bei der Organisation wird deutlich verbessert, da Strukturänderungen schnell und einfach implementiert werden können. Selbst die Neustrukturierung ganzer Büros ist möglich, da die Netzwerkverkabelung kein Problem mehr darstellt.

* Die drahtlose Technologie ermöglicht die Nutzung ganz neuer Technologieanwendungen und Lösungen für eine Unternehmensumgebung. Geräte wie PDAs (Personal Digital Assistants) und Tablet PCs können nahtlos in eine Netzwerkumgebung integriert werden. Mitarbeiter und Unternehmensfunktionen, die zuvor keine Informationstechnologie verwenden konnten, haben jetzt die Möglichkeit, die Vorteile der Netzwerkkonnektivität zu nutzen. In Kantinen, Fertigungsbereichen, Krankenzimmern, Verkaufsräumen, Restaurants und sogar Werkshallen kann jetzt die Produktivität gesteigert werden, da Technologielösungen problemlos eingesetzt werden können.


Vorteile beim Betrieb

Die Vorteile beim Betrieb von drahtloser Technologie sind ebenfalls vielfältig und hängen vom jeweiligen Unternehmenstyp und den genutzten Einrichtungen ab. Zu diesem Vorteilen zählen folgende Punkte:
* Die Bereitstellungskosten für das Netzwerk werden deutlich verringert, da die Abhängigkeit von der kabelgebundenen Netzwerkinfrastruktur verringert wird. Bereiche, in denen Netzwerkkonnektivität bislang in der Praxis nicht bereitgestellt werden konnte, sind jetzt durch WLAN-Technologie kostengünstig erreichbar. Dies schließt Bereiche im Freien oder verteilte Büros ein.

* Die Skalierbarkeit des Netzwerks wird verbessert, und das Netzwerk kann effizienter auf verschiedene Nachfragestufen reagieren, da die Bereitstellung vereinfacht wird. Zudem ist es einfacher möglich, drahtlose Zugriffspunkte zur Vermeidung lokaler Überlastungen an andere Standorte zu verlegen, als die Anzahl der Netzwerkanschlüsse vor Ort zu erhöhen.

* Der Umfang des Kapitals, das von der Infrastruktur gebunden wird, kann verringert werden, da die Netzwerkausrüstung im Gegensatz zur Infrastruktur bei einem kabelgebundenen Netzwerk kein unbewegliches Inventar darstellt. Dies ermöglicht mehr Flexibilität für die künftige Expansion oder bei einem unter Umständen erforderlichen Standortwechsel. Drahtlose Hochgeschwindigkeitsverbindungen (802.11a/g/n) sind zudem eine kostengünstige Alternative zum Ersetzen alter und langsamer Ethernet- oder Token Ring-Kabel.


Sicherheitsanfälligkeiten bei drahtlosen Netzwerken

Um das Sicherheitsniveau der verschiedenen Sicherheitslösungen einschätzen zu können, die für drahtlose Netzwerke verfügbar sind, müssen zunächst Kenntnisse zu den Bedrohungen für drahtlose Netzwerke vorhanden sein. Die Sicherheitsanfälligkeiten und Angriffsprofile, die bei herkömmlichen Netzwerken berücksichtigt werden müssen, sind allgemein bekannt. Drahtlose Netzwerke weisen jedoch Sicherheitsanfälligkeiten auf, die über diese herkömmlichen Risiken hinausgehen.

**Tabelle 1. Typische WLAN-Sicherheitsbedrohungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Bedrohung

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Offenlegung von Daten durch Lauschen

</td>

<td style="border:1px solid black;">


Das Belauschen von nicht gesichertem drahtlosen Datenverkehr kann zur Offenlegung vertraulicher Daten, dem Herausfinden der Anmeldeinformationen von Benutzern und sogar zum Diebstahl persönlicher Daten führen. Raffinierte Angreifer können die durch Lauschen gesammelten Informationen verwenden, um Angriffe auf Systeme vorzunehmen, die anderenfalls nicht gefährdet wären.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Abfangen und Ändern von übertragenen Daten

</td>

<td style="border:1px solid black;">


Ein Angreifer, der auf Netzwerkressourcen zugreifen kann, ist auch in der Lage, gefährliche Systeme in ein Netzwerk einzufügen, die Daten abfangen und ändern können, die zwischen zwei zulässigen Systemen weitergeleitet werden.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Spoofing

</td>

<td style="border:1px solid black;">


Der Zugriff auf ein internes Netzwerk gibt Angreifern die Möglichkeit, Daten zu fälschen, damit sie wie zulässiger Datenverkehr wirken. Solche Angriffe können gefälschte E-Mail-Nachrichten umfassen, denen von internen Benutzern bereitwilliger vertraut wird als Mitteilungen von externen Quellen. Auf diese Weise entsteht eine Plattform für „Social Engineering“-Angriffe und das Einschleusen von Trojanern.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Denial of Service (DoS)

</td>

<td style="border:1px solid black;">


Unabhängig von der implementierten Sicherheitslösung ist ein WLAN für DoS-Angriffe anfällig, ob sie nun absichtlich oder versehentlich erfolgen. Solche Unterbrechungen können eine so einfache Ursache wie einen Mikrowellenherd haben oder auf ein Gerät zurückzuführen sein, das für das Überlasten eines Netzwerks mit wahllosem Datenverkehr konfiguriert wurde.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Freies Laden   
(Ressourcendiebstahl)

</td>

<td style="border:1px solid black;">


Einige Eindringlinge sind möglicherweise ausschließlich an kostenlosem Zugang zum Internet interessiert. Obwohl diese Aktivitäten weder unmittelbar schädlich noch bösartig sind, können sie zu einer langsameren Netzwerkkonnektivität für legitime Benutzer führen oder einem unverwalteten Vektor für Bedrohungen durch Malware werden.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zufällige Bedrohungen und nicht verwaltete Verbindungen

</td>

<td style="border:1px solid black;">


In ungesicherten WLAN-Umgebungen kann jeder Besucher Zugriff auf das interne Netzwerk erhalten, indem er einfach ein Gerät startet, das auf drahtlose Netzwerke zugreifen kann. Solche nicht verwalteten Geräte könnten bereits gefährdet sein oder einem Angreifer einen Angriffspunkt gegen ein Netzwerk zur Verfügung stellen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Riskante WLAN-Zugriffspunkte

</td>

<td style="border:1px solid black;">


Selbst wenn ein Unternehmen über kein drahtloses Netzwerk verfügt, kann es dennoch durch Sicherheitsbedrohungen durch nicht verwaltete drahtlose Netzwerke gefährdet sein. Drahtlose Geräte sind relativ kostengünstig, so dass jeder Mitarbeiter prinzipiell ein nicht verwaltetes und ungeschütztes Netzwerk innerhalb einer Umgebung einrichten könnte.

</td>

</tr>

</table>


Obwohl viele dieser Sicherheitsrisiken bei der drahtlosen Datenübertragung angesichts des hohen Sicherheitsbewusstseins heutiger Unternehmen offensichtlich sind, blieben diese Themen bei der Einführung der ersten Generation der drahtlosen Sicherheitstechnologie häufig unbeachtet. Als WEP zum Sichern drahtloser Datenübertragungen konzipiert wurde, schien es kaum erforderlich zu sein, die Sicherheitsmängel beim drahtlosen Übertragen von Daten zu kompensieren, die bei kabelgebundenen Übertragungen in dieser Form nicht vorhanden sind. Der Grund hierfür bestand darin, dass die Technologie so neu war, dass sich nur wenige Leute über die möglichen Bedrohungen Gedanken gemacht hatten, denen solche Netzwerke möglicherweise ausgesetzt sind. Als die Angreifer immer ausgefeiltere Methoden einsetzten, wurde klar, dass bei der drahtlosen Datenübertragung potenziell gefährliche Umgebungen überbrückt werden müssen und dass daher die Kommunikation genauso gut gesichert werden muss wie bei der kabelgebundenen LAN-Kommunikation.

Nachdem die Schwächen bei der Sicherheit von WEP einem breiten Publikum bekannt waren, änderte sich das Umfeld der Netzwerksicherheit rasch. Geschichten von War-Drivern wurden in den Medien erwähnt, während die Regierungen an Gesetzen arbeiteten, um der Industrie Vorgaben hinsichtlich der Sicherheit von allgemeinen und persönlichen Daten bereitzustellen. Als Reaktion auf diese Entwicklungen verwarfen viele Unternehmen entweder den Einsatz drahtloser Technologie als unpraktikabel und unsicher oder entwickelten komplexe Problemumgehungen, um die Fehler im WEP-Standard zu beheben.

Einige dieser komplexen Lösungen zur Problemumgehung werden noch heute verwendet und sogar vermarktet. Allerdings zeigen die folgenden Abschnitte, dass diese komplexen Lösungen nicht mehr erforderlich sind, um drahtlose Netzwerke gegen solche Bedrohungen zu sichern. Daher sollten diese Lösungen neu bewertet werden, da bei der Weiterentwicklung der drahtlosen Technologie die geänderten Sicherheitsanforderungen berücksichtigt wurden.

Auswählen der richtigen WLAN-Sicherheitslösung

Seitdem die technologischen Schwächen der ersten WLAN-Generation enthüllt wurden, sind große Anstrengungen unternommen worden, um den Sicherheitsanfälligkeiten bei der Drahtlostechnologie Rechnung zu tragen. Während sich die Industrie für Drahtlostechnologie, Microsoft und andere Anbieter auf das Verbessern der Standards für die drahtlose Datenübertragung konzentrierten, arbeiteten viele andere Analysten, Anbieter von Netzwerksicherheitslösungen und andere an der Umgehung der Schwächen im älteren Standard für drahtlose Netzwerke. Dies hat zu einer Vielzahl von Ansätzen zur Behebung von Sicherheitsproblemen im Drahtlosbereich geführt.

Abgesehen von der nahe liegendsten Lösung, dem Verzicht auf die Implementierung von WLAN-Technologie, werden die wichtigsten Alternativen in der folgenden Tabelle verglichen.

**Tabelle 2. Vergleich von WLAN-Sicherheitslösungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Funktion

</th>

<th style="border:1px solid black;">

WPA und WPA2

</th>

<th style="border:1px solid black;">

Statisches WEP

</th>

<th style="border:1px solid black;">

VPN

</th>

<th style="border:1px solid black;">

IPsec

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Strenge Authentifizierung

(siehe Hinweis)

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja, nur bei Nichtverwendung der   
Authentifizierung mit installiertem Schlüssel

</td>

<td style="border:1px solid black;">


Ja, bei Verwendung eines Zertifikats oder von Kerberos-Authentifizierung

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Starke Datenverschlüsselung

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Transparente Verbindung und erneute Verbindung

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Benutzerauthentifizierung

(siehe Hinweis)

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Computerauthentifizierung

(siehe Hinweis)

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schützt Broadcast- und Multicastübertragung

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zusätzliche Netzwerkgeräte erforderlich

</td>

<td style="border:1px solid black;">


Ja, RADIUS-Server

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Ja, VPN- und RADIUS-Server

</td>

<td style="border:1px solid black;">


Nein

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Sichert den Zugriff auf das WLAN statt nur auf die Pakete

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Ja

</td>

<td style="border:1px solid black;">


Nein

</td>

<td style="border:1px solid black;">


Nein

</td>

</tr>

</table>


**Hinweis**   Was die strenge Authentifizierung betrifft, verwenden viele VPN-Implementierungen auf der Grundlage eines IPsec-Tunnelmodus ein Authentifizierungsschema mit einem schwachen installierten Schlüssel mit der Bezeichnung XAuth.  
Aktuelle Versionen des Betriebssystems Windows unterstützen nicht die Authentifizierung von IPsec-Verbindungen. Diese Funktionalität wird jedoch mit Windows Vista und Longhorn verfügbar sein.   
Computerauthentifizierung bedeutet, dass der Computer weiterhin mit dem WLAN und LAN verbunden bleibt, selbst wenn kein Benutzer am Computer angemeldet ist. Diese Fähigkeit ist für manche domänenbasierten Funktionen wie Roamingprofile erforderlich.

Wie diese Tabelle zeigt, muss eine Reihe von Faktoren berücksichtigt werden, wenn die verschiedenen Möglichkeiten zum Sichern von drahtlosen Netzwerken untersucht werden. Bei einer solchen Analyse müssen viele Punkte berücksichtigt werden – von den Kosten für die Implementierung und Verwaltung bis hin zur allgemeinen Sicherheit der betreffenden Lösung. Jeder Ansatz hat Vor- und Nachteile. Daher ist für jede Lösung eine detaillierte Untersuchung erforderlich, um sicherzustellen, dass eine fundierte Entscheidung getroffen werden kann.

Um das Verständnis der verfügbaren Optionen zum Sichern von WLAN-Implementierungen zu vereinfachen, werden die folgenden Themen detailliert besprochen. Dabei wurden die einzelnen behandelten Methoden nach der jeweils bereitgestellten Sicherheitsstufe sortiert.
* Keine Bereitstellung von WLAN-Technologie

* Verwenden von WPA mit EAP-TLS

* Verwenden von WPA mit PEAP-MS-CHAP v2

* Verwenden von WPA mit PEAP-MS-CHAP v2 und Zertifikatsdiensten

* Verwenden eines VPN

* Verwenden von IPsec

* Verwenden von WEP

* Keine WLAN-Sicherheit


Keine Bereitstellung von WLAN-Technologie

Unter Sicherheitsexperten gilt das Motto, dass das sicherste System stets ein System ist, das nie aktiviert wird. Daher besteht die sicherste Methode bei der Bereitstellung jeglicher Technologie einschließlich drahtloser Netzwerke darin, sie nie bereitzustellen. Das Problem bei diesem Ansatz besteht natürlich darin, dass ein Unternehmen, das niemals Technologie einsetzt, an Wettbewerbsfähigkeit verliert. Dies gilt insbesondere für die heutige Geschäftswelt, in der jeder Wettbewerbsvorteil, insbesondere mit Blick auf Technologie, zählt.

Wie zuvor erwähnt, muss jedes Unternehmen seine eigenen Anforderungen und die individuelle Risikobereitschaft untersuchen. Bei jeder Technologie, die in Betracht gezogen wird, muss das Risiko abgeschätzt werden, und drahtlose Technologie stellt hierbei keine Ausnahme dar. Drahtlose Netzwerke bieten viele Vorteile, die jedoch möglicherweise unterschätzt werden oder bei einem bestimmten Unternehmen nicht genutzt werden können.

Beim Untersuchen der geeigneten drahtlosen Sicherheitslösung für ein Unternehmen müssen alle Optionen berücksichtigt werden. Dazu zählt auch der Verzicht auf die Bereitstellung einer drahtlosen Lösung. Wenn ein Unternehmen jedoch bestimmen sollte, dass es für die Bereitstellung eines WLAN nicht bereit ist, sollte diese Entscheidung zugleich die aktive Umsetzung einer Unternehmensrichtlinie nach sich ziehen, die die Bereitstellung von WLANs durch Endbenutzer untersagt. Diese potenziell gefährlichen WLANs könnten die Netzwerksicherheit des Unternehmens gefährden.

Verwenden von WPA mit EAP-TLS

WPA oder WPA2 mit EAP-TLS (Extensible Authentication-Protokoll Transport Layer Security) mit Benutzer- und Computerzertifikaten ist die stärkste Methode der 802.1X-Authentifizierung, die von den aktuellen Versionen der Windows-basierten drahtlosen Clients unterstützt wird. EAP-TLS verwendet digitale Zertifikate, um gegenseitige Authentifizierung bereitzustellen. Dabei nimmt der drahtlose Client eine Authentifizierung am Authentifizierungsserver vor, und umgekehrt. Für die EAP-TLS-Authentifizierung ist eine öffentliche Schlüsselinfrastruktur (PKI) erforderlich, um Zertifikate auszustellen und auf dem neuesten Stand zu halten. Für die höchste Sicherheitsstufe sollte die PKI so konfiguriert sein, dass sowohl Benutzer- als auch Computerzertifikate für den drahtlosen Zugriff ausgestellt werden.

Aufgrund der Implementierungskosten und des Verwaltungsaufwands für PKIs war diese äußerst sichere Lösung auf mittelgroße oder große Unternehmen beschränkt. Sie kann jedoch heute auch in kleinen Unternehmensumgebungen verwendet werden, da inzwischen Microsoft Small Business Server eingeführt wurde, der die zugrunde liegenden Zertifikatsdienste bereitstellt, deren Implementierung für EAP-TLS erforderlich ist.

**Hinweis**   Derzeit gibt es keine unterstützenden Gruppenrichtlinienobjekte (GPOs) für den WPA2-Standard, was die Fähigkeit zum effizienten Implementieren dieses Standards in größeren Umgebungen beeinträchtigen kann. Allerdings werden derzeit Updates für Windows Server 2003 und Windows XP entwickelt, um GPO-Unterstützung für WPA2 hinzuzufügen. Die nächste Generation von Windows, Vista und Longhorn, wird systemeigene Unterstützung für den WPA2-Standard aufweisen.

Verwenden von WPA mit PEAP-MS-CHAP v2

WPA oder WPA2 mit geschütztem EAP (Protected EAP, PEAP) und Microsoft Challenge Handshake Authentication-Protokoll Version 2 (MS-CHAP v2) mit strengen Kennwortanforderungen ist die zweitsicherste Implementierung, die von den aktuellen Versionen von Windows-basierten Clients unterstützt wird. Wenn eine PKI-Bereitstellung nicht durchführbar ist, stellt PEAP-MS-CHAP v2 eine gangbare und sichere Option zum Bereitstellen eines zuverlässigen drahtlosen Netzwerks dar. Bei PEAP handelt es sich um ein unidirektionales Authentifizierungsschema, das TLS zum Erstellen eines verschlüsselten Kanals vom Authentifizierungsserver verwendet, über den der Client ein anderes Protokoll einsetzt, um sich selbst zu authentifizieren. Ursprünglich für DFÜ- und VPN-Remotezugriff entwickelt, kann MS-CHAP v2 die strenge kennwortbasierte Authentifizierung von drahtlosen Clients unterstützen, falls strenge Kennwortrichtlinien im Netzwerk verwendet werden.

Verwenden von WPA mit PEAP-MS-CHAP v2 und Zertifikatsdiensten

Es ist möglich, die Verwendung von Zertifikatsdiensten mit einer kennwortbasierten PEAP-MS-CHAP v2-Lösung bei Unternehmen zu verbinden, die Elemente beider Ansätze in ihrer Lösung benötigen. Allerdings kann durch das Hinzufügen von PEAP-MS-CHAP v2 keine deutliche Steigerung der Sicherheit verglichen mit der bereits relativ sicheren EAP-TLS-Lösung erreicht werden. Dies gilt zumindest zum Zeitpunkt der Erstellung dieses Dokuments. Tatsächlich wird durch die Verwendung von PEAP-MS-CHAP v2 mit EAP-TLS der Authentifizierungsprozess verlangsamt, da zwei TLS-Kanäle ineinander erstellt werden. Diese doppelte Verschlüsselung bringt keinen zusätzlichen Nutzen.

Verwenden eines VPN

Als die Schwächen bei der Sicherheit von WEP erstmals entdeckt wurden, bestand eine der ersten Reaktionen von vielen Sicherheitsexperten und führenden Managern darin, VPNs zum Sichern von drahtlosen Netzwerken zu verwenden. Bei der VPN-Technologie handelt es sich gewiss um eine sichere und bewährte Methode zum Schützen von Netzwerkkommunikation, die über potenziell gefährliche Netzwerke wie das Internet geleitet wird. Diese Lösung zum Beheben der Sicherheitsprobleme bei WEP wird immer noch in vielen Umgebungen genutzt.

Obwohl es sich dabei vom Standpunkt der Sicherheit um eine vorteilhafte Lösung zu handeln scheint, bringt diese Lösung einige offensichtliche Schwächen mit sich. Daher ist dieser Ansatz im Vergleich zur Flexibilität von Lösungen unter Verwendung von WPA weniger attraktiv, da WPA speziell mit Blick auf Bedrohungen bei der drahtlosen Kommunikation entwickelt wurde. Obwohl es durchaus möglich ist, WPA-Lösungen in Verbindung mit VPN-Technologie zum Sichern eines drahtlosen Netzwerks zu implementieren, bringen solche Lösungen keine Vorteile verglichen mit ausschließlich WPA-basierten Lösungen. Dies gilt insbesondere dann, wenn die zusätzliche Komplexitätsebene für drahtlose Netzwerke berücksichtigt wird, die durch das Einfügen einer VPN-Lösung in die Mischung entsteht.

Auch die Nutzbarkeit stellt einen weiteren Faktor dar, der untersucht werden muss, wenn ein VPN als möglicher Bestandteil einer WLAN-Sicherheitslösung in Betracht gezogen wird. Obwohl die zusätzlichen Authentifizierungsanforderungen und die Grenzwerte für die Zeitüberschreitung bei VPNs von Benutzern bei der Verbindung mit einem Unternehmensnetzwerk über das Internet erwartet werden, erscheint dies einem Benutzer möglicherweise beschwerlich, der den problemlosen Zugriff auf Ressourcen innerhalb eines LAN gewohnt ist.

Einige Unternehmen bevorzugen diese Lösung unter Umständen einfach deshalb, weil sie bereits eine VPN-Lösung für Remotebenutzer eingerichtet haben und daher das vorhandene System besser ausnutzen möchten, um dessen Kosten zu rechtfertigen. Wenn dies der Fall ist, sollten unter anderem die folgenden zusätzlichen Punkte berücksichtigt werden, bevor die Lösung umgesetzt wird:
* Da eine VPN-Verbindung aufgebaut werden muss, bevor die Kommunikation durch den Tunnel erlaubt ist, gelten Gruppenrichtlinien für Computer nicht, wenn sich der Benutzer nach der Anmeldung am lokalen Computer mit dem VPN verbindet. (Wenn der Benutzer beim Anmelden an den Computer die **Anmeldung mit DFÜ-Netzwerk** auswählt, wird die VPN-Verbindung zuerst aufgebaut, und die Gruppenrichtlinie gilt.)

* Die meisten VPN-Server sind für das Sichern langsamerer Verbindungen wie DFÜ-Verbindungen oder Breitbandverkehr konzipiert und könnten zu einem Engpass im Netzwerk werden, falls viele Hochgeschwindigkeitsverbindungen aufgebaut werden.

* Je nach VPN-Konfiguration stellen die Benutzer möglicherweise Probleme beim Roaming zwischen drahtlosen Zugriffspunkten fest, da VPNs häufig Verbindungen selbst nach sehr kurzen Unterbrechungen beenden. Dies hätte zur Folge, dass sich der Benutzer bei jedem Wechsel von einem Zugriffspunkt zu einem anderen erneut manuell authentifizieren muss. Dasselbe Verhalten würde auftreten, wenn der Computer eines Benutzers in den Standbymodus übergeht.


Verwenden von IPsec

Die Verwendung von IPsec zum Sichern drahtloser Netzwerke entstand aus derselben Anforderung wie die Verwendung von VPNs zum Sichern von WLANs: als Problemumgehung für die Fehler, die in WEP gefunden wurden. Natürlich ist IPsec eine zuverlässige Methode zum Sichern vieler spezifischer Arten von Netzwerkverkehr, und es spricht auch einiges für die Verwendung von IPsec bei WLANs. Zu diesen Gründen zählen die Transparenz, die Unabhängigkeit von hardwareseitigen Zwängen der WLAN-Technologie sowie der geringe Verwaltungsaufwand, da keine zusätzlichen Server oder Softwareprogramme für den Einsatz erforderlich sind.

Allerdings gibt es bei der Verwendung von IPsec zum Sichern drahtloser Netzwerke einige Probleme:
* IPsec ist nicht in der Lage, Broadcast- oder Multicastübertragungen zu schützen, da es nur die Kommunikation zwischen zwei Parteien regelt, die sich gegenseitig authentifiziert und Schlüssel ausgetauscht haben.

* IPsec schützt nicht das drahtlose Netzwerk selbst, sondern nur die Netzwerkpakete.

* Obwohl IPsec für die Benutzer transparent ist, gilt dies nicht in gleichem Maße für die Netzwerkgeräte, da es auf der Netzwerkebene und nicht auf der MAC-Ebene ausgeführt wird. Dadurch entstehen zusätzliche Anforderungen an Firewallregeln.

* Alle Geräte, die IPsec nicht verwenden können, sind durch Abhörmaßnahmen oder Angriffe durch Benutzer gefährdet, die WLAN-Datenverkehr überwachen können.

* Die IPsec-Richtlinienverwaltung in größeren Umgebungen kann kompliziert werden, wenn IPsec zum Bereitstellen von Endpunktschutz für andere Anwendungen zusätzlich zum Schützen des Datenverkehrs im drahtlosen Netzwerk verwendet wird.


Verwenden von WEP

Die grundlegendste Form der 802.11-basierten Sicherheit ist statisches WEP, das einen installierten Schlüssel für das Steuern des Zugriffs verwendet. Hierbei wird derselbe Schlüssel als Grundlage für das Verschlüsseln drahtlosen Datenverkehrs verwendet. Der größte Vorteil dieser Methode liegt in ihrer Einfachheit. Obwohl sie gegenüber einer ungeschützten Drahtloskonfiguration eine geringfügige Verbesserung der Sicherheit mit sich bringt, leidet sie allerdings unter einigen ernsthaften Problemen bei Verwaltung und Sicherheit. Hierbei ist insbesondere zu nennen, dass es Minuten bis Stunden erfordern kann, um den installierten Schlüssel und die SSID (falls nicht mittels Broadcast übermittelt) in einem WEP-geschützten WLAN zu ermitteln, wenn es darum geht, über einen gewöhnlichen Laptop oder über im Internet verfügbare Tools Zugriff auf ein Netzwerk zu erlangen.

Eine Methode zum Verbessern des statischen WEP besteht darin, die Zugriffspunkte mithilfe von MAC-Filterung so zu konfigurieren, dass nur eine vordefinierte Gruppe von Clients auf das Netzwerk zugreifen kann. Allerdings kann auch bei diesem Ansatz auf relativ einfache Weise ein Angriff durch die Verwendung von Tools zum Ermitteln und Fälschen der MAC-Adressen der Computer erfolgen, die mit einem WLAN verbunden sind.

Es ist möglich, einige Kombinationen aus Sicherheitstechnologien mit WEP zu verwenden, um die Sicherheit in Umgebungen etwas zu erhöhen, die weder WPA noch WPA2 unterstützen. Aber selbst diese Konfigurationen sind nicht zu empfehlen, es sei denn, als Übergangsphase zwischen einer ungesicherten WLAN-Implementierung und einer sicheren WPA-basierten Konfiguration. Es stehen folgende Methoden zur Verfügung (absteigend nach Sicherheit sortiert):
* WEP mit 802.1X-Authentifizierung unter Verwendung von EAP-TLS mit Benutzer- und Computerzertifikaten und erzwungener erneuter Authentifizierung in regelmäßigen Abständen.

* WEP mit 802.1X-Authentifizierung unter Verwendung von PEAP-MS-CHAP v2 mit strengen Richtlinien für die Benutzerkennwörter und erzwungener erneuter Authentifizierung in regelmäßigen Abständen.


Keine WLAN-Sicherheit

Obwohl die Implementierung eines ungesicherten drahtlosen Netzwerks für mittelgroße Unternehmensumgebungen im Normalfall nicht zu empfehlen ist, gibt es einige wenige Situationen, in denen eine ungesicherte drahtlose Netzwerkkonfiguration die bevorzugte Lösung sein kann. Beispielsweise haben viele Städte und Gemeinden die Implementierung von kostenlosen drahtlosen Zugriffszonen in Betracht gezogen oder bereits vorgenommen. In dieser Situation könnte es empfehlenswert sein, ein Netzwerk aus ungesicherten drahtlosen Zugriffspunkten zu verwenden, die lediglich direkte Verbindungen mit dem Internet bereitstellen. Allerdings sollte in jedem Fall berücksichtigt werden, dass ungesicherte drahtlose Netzwerke gegenüber einer Vielzahl von Angriffen äußerst gefährdet sind.

WPA oder WPA2

Die Protokolle WPA (Wi-Fi Protected Access) und WPA2 (Wi-Fi Protected Access 2) wurden jeweils speziell gegen Bedrohungen entwickelt, denen IEEE 802.11-basierte drahtlose Netzwerke ausgesetzt sind. Es gibt jedoch einige Unterschiede zwischen den beiden Protokollen. WPA wurde im Jahr 2003 als Reaktion auf die Sicherheitsschwächen im WEP-Standard entwickelt und trug diesen Fehlern auf wirksame Weise Rechnung. Hierzu erfolgte die Implementierung von Unterstützung für gegenseitige Authentifizierung, die Verwendung von TKIP für die Datenverschlüsselung und die Aufnahme einer Integritätsprüfung für signierte Nachrichten, um Spoofing zu bekämpfen und Angriffe abzuwehren. WPA2 verbessert diese Sicherheitsstufe durch die Verwendung von AES anstelle von TKIP zum Sichern des Netzwerkverkehrs und sollte daher stets gegenüber dem WPA-Standard bevorzugt werden.

Sowohl WPA als auch WPA2 sind wesentlich sicherer als WEP. Bei ordnungsgemäßer Einrichtung sind derzeit in keinem der beiden Protokolle Sicherheitsfehler bekannt. Allerdings gilt WPA2 weithin als sicherer als WPA. Daher sollte nach Möglichkeit WPA2 verwendet werden, solange die Infrastruktur dies unterstützt und der zusätzliche Verwaltungsaufwand bewältigt werden kann.

Die meisten Geräte für den drahtlosen Zugriff unterstützen heute WPA2. Gleiches gilt für die aktuellsten Versionen von Windows, insbesondere Windows XP mit Service Pack 2 (SP2) und Windows Server 2003 mit SP1. Drahtlose Geräte und Clients, die WPA2 unterstützen, können auch den älteren WPA-Standard verwenden, falls einige drahtlose Zugriffspunkte oder Clients in einer Umgebung WPA2 nicht unterstützen.

**Hinweis**   Windows XP SP2-basierte Clients benötigen ein zusätzliches Updatepaket, das [Update für WPA2/WPS IE](http://support.microsoft.com/default.aspx?scid=kb;en-us;893357), um die WPA2-Zertifizierung zu unterstützen. Weitere Informationen über dieses Update finden Sie unter http://support.microsoft.com/default.aspx?scid=kb;en-us;893357.  
Außerdem weisen aktuelle Versionen von Windows keine GPO-Unterstützung für WPA2 auf, was ein beträchtlicher Nachteil bei der Verwaltung ist und die Implementierung von WPA2 wesentlich komplexer macht als von WPA. Dies könnte ein zentraler Faktor bei der Entscheidung für WPA oder WPA2 sein, da beide Standards relativ sicher sind.


#### Entwickeln einer sicheren WLAN-Lösung

Im vorherigen Abschnitt wurden Hintergrundinformationen zu den verfügbaren WLAN-Sicherheitsoptionen vermittelt. Zudem wurde erläutert, welchen Bedrohungen drahtlose Netzwerke üblicherweise ausgesetzt sind und wie jeder Ansatz diesen Bedrohungen entweder Rechnung trägt oder durch sie gefährdet ist. Anhand dieser Informationen ist es möglich, fundierte Entscheidungen zu treffen, wenn eine Entscheidung für eine bestimmte Option mit Blick auf eine spezifische Unternehmensumgebung getroffen werden soll.

Die aktuellsten Sicherheitsverbesserungen bei Standards für drahtlose Netzwerke erfolgten mit der Implementierung von WPA und WPA2. Dabei wurde den ernsthaften Sicherheitsmängeln in WEP Rechnung getragen, wodurch Problemumgehungen wie die Verwendung von IPsec oder eines VPN zum Sichern drahtloser Verbindungen keine große Rolle mehr spielen. Die Option zum Verwenden von statischem oder dynamischem WEP sind unter keinen Umständen empfehlenswert, und auch der Verzicht auf Sicherheitsfunktionalität ist nur in wenigen Situationen nützlich. Angesichts dieser Ausgangssituation müssen nur wenige Optionen durchdacht werden, wenn eine umfassende und effiziente Sicherheitslösung für WLAN-Implementierungen formuliert werden soll.

Dieser Abschnitt dient als Leitfaden für Entscheidungsträger beim Auswählen eines der empfohlenen Ansätze zum Sichern drahtloser Netzwerke. Diese von Microsoft empfohlenen Lösungen werden von Branchenanalysten, Sicherheitsexperten und führenden Anbietern als sicherste Methoden zum Implementieren eines sicheren und effizienten drahtlosen Netzwerks weithin anerkannt. Auch wenn sich dieses Dokument auf die Methode konzentriert, die für eine mittelgroße Unternehmensumgebung am besten geeignet ist, sollten dennoch alle Optionen berücksichtigt werden. Darüber hinaus soll ein vollständiger Prozess zur Entscheidungsfindung durchlaufen werden, da es immer Ausnahmen von der Regel gibt.

Der Entscheidungsprozess von Microsoft für ein sicheres WLAN

Es gibt zwei empfohlene Prozesse zum Gewährleisten von WLAN-Sicherheit sowie einen dritten gemischten Ansatz. Dabei handelt es sich um folgende Lösungen (angeordnet nach Sicherheitsstufe):
* WPA2 mit EAP-TLS unter Verwendung von Zertifikatsdiensten

* WPA2 mit PEAP-MS-CHAPv2


Neben der jeweiligen Sicherheitsstufe spielen bei der Entscheidung für einen dieser beiden Ansätze auch die Ressourcen eine Rolle, die zum Implementieren und Unterstützen jeder Lösung erforderlich sind.

WPA oder WPA2 mit PEAP-MS-CHAPv2 stellt geringere Anforderungen an die technischen Kenntnisse und die vorhandene Ausstattung, da keine zugrunde liegende Infrastruktur für Zertifikate erforderlich ist. Da derzeit alle Geräte auf dem Markt WPA2-zertifiziert und relativ erschwinglich sind, ist es sinnvoll, Geräte mit Unterstützung von WPA2 zu verwenden, selbst wenn WPA aufgrund der derzeit vorhandenen Vorteile gegenüber WPA2 bei der Verwaltung verwendet wird. Die WPA2 AES-Verschlüsselungsmethode wird weithin als sicherer als WPA mit TKIP betrachtet, und angesichts der GPO-Unterstützung, die für WPA2 geplant ist, spricht vieles dafür, bereits jetzt die Grundlage für eine zukünftige WPA2-Implementierung zu legen.

Verwenden von WPA oder WPA2 mit EAP-TLS ist die sicherste verfügbare Option zum Sichern eines WLAN, bringt aber höhere Kosten für Implementierung und Verwaltung mit sich, da diese Methode auf einer zugrunde liegenden Infrastruktur für Zertifikate beruht. Allerdings sind in vielen mittelgroßen Unternehmensumgebungen bereits Systeme vorhanden, die die erforderlichen Anforderungen für WPA2 mit EAP-TLS erfüllen. Daher wäre dies tatsächlich für viele Unternehmen die attraktivere Option. Selbst ohne das Vorhandensein der erforderlichen Technologie benötigen viele Unternehmen dieselbe Technologie, auf der diese Lösung beruht, nämlich Zertifikate und RADIUS. Daher gibt es sogar in diesem Fall einige sehr gute wirtschaftliche und technische Gründe zum Implementieren dieser Lösung.


**Abbildung 1. Der Microsoft WLAN-Entscheidungsbaum**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875845.swcg1_big(de-de,technet.10).gif)

Das Flussdiagramm in Abbildung 1 wurde in früheren Leitfäden von Microsoft verwendet, um Unternehmen dabei zu unterstützen, den am besten geeigneten sicheren WLAN-Ansatz für ihre Umgebung auszuwählen. Dabei werden bestimmte Annahmen hinsichtlich der Definition eines großen Unternehmens getroffen. Bei Verwendung dieses Flussdiagramms müssen Sie beachten, dass unter einem großen Unternehmen ein Unternehmen verstanden wird, das 500 oder mehr Mitarbeiter sowie mindestens fünf professionelle Techniker in der IT-Abteilung aufweist.

Wie bereits erwähnt, ist der Entscheidungsbaum in diesem Fall etwas irreführend, da viele mittelgroße Unternehmen, die ja die Zielgruppe dieses Dokuments sind, über die Ressourcen und erforderlichen Fähigkeiten zum Implementieren von WPA2 EAP-TLS mit Zertifikatsdiensten verfügen. Dies gilt vor dem Hintergrund, dass die meisten mittelgroßen Unternehmen mindestens über fünf IT-Mitarbeiter verfügen und die zusätzlichen Anforderungen an die Infrastruktur für eine grundlegende EAP-TLS-Implementierung erfüllen können (vier zusätzliche Server, von denen einer nicht mit dem Netzwerk verbunden wird).

Angesichts dieser Tatsachen wird klar, dass für die meisten mittelgroßen Unternehmen die beste Lösung in WPA2 unter Verwendung von EAP-TLS mit Zertifikatsdiensten besteht. Daher behandelt dieses Dokument schwerpunktmäßig diese Lösung. Allerdings gibt es immer gerechtfertigte Ausnahmen von dieser Regel, und wenn ein Unternehmen einen anderen Ansatz benötigt, gibt es zahlreiche Leitfäden für die Berücksichtigung dieser Anforderungen. Insbesondere für den Fall, dass WPA mit PEAP-MS-CHAP v2 bevorzugt wird, erhalten Sie zusätzliche Informationen im Artikel zum [Sichern von drahtlosen LANs mit PEAP und Kennwörtern](http://go.microsoft.com/fwlink/?linkid=23459) unter http://go.microsoft.com/fwlink/?linkid=23459

Serveranforderungen bei EAP-TLS

Wie zuvor kurz angesprochen, sind für EAP-TLS mindestens vier Server erforderlich (oder mehr, wenn eine verteilte oder größere Umgebung dies erfordert), von denen zwei als redundante Server für den Internetauthentifizierungsdienst (IAS) genutzt werden (die Microsoft-Implementierung von RADIUS) und zwei Bestandteil einer grundlegenden Infrastruktur für Zertifikate (PKI) sind. Von den zwei Zertifikatsservern wird die Stammzertifizierungsstelle (CA) separat angeordnet und nicht mit dem Netzwerk verbunden, um das Stammzertifikat zu schützen.

**Tabelle 3. Empfohlene Hardwarevoraussetzungen für den Server mit der Stammzertifizierungsstelle**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Komponente

</th>

<th style="border:1px solid black;">

Anforderung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


CPU

</td>

<td style="border:1px solid black;">


Einzelne CPU mit 733 MHz oder höher

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Speicher

</td>

<td style="border:1px solid black;">


256 MB RAM

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Netzwerkschnittelle

</td>

<td style="border:1px solid black;">


Keine (oder deaktiviert)

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Datenträgerspeicher

</td>

<td style="border:1px solid black;">


IDE- oder SCSI-RAID-Controller

2 x 18-GB-Festplatte, konfiguriert als einzelnes RAID 1-Volume (Laufwerk C)

Lokaler Wechseldatenträger für Datenübertragung (Stammzertifikat)

</td>

</tr>

</table>


Wie die Tabelle zeigt, sind die Anforderungen auf Grundlage der allgemeinen Anforderungen für die Windows Server 2003 Standard Edition für die Stammzertifizierungsstelle ziemlich gering. Daher kann hierfür selbst eine ältere Plattform eingesetzt werden, die bereits außer Dienst gestellt werden sollte, oder es kann ein virtueller Computer erstellt werden. Viele Kunden empfinden die Verwendung eines Laptops als effiziente Lösung, da dieser auf einfache Weise in einem Computerraum physisch gesichert werden kann. Unabhängig davon, welcher Ansatz zum Erstellen der Stammzertifizierungsstelle gewählt wird, muss sichergestellt werden, dass der betreffende Computer zuverlässig gestartet oder wiederhergestellt werden kann.

Die Hardwareanforderungen an die ausstellende Zertifizierungsstelle sind ähnlich. Allerdings gibt es hier noch zusätzliche Anforderungen an den Speicherplatz, und der Server muss mit dem Netzwerk verbunden sein. Da dieser Server alle ausgestellten Zertifikate speichern muss, wird empfohlen, dass der Server mit einer Festplattenkapazität von mindestens 2 GB für jeweils 1.000 Benutzer ausgestattet wird.

Die Anforderungen an Radius-Server sind höher, da diese Server von entscheidender Bedeutung für das Aufrechterhalten der WLAN-Funktionalität sind. Sie müssen in der Lage sein, viele Authentifizierungsversuche in kurzer Zeit zu bewältigen. Daher ist möglicherweise eine robustere Hardwareplattform für Umgebungen erforderlich, in denen Tausende von drahtlosen Clients vorhanden sind. Obwohl die Zertifizierungsstellen lediglich Windows Server 2003 Standard Edition verwenden müssen, ist es möglicherweise erforderlich, auf den IAS-Servern die Enterprise Edition auszuführen, da die Standard Edition lediglich 50 RADIUS-Clients unterstützt.

Daher wird allgemein empfohlen, dass IAS auf Domänencontrollern installiert wird, da hierdurch der Bedarf an zusätzlicher Serverhardware durch Nutzen der vorhandenen robusten Serverplattformen verringert wird, wie sie für Domänencontroller erforderlich sind. Durch die Verwendung von IAS auf Domänencontrollern wird die Leistung von IAS tatsächlich gesteigert, indem der Netzwerkverkehr verringert wird, der zwischen Domänencontrollern und IAS für die Benutzerauthentifizierung entsteht.

Failover und Redundanz sowie Überlegungen zum Remotestandort spielen ebenfalls eine Rolle, wenn die Anforderungen an RADIUS-Server ermittelt werden. Obwohl die empfohlene Mindestanforderung zwei IAS-Server vorsieht, weisen manche Unternehmen möglicherweise viele Remotestandorte auf und benötigen IAS-Server an einigen dieser Standorte. Einige Unternehmen haben möglicherweise auch höhere Anforderungen an Serverredundanz oder Lastenausgleich.

Obwohl nichts gegen die Verwendung von Multifunktionsservern als RADIUS-Server spricht, muss die zusätzliche Belastung berücksichtigt werden, denen dieser Server ausgesetzt wird. Zudem muss die Art dieser Anforderungen untersucht werden. Ein RADIUS-Server sollte so skalierbar sein, dass er auch Situationen bewältigt, in denen alle drahtlosen Clients versuchen, in kurzer Zeit eine Verbindung herzustellen.

Zertifikate

Unabhängig davon, welcher WPA-Ansatz zum Sichern eines WLAN ausgewählt wird, sind Zertifikate in verschiedenen Formen als Bestandteil dieser Lösung erforderlich. Für PEAP sind nur Zertifikate auf dem Authentifizierungsserver erforderlich. Daher wäre es möglich, einfach den Zertifikatsdienst eines Drittanbieters zu verwenden, um die benötigten Zertifikate bereitzustellen. Dies würde bedeuten, dass eine PKI-Implementierung nicht erforderlich wäre. Dies ist der Hauptgrund, weshalb der PEAP-Ansatz für kleinere Unternehmen empfohlen wird, die möglicherweise nicht über die nötige Erfahrung oder Ressourcen zum Implementieren und Unterstützen einer Infrastruktur für Zertifikate verfügen.

Die von Windows unterstützte Implementierung von EAP-TLS unter Verwendung von Zertifikatsdiensten erfordert nicht unbedingt eine zugrunde liegende PKI, um das Ausstellen von Zertifikaten zu unterstützen. Da jedoch jeder Client über ein Zertifikat verfügen muss, um die Authentifizierung mit dem RADIUS-Server vorzunehmen, kann die Verwendung von Zertifikaten von Drittanbietern aus Kostengründen möglicherweise nur für besonders kleine Unternehmen die geeignete Methode sein. Dieselben Überlegungen sind erforderlich, wenn PEAP mit Zertifikatsdiensten kombiniert werden soll.

Wenn ein Unternehmen bereits über eine PKI verfügt, ist der Entscheidungsprozess einfacher. Wenn die Komponenten schon vorhanden sind, können sie ohne weiteres genutzt werden, so dass die sicherste Option für die WLAN-Sicherheit implementiert werden kann. Selbst wenn noch keine PKI-Implementierung eingerichtet wurde, könnte bei mittelgroßen Unternehmen die Investition in eine Infrastruktur für Zertifikate empfehlenswert sein, da solche Implementierungen unter anderem für folgende Zwecke verwendet werden können:
* Codesignaturen

* Sichere E-Mail-Übertragung

* Sichere Bereitstellung von Webinhalten

* VPN-Sicherheit

* Verschlüsselte Dateidienste


Unter Berücksichtigung aller Faktoren ist der Ansatz zur Verwendung von Zertifikatsdiensten entweder mit EAP-TLS oder PEAP für mittelgroße Unternehmen am besten geeignet und steht daher im Mittelpunkt dieses Dokuments.

Erstellen einer Zertifikatverwendungserklärung

Die anfängliche Planung für eine PKI sollte eine Dokumentation umfassen, in der beschrieben wird, wie Zertifikate in der Unternehmensumgebung verwendet werden. Obwohl solche Entscheidungen nach Bedarf abgeändert werden können, ist es wichtig, zuerst eine formale Richtlinie zu Zertifikaten zu erstellen.

Bei einer Zertifikatsrichtlinie handelt es sich um eine Reihe von Regeln, die für die PKI gelten. In der Richtlinie sind Informationen zur Anwendbarkeit von Zertifikaten auf bestimmte Gruppen innerhalb des Unternehmens oder Anwendungen mit gemeinsamen Sicherheitsanforderungen erfasst. Eine Zertifikatverwendungserklärung legt die Verfahren fest, die ein Unternehmen zum Verwalten der ausgestellten Zertifikate verwendet. Sie beschreibt, wie die Zertifikatsrichtlinie im Kontext der Infrastruktur der Unternehmenssysteme und der Richtlinien für die Betriebsabläufe interpretiert wird. Obwohl eine Zertifikatsrichtlinie ein unternehmensweites Dokument ist, wird für eine Zertifizierungsstelle jeweils eine spezifische Zertifikatverwendungserklärung erstellt. Wenn Zertifizierungsstellen dieselben Aufgaben erfüllen, ist es auch möglich, dass eine gemeinsame Zertifikatverwendungserklärung verwendet wird.

In manchen Unternehmen handelt es sich bei diesen Vorgaben um juristische Dokumente, die unter Berücksichtigung gesetzlicher Anforderungen für die jeweiligen Industriezweige erstellt werden müssen. In diesem Fall ist für die Erstellung kompetente juristische Unterstützung erforderlich. Selbst wenn ein Unternehmen nicht solchen Anforderungen unterliegt, empfiehlt sich dennoch das Erstellen dieser Dokumente.

Hierarchie der Zertifizierungsstellen

Der in diesem Handbuch beschriebene Entwurf verwendet ein hierarchisches Vertrauensmodell mit einem einzelnen internen Stamm. Dieser Ansatz weist eine Reihe von Vor- und Nachteilen auf. Daher ist möglicherweise eine weitere Diskussion erforderlich, um zu bestimmen, ob dieser spezielle Ansatz in dem Unternehmen geeignet ist, in dem er implementiert werden soll. Weitere Informationen zu diesem Thema finden Sie im Kapitel [Designing a Public Key Infrastructure](http://technet2.microsoft.com/windowsserver/en/library/b1ee9920-d7ef-4ce5-b63c-3661c72e0f0b1033.mspx) (Entwerfen einer Public Key-Infrastruktur; in englischer Sprache) des Windows Server 2003-Bereitstellungskits unter http://technet2.microsoft.com/WindowsServer/en/library/b1ee9920-d7ef-4ce5-b63c-3661c72e0f0b1033.mspx.


**Abbildung 2. Hierarchie der Zertifizierungsstellen**
 

Sichern der Stammzertifizierungsstelle

Die Microsoft-Implementierung von EAP-TLS funktioniert erst dann, wenn die Stammzertifizierungsstelle nicht Bestandteil des Netzwerks ist. Es gibt eine Reihe von guten Sicherheitsgründen für die Verwendung eines Entwurfs mit einer separaten Stammzertifizierungsstelle anstelle einer Stammzertifizierungsstelle für das gesamte Unternehmen. Daher ist dies in der Regel der empfohlene Ansatz für alle PKI-Implementierungen.

Da ein solcher Ansatz wie eine Verschwendung von Ressourcen wirken mag, gibt es einige Methoden, mit denen ein Unternehmen mindestens einen Teil der Hardware erneut bereitstellen kann, die zum Erstellen einer nicht mit dem Netzwerk verbundenen Stammzertifizierungsstelle verwendet wurde. Dazu zählen unter anderem folgende Vorschläge:
* Nach dem Erstellen und Verteilen des Stammzertifikats an eine ausstellende Zertifizierungsstelle können die Festplatten aus der Stammzertifizierungsstelle ausgebaut und an einem sicheren Ort aufbewahrt werden, bis sie wieder benötigt werden. Der Nachteil dieses Ansatzes besteht darin, dass in einer Situation, in der die Stammzertifizierungsstelle wieder benötigt wird, die zugehörige Hardware für diese Laufwerke wieder beschafft werden müsste.

* Nach dem Erstellen und Verteilen des Stammzertifikats an eine ausstellende Zertifizierungsstelle kann ein Abbild des Servers durch eine Sicherung erstellt und auf Bändern oder anderen Offlinemedien gespeichert werden. Dadurch kann die Serverhardware wiederverwendet werden. Auch hier besteht dasselbe Problem wie zuvor, dass die Hardware wiederum beschafft werden müsste, sobald sie erneut benötigt wird.

* Verwenden Sie einen virtuellen Server, virtuellen PC oder eine andere Software zum Erstellen virtueller Computer, um die Stammzertifizierungsstelle zu erstellen. Nachdem das Stammzertifikat erstellt und verteilt wurde, kann das Abbild des virtuellen Computers auf einem Offlinedatenträger gespeichert und archiviert werden, falls es wieder benötigt wird. Wenn eine allgemeine Standardplattform (z. B. ein standardmäßiges Desktopsystem für Ihr Unternehmen, sofern es die Hardwareanforderungen erfüllt) für diesen Ansatz verwendet wird, ist es einfacher, die benötigte Hardware wiederzubeschaffen, falls die Stammzertifizierungsstelle erneut benötigt wird.

* Erstellen Sie die Offline-Stammzertifizierungsstelle auf einem Laptop des Vorjahres, und bewahren Sie diesen an einer sicheren Stelle im Computerraum auf. Auf diese Weise kann eine Hardwareressource genutzt werden, die anderenfalls vermutlich entsorgt würde.


Internetauthentifizierung

Internetauthentifizierungsdienst (IAS) ist die Microsoft-Implementierung eines RADIUS- und Proxyservers. IAS kann zentral Aufgaben wie Authentifizierung, Autorisierung und Kontoführung für eine Vielzahl von Netzwerkverbindungen ausführen. IAS kann mit anderen RADIUS-Servern für die Weiterleitung von Authentifizierung, Autorisierung und Kontoführung genutzt werden. Die Nutzung ist gemeinsam mit anderen VPN-Servern wie Routing- und Fernzugriffservern oder mit weiterer Netzwerkinfrastruktur wie drahtlosen Zugriffspunkten möglich.

Beim Entwickeln eines Bereitstellungsplans für eine IAS-Infrastruktur ist es wichtig, dass die Vorzüge einer IAS-basierten RADIUS-Infrastruktur genutzt werden, da sie nicht für den Zugriff auf ein einzelnes isoliertes Netzwerk vorgesehen ist. Daher sollte bei Planung und Bereitstellung einer IAS-Infrastruktur eine Entscheidung getroffen werden, ob ein zentraler Dienst für die Verwaltung von Netzwerkzugriffen verwendet werden soll, was die Verwendung einer zentralisierten Kontendatenbank wie Active Directory einschließt. Zudem sollte sichergestellt werden, dass die derzeitigen und künftigen Anforderungen des Unternehmens erfüllt werden. Mit anderen Worten: Bei der Bereitstellung einer IAS-Infrastruktur sollten strategische und nicht nur taktische Erwägungen angestellt werden.

Dieses Handbuch beschäftigt sich nur in dem Maße mit der IAS-Planung und -Bereitstellung, wie dies mit dem Erstellen einer sicheren drahtlosen Infrastruktur zu tun hat. Weitere Informationen über Möglichkeiten bei der IAS-Planung und -Bereitstellung sowie zugehörige Themen finden Sie im Abschnitt zu Bereitstellungsressourcen der Homepage des [Internetauthentifizierungsdiensts](http://www.microsoft.com/technet/itsolutions/network/ias/default.mspx) unter www.microsoft.com/technet/itsolutions/network/ias/default.mspx.

Bereits vorhandene RADIUS-Implementierungen

Obwohl diese Lösung in bereits vorhandene RADIUS-Implementierungen integriert werden kann, enthält dieses Handbuch keine Informationen zu den entsprechenden Verfahren. In den meisten Fällen wäre es von Vorteil, IAS für die in diesem Handbuch beschriebenen Funktionen zu nutzen. Um dieses Ziel zu erreichen, können entweder ältere Plattformen auf Windows 2003 Server aktualisiert werden, um als zentrale RADIUS-Server zu dienen, oder es können vorhandene RADIUS-Server geändert werden, um als Proxy den RADIUS-Datenverkehr auf die neuen Windows Server 2003-basierten RADIUS-Server umzuleiten.

Einen detaillierten Leitfaden zur Planung der Migration der vorhandenen RADIUS-Infrastruktur auf Windows Server 2003-basierte RADIUS-Server finden Sie auf der Seite [IAS Technical Reference](http://technet2.microsoft.com/windowsserver/en/library/8f5c89d5-fdaf-430c-9ef4-318f8c15baf11033.mspx) (Technische Referenz zu IAS; in englischer Sprache) unter http://technet2.microsoft.com/WindowsServer/en/Library/8f5c89d5-fdaf-430c-9ef4-318f8c15baf11033.mspx. Sie haben auch die Möglichkeit, sich an einen Microsoft-Kundenbetreuer oder einen zuständigen Mitarbeiter der Microsoft Consulting Services zu wenden.

Failover und Lastenausgleich bei RADIUS-Servern

Da RADIUS eine entscheidende Komponente jeder drahtlosen 802.1X-Sicherheitslösung darstellt, ist die Verfügbarkeit eines drahtlosen Netzwerks von der Verfügbarkeit der RADIUS-Server abhängig. Daher muss eine RADIUS-Lösung, die drahtlose Netzwerke unterstützt, zuverlässig und redundant sein und schnell ansprechen, um sicherzustellen, dass Verfügbarkeit und Leistung einem drahtgebundenen Netzwerk entsprechen. Daher wird allgemein empfohlen, IAS auf vorhandenen Domänencontrollern zu installieren.

Vor der Entscheidung für eine Strategie für den Lastenausgleich muss berücksichtigt werden, dass EAP durch 802.1X innerhalb von RADIUS (EAP-RADIUS) zwischen dem drahtlosen Zugriffspunkt und dem RADIUS-Server implementiert wird. Obwohl RADIUS selbst UDP verwendet, handelt es sich bei EAP um ein sitzungsorientiertes Protokoll, das innerhalb von RADIUS in einem Tunnel weitergeleitet wird. Dies bedeutet, dass die mehrfachen EAP-RADIUS-Pakete, aus denen ein einzelner Authentifizierungsvorgang besteht, zum selben RADIUS-Server zurückkehren müssen, da anderenfalls dieser spezielle Authentifizierungsversuch nicht erfolgreich abgeschlossen wird.

Es gibt zwei Ansätze für Lastenausgleich und Failover auf IAS-Servern hinsichtlich drahtloser Netzwerke. Der erste Ansatz besteht darin, IAS-Proxyserver mit RADIUS-Servergruppen zu verwenden. Der zweite Ansatz sieht vor, primäre und sekundäre RADIUS-Server durch Hardwareeinstellungen an den drahtlosen Zugriffspunkten zu konfigurieren. In der folgenden Tabelle sind die Vor- und Nachteile der einzelnen Ansätze aufgeführt.

**Tabelle 4. RADIUS-Failover und Lastenausgleich für EAP**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Methode

</th>

<th style="border:1px solid black;">

Vorteile

</th>

<th style="border:1px solid black;">

Nachteile

</th>

</tr>

<tr>

<td style="border:1px solid black;">


IAS-Proxys mit RADIUS-Servergruppen

</td>

<td style="border:1px solid black;">

* Ausfallerkennung für RADIUS-Dienste mit Failover und Failback

* Verteilung der Datenverkehrslast gemäß den Eigenschaften des Datenverkehrs

* Behält den EAP-Sitzungszustand während des Lastenausgleichs bei

* Konfigurierbare Anforderungsverteilung an Server gemäß Prioritäts- und Lasteinstellungen


</td>

<td style="border:1px solid black;">

* Zusätzliche IAS-Server erforderlich

* Erfordert weiterhin die Konfiguration von primären und sekundären Proxy-RADIUS-Serveradressen


</td>

</tr>

<tr>

<td style="border:1px solid black;">


Primäre und sekundäre RADIUS-Servereinstellungen an drahtlosen Zugriffspunkten

</td>

<td style="border:1px solid black;">

* Einfachere Konfiguration für kleinere Umgebungen

* Drahtloser Zugriffspunkt erkennt Ausfall bei Datenverkehr und führt Failover aus

* Verwendet die systemeigene Funktionalität von drahtlosen Zugriffspunkten


</td>

<td style="border:1px solid black;">

* Erfordert mehr Aufwand für Planung und Überwachung für primäre und sekundäre RADIUS-Datenverkehrsverteilung

* Einige drahtlose Zugriffspunkte unterstützen weiterhin nicht die Failbackfunktionalität, was zu nicht ausgeglichenen Datenverkehrslasten führen kann.


</td>

</tr>

</table>


Größere Unternehmen sollten die Verwendung von RADIUS-Proxys in Betracht ziehen, die in RADIUS-Servergruppen konfiguriert sind, um die Lasten auf RADIUS-Servern zu verteilen. Dies ermöglicht ein höheres Maß an Flexibilität, da die Verteilung des Datenverkehrs zusätzlich zur Gewichtung und Priorisierung auch nach einigen konfigurierbaren Elementen erfolgt, zu denen der RADIUS-Datenverkehrstyp und RADIUS-Attribute zählen. Dieser Architekturtyp ermöglicht auch die größte Flexibilität und Skalierbarkeit für das Bearbeiten von Authentifizierungsanforderungen und stellt gleichzeitig geringere Anforderungen an die Verwaltung.

Die einfachere Funktionalität zum RADIUS-Serverfailover, die in die drahtlosen Zugriffspunkte integriert ist, kann ein ausreichendes Maß an Ausfallsicherheit für die meisten Unternehmen bereitstellen, ist aber im Vergleich zur Verwendung von Proxyservergruppen keine sehr leistungsfähige Lösung. Allerdings ist der Migrationspfad von dieser Architektur zu Failover und Lastenausgleich auf der Grundlage von RADIUS-Proxyservern relativ einfach, so dass diese Lösung durchaus ausbaufähig ist. Bei Unternehmen, die lediglich eine kleine oder begrenzte Abdeckung mit Drahtlostechnologie in Betracht ziehen, kann diese Lösung einfach implementiert werden und bietet gute Effizienz. Allerdings wachsen die Anforderungen an Verwaltung und Implementierung, wenn die Größe und Komplexität eines drahtlosen Netzwerks wächst, da jedes Gerät sorgfältig überwacht und geplant werden muss, um einen effizienten Lastenausgleich über alle Server hinweg zu gewährleisten.


**Abbildung 3. Methoden für RADIUS WLAN-Failover und Lastenausgleich**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875845.swcg3_big(de-de,technet.10).gif)

Lastenausgleich mit der integrierten Funktionalität von drahtlosen Zugriffspunkten erfordert die Konfiguration von ungefähr der Hälfte der drahtlosen Zugriffspunkte an jedem Standort für die Verwendung des primären RADIUS-Servers bzw. des sekundären Servers, während die andere Hälfte der drahtlosen Zugriffspunkte eine umgekehrte Zuordnung in den Feldern für primäre und sekundäre Server verwendet. Dies wird in Abbildung 3 näher beschrieben. Der hohe Verwaltungsaufwand wird offensichtlich, da an manchen Zugriffspunkten eine höhere Last auftritt als an anderen und daher ein hohes Maß an Überwachung erforderlich ist, um einen effizienten Lastenausgleich zu erreichen.

RADIUS-Protokollierungsanforderungen

IAS-Server sind in der Lage, zwei Typen von optionalen Ereignissen zu protokollieren:
* Erfolgreiche und fehlgeschlagene Authentifizierungsversuche.

* RADIUS-Authentifizierung und Kontoinformation


Authentifizierungsereignisse werden von Geräten und Benutzern generiert, wenn versucht wird, auf das WLAN zuzugreifen. Die Ereignisse werden von IAS im Systemereignisprotokoll von Windows Server 2003 aufgezeichnet. Diese Ereignisse sind für die Problembehandlung nützlich und zugleich wichtiger Bestandteil eines Systems zur Sicherheitsprüfung und Einbrucherkennung. Diese Ereignisse sollten anfänglich sowohl für Erfolgs- als auch Fehlerereignisse aktiviert werden, später jedoch gefiltert werden, um einen Überlauf des Systemereignisprotokolls zu vermeiden. Die Verwendung der Protokollierung für RADIUS-Authentifizierungsanforderungen macht den Rückgriff auf diese Ereignisse aus Sicherheitsgründen unnötig, falls aktiviert.

Zentrale oder verteilte IAS-Server

Eine zentrale IAS-Serverarchitektur sollte als Ausgangspunkt für die meisten mittelgroßen Unternehmen betrachtet werden, da die meisten Unternehmen dieser Größe über robuste Hochgeschwindigkeits-WAN-Verbindungen zu Remoteeinrichtungen verfügen. Zudem benötigt der RADIUS-Datenverkehr nicht viel Bandbreite, da er für die Verwendung über WAN-Links und DFÜ-Verbindungen konzipiert wurde. Ein zentralisierter Entwurf ist auch kostengünstiger, solange eine zugrunde liegende redundante Hochgeschwindigkeits-WAN-Infrastruktur bereits vorhanden ist.

Selbst dann muss die aktuelle Kapazität der vorhandenen WAN-Links sorgfältig analysiert werden, um zu bestimmen, ob es sich dabei um die beste Option handelt, da bei anderen Kommunikationsarten wie DHCP-Datenverkehr Zeitüberschreitungen auftreten könnten, während auf das Ende von 802.1X-Authentifizierungsversuchen über stauträchtige Verbindungen gewartet wird. Die Clientkonnektivität ist nicht das einzige zu berücksichtigende Problem, wenn die Entscheidung für oder gegen eine zentralisierte IAS-Architektur ansteht, da auch die Kommunikation zwischen IAS-Servern und Domänencontrollern robuste Netzwerkverbindungen erfordert, um Zeitüberschreitungen beim Bestimmen der Netzwerkzugriffsrechte und Gruppenmitgliedschaften zu vermeiden.

Einige Unternehmen sind möglicherweise nicht in der Lage, eine zentralisierte Architektur zu nutzen, da redundante WAN-Verbindungen mit hoher Bandbreite und die hoch entwickelte Netzwerkausrüstung hohe Kosten verursachen. Solche Unternehmen werden sich für einen verteilten IAS-Entwurf entscheiden. Dies gilt insbesondere dann, wenn eine dezentrale Serverinfrastruktur bereits vorhanden ist.

Ein weiterer Ansatz besteht in der Verwendung einer Mischung aus beiden Lösungen. Dabei werden IAS-Server strategisch an Standorten platziert, die die Infrastruktur unterstützen können. Diese Server stellen die Authentifizierung für Zweigniederlassungen bereit, die möglicherweise nicht über eine zugrunde liegende Serverbasis verfügen, wie dies in der folgenden Abbildung gezeigt wird.


**Abbildung 4. Gemischter Ansatz für IAS WLAN-Infrastruktur**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875845.swcg4_big(de-de,technet.10).gif)
 

In diesem Handbuch werden alle drei Modelle behandelt. Es wird beschrieben, wie große zentrale Niederlassungen mit zwei RADIUS-Servern konfiguriert werden, die sowohl lokale als auch Remoteanforderungen bearbeiten können, und es wird erläutert, wie große Homeoffices mit optionalen Einzelserver-Zweigstellen konfiguriert werden können.

**Hinweis**   Auch hierbei hängt der WLAN-Zugriff in den Remoteniederlassungen ohne Serverinfrastruktur von der WAN-Verfügbarkeit ab.

Aspekte der Platzierung von IAS-Servern und der Kollokation

Um den Zugang zu WLAN-Diensten aufrechtzuerhalten, müssen mindestens zwei RADIUS-Server für jede unabhängige Active Directory-Gesamtstruktur vorhanden sein. Neben dieser grundlegenden Anforderung gibt es eine Reihe von Faktoren, die bestimmen, wie viele Server erforderlich sind und ob sie möglicherweise für die Kollokation mit anderen Serverfunktionen geeignet sind.

Im Allgemeinen sollte sich die Platzierung der IAS-Server an der Platzierung der Domänencontroller orientieren. Wenn also eine Niederlassung bereits einen Hochgeschwindigkeits-WAN-Link zu einer anderen Niederlassung für Domänendienste verwendet, sollte diese Niederlassung in den meisten Fällen auch einen Remote-RADIUS-Server verwenden. Größere Niederlassungen, die bereits über eigene Domänencontroller verfügen, benötigen wahrscheinlich mindestens einen RADIUS-Server mit einem möglichen Failover, der sich je nach vorhandenem WAN-Link an anderer Stelle befindet. Die vorhandene Kapazität des WAN-Links muss sorgfältig geprüft werden, wenn die Platzierung der RADIUS-Server mit Blick auf die Zuverlässigkeit der Authentifizierung für lokale Benutzer geplant wird. Gleiches gilt für die Platzierung der für die Authentifizierung verwendeten Domänencontroller, was auf den zusätzlich generierten Datenverkehr zurückzuführen ist. Aus Gründen der Leistungssteigerung sollten sich die RADIUS-Server in der Stammdomäne einer Gesamtstruktur befinden, um die Kerberos-Abläufe zu optimieren.

Darüber hinaus ist zu überlegen, ob es sinnvoll wäre, zusätzliche Server an Remotestandorten zu platzieren, wenn dort ein entsprechender Bedarf besteht. Manche kleinere Niederlassungen verfügen möglicherweise nicht über ausreichend Platz oder die erforderliche Infrastruktur, um zusätzliche Serverhardware zu unterstützen. Um diesen Problemen Rechnung zu tragen, ist es möglich, einen IAS-Server mit einem Active Directory-Domänencontroller auf derselben Festplatte zu betreiben. In der folgenden Tabelle werden einige Vor- und Nachteile dieses Ansatzes beschrieben.

**Tabelle 5. Aspekte der gemeinsamen Platzierung von IAS und Domänencontroller**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

IAS-Standort

</th>

<th style="border:1px solid black;">

Vorteile

</th>

<th style="border:1px solid black;">

Nachteile

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Gemeinsam auf Domänencontroller platziert

</td>

<td style="border:1px solid black;">

* Leistung von Authentifizierung und Autorisierung für Benutzer und Computer steigt

* Verringert die Anforderungen an zusätzliche Serverhardware


</td>

<td style="border:1px solid black;">

* Keine Trennung der administrativen IAS-Gruppen von Domänenadministratoren

* Keine inhärente Trennung von Problemen mit Fehlern oder Leistung, die auf gemeinsam gehostete Dienste zurückzuführen sind


</td>

</tr>

<tr>

<td style="border:1px solid black;">


Unabhängige IAS-Server

</td>

<td style="border:1px solid black;">

* Trennung der IAS-Verwaltung von den Domänenadministratoren

* IAS-Last und -Verhalten beeinträchtigt nicht den Domänencontroller


</td>

<td style="border:1px solid black;">

* Zusätzliche Serverhardware erforderlich.


</td>

</tr>

</table>


Wie diese Tabelle zeigt, gibt es gute Gründe, weshalb viele Unternehmen über Richtlinien verfügen, die die Funktionalität von Domänencontrollern auf ihre eigenen Server begrenzen, da diese für die Netzwerkumgebung von so entscheidender Bedeutung sind. Möglicherweise gibt es auch Sicherheitsbedenken hinsichtlich der Platzierung von IAS-Diensten auf einem Domänencontroller, wenn eine Trennung der Aufgaben zwischen beiden administrativen Gruppen vorhanden ist, da es keine inhärente Trennung der IAS-Verwaltung von Funktionen der lokalen Windows-Administratorengruppe gibt. Diese Themen müssen berücksichtigt werden, bevor über ein mögliches gemeinsames Hosten der IAS-Dienste entschieden wird. Bei einer entsprechenden Entscheidung hierfür können gewisse Leistungsvorteile genutzt werden, vom offensichtlichen Kostenvorteil ganz zu schweigen, der besonders bei Remotestandorten zum Tragen kommt.

Um den Kostenfaktor beim Hinzufügen von Serverhardware zu Remoteniederlassungen auszugleichen, besteht die Möglichkeit, Domänencontroller zu verwenden, die möglicherweise bereits an Remotestandorten vorhanden sind. Die IAS-Server können entweder direkt oder durch Hinzufügen eines virtuellen Computers zum vorhandenen Domänencontroller realisiert werden.

Einschätzen von Serverbelastung und Hardwareanforderungen

Beim Ermitteln der potenziellen Serverlast sollte vom ungünstigsten Fall ausgegangen werden. Insbesondere sollte bedacht werden, was geschieht, wenn alle potenziellen WLAN-Nutzer eine Authentifizierung in kurzer Zeit während eines Failoverereignisses ausführen müssen. Der optimale Entwurf stellt die Mindestanzahl von Servern für robusten Betrieb zur Verfügung und lässt noch Raum für künftiges Wachstum nach Bedarf.

Die folgenden Informationen sollten berücksichtigt werden, wenn die Planung für die IAS-Serverlasten und -Anforderungen erstellt wird:
* Die Anzahl der Benutzer und Geräte, die Authentifizierung und Kontoführung benötigen

* Die Authentifizierungsoptionen wie EAP-Typ und Häufigkeit der erneuten Authentifizierung

* RADIUS-Optionen wie Protokollierungsdetails und IAS-Softwarenachverfolgung


Bei dieser Lösung, dem Verwenden von WPA oder WPA2 mit EAP-TLS-Zertifikatsdiensten, ist nicht zu vergessen, dass im Gegensatz zu WEP bei WPA und WPA2 geringere Anforderungen hinsichtlich der erzwungenen erneuten Authentifizierung zum Aktualisieren von Sitzungsschlüsseln bestehen, so dass in dieser Hinsicht weniger Verwaltungsaufwand erforderlich ist. Außerdem ist zu erwähnen, dass EAP-TLS ein rechenintensives Verfahren für öffentliche Schlüssel bei jeder anfänglichen Authentifizierung erfordert, später jedoch zwischengespeicherte Anmeldeinformationen bei jeder nachfolgenden Anmeldung eine schnelle erneute Verbindung ermöglichen. Dies gilt bis zum Ablaufen der zwischengespeicherten Anmeldeinformationen, was standardmäßig nach jeweils acht Stunden erfolgt. In diesem Zusammenhang ist auch wichtig, dass die erneute Authentifizierung stattfindet, wenn ein Client per Roaming von einem drahtlosen Zugriffspunkt, der mit einem RADIUS-Server eine Authentifizierung durchführt, zu einem anderen drahtlosen Zugriffspunkt wechselt, der eine Authentifizierung mit einem anderen Authentifizierungsserver durchführt. Dies erfolgt nur einmal pro Authentifizierungsserver und ist für den Benutzer transparent.

Beim Einschätzen der IAS-Serverkapazität ist es hilfreich, die Anzahl der Authentifizierungen pro Sekunde zur Schätzung der potenziellen Belastung heranzuziehen. Die folgende Tabelle zeigt die geschätzte Kapazität von Authentifizierungen pro Sekunde bei einem IAS-Servers mit Active Directory auf einer Plattform mit Intel Pentium 4 2-GHz-CPU.

**Tabelle 6. Authentifizierungen pro Sekunde**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Authentifizierungstyp

</th>

<th style="border:1px solid black;">

Authentifizierungen pro Sekunde

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Neue EAP-TLS-Authentifizierungen

</td>

<td style="border:1px solid black;">


36

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Neue EAP-TLS-Authentifizierungen mit Offload-Card-Unterstützung

</td>

<td style="border:1px solid black;">


50

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Authentifizierungen mit schneller Wiederherstellung der Verbindung

</td>

<td style="border:1px solid black;">


166

</td>

</tr>

</table>


**Hinweis**   Die Informationen in dieser Tabelle sollten nur als Schätzung betrachtet werden, die zur Planung der Kapazitäten als mögliche Richtlinie herangezogen wird.

In dieser Tabelle wird vorgeschlagen, dass ein solcher Server in der Lage wäre, 36 neue Authentifizierungen pro Sekunde bei einem Failover oder einem Ereignis mit Spitzenbelastung zu verarbeiten und somit rund 3 Sekunden für die Authentifizierung von 100 Benutzern benötigen würde.

Ein weiterer Faktor, der berücksichtigt werden muss, ist die Auswirkung der datenträgerbasierten Protokollierung auf die Authentifizierungszeiten. Ein langsames Datenträger-Subsystem kann einen negativen Einfluss auf die Authentifizierungszeiten haben, wenn eine detaillierte Protokollierung zum Nachverfolgen der Authentifizierungsaktivitäten verwendet wird. Stellen Sie daher sicher, dass Sie ein schnelles Datenträger-Subsystem verwenden, um auf jedem IAS-Server eine vernünftige Reaktionszeit zu erreichen.

WPA 802.11-Authentifizierung

Die Verwendung einer Infrastruktur für Zertifikate und RADIUS zum Sichern drahtloser Kommunikation durch Benutzer- und Geräteauthentifizierung wurde nun behandelt. Als Nächstes stellt sich die Frage, wie die zwischen den drahtlosen Geräten ausgetauschten Daten vor Abhörmaßnahmen und anderen Risiken geschützt werden können.

Die Verwendung von Funkübertragungen wird von jeher als unsicherer als kabelgebundene Kommunikation betrachtet, da es wesentlich weniger Aufwand erfordert, drahtlos übertragene Daten abzufangen als ein Kabel oder eine Verteilertafel anzuzapfen. Dies gilt insbesondere für den Fall, dass Portsicherheit verwendet wird. Um den systembedingten Unsicherheiten der drahtlosen Kommunikation entgegenzuwirken, ist es erforderlich, die Daten zu verschlüsseln. Auf diese Weise erhalten Personen, die die Kommunikation abhören, keine einfach zu lesenden Informationen.

Die anfänglichen WEP-Spezifikationen für drahtlose Verschlüsselung erwiesen sich als unzureichend für diese Aufgabe. Daher wurde zur Problemumgehung WPA entwickelt, eine Untergruppe der 802.11i-Spezifikation, die zu diesem Zeitpunkt noch nicht endgültig fertig gestellt war. Schließlich wurde WPA2 als vollständige Implementierung des nunmehr offiziellen Standards 802.11i erstellt. Der größte Unterschied zwischen WPA und WPA2 besteht in der Verschlüsselungsmethode. WPA verwendet hierzu TKIP, während WPA2 den AES-CCMP-Standard verwendet, der ein höheres Maß an Sicherheit gewährleistet.

Obwohl die in diesem Handbuch vorgestellte Lösung verwendet werden kann, um WEP oder WPA zu sichern, wird die Verwendung von WPA2 empfohlen. Auf diese Weise kann das höchste und zuverlässigste Sicherheitsniveau erreicht werden, das für die drahtlose Kommunikation verfügbar ist, falls die zugehörigen Verwaltungsaufgaben bewältigt werden können. Anderenfalls stellt auch die Verwendung von WPA gemeinsam mit der in diesem Handbuch vorgestellten Lösung ein angemessenes Sicherheitsniveau zur Verfügung.

Anforderungen an die Clients

Die in diesem Handbuch skizzierte Lösung wurde für Clientcomputer mit Unterstützung für Drahtlostechnologie entworfen, die Windows XP Professional mit SP2 oder Windows XP Tablet Edition als Betriebssystem verwenden. Diese Versionen des Betriebssystems Windows bieten integrierte Unterstützung für 802.1X und WLAN. Außerdem stellen Clients auf der Grundlage von Windows XP die Funktionalität für automatische Registrierung und Erneuerung von Zertifikaten bereit, was eine zertifikatbasierte Lösung wie diese besonders dann sehr kostengünstig gestaltet, wenn sie an eine Infrastruktur für Zertifikate angebunden ist.

Obwohl Windows XP SP2 integrierte Unterstützung für WPA aufweist, muss ein zusätzliches Update installiert werden, um die Unterstützung für IEEE 802.11i WPA2 auf Windows XP SP2-basierten Clients zu ermöglichen. Weitere Informationen über dieses zusätzliche Update sowie Downloadanweisungen finden Sie unter Wi-Fi Protected Access 2 (WPA2)/Wireless Provisioning Service Information Element (WPS IE) update  
for Windows XP with Service Pack 2 (Update für Windows XP mit Service Pack 2 und WPA2/WPS IE; in englischer Sprache) unter http://support.microsoft.com/default.aspx?scid=kb;en-us;893357.

Anforderungen an die Serverinfrastruktur

Wie zuvor besprochen, erfordert diese Lösung die Verwendung der Zertifikatsdienste und IAS-Komponenten von Windows Server 2003. Einige integrierte Funktionen, die von der Implementierung der Zertifikatsdienste in Windows Server 2003 unterstützt werden, sind spezifisch für 802.1X-WLANs. Obwohl IAS und Zertifikatsdienste auf älteren Versionen von Windows bereitgestellt werden können, wurde dieses Handbuch speziell für eine Windows Server 2003 Active Directory-Umgebung geschrieben.

Anforderungen an die drahtlosen Zugriffspunkte

Dieses Handbuch konzentriert sich auf die Sicherheitskomponente einer WLAN-Lösung. Daher erhalten Sie keine Anweisungen für die Bereitstellung, Positionierung oder Kanalauswahl für die Hardware der drahtlosen Zugriffspunkte. Weitere Informationen zu spezifischen Themen hinsichtlich der Hardware drahtloser Zugriffspunkte, zur Konfiguration sowie Hinweise zur Platzierung finden Sie in der beiliegenden Gerätedokumentation oder auf der Website des Herstellers.

Diese Lösung ist am sichersten, wenn sie in Verbindung mit einem drahtlosen Zugriffspunkt verwendet wird, der gemäß IEEE 802.11i WPA2 zertifiziert ist und integrierte Funktionalität für Failover/Failback bietet. Es ist möglich, diese Lösung mit WPA-zertifizierter Ausrüstung zu implementieren, ohne größere Änderungen an der hier beschriebenen Methode vornehmen zu müssen. Auch in diesem Fall wird ein sehr hohes Niveau an Sicherheit erreicht. Obwohl es auch möglich ist, diese Lösung mit dem WEP-Standard zu implementieren, wird dies nicht empfohlen und in diesem Handbuch auch nicht unterstützt.


#### Bereitstellung und Verwaltung

Obwohl dieser Abschnitt schrittweise Anweisungen zur Installation und Konfiguration von Servern und Diensten enthält, die für die Lösung erforderlich sind, werden die tatsächlichen Installations- und Konfigurationsschritte nicht beschrieben, die für Betriebssysteme wie Windows Server 2003 und Windows XP Professional nötig sind. Es wird davon ausgegangen, dass die meisten Unternehmen entsprechende Implementierungsprozesse und Richtlinien für die Absicherung eingerichtet haben.

Zertifikate

Obwohl dieser Abschnitt detaillierte Anweisungen für die Installation einer PKI enthält, werden keinerlei Details für das Erstellen der Serverkonfiguration oder das Absichern genannt. Der Grund hierfür liegt darin, dass davon ausgegangen werden kann, dass für diese Vorgänge bereits standardisierte Verfahren vorhanden sind.

Zudem wird angenommen, dass die Server für die Zertifizierungsstelle bereits mit einem Basisabbild konfiguriert und mit einem standardisierten Unternehmensprozess abgesichert wurden, bevor diese Phase der Lösung eingeleitet wird.

**Hinweis**   Beachten Sie, dass die Stammzertifizierungsstelle nie mit dem Netzwerk verbunden wird. Daher sollten alle Schritte beim Konfigurieren eines Servers im Unternehmen und zum Absichern, die eine Netzwerkverbindung voraussetzen, entsprechend geändert werden.

Zuvor benötigte benutzerdefinierte Konfigurationsinformationen

In der folgenden Tabelle werden unternehmensspezifische Parameter aufgeführt, die gesammelt oder festgelegt werden müssen, bevor eine Bereitstellung der später in diesem Handbuch beschriebenen Lösung erfolgt. Im gesamten Handbuch werden Platzhalter verwendet, um Einstellungen zu beschreiben. Dabei wird ein ähnliches Format wie beim Namen der Einstellung verwendet. Beispielsweise könnte der DNS-Name einer Stammdomäne in einer Active Directory-Gesamtstruktur als *DomainName*.com angezeigt werden. Die kursiv formatierten Werte sollten durch die spezifischen Unternehmensinformationen ersetzt werden, die während dieses Prozesses gesammelt werden.

**Tabelle 7. Benutzerdefinierte Konfigurationsinformationen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Referenz

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


DNS-Name der Active Directory-Gesamtstruktur

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Distinguished Name (DN) des Stamms der Gesamtstruktur

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


NetBIOS-Name der Domäne

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


NetBIOS-Name der Stammzertifizierungsstellen-Arbeitsgruppe

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Servername der Stammzertifizierungsstelle

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Servername der ausstellenden Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


X.500 CN der Stammzertifizierungsstelle

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


X.500 CN der ausstellenden Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Vollqualifizierter Hostname des Webservers, der zum Veröffentlichen der Zertifikate der Zertifizierungsstelle verwendet wird

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

</table>


Erforderliche Konfigurationselemente für die Lösung

Die in der folgenden Tabelle genannten Einstellungen müssen unter normalen Umständen nicht geändert werden. Stellen Sie sicher, dass alle Auswirkungen und Abhängigkeiten in Zusammenhang mit dem Ändern dieser Parameter vollständig klar sind, bevor die hier aufgeführten Einstellungen geändert werden.

**Tabelle 8. Vorgeschriebene Konfigurationselemente für die Lösung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Referenz

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


**Administratorfunktion-Sicherheitsgruppen**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administratoren des Konfigurationscontainers „Public Key Services“

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


Enterprise PKI Admins

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administrative Gruppe mit Erlaubnis zum Veröffentlichen von CRLs und Zertifizierungsstellen-Zertifikaten für Container mit Unternehmenskonfiguration

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


Enterprise PKI Publishers

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administrative Gruppe, die Zertifizierungsstellen konfiguriert und wartet und die Fähigkeit zum Zuweisen aller anderen Zertifizierungsstellenfunktionen und zum Erneuern des Zertifikats für die Zertifizierungsstelle steuert.

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


CA Admins

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administrative Gruppe, die die Registrierung für Zertifikate sowie Sperrungsanforderungen genehmigt (Funktion „CA Officer“)

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


Certificate Managers

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administrative Gruppe, die die Prüfung der Zertifizierungsstelle und die Sicherheitsprotokolle verwaltet.

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


CA Auditors

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Administrative Gruppe, die Sicherungen der Zertifizierungsstelle verwaltet

</td>

<td style="border:1px solid black;">


ca_setup.wsf

</td>

<td style="border:1px solid black;">


CA Backup Operators

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**IIS-Konfiguration**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Name des virtuellen IIS-Verzeichnisses, das zum Veröffentlichen des Zertifikats der Zertifizierungsstelle und für CRL-Informationen verwendet wird.

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


pki

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Physischer Pfad auf der ausstellenden Zertifizierungsstelle, der dem virtuellen IIS-Verzeichnis zugeordnet wird

</td>

<td style="border:1px solid black;">


C:\CAWWWPub

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**Allgemeine Parameter der Zertifizierungsstelle**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Laufwerk und Pfad für Anforderungsdateien der Zertifikatsdienste

</td>

<td style="border:1px solid black;">


C:\CAConfig

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Laufwerk und Pfad für Datenbankprotokolle der Zertifikatsdienste

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


%windir%\System32\CertLog

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**Konfiguration der Stammzertifizierungsstelle**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Schlüssellänge der Stammzertifizierungsstelle (siehe Hinweis)

</td>

<td style="border:1px solid black;">


4096

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Gültigkeitsdauer des Zertifikats der Stammzertifizierungsstelle (Jahre)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


16

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Maximale Gültigkeitsdauer für Zertifikate, die von der Stammzertifizierungsstelle ausgestellt werden (Jahre)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


8

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CRL-Veröffentlichungsintervall der Stammzertifizierungsstelle (Monate)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


6

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CRL-Überlappungsdauer (Tage)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


10

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Delta-CRL-Veröffentlichungsdauer für Stammzertifizierungsstelle (Stunden, 0=deaktivieren)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**Konfiguration der ausstellenden Zertifizierungsstelle**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Laufwerk und Pfad für Datenbank der Zertifikatsdienste.

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


D:\CertLog

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Länge des Schlüssels der ausstellenden Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


2048

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Gültigkeitsdauer des Zertifikats der ausstellenden Zertifizierungsstelle (Jahre)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


8

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Maximale Gültigkeitsdauer für Zertifikate der ausstellenden Zertifizierungsstelle (Jahre)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


4

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CRL-Veröffentlichungsintervall der ausstellenden Zertifizierungsstelle (Tage)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


7

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CRL-Überlappungsdauer (Tage)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


4

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Delta-CRL-Veröffentlichungsdauer für ausstellende Zertifizierungsstelle (Tage, 0=deaktivieren)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Delta-CRL-Überlappungsdauer. (Tage)

</td>

<td style="border:1px solid black;">


Pkiparams.vbs

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


**Verschiedenes**

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad der Installationsskripts

</td>

<td style="border:1px solid black;">


 

</td>

<td style="border:1px solid black;">


C:\MSSScripts

</td>

</tr>

</table>


**Hinweis**   Die Verwendung von Schlüsseln mit einer Länge von 4096 Bit kann gewisse Kompatibilitätsprobleme verursachen, wenn sie von einigen Geräten oder älterer Software von anderen Anbietern genutzt werden. Alle Anwendungen, die von der Stammzertifizierungsstelle ausgestellte Zertifikate verwenden könnten, sollten mit Zertifikatsschlüsseln dieser Größe getestet werden, um die ordnungsgemäße Funktionalität sicherzustellen. Die Schlüssellänge der Stammzertifizierungsstelle kann auf 2048 Bit verringert werden, wenn Bedenken hinsichtlich der Kompatibilität der Schlüssellänge bestehen.

Installieren der Konfigurationsskripts auf den Servern der Zertifizierungsstelle

Die Unterstützungsskripts, die gemeinsam mit diesem Leitfaden bereitgestellt werden, sollen Sie beim Einrichten der in den folgenden Abschnitten bereitgestellten Lösung unterstützen. Diese Skripts müssen auf jedem Server der Zertifizierungsstelle installiert werden. Sie dürfen nicht gelöscht werden, nachdem sie zur Unterstützung des Betriebs dieser Server verwendet wurden. Um diese Skripts zu installieren, erstellen Sie zuerst einen Ordner mit der Bezeichnung „C:\MSSskripts“, und kopieren Sie dann die Skripts in dieses Verzeichnis.

Installieren und Konfigurieren von IIS auf dem Server für die ausstellende Zertifizierungsstelle

Internetinformationsdienste (IIS) wird als Downloadpunkt für Nicht-Windows-Clients verwendet, um Zertifikate und CRLs der Zertifizierungsstelle abzurufen. Die Stammzertifizierungsstelle muss diesen Dienst nicht zur Verfügung stellen, da sie nicht mit einem Netzwerk verbunden ist. Die ausstellende Zertifizierungsstelle sollte jedoch über Zugriff auf diesen Dienst verfügen.

IIS kann auch verwendet werden, um die webbasierten Registrierungsseiten der Zertifikatsdienste zu hosten, obwohl diese in der vorliegenden Lösung nicht verwendet werden. Wenn die webbasierten Registrierungsseiten auf einem anderen System als der ausstellenden Zertifizierungsstelle installiert werden, muss dieser Server als „Für Delegierungszwecke vertraut“ gekennzeichnet werden, indem diese Eigenschaft im Computerobjekt des Servers in Active Directory festgelegt wird.

IIS kann mit „Windows-Komponenten hinzufügen/entfernen“ installiert werden. Diese Option finden Sie in der Systemsteuerung unter „Software“. Die folgende Liste zeigt die Komponenten, die installiert werden müssen:
* Anwendungsserver

* COM+-Zugriff über Netzwerk aktivieren

* Internetinformationsdienste

* Gemeinsame Dateien

* Internetinformationsdienste-Manager

* WWW-Dienst


**So installieren Sie IIS**
* Führen Sie folgenden Befehl an einer Eingabeaufforderung aus:
Sysocmgr /i:sysoc.inf /u:C:\MSSScripts\OC_AddIIS.txt
Dieser Befehl weist den Manager für die Installation optionaler Komponenten an, die Komponentenkonfigurationen zu verwenden, die in der Installationsdatei „C:\MSSScripts\OC_AddIIS.txt“ für unbeaufsichtigte Installationen gespeichert sind. Dort wurde folgende Konfiguration gespeichert:
[Components]complusnetwork = Oniis_common = Oniis_asp = Oniis_inetmgr = Oniis_www = On
**Hinweis**    ASP (Active Server Pages) ist in dieser Konfigurationsdatei aktiviert. Wenn die webbasierten Registrierungsseiten der Zertifikatsdienste nicht benötigt werden, sollte ASP durch Löschen der Zeile **iis_asp = on** vor dem Ausführen von „sysocmgr.exe“ deaktiviert werden. Diese Einstellung kann bei Bedarf später aktiviert werden.

* Führen Sie den Manager für die Installation optionaler Komponenten nochmals aus, und überprüfen Sie, ob die installierten Komponenten mit den zuvor aufgeführten Komponenten übereinstimmen.
sysocmgr /i:sysoc.inf
Es sind keine weiteren Unterkomponenten des Anwendungsservers erforderlich. Daher müssen keine anderen Komponenten ausgewählt werden.

Konfigurieren von IIS für AIA und Veröffentlichung des Verteilungspunkts der Zertifikatssperrlisten auf der ausstellenden Zertifizierungsstelle
Ein virtuelles Verzeichnis muss auf IIS erstellt werden, das als HTTP-Speicherort für das Zertifikat der Zertifizierungsstelle und CRL-Publishingpoints (als AIA (Authority Information Access, Zugriff auf Stelleninformationen) bzw. CDP (CRL Distribution Point, Sperrlisten-Verteilungspunkt) bezeichnet) verwendet wird.

**So erstellen Sie ein virtuelles Verzeichnis auf IIS**
* Melden Sie sich am IIS-Server mit lokalen Administratorrechten an.

* Erstellen Sie einen Ordner mit der Bezeichnung **C:\CAWWWPub**, der die Zertifikate und CRLs der Zertifizierungsstelle enthält.

* Legen Sie folgende Sicherheitseinstellungen für den Ordner gemäß Tabelle fest:

**Tabelle 9. Berechtigungen für das virtuelle Verzeichnis**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Benutzer/Gruppe

</th>

<th style="border:1px solid black;">

Berechtigung

</th>

<th style="border:1px solid black;">

Erlauben/Verweigern

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Administratoren

</td>

<td style="border:1px solid black;">


Vollzugriff

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


System

</td>

<td style="border:1px solid black;">


Vollzugriff

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Ersteller-Besitzer

</td>

<td style="border:1px solid black;">


Vollzugriff (nur Unterordner und Dateien)

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Benutzer

</td>

<td style="border:1px solid black;">


Ordnerinhalte lesen und auflisten

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


IIS_WPG

</td>

<td style="border:1px solid black;">


Ordnerinhalte lesen und auflisten

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Internetgastkonto

</td>

<td style="border:1px solid black;">


Schreiben

</td>

<td style="border:1px solid black;">


Verweigern

</td>

</tr>

</table>


* Verwenden Sie die IIS-Verwaltungskonsole, um ein neues virtuelles Verzeichnis unter der standardmäßigen Website zu erstellen:
* Geben Sie dem virtuellen Verzeichnis den Namen **pki**

* Geben Sie **C:\CAWWWPub** als Pfad an.


* Deaktivieren Sie das Kontrollkästchen **Skripts ausführen** unter den Zugriffsberechtigungen für das virtuelle Verzeichnis.

* Vergewissern Sie sich, dass die anonyme Authentifizierung für das virtuelle Verzeichnis aktiviert ist.

Auswählen eines DNS-Alias für den HTTP-Publishingpoint
Ein generischer DNS-Alias (CNAME) sollte erstellt werden, um den IIS-Server aufzulösen, der CDP und AIA hostet. Dieser DNS-Alias sollte beim Konfigurieren der CDP- und AIA-Pfade für die Zertifizierungsstellen in den nachfolgenden Abschnitten verwendet werden. Durch die Verwendung von Aliasen können die Publishingpoints von Zertifizierungsstellen einfach auf andere Server oder Netzwerkstandorte verschoben werden, ohne dass Zertifikate der Zertifizierungsstelle neu ausgestellt werden müssen.

Weitere Komponenten für Konfiguration und Betriebssystem

Zusätzlich zu den bislang genannten Konfigurationsschritten sollten einige weitere Elemente beachtet werden:
* Aktualisieren Sie den Stammzertifikatdienst. Der Dienst zum Aktualisieren der Stammzertifikate sollte deaktiviert werden, da es nicht empfehlenswert ist, die Stammvertrauensstellung der Zertifizierungsstellen automatisch zu aktualisieren. Um diesen Dienst zu entfernen, müssen Sie lediglich den folgenden Befehl an einer Eingabeaufforderung ausführen:
sysocmgr /i:sysoc.inf /u:C:\MSSScripts\OC_RemoveRootUpdate.txt
Die Datei „OC_RemoveRootUpdate.txt“ enthält die folgenden Zeilen:
[Components]rootautoupdate = off
* Stellen Sie sicher, dass die Stammzertifizierungsstelle über keine Netzwerkkonnektivität verfügt und dass die ausstellende Zertifizierungsstelle weder eingehende noch ausgehende Internetkonnektivität aufweist.

* Überprüfen Sie, ob durch die Installation von IIS möglicherweise zusätzliche Service Packs und Updates erforderlich werden.

* Installieren Sie die Supporttools von Windows Server 2003. Diese sind nicht unbedingt notwendig, es ist aber hilfreich, auf diese Tools für bestimmte Vorgänge auf Zertifizierungsstellen und für die allgemeine Problembehandlung zugreifen zu können.

* Installieren Sie CAPICOM. CAPICOM 2.1 ist auf der Stammzertifizierungsstelle und der ausstellenden Zertifizierungsstelle für einige der Setup- und Verwaltungsskripts erforderlich, die mit diesem Handbuch bereitgestellt werden. Weitere Informationen zu [CAPICOM](http://www.microsoft.com/downloads/details.aspx?familyid=860ee43a-a843-462f-abb5-ff88ea5896f6&amp;displaylang=en) sowie einen Link zur Downloadseite finden Sie unter www.microsoft.com/downloads/details.aspx?FamilyID=860ee43a-a843-462f-abb5-ff88ea5896f6&amp;DisplayLang=en.


Vorbereiten von Active Directory für die PKI

Die grundlegenden Anforderungen an eine Active Directory-Domäneninfrastruktur, die in diesem Abschnitt beschrieben werden, beruhen auf der Active Directory-Architektur von Microsoft Windows Server 2003. Wenn die verwendete Implementierung von Active Directory auf Windows 2000 beruht, gelten möglicherweise andere Anforderungen. Weitere Informationen über zusätzliche Anforderungen an eine Windows 2000-basierte Domänenstruktur finden Sie unter [So können Sie Domänen- und Gesamtstrukturfunktionsebenen in Windows Server 2003 heraufstufen](http://support.microsoft.com/kb/322692) unter http://support.microsoft.com/kb/322692.

Diese Lösung erfordert auch ein Mindestmaß an Domänenfunktionsebene im einheitlichen Modus von Windows 2000. Dies gilt zumindest für die Domäne, auf der die Server der Zertifizierungsstelle installiert werden. Diese Anforderung existiert, da diese Lösung universelle Gruppen von Active Directory verwendet, die im einheitlichen Modus von Windows 2000 und höher verfügbar sind.
Erstellen von administrativen Gruppen für PKI und Zertifizierungsstelle
Bei dieser Lösung werden mehrere Sicherheitsgruppen definiert, die unterschiedlichen Administratorfunktionen entsprechen. Dieser Ansatz ermöglicht ein hohes Maß an Kontrolle über die Delegation bei der Verwaltung der Zertifizierungsstelle gemäß dem Sicherheitsprinzip, wonach immer nur das Mindestmaß an Rechten eingeräumt wird. Allerdings gibt es keine weiteren Gründe, aus denen sie unbedingt verwendet werden müssten, falls sie nicht mit einem spezifischen Verwaltungsmodell in einem Unternehmen übereinstimmen.

**So erstellen Sie administrative Gruppen für die Zertifizierungsstelle in einer Domäne**
* Melden Sie sich an einem Computer in der Domäne mit einem Konto an, das Ihnen die Rechte zum Erstellen von Benutzer- und Gruppenobjekten im Container „Benutzer“ einräumt.

* Führen Sie den folgenden Befehl aus, um die Verwaltungsgruppen für die Zertifizierungsstelle der Domäne zu erstellen:
Cscript //job:CertDomainGroups C:\MSSScripts\ca_setup.wsf
Dieses Skript erstellt die Sicherheitsgruppen, die in der folgenden Tabelle aufgeführt werden. Diese Gruppen werden als universelle Gruppen im Container „Benutzer“ der Domäne erstellt und können in eine besser geeignete OU verschoben werden, falls dies durch bereits vorhandene Unternehmensrichtlinien verlangt werden sollte.

**Tabelle 10. Gruppennamen und Aufgaben**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Gruppenname

</th>

<th style="border:1px solid black;">

Aufgabe

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Enterprise PKI Admins

</td>

<td style="border:1px solid black;">


Administratoren des Konfigurationscontainers „Public Key Services“

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Enterprise PKI Publishers

</td>

<td style="border:1px solid black;">


Erlaubnis zum Veröffentlichen von CRLs und Zertifikaten der Zertifizierungsstelle im Konfigurationscontainer „Unternehmen“.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CA Admins

</td>

<td style="border:1px solid black;">


Vollzugriff auf die Zertifizierungsstelle, einschließlich der Fähigkeit zum Bestimmen der Mitgliedschaft anderer Funktionen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Certificate Managers

</td>

<td style="border:1px solid black;">


Verwalten des Ausstellens und Sperrens von Zertifikaten

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CA Auditors

</td>

<td style="border:1px solid black;">


Verwalten der Prüfungsdaten für die Zertifizierungsstelle

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CA Backup Operators

</td>

<td style="border:1px solid black;">


Verfügen über die Berechtigung zum Sichern und Wiederherstellen der Schlüssel und Daten der Zertifizierungsstelle.

</td>

</tr>

</table>



Die Installationsverfahren im verbleibenden Dokument erfordern die Verwendung von Konten, die Mitglied von „Enterprise PKI Admins“, „Enterprise PKI Publishers“ und „CA Admins“ sind. Daher sollten in diesen Gruppen die entsprechenden Konten erstellt werden, bevor fortgefahren wird. Wenn nur eine einzige Person für alle Funktionen hinsichtlich der Zertifizierungsstelle verantwortlich ist, könnte allen Gruppen ein einziges Konto zugewiesen werden. Allerdings gibt es in den meisten Unternehmen eine gewisse Trennung zwischen den Funktionen und Aufgaben bei den Mitarbeitern, wenngleich nicht so komplex wie in der vorherigen Tabelle. Für Unternehmen mit einer vereinfachten Aufgabentrennung sind im folgenden Diagramm die üblichen Unterteilungen der Aufgaben aufgeführt.

**Tabelle 11. Vereinfachtes Administrationsmodell**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Administratorfunktion

</th>

<th style="border:1px solid black;">

Gruppenmitgliedschaft

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Administrator der Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


Enterprise PKI Admins, CA Admins, Certificate Managers, Administrators

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CA Auditor

</td>

<td style="border:1px solid black;">


CA Auditors, Administrators

</td>

</tr>

<tr>

<td style="border:1px solid black;">


CA Backup Operator

</td>

<td style="border:1px solid black;">


CA Backup Operators

</td>

</tr>

</table>

Empfohlene OU-Struktur der Domäne
Es gibt eine Reihe von Gruppen und Benutzerkonten, die mit der Verwaltung und dem Betrieb einer PKI verknüpft sind. In Abhängigkeit von den vorhandenen Richtlinien ist es möglicherweise erforderlich, diese Gruppen und Benutzer in einer spezifischen OU-Struktur zu organisieren. Da diese Struktur möglicherweise durch bereits vorhandene Unternehmensrichtlinien vorgegeben wird, handelt es sich beim Folgenden um eine empfohlene Struktur, die nach Bedarf geändert werden kann.

**So erstellen Sie eine OU-Hierarchie der Zertifikatsdienste**
* Melden Sie sich mit einem Konto an, das über Berechtigungen zum Erstellen von OUs verfügt, und delegieren Sie Berechtigungen innerhalb dieser OUs.

* Erstellen Sie eine OU-Struktur anhand der folgenden Tabelle:

**Tabelle 12. Beispiel für eine OU-Struktur**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Organisationseinheit

</th>

<th style="border:1px solid black;">

Aufgabe

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Zertifikatsdienste

</td>

<td style="border:1px solid black;">


Übergeordnete OU

</td>

</tr>

<tr>

<td style="border:1px solid black;">


\-Zertifikatsdienste-Administration

</td>

<td style="border:1px solid black;">


Enthält administrative Gruppen für das Verwalten der Zertifizierungsstellen und die Konfiguration der Unternehmens-PKI.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


\-Zertifikatvorlagen-Verwaltung

</td>

<td style="border:1px solid black;">


Enthält Gruppen für das Verwalten der einzelnen Zertifikatvorlagen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


\-Zertifikatvorlagen-Registrierung

</td>

<td style="border:1px solid black;">


Enthält Gruppen mit Berechtigungen zum Registrieren oder automatischen Registrieren für Vorlagen desselben Namens. Die Kontrolle dieser Gruppen kann an das entsprechende Personal delegiert werden, ohne die Vorlagen ändern zu müssen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


\-Zertifikatsdienste-Testbenutzer

</td>

<td style="border:1px solid black;">


Enthält vorübergehende Testkonten.

</td>

</tr>

</table>


* Räumen Sie der Gruppe „Enterprise PKI Admins“ die Berechtigungen zum Erstellen und Löschen von Gruppen innerhalb der Zertifikatsdienste-OU und deren untergeordneten Containern ein.

Einräumen von Berechtigungen für den Container „Public Key Services“
Die Sicherheitseinstellung des Containers „Public Key Services“ muss geändert werden, um „Enterprise PKI Admins“ das Installieren von Zertifizierungsstellen des Unternehmens und das Konfigurieren von Zertifikatvorlagen zu ermöglichen, ohne dass die Konten der Gruppe Mitglieder der Gruppe „Enterprise Admins“ sein müssen. Dies ist auch erforderlich um „Enterprise PKI Publishers“ das Veröffentlichen der Zertifikatssperrlisten und Zertifikate der Zertifizierungsstelle zu ermöglichen, ohne hierfür über die Rechte von „Enterprise Admin“ verfügen zu müssen.

Um die folgenden Änderungen vorzunehmen, muss ein Konto verwendet werden, das dem Unternehmensadministrator in Active Directory entspricht.

**So gewähren Sie „Enterprise PKI Admins“ Berechtigungen**
* Melden Sie sich als Mitglied der Sicherheitsgruppe „Enterprise Admins“ an.

* Zeigen Sie im MMC-Snap-In für Active Directory-Standorte und -Dienste im Menü **Ansicht** den Knoten **Dienste** an, wechseln Sie dann zum untergeordneten Container „Public Key Services“, und öffnen Sie dessen Eigenschaften.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe „Enterprise PKI Admins“ hinzu, und räumen Sie dieser Gruppe Vollzugriff auf diese Gruppe ein.

* Bearbeiten Sie in **Erweiterte Ansicht** die Berechtigungen dieser Gruppe, um sicherzustellen, dass Vollzugriff für dieses Objekt und alle untergeordneten Objekte vorhanden ist.

* Wählen Sie den Container **Dienste** aus, und öffnen Sie dessen Eigenschaften.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe „Enterprise PKI Admins“ hinzu, und gewähren Sie dieser Gruppe Vollzugriff.

* Bearbeiten Sie in **Erweiterte Ansicht** die Berechtigungen dieser Gruppe, um sicherzustellen, dass Vollzugriff nur für dieses Objekt vorhanden ist.


**So gewähren Sie Berechtigungen für „Enterprise PKI Publishers“**
* Melden Sie sich als Mitglied der Sicherheitsgruppe „Enterprise Admins“ an.

* Zeigen Sie im MMS-Snap-In für Active Directory-Standorte und -Dienste den Knoten **Dienste** an, und öffnen Sie die Eigenschaften für den Container „Public Key Services\AIA“.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe „Enterprise PKI Publishers“ hinzu, und gewähren Sie dieser Gruppe die folgenden Berechtigungen:
* Lesen

* Schreiben

* Alle untergeordneten Objekte erstellen

* Alle untergeordneten Objekte löschen


* Bearbeiten Sie in **Erweiterte Ansicht** die Berechtigungen dieser Gruppe, um sicherzustellen, dass die Berechtigungen auf dieses Objekt und alle untergeordneten Objekte angewendet werden.

* Wiederholen Sie die Schritte 2 bis 4 für die folgenden Container:
* Public Key Services\CDP

* Public Key Services\Zertifizierungsstellen


Gewähren von Berechtigungen für die Gruppe „Zertifikatherausgeber“
Alle Computerkonten der Unternehmenszertifizierungsstelle in der Domäne befinden sich in der Sicherheitsgruppe „Zertifikatherausgeber“. Diese Gruppe wird verwendet, um Berechtigungen auf Benutzer- und Computerobjekte sowie auf die Objekte im CDP-Container anzuwenden, die im vorherigen Verfahren erwähnt wurden. Immer wenn eine Zertifizierungsstelle installiert wird, muss deren zugehöriges Computerkonto zu dieser Gruppe hinzugefügt werden.

Um den Mitgliedern der Gruppe „Enterprise PKI Admins“ das Installieren von Unternehmenszertifizierungsstellen zu erlauben, müssen die Berechtigungen für diese Gruppe geändert werden.

**So gewähren Sie den Zertifikatherausgebern die Berechtigungen zum Ändern der Mitgliedschaft**
* Melden Sie sich als Mitglied der Domänenadministratoren für die Domäne an, in der die ausstellenden Zertifizierungsstellen installiert werden.

* Öffnen Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer.

* Vergewissern Sie sich im Menü **Ansicht** der MMC, dass **Erweiterte Funktionen** ausgewählt ist.

* Suchen Sie die Gruppe „Zertifikatherausgeber“ (standardmäßig im Container „Benutzer“), und zeigen Sie die Eigenschaften der Gruppe an.

* Fügen Sie von der Registerkarte **Sicherheit** die Gruppe „Enterprise PKI Admins“ hinzu, und klicken Sie auf die Schaltfläche **Erweitert.**  

* Wählen Sie die Gruppe „Enterprise PKI Admins“ in der Liste aus, und klicken Sie auf die Schaltfläche **Bearbeiten.**  

* Wählen Sie die Registerkarte **Eigenschaften** aus, und stellen Sie sicher, dass **Nur dieses Objekt** im Feld **Übernehmen für** ausgewählt ist.

* Führen Sie den Bildlauf nach unten aus, und klicken Sie für die Gruppe „Mitglieder“ auf das Feld **Schreiben** in der Spalte **Zulassen.**  

* Speichern Sie die Änderungen, und schließen Sie jedes Dialogfeld jeweils durch Klicken auf **OK.**  

* Starten Sie den Server der ausstellenden Zertifizierungsstelle neu, bevor Sie die Komponente Zertifikatsdienste installieren. Ein Neustart ermöglicht dem Server die Übernahme der neuen Gruppenmitgliedschaft in sein Zugriffstoken.

Gewähren von Wiederherstellungsberechtigungen für „Enterprise PKI Admins“
Der Vorgang zum Installieren von Zertifikatsdiensten erfordert das Benutzerrecht zum Wiederherstellen von Dateien und Verzeichnissen in der Domäne, in der die Unternehmenszertifizierungsstelle platziert wird. Dieses Recht ist insbesondere erforderlich, um das Zusammenführen von Sicherheitsbeschreibungen für die Vorlagen und andere Verzeichnisobjekte zu ermöglichen, wodurch den Domänen-PKI-Objekten die richtigen Berechtigungen gewährt werden. Die vordefinierten Domänengruppen „Administratoren“, „Server-Operatoren“ und „Sicherungs-Operatoren“ weisen standardmäßig dieses Recht auf.

Da die Gruppe „Enterprise PKI Admins“ zum Installieren der Zertifizierungsstelle verwendet wird, muss das Benutzerrecht zum Wiederherstellen von Dateien und Verzeichnissen dieser Gruppe gewährt werden.

**So gewähren Sie die Wiederherstellungsrechte für „Enterprise PKI Admins“**
* Melden Sie sich als Mitglied der Domänenadministratoren innerhalb der Domäne an, in der die ausstellende Zertifizierungsstelle installiert wird.

* Öffnen Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer.

* Wählen Sie die OU „Domänencontroller“ aus, und öffnen Sie die Eigenschaften dieser OU.

* Wählen Sie auf der Registerkarte **Gruppenrichtlinie** das Gruppenrichtlinienobjekt **Standard-Domänencontrollerrichtlinie** aus, und klicken Sie dann auf **Bearbeiten.**  

* Wechseln Sie zu Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien\Zuweisen von Benutzerrechten, und doppelklicken Sie auf **Wiederherstellen von Dateien und Verzeichnissen.**  

* Fügen Sie die Gruppe „Enterprise PKI Admins“ zur angezeigten Liste hinzu.

* Schließen Sie das Dialogfeld und die MMC zum Bearbeiten von Gruppenrichtlinienobjekten.

**Hinweis**   Wenn es weitere Gruppenrichtlinienobjekte gibt, die das Benutzerrecht zum Wiederherstellen von Dateien und Verzeichnissen festlegen, muss dieses Verfahren für das Gruppenrichtlinienobjekt mit der höchsten Priorität statt für die Standard-Domänencontrollerrichtlinie ausgeführt werden. Die Einstellungen für die Benutzerrechte sind nicht kumulativ, und nur das zuletzt angewendete Gruppenrichtlinienobjekt, das über dieses Recht verfügt, ist wirksam.


Bereitstellen eines Servers für die Stammzertifizierungsstelle

Wie zuvor erwähnt, stellt dieses Handbuch keine schrittweisen Anweisungen für die Installation von Windows Server 2003 zur Verfügung, da die meisten Unternehmen bereits über einen dokumentierten Prozess für die Inbetriebnahme des Servers verfügen. Allerdings unterscheiden sich Server für Stammzertifizierungsstellen in gewisser Hinsicht von anderen Servern, da sie niemals mit einem Netzwerk verbunden sein sollten, um jegliche Gefährdung auszuschließen.

Daher muss sichergestellt werden, dass der Server für die Stammzertifizierungsstelle während des Erstellens des Servers nicht mit dem Netzwerk verbunden ist und dass zu einem bestimmten Zeitpunkt die Netzwerkadapter deaktiviert werden, um zu gewährleisten, dass nie eine versehentliche Netzwerkverbindung hergestellt wird. Außerdem ist zu beachten, dass sich der Server in einer Arbeitsgruppe befindet und dass der Arbeitsgruppenname vor der Installation ausgewählt und dokumentiert werden sollte, da der Server nicht mit dem Netzwerk verbunden wird.

**Hinweis**   Selbst wenn die Stammzertifizierungsstelle offline erstellt und betrieben wird, ist es wichtig, dass deren Name innerhalb der Netzwerkumgebung eindeutig ist.
Datei „CAPolicy.inf“
Nach dem Vorbereiten der erforderlichen Serverhardware für einen Server für die Stammzertifizierungsstelle und dem Installieren des Betriebssystems besteht der nächste Schritt im Erstellen einer Datei „capolicy.inf“. Die Datei „capolicy.inf“ ist zum Erstellen einer Stammzertifizierungsstelle erforderlich, da in ihr die Merkmale des selbst signierten Zertifikats der Stammzertifizierungsstelle angegeben werden, darunter die Schlüssellänge und die Gültigkeitsdauer des Zertifikats.

CRL- und AIA-Informationen sind für ein Zertifikat der Stammzertifizierungsstelle nicht erforderlich. Daher wird für die Parameter „CRLDistributionPoint“ und „AuthorityInformationAccess“ in der Datei „capolicy.inf“ der Wert „Empty“ eingetragen.

**So erstellen Sie eine Datei „capolicy.inf“**
* Erstellen Sie mit einem Texteditor wie Editor eine Textdatei mit dem folgenden Text:
[version]Signature=”$Windows NT$”[Certsrv_server]RednewalKeyLength=4096RenewalValidityPeriod=YearsRenewalValidityPeriodUnits=16[CRLDistributionPoint]Empty=true[AuthorityInformationAccess]Empty=true
* Wenn eine Zertifikatverwendungserklärung (CPS) für diese Zertifizierungsstelle definiert wurde, nehmen Sie folgende Zeilen in die Datei „capolicy.inf“ auf, wobei Sie die kursiv gedruckten Werte durch die spezifischen Werte für diese Implementierung ersetzen:
[CAPolicy]Policies=company CPS name[company CPS name]OID=the.company.OIDURL=”http://www.companyurl.com/cpspagename.htm”
* Speichern Sie diese Textdatei als *%windir%*\capolicy.inf (ersetzen Sie *%windir%* durch den absoluten Pfad des Ordners, in dem Windows installiert ist, beispielsweise „C:\Windows“). Ein Administrator oder Konto mit entsprechenden Berechtigungen muss verwendet werden, um die Datei im Windows-Ordner zu speichern und diesen Schritt abzuschließen.

Installieren der Softwarekomponenten für Zertifikatsdienste
Verwenden Sie den Assistenten für Windows-Komponenten, um die Softwarekomponenten der Zertifizierungsstelle zu installieren. Bitte beachten Sie, dass Sie das Installationsmedium von Windows Server 2003 benötigen, um diese Installation abzuschließen.

**So installieren Sie Zertifikatsdienste**
* Melden Sie sich als Mitglied der lokalen Administratorgruppe an, und führen Sie den Manager für die Installation optionaler Komponenten aus, oder verwenden Sie die Systemsteuerung und dort die Option „Software“ und „Programme ändern oder entfernen“ bzw. „Windows-Komponenten hinzufügen/entfernen“.
sysocmgr /i:sysoc.inf
* Wählen Sie die Komponente „Zertifikatsdienste“ aus (klicken Sie auf **Ja**, um die Warnung zum Umbenennen zu bestätigen).

* Wählen Sie für den Typ der Zertifizierungsstelle **Eigenständige Stammzertifizierungsstelle** aus, und vergewissern Sie sich, dass das Kontrollkästchen **Schlüsselpaar und ein Zertifizierungsstellenzertifikat mit diesen Einstellungen erstellen** aktiviert ist.

* Lassen Sie die Einstellungen im Dialogfeld **Öffentlich-privates Schlüsselpaar** unverändert bei den Standardwerten mit Ausnahme des Feldes **Schlüssellänge**, in dem der Wert **4096** eingegeben werden sollte, und des **Anbietertyps**, in dem die Einstellung **Microsoft Strong Cryptographic Provider** festgelegt werden sollte.

* Geben Sie die Erkennungsdaten der Zertifizierungsstelle ein, die Sie in der vorbereitenden Phase für die folgenden Felder gesammelt haben:
* Allgemeiner Name der Zertifizierungsstelle:

* Suffix des definierten Namens:

* Gültigkeitsdauer: 8 Jahre


Zu diesem Zeitpunkt erstellt der Anbietertyp das Schlüsselpaar, das in den Schlüsselspeicher des lokalen Computers geschrieben wird.

**Hinweis**   Wenn eine Zertifizierungsstelle zuvor auf diesem System installiert wurde, werden Sie in einem Dialogfeld gewarnt, dass der private Schlüssel der vorherigen Installation überschrieben wird. Vergewissern Sie sich, dass dieser Schlüssel vor dem Fortfahren nie wieder benötigt wird.

* Belassen Sie die Speicherorte der Zertifikatsdatenbank, Datenbankprotokolle und des Konfigurationsordners bei dem jeweiligen Standardwert. Zu diesem Zeitpunkt installiert der Manager für die Installation optionaler Komponenten die Komponenten der Zertifikatsdienste, und das Installationsmedium von Windows Server 2003 ist erforderlich.

* Klicken Sie auf **OK**, um Warnungen über IIS zu bestätigen und mit der Installation bis zum Abschluss fortzufahren.

Konfigurieren der Eigenschaften der Stammzertifizierungsstelle
Eine Reihe von umgebungsspezifischen Parametern wird verwendet, wenn die Stammzertifizierungsstelle gemäß Beschreibung in diesem Abschnitt konfiguriert wird. Diese Parameter sollten gemäß vorheriger Beschreibung im Abschnitt zu den erforderlichen Informationen in diesem Handbuch gesammelt werden, bevor fortgefahren wird.

**So konfigurieren Sie die Eigenschaften der Stammzertifizierungsstelle**
* Melden Sie sich am Server mit der Zertifizierungsstelle als Gruppenmitglied der lokalen Administratoren an.

* Passen Sie das Skript „C:\MSSScripts\pkiparams.vbs“ an, um folgende Zeile aufzunehmen:
* Ändern Sie den Wert der Einstellung AD_ROOT_DN, um ihn an den Stammdomänen-DN der Active Directory-Gesamtstruktur anzupassen.

* Ändern Sie die Einstellung HTTP_PKI_VROOT, um sie an den HTTP-Pfad zum virtuellen IIS-Verzeichnis anzupassen, das zuvor eingerichtet wurde.


* Führen Sie das folgende Skript aus:
Cscript //job:RootCAConfig C:\MSSScripts\ca_setup.wsf
Konfigurieren der Administratorfunktionen
Die zuvor erstellten Sicherheitsgruppen müssen Administratorfunktionen wie „Prüfer“ und „Zertifikatverwaltung“ zugeordnet werden, um verwendet werden zu können.

**Hinweis**   Obwohl die meisten mittelgroßen Unternehmen vermutlich das vereinfachte Delegationsmodell verwenden, das zuvor in diesem Handbuch erwähnt wurde, wird hier ein flexibleres Modell gezeigt, falls eine stärkere Trennung erforderlich ist.

**So konfigurieren Sie Administratorfunktionen für die Stammzertifizierungsstelle**
* Klicken Sie in der Verwaltungskonsole für die Zertifizierungsstelle auf **Eigenschaften.**  

* Klicken Sie auf die Registerkarte **Sicherheit**, und fügen Sie die lokalen Sicherheitsgruppen hinzu, die in der folgenden Tabelle aufgeführt werden. Fügen Sie die gezeigte Berechtigung für jede Gruppe hinzu.

**Tabelle 13. Einträge für die Berechtigung der Zertifizierungsstelle**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Gruppe

</th>

<th style="border:1px solid black;">

Berechtigung

</th>

<th style="border:1px solid black;">

Erlauben/Verweigern

</th>

</tr>

<tr>

<td style="border:1px solid black;">


CA Admins

</td>

<td style="border:1px solid black;">


Verwalten der Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Certificate Managers

</td>

<td style="border:1px solid black;">


Ausstellen und Verwalten von Zertifikaten

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

</table>


* Weitere Sicherheitsfunktionen für die Zertifizierungsstelle für diesen Server wurden bereits über die zuvor angewendete Sicherheitsrichtlinie definiert.

Übertragen des Zertifikats der Stammzertifizierungsstelle und der CRL auf Datenträger
Das Zertifikat der Stammzertifizierungsstelle und die CRL müssen von der Zertifizierungsstelle kopiert werden, damit sie für Active Directory und das IIS-Zertifikat und den CRL-Veröffentlichungsserver veröffentlicht werden können. Obwohl in diesem Beispiel die Verwendung eines Datenträgers beschrieben wird, kann jedes tragbare Medium verwendet werden (einschließlich USB-Laufwerke).

**So kopieren Sie das Zertifikat der Stammzertifizierungsstelle und die CRL auf einen Datenträger**
* Melden Sie sich an der Stammzertifizierungsstelle als Mitglied der lokalen Gruppe „CA Admins“ an, und legen Sie das tragbare Medium in den Server ein.

* Führen Sie das folgende Skript aus, um das Zertifikat der Zertifizierungsstelle auf einen Datenträger zu kopieren:
Cscript //job:GetCACerts C:\MSSScripts\CA_Operations.wsf
* Führen Sie das folgende Skript aus, um die CRL der Zertifizierungsstelle auf einen Datenträger zu kopieren:
Cscript //job:GetCRLs C:\MSSScripts\CA_Operations.wsf
* Beschriften Sie den Datenträger mit einem aussagekräftigen Titel und dem Datum, und bewahren Sie ihn für die spätere Verwendung auf.


Veröffentlichen der Informationen zur Stammzertifizierungsstelle

Vor der Installation der ausstellenden Zertifizierungsstelle muss das Zertifikat der Stammzertifizierungsstelle für den Stammspeicher veröffentlicht werden, der für Active Directory vertrauenswürdig ist, und die Stamm-CRL muss für den Active Directory CDP-Container veröffentlicht werden. Dieser Prozess hat zur Folge, dass alle Domänenmitglieder das Zertifikat der Stammzertifizierungsstelle in ihre eigenen vertrauenswürdigen Stammspeicher importieren. Dadurch können sie den Sperrungsstatus aller Zertifikate überprüfen, die von der Stammzertifizierungsstelle ausgestellt werden.

Es empfiehlt sich, die ausstellende Zertifizierungsstelle zum Ausführen dieses Verfahrens zu verwenden, da dort die erforderliche Datei „Certutil.exe“ ebenso vorhanden ist wie die Bibliotheken „certadm.dll“ und „certcli.dll“. Es könnte jedoch jeder Mitgliedserver verwendet werden, solange „certutil.exe“ und die unterstützenden DLL-Dateien auf diesem Windows Server 2003-basierten System installiert sind.

**So veröffentlichen Sie das Zertifikat der Stammzertifizierungsstelle und die CRL für Active Directory**
* Melden Sie sich an einem Mitgliedscomputer der Domäne an, der die zuvor erwähnten Anforderungen als Mitglied der Gruppe „Enterprise PKI Admins“ erfüllt, und legen Sie den Datenträger ein, der zum Speichern des Zertifikats der Stammzertifizierungsstelle und der CRL erstellt wurde.

* Führen Sie das folgende Skript aus, um das Zertifikat der Zertifizierungsstelle für Active Directory zu veröffentlichen.
Cscript //job:PublishCertstoAD C:\MSSScripts\CA_Operations.wsf
* Führen Sie das folgende Skript aus, um die CRL für Active Directory zu veröffentlichen
Cscript //job:PublishCRLstoAD C:\MSSScript\CA_Operations.wsf
Veröffentlichen des Zertifikats der Stammzertifizierungsstelle und der CRL auf dem Webserver
Diese Aufgabe ist erforderlich, da HTTP-Versionen der CDP- und AIA-URLs in den Erweiterungen der von dieser Zertifizierungsstelle ausgestellten Zertifikate angegeben sind. Wenn diese Erweiterungen vorhanden sind, müssen sie von den veröffentlichenden CRLs und Zertifikaten für die darin konfigurierten URLs berücksichtigt werden.

**Hinweis**   Dieses Verfahren hängt nicht davon ab, ob sich der veröffentlichende CDP- und AIA-Webserver in der ausstellenden Zertifizierungsstelle befindet. Es wird jedoch davon ausgegangen, dass das virtuelle Verzeichnis mit dem Verzeichnis übereinstimmt, das zuvor für die Konfiguration von IIS eingerichtet wurde („C:\CAWWWPub“). Wenn ein unterschiedlicher Pfad ausgewählt wurde, muss der Wert WWW_LOCAL_PUB_PATH im Skript „PKIParams.vbs“ geändert werden.

**So veröffentlichen Sie das Zertifikat der Stammzertifizierungsstelle und die CRL für die Web-URL**
* Melden Sie sich am Webserver als lokaler Administrator oder unter einem gleichwertigen Konto an.

* Stellen Sie sicher, dass der Datenträger mit dem Zertifikat der Stammzertifizierungsstelle und der CRL eingelegt ist

* Führen Sie das folgende Skript aus, um das Zertifikat der Zertifizierungsstelle im Ordner des Webservers zu veröffentlichen:
Cscript //job:PublishRootCerttoIISC:\MSSScripts\CA_Operations.wsf
* Führen Sie das folgende Skript aus, um die CRLs der Zertifizierungsstelle im Ordner des Webservers zu veröffentlichen:
Cscript //job:PublishRootCRLstoIISC:\MSSScripts\CA_Operations.wsf

Bereitstellen eines Servers mit einer ausstellenden Zertifizierungsstelle

Nachdem nun die Stammzertifizierungsstelle installiert und deren Zertifikate veröffentlicht wurden, kann der Server mit der ausstellenden Zertifizierungsstelle bereitgestellt werden. Das Installieren von Zertifikatsdiensten erfordert eine komplexe Reihe von Interaktionen zwischen der ausstellenden Zertifizierungsstelle, der Stammzertifizierungsstelle, Active Directory und dem Webserver. Diese Interaktionen können einfacher nachvollzogen werden, wenn das folgende Diagramm als Referenz herangezogen wird.


**Abbildung 5. Prozess zur Zertifikatsinstallation**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875845.swcg5_big(de-de,technet.10).gif)

Dieses Diagramm enthält folgende durchnummerierte interaktive Schritte:
* Veröffentlichen des Zertifikats der Stammzertifizierungsstelle und der CRL für Active Directory mit einem Wechselmedium.

* Veröffentlichen des Zertifikats der Stammzertifizierungsstelle und der CRL für den Webserver mit einem Wechselmedium.

* Installieren der Software für Zertifikatsdienste, welche eine Zertifikatsanforderung erzeugt, die mit einem Wechselmedium an die Stammzertifizierungsstelle übergeben wird, wo ein Zertifikat auf Grundlage dieser Anforderung ausgestellt wird.

* Installieren des entsprechenden Zertifikats der ausstellenden Zertifizierungsstelle mit einem Wechselmedium.

* Veröffentlichen des Zertifikats der ausstellenden Zertifizierungsstelle und der CRL für den Webserver.


    x.   Dieser Schritt erfolgt automatisch während der Installationsroutine der Unternehmenszertifizierungsstelle.
Vorbereiten der Datei „capolicy.inf“ für die ausstellende Zertifizierungsstelle
Obwohl eine Datei „capolicy.inf“ nicht für die ausstellende Zertifizierungsstelle erforderlich ist, wird diese Datei benötigt, falls die von der Zertifizierungsstelle verwendete Schlüsselgröße geändert werden muss. Diese Datei sollte erstellt werden, bevor die ausstellende Zertifizierungsstelle eingerichtet wird. Dies ist empfehlenswert, obwohl diese Datei bei Bedarf später hinzugefügt werden kann, gefolgt von der Erneuerung des Zertifikats der Zertifizierungsstelle.

**So erstellen Sie eine Datei „capolicy.inf“**
* Melden Sie sich am Server mit der ausstellenden Zertifizierungsstelle mit einem lokalen Administratorkonto oder einem gleichwertigen Konto an.

* Erstellen Sie mit einem Texteditor wie Editor eine Textdatei mit den folgenden Informationen:
[Version]Signature= “$Windows NT$”[Certsrv_Server]RenewalKeyLength=2048
* Wenn eine Zertifikatverwendungserklärung (CPS) für diese Zertifizierungsstelle definiert ist, nehmen Sie die folgenden Zeilen in die Datei „capolicy.inf“ auf:
[CAPolicy]Policies=policyname[policyname]OID=the.org.oidURL=”http://the.org.url/TheCPSPage.htm”
**Hinweis**   Kursiv formatierte Elemente müssen durch unternehmensspezifische Informationen ersetzt werden.

* Speichern Sie die Datei als *%windir%*\Capolicy.inf (ersetzen Sie *%windir%* durch den absoluten Pfad zum Windows-Installationsordner wie „C:\Windows“).

Installieren der Softwarekomponenten für Zertifikatsdienste
Wie beim Installieren der Zertifikatsdienste auf der Stammzertifizierungsstelle ist auch bei diesem Schritt die Verwendung des Windows Server 2003-Installationsmediums gemeinsam mit dem Assistenten für Windows-Komponenten erforderlich.

**So installieren Sie Zertifikatsdienste**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle als Mitglied der lokalen Administratorgruppe oder mit einem gleichwertigen Konto an, und führen Sie den Manager für die Installation optionaler Komponenten aus:
sysocmgr /i:sysoc.inf
* Wählen Sie die Komponente der Zertifikatsdienste aus, und klicken Sie auf **OK**, um das Dialogfeld mit einer Warnung zum Umbenennen zu bestätigen.

* Wählen Sie den Zertifizierungsstellentyp als untergeordnete Zertifizierungsstelle des Unternehmens aus, und vergewissern Sie sich, dass das Kontrollkästchen **Schlüsselpaar und ein Zertifizierungsstellenzertifikat mit diesen Einstellungen erstellen** aktiviert ist.

* Behalten Sie die Standardeinstellungen im Dialogfeld **Öffentlich-privates Schlüsselpaar** bei, mit Ausnahme folgender Einstellung:
* Schlüssellänge – 2048 Bit

* Anbietertyp – Microsoft Strong Cryptographic Provider


* Geben Sie die kennzeichnenden Informationen zur Zertifizierungsstelle wie folgt ein:
* Allgemeiner Name der Zertifizierungsstelle

* Suffix des definierten Namens

* Gültigkeitsdauer: (gemäß Vorgabe durch übergeordnete Zertifizierungsstelle)


* Der Anbieter erstellt zu diesem Zeitpunkt ein Schlüsselpaar und schreibt es in den Schlüsselspeicher des lokalen Computers.

* Geben Sie die Speicherorte von Zertifikatsdatenbank, Datenbankprotokollen und Konfiguration wie folgt an:
* Zertifikatsdatenbank: D:\CertLog

* Zertifikatsdatenbankprotokoll: %windir%\System32\CertLog

* Freigegebener Ordner: Deaktiviert


Die Datenbank und die Protokolle der Zertifizierungsstelle sollten nach Möglichkeit auf verschiedenen physischen Volumes gespeichert werden, um Leistung und Stabilität zu steigern. Die Zertifikatsdatenbank und die Datenbankprotokolle müssen sich jeweils auf lokalen NTFS-formatierten Laufwerken befinden.

* Zu diesem Zeitpunkt wird eine Anforderungsdatei für Zertifikatsdienste erstellt, die auf einen Datenträger kopiert werden sollte. Der Manager für die Installation optionaler Komponenten installiert dann die Komponenten der Zertifikatsdienste, wofür Zugriff auf die Installationsmedien von Windows Server 2003 erforderlich ist.

* Klicken Sie auf **OK**, um die Warnung zu IIS zu bestätigen, und setzen Sie die Installation bis zum Abschluss fort. Der Setup-Assistent zeigt die Mitteilung an, dass ein Zertifikat von der übergeordneten Zertifizierungsstelle vor dem Fortfahren erforderlich ist.

Übergeben der Zertifikatsanforderung an die Stammzertifizierungsstelle
Zu diesem Zeitpunkt muss die Zertifikatsanforderung der ausstellenden Zertifizierungsstelle an die Stammzertifizierungsstelle übergeben werden, damit die Anforderung signiert und ein Zertifikat für die ausstellende Zertifizierungsstelle ausgestellt wird.

**So übergeben Sie die Zertifikatsanforderung an die Stammzertifizierungsstelle**
* Melden Sie sich an der Stammzertifizierungsstelle mit einem Mitgliedskonto der Gruppe „Certificate Managers“ an.

* Vergewissern Sie sich, dass sich der Datenträger im Laufwerk befindet, der zum Speichern der Anforderungsdatei für Zertifikatsdienste verwendet wird.

* Wählen Sie im Menü **CA-Aufgaben** in der Verwaltungskonsole für die Zertifizierungsstelle **Neue Anforderung einreichen**, und reichen Sie dann die Anforderung ein, die von der ausstellenden Zertifizierungsstelle übertragen wurde.

* Suchen Sie nach dem neu ausgestellten Zertifikat im Container „Ausgestellte Zertifikate“, und öffnen Sie es.

* Überprüfen Sie, dass die Zertifikatdetails korrekt sind, und exportieren Sie dann durch Klicken auf „In Datei kopieren“ das Zertifikat in eine Datei. Speichern Sie diese Datei als PKCS#7-Datei auf einen Datenträger, und wählen Sie die Option, dass alle möglichen Zertifikate in die Kette aufgenommen werden sollen.

Aktualisieren der Zertifikatsinformationen für die ausstellende Zertifizierungsstelle
Das Zertifikat der Stammzertifizierungsstelle wurde bereits für den vertrauenswürdigen Stammspeicher von Active Directory veröffentlicht. Jetzt sollte überprüft werden, ob die ausstellende Zertifizierungsstelle diese Informationen heruntergeladen und das Zertifikat in ihrem eigenen Stammspeicher platziert hat.

**So aktualisieren und überprüfen Sie die Zertifikatvertrauensinformationen auf der ausstellenden Zertifizierungsstelle**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle als lokaler Administrator oder unter einem gleichwertigen Konto an.

* Führen Sie folgenden Befehl an einer Eingabeaufforderung aus:
certutil –pulse
Dieser Befehl zwingt die Zertifizierungsstelle zum Herunterladen der neuen vertrauenswürdigen Stamminformationen aus dem Verzeichnis sowie zum Einfügen des Zertifikats der Stammzertifizierungsstelle in den eigenen vertrauenswürdigen Stammspeicher. Obwohl dieser Schritt nicht notwendig ist, kann er vor dem Fortfahren zur Überprüfung herangezogen werden, ob die früheren Schritte zur Veröffentlichung erfolgreich waren.

* Führen Sie „mmc.exe“ aus, und fügen Sie das Snap-In Zertifikate hinzu.

* Wählen Sie **Computerkonto** als zu verwaltenden Zertifikatspeicher aus.

* Vergewissern Sie sich, dass sich das Zertifikat der Stammzertifizierungsstelle im Ordner „Vertrauenswürdige Ursprungszertifizierungsagenturen“ befindet.

Installieren des Zertifikats auf der ausstellenden Zertifizierungsstelle
Die signierte Antwort der Stammzertifizierungsstelle wurde als PKCS#7-Zertifikatspaket erstellt und kann jetzt auf der ausstellenden Zertifizierungsstelle installiert werden. Um das Zertifikat der Zertifizierungsstelle im NTAuth-Speicher von Active Directory zu veröffentlichen, in dem die Zertifizierungsstelle als Unternehmenszertifizierungsstelle gekennzeichnet wird, muss das Zertifikat der Zertifizierungsstelle mit einem Konto installiert werden, das sowohl Mitglieder der Gruppe „Enterprise PKI Admins“ als auch der lokalen Administratorgruppe auf der ausstellenden Zertifizierungsstelle ist. Die zuerst genannte Gruppe hat die Rechte zum Installieren des Zertifikats der Zertifizierungsstelle im Verzeichnis, und die danach genannte Gruppe hat die Rechte zum Installieren des Zertifikats auf dem Server der Zertifizierungsstelle. Wenn das einfache Administrationsmodell verwendet wird, das zuvor erwähnt wurde, ist die Funktion „CA Admins“ bereits ein Mitglied in beiden Gruppen.

**So installieren Sie das Zertifikat der ausstellenden Zertifizierungsstelle**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle mit einem Konto an, das sowohl ein Mitglied der Gruppe „Enterprise PKI Admins“ als auch der lokalen Administratorgruppe ist.

* Legen Sie den Datenträger ein, auf dem das signierte, von der Stammzertifizierungsstelle ausgestellte Zertifikat gespeichert wurde.

* Wählen Sie im Menü **CA-Aufgaben** die Option **Zertifikat installieren** in der Verwaltungskonsole für die Zertifizierungsstelle aus, um das Zertifikat der ausstellenden Zertifizierungsstelle vom Datenträger zu installieren.

Die Zertifizierungsstelle sollte zu diesem Zeitpunkt gestartet werden.

Konfigurieren der Eigenschaften der ausstellenden Zertifizierungsstelle
Mit dem folgenden Verfahren werden die umgebungsspezifischen Parameter konfiguriert, die während des Abschnitts zur Ermittlung der erforderlichen Informationen auf der ausstellenden Zertifizierungsstelle gesammelt wurden. Bevor Sie mit diesem Schritt fortfahren, müssen Sie sicherstellen, dass die in den vorherigen Schritten gesammelten unternehmensspezifischen Informationen in die Datei „C:\MSSScripts\pkiparams.vbs“ auf der Stammzertifizierungsstelle eingefügt wurden und dass diese Änderungen auch auf die ausstellende Zertifizierungsstelle übertragen wurden.

**So konfigurieren Sie die Eigenschaften der ausstellenden Zertifizierungsstelle**
* Melden Sie sich am Server der ausstellenden Zertifizierungsstelle als Mitglied der lokalen Administratorgruppe an.

* Überprüfen Sie, ob die an „C:\MSSScripts\pkiparams.vbs“ vorgenommenen Änderungen den umgebungsspezifischen Einstellungen entsprechen, die zuvor in diesem Abschnitt beschrieben wurden.

* Führen Sie das folgende Skript aus:
Cscript //job:IssCAConfig C:\MSSScripts\ca_setup.wsf
Konfigurieren der Administratorfunktionen der ausstellenden Zertifizierungsstelle
Damit die in diesem Handbuch beschriebenen Administratorfunktionen verwendet werden können, müssen sie Sicherheitsgruppen zugewiesen sein. Wie zuvor erwähnt, werden bei diesem Verfahren die detaillierten Funktionen implementiert, die mit Blick auf höchste Flexibilität und Trennung der Verantwortlichkeiten entworfen wurde. Dennoch muss festgehalten werden, dass auch die vereinfachten Funktionen für die meisten mittelgroßen Unternehmen ausreichend wären.

**So konfigurieren Sie Funktionen für die ausstellende Zertifizierungsstelle**
* Melden Sie sich am Server der ausstellenden Zertifizierungsstelle als Mitglied der lokalen Administratorgruppe an.

* Klicken Sie in der Verwaltungskonsole für die Zertifizierungsstelle auf „Eigenschaften“, um die Eigenschaften der Zertifizierungsstelle zu bearbeiten.

* Klicken Sie auf die Registerkarte **Sicherheit**, und fügen Sie die Domänensicherheitsgruppen hinzu, die in der folgenden Tabelle aufgeführt werden. Fügen Sie die gezeigten Berechtigungen für jede Gruppe hinzu.

**Tabelle 14. Berechtigungen für die ausstellende Zertifizierungsstelle**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Gruppe

</th>

<th style="border:1px solid black;">

Berechtigung

</th>

<th style="border:1px solid black;">

Erlauben/Verweigern

</th>

</tr>

<tr>

<td style="border:1px solid black;">


CA Admins

</td>

<td style="border:1px solid black;">


Verwalten der Zertifizierungsstelle

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Certificate Managers

</td>

<td style="border:1px solid black;">


Ausstellen und Verwalten von Zertifikaten

</td>

<td style="border:1px solid black;">


Erlauben

</td>

</tr>

</table>


* Die Gruppe „CA Auditors“ sollte zur lokalen Administratorgruppe hinzugefügt werden, obwohl diese Gruppe bereits durch die zuvor angewendete Sicherheitsrichtlinie teilweise definiert wurde.


Veröffentlichen der Informationen zur ausstellenden Zertifizierungsstelle

Obwohl Zertifikate und CRLs automatisch von der ausstellenden Zertifizierungsstelle für Active Directory veröffentlicht werden, gilt dies nicht für die Veröffentlichung des Zertifikats der Zertifizierungsstelle und die CRLs für die HTTP-CDP- und AIA-Pfade. Um die Veröffentlichung des Zertifikats der Zertifizierungsstelle für die HTTP-CDP- und AIA-Pfade zu automatisieren, muss ein geplanter Auftrag vorhanden sein, um diese Aufgabe auszuführen.

Die Zertifikate der Zertifizierungsstelle werden sehr selten aktualisiert. Daher können sie mit dem folgenden Prozess manuell für AIA veröffentlicht werden.

**So veröffentlichen Sie das Zertifikat der ausstellenden Zertifizierungsstelle**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle mit einem Konto an, das über die Berechtigungen zum Schreiben in den veröffentlichten Webserverordner verfügt.

* Aktualisieren Sie den Parameter WWW_REMOTE_PUB_PATH in „C:\MSSScripts\PKIParams.vbs“, um diesen an den Zielpfad des Webserverordners anzupassen.
* Wenn sich der Webserver auf einem Remoteserver befindet, müssen Sie sicherstellen, dass der Webserverordner freigegeben ist. Zudem müssen Sie diesen UNC-Pfad für den freigegebenen Ordner aufzeichnen.

* Wenn sich der Webserver auf demselben Server wie die Zertifizierungsstelle befindet, müssen Sie den lokalen Pfad zu diesem Ordner aufzeichnen. (Standardmäßig lautet der lokale Pfad „C:\CAWWWPub“)


* Führen Sie das folgende Skript aus, um das Zertifikat der Zertifizierungsstelle auf dem Webserver zu veröffentlichen:
Cscript //job:PublishIssCertsToIIS C:\MSSScripts\CA_Operations.wsf
**Hinweis**   Bei diesem Verfahren wird vom Vorhandensein interner Webserver ausgegangen. Wenn die Zertifikate für einen mit dem Internet verbundenen Webserver herausgegeben werden sollen, sind zusätzliche Schritte erforderlich, da diese Lösung auf der Windows-Netzwerkdateifreigabe beruht, die normalerweise von Internetfirewalls blockiert werden.


CRLs werden häufiger als Zertifikate der Zertifizierungsstelle veröffentlicht. Daher ist eine automatisierte Methode zu deren Veröffentlichung auf dem Webserver erforderlich.

**So automatisieren Sie die Veröffentlichung von CRLs**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle mit einem Konto an, das Mitglied der lokalen Administratoren ist.

* Vergewissern Sie sich, dass auf den Webserverordner von diesem Server zugegriffen werden kann.

* Wenn sich der Webserver an einem Remotestandort befindet, benötigt die ausstellende Zertifizierungsstelle Schreibzugriff auf den Dateisystemordner (Änderungszugriff zulassen) und auf die Freigabe (Freigabezugriff zulassen). Wenn der Remotewebserver ein Mitglied der Gesamtstruktur ist, sollte die Gruppe „Zertifikatherausgeber“ der Domäne verwendet werden, um Zugriff zu erteilen. Dadurch wird sichergestellt, dass jede Unternehmenszertifizierungsstelle Zertifikate und CRLs veröffentlichen kann.

* Erstellen Sie mit dem folgenden Befehl einen geplanten Auftrag, um die CRLs zu kopieren:

**Hinweis**   Einige Teile des folgenden Codeausschnitts werden nur aus Gründen der besseren Lesbarkeit in mehreren Zeilen angezeigt. Der Code sollte jedoch in einer einzelnen Zeile eingegeben werden.
schtasks /creat /tn “Publish CRLs” /tr “cscript.exe //job:PublishIssCRLsToIIS C:\MSSScripts\CA_Operations.wsf” /sc Hourly /ru “System”
Entfernen von unerwünschten Vorlagen der ausstellenden Zertifizierungsstelle
Es wird allgemein empfohlen, Vorlagen zu entfernen, die nicht verwendeten Zertifikattypen entsprechen, damit diese nicht versehentlich veröffentlicht werden können. Diese Vorlagen können bei Bedarf auf einfache Weise neu erstellt werden, da sie immer im Verzeichnis verfügbar sind.

**So entfernen Sie unerwünschte Vorlagen aus der ausstellenden Zertifizierungsstelle**
* Melden Sie sich als Mitglied der Domänengruppe „CA Admins“ an.

* Wählen Sie den Container „Zertifikatvorlagen“ in der Verwaltungskonsole für die Zertifizierungsstelle aus.

* Entfernen Sie die folgenden Vorlagentypen:
* EFS-Wiederherstellungs-Agent

* Basis-EFS

* Webserver

* Computer

* Benutzer

* Untergeordnete Zertifizierungsstelle

* Administrator



Internetauthentifizierung

Dieser Abschnitt stellt Ihnen detaillierte Informationen zur Verfügung, die Ihnen bei der Implementierung einer RADIUS-Infrastruktur helfen. Diese Infrastruktur unterstützt die sichere WLAN-Lösung, die in diesem Handbuch beschrieben wird. Die in diesem Handbuch implementierte RADIUS-Infrastruktur beruht auf Windows Server 2003 IAS (Internet Authentication Servers).

Entwurf der RADIUS-Infrastruktur

Die folgenden Tabellen können als Arbeitsblätter verwendet werden, in denen die erforderlichen Informationen gesammelt werden, auf die im gesamten Handbuch Bezug genommen wird. Einige dieser Informationen werden mit Skripts festgelegt, die diesem Leitfaden beigefügt sind oder manuell gemäß den Listen in den entsprechenden Abschnitten eingegeben werden können.
Zuvor benötigte benutzerdefinierte Konfigurationsinformationen
In der folgenden Tabelle werden Informationen aufgeführt, die für jedes einzelne Unternehmen spezifisch sind. Stellen Sie sicher, dass die Informationen gesammelt, diskutiert und aufgezeichnet werden, bevor Sie fortfahren.

**Tabelle 15. Benutzerdefinierte Konfigurationseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


DNS-Name der Stammdomäne der Active Directory-Gesamtstruktur

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


NetBIOS-Name der Domäne

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Primärer IAS-Servername

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Sekundärer IAS-Servername

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

</table>

Zuvor benötigte, durch die Lösung vorgegebene Konfigurationsinformationen
In der folgenden Tabelle werden Einstellungen aufgeführt, die nur dann geändert werden müssen, wenn ein bestimmter Grund vorliegt. Vergewissern Sie sich, dass die Auswirkungen und Abhängigkeiten durch Änderungen vollkommen klar sind und eingeplant werden, bevor Parameter geändert werden. Dies schließt auch Änderungen an Skripts ein, die möglicherweise erforderlich sind.

**Tabelle 16. Lösungsdefinierte Konfigurationseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Vollständiger Name der administrativen Gruppe, die die IAS-Konfiguration kontrolliert

</td>

<td style="border:1px solid black;">


IAS Admins

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Vollständiger Name der Gruppe, die die Protokolle für die IAS-Authentifizierung und die Kontoführungsanforderungen überwacht

</td>

<td style="border:1px solid black;">


IAS Security Auditors

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad für Installationsskripts

</td>

<td style="border:1px solid black;">


C:\MSSScripts

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Batchdatei für IAS-Konfigurationsexport

</td>

<td style="border:1px solid black;">


IASExport.bat

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Batchdatei für IAS-Konfigurationsimport

</td>

<td style="border:1px solid black;">


IASImport.bat

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Batchdatei für IAS RADIUS-Clientkonfigurationsexport

</td>

<td style="border:1px solid black;">


IASClientExport.bat

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Batchdatei für IAS RADIUS-Clientkonfigurationsimport

</td>

<td style="border:1px solid black;">


PIASClientImport.bat

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad für Konfigurationssicherungsdateien

</td>

<td style="border:1px solid black;">


D:\IASConfig

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Speicherort der Protokolle für IAS-Authentifizierung und Überwachungsanforderungen

</td>

<td style="border:1px solid black;">


D:\IASLogs

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Freigabename der RADIUS-Anforderungsprotokolle

</td>

<td style="border:1px solid black;">


IASLogs

</td>

</tr>

</table>


IAS-Serverbereitstellung

Die in den nachfolgenden Abschnitten beschriebene Lösung umfasst zwei zentral angeordnete IAS-Server, die als RADIUS-Server für die WLAN-Zugriffsteuerung konfiguriert sind. Vor diesem Hintergrund sollten die folgenden Aufgaben abgeschlossen werden, bevor fortgefahren wird.
* Die Serverhardware sollte zugewiesen und konfiguriert werden.

* Das Serverbetriebssystem sollte gemäß den gegebenenfalls geltenden Unternehmensverfahren installiert und konfiguriert werden.

* Active Directory sollte vorhanden sein und normal funktionieren.

* Die Absicherungsverfahren des Unternehmens für Server und zusätzliche Anwendungen gemäß gültigen Richtlinien sollten umgesetzt sein.

Installieren der Konfigurationsskripts
Zahlreiche Unterstützungsskripts wurden mit dieser Lösung bereitgestellt, um die Implementierung zu vereinfachen. Diese Skripts müssen auf jedem Server installiert werden, bevor fortgefahren wird. Sie dürfen nicht gelöscht werden, selbst wenn die in diesem Handbuch beschriebenen Schritte abgeschlossen wurden.

**So installieren Sie die Setupskripts**
* Erstellen Sie einen Ordner mit dem Namen „C:\MSSScripts“.

* Kopieren Sie die Skripts von der Verteilerquelle in den oben erstellten Ordner.

Zusätzliche Anforderungen an die Serversoftware
Zusätzlich zum Serverbetriebssystem und allen anderen Anwendungen, die gemäß einer festgelegten Richtlinie zur Serverkonfiguration erforderlich sein könnten, müssen die Programmdatei CAPICOM 2.1 und die unterstützende DLL-Bibliothek installiert werden, um die von diesem Handbuch bereitgestellten Skripts zu unterstützen.

Weitere Informationen zu [CAPICOM](http://www.microsoft.com/downloads/details.aspx?familyid=860ee43a-a843-462f-abb5-ff88ea5896f6&amp;displaylang=en) einschließlich des Links für den Download und der Installationsanweisungen finden Sie unter www.microsoft.com/downloads/details.aspx?FamilyID=860ee43a-a843-462f-abb5-ff88ea5896f6&amp;DisplayLang=en
Konfigurieren der administrativen Gruppen für IAS
Der folgende Skriptbefehl erstellt die Sicherheitsgruppen „IAS Admins“ und „IAS Security Auditors“:
Cscript //job:CreateIASGroups C:\MSSScripts\IAS_Tools.wsf
In Umgebungen mit mehreren Domänen sollten diese Gruppen in derselben Domäne erstellt werden, in der sich die IAS-Server befinden.

Nach dem Erstellen der erforderlichen Gruppen müssen sie konfiguriert werden, um IAS-Konfigurationsaufgaben auszuführen. Gehen Sie hierzu wie folgt vor:
* Fügen Sie die globale Gruppe „IAS Admins“ in der Domäne zur lokalen Administratorgruppe auf jedem IAS-Server hinzu.

* Wenn IAS auf Domänencontrollern installiert ist, muss die Gruppe „IAS Admins“ zur Administratorgruppe für die Domäne hinzugefügt werden.

* Die Gruppen „IAS Admins“ und „IAS Security Auditors“ müssen mit den entsprechenden Benutzerkonten gefüllt werden.

Konfigurieren der Sicherheitseinstellungen des Serversystems
Wie zuvor erwähnt, wird in diesem Handbuch davon ausgegangen, dass die meisten mittelgroßen Unternehmen Verfahren und Richtlinien zum Absichern von Servern eingerichtet haben. Aus diesem Grund gibt es keine detaillierten Anweisungen für den Prozess zum Sichern der Server, der für diese Lösung erforderlich ist. Wenn keine Richtlinien oder Verfahren zum Absichern der Server vorhanden sind, oder wenn weitere Informationen zum Sichern von IAS-Servern erforderlich sind, finden Sie im [Sicherheitshandbuch für Windows Server](http://go.microsoft.com/fwlink/?linkid=14846) unter http://go.microsoft.com/fwlink/?LinkId=14846 weitere Informationen.

Installieren und Konfigurieren von IAS

Der folgende Abschnitt beschreibt die Installation von IAS auf Servern. Es ist wichtig, dass jeder Installations- und Konfigurationsschritt auf jedem IAS-Server ausgeführt wird.

Die Installation von IAS erfolgt durch Auswählen der Komponente „Netzwerkdienste – Internetauthentifizierungsdienst“ im Windows Manager für die Installation optionaler Komponenten (zugänglich über „Windows-Komponenten hinzufügen/entfernen“ in der Systemsteuerung). Zum Vereinfachen dieses Prozesses verwenden Sie das folgende Skript:
sysocmgr /i:sysoc.inf /u:C:\MSSScripts\OC_AddIAS.txtRegistrieren von IAS in Active Directory
Die IAS-Server müssen in jeder Domäne registriert werden. Hierzu muss das Computerkonto eines jeden IAS-Servers zu einem Mitglied der Sicherheitsgruppe „RAS and IAS Servers“ innerhalb jeder Domäne gemacht werden, die für die Authentifizierung erforderlich sind. Die Mitgliedschaft in diesen Gruppen stellt sicher, dass die IAS-Server über die Berechtigung zum Lesen der Remotezugriffseigenschaften aller Benutzer- und Computerkonten in den Domänen verfügen.

**So registrieren Sie IAS in Active Directory**
* Melden Sie sich an jedem Server mit einem Konto an, das über die Domänenadministratorberechtigung für die Domänen verfügt, in denen der IAS-Server registriert werden muss.

* Führen Sie für die Standarddomäne den folgenden Befehl an einer Eingabeaufforderung aus:
netsh ras add registeredserver
* Führen Sie für andere Domänen als die Standarddomäne den folgenden Befehl an einer Eingabeaufforderung aus:
netsh ras add registeredserver domain = DomainName
**Hinweis**   Als Alternative kann das Computerobjekt „IAS Server“ über das MMC-Snap-In für Active Directory-Benutzer und -Computer zu den Sicherheitsgruppen „RAS and IAS Servers“ hinzugefügt werden.

Erstellen und Sichern von IAS-Datenverzeichnissen
Es gibt einige Verzeichnisanforderungen für das Speichern von Konfigurations- und Protokolldaten auf IAS-Servern. Um den Konfigurationsprozess zum Erstellen und Sichern dieser Verzeichnisse zu vereinfachen, kann die folgende Batchdatei an der Eingabeaufforderung verwendet werden:
C:\MSSScripts\IAS_Data.bat
**Hinweis**   Möglicherweise ist es erforderlich, die Einträge für %*DomainName*% zu bearbeiten und zu ersetzen, um dem NETBIOS-Domänennamen der spezifischen Umgebung in dieser Batchdatei Rechnung zu tragen, bevor sie ausgeführt wird.

Konfigurieren des primären IAS-Servers

Der Server, der als primärer IAS-Server ausgewählt wird, muss vor allen anderen IAS-Servern in der Umgebung konfiguriert werden, da er als Vorlage für das Konfigurieren der Einstellungen auf allen nachfolgenden IAS-Servern dient.
Protokollieren von Authentifizierungs- und Kontoführungsanforderungen
IAS führt in der Standardeinstellung die Protokollierung von RADIUS-Authentifizierungs- und Kontoführungsanforderungen aus. Beides sollte jedoch aktiviert werden, um sicherzustellen, dass Sicherheitsereignisse aufgezeichnet werden und verwendet werden können, falls eine Untersuchung erforderlich wird.

**So konfigurieren Sie die Protokollierung von Authentifizierungs- und Kontoführungsanforderungen**
* Wählen Sie im MMC-Snap-In für den Internetauthentifizierungsdienst die Einstellung „RAS-Protokollierung“ aus, und zeigen Sie dann die Eigenschaften der Protokollierungsmethode „Lokale Datei“ an.

* Wählen Sie Kontoführungsanforderungen und Authentifizierungsanforderungen aus.

* Vergewissern Sie sich, dass für das Protokolldateiverzeichnis die Einstellung „D:\IASLogs“ sowie ein datenbankkompatibles Format ausgewählt wurden (auf diese Weise können die Protokolle direkt in Datenbanken wie Microsoft SQL Server™ importiert werden).


WLAN 802.1X-Authentifizierung

Dieser Abschnitt beschreibt schrittweise den Prozess zum Implementieren der WLAN-Sicherheit mit der 802.1X-Protokollspezifikation bei den Plattformen Windows Server 2003 und Windows XP SP1. Diese Anweisungen enthalten Informationen zur Konfiguration von Active Directory-Gruppen, der Bereitstellung von X.509-Zertifikaten, Änderung der IAS-Servereinstellungen, Bereitstellung einer WLAN-Gruppenrichtlinie sowie einige Tipps zum Konfigurieren von drahtlosen Zugriffspunkten für die Unterstützung der 802.1X EAP-TLS-Implementierung, auf der dieses Handbuch basiert.

Vorbereiten der Umgebung für ein sicheres WLAN

Nachdem nun die zugrunde liegenden Zertifikat- und RADIUS-Infrastrukturen vorhanden sind, können die eigentlichen spezifischen Konfigurationsschritte für 802.1X implementiert werden. Die folgenden Tabellen mit erforderlichen Einstellungen können Sie beim Prozess zum Sammeln von Informationen unterstützen, der vor der eigentlichen Implementierung erfolgen muss. Einige dieser Einstellungen werden manuell aktiviert, während andere Einstellungen Bestandteil der Skripts sind, die mit diesem Handbuch bereitgestellt wurden.
Zuvor benötigte benutzerdefinierte Konfigurationseinstellungen
In der folgenden Tabelle werden unternehmensspezifische Parameter aufgeführt, die gesammelt oder festgelegt werden müssen, bevor mit dieser Phase der Implementierung eines sicheren WLAN fortgefahren wird. Der bereitgestellte Platz kann verwendet werden, um die Einstellungen aufzuzeichnen, die für jede spezifische Umgebung erforderlich sind.

**Tabelle 17. Zuvor benötigte benutzerdefinierte Einstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


DNS-Name der Stammdomäne der Active Directory-Gesamtstruktur

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


NetBIOS-Domänenname

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Primärer IAS-Servername

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Sekundärer IAS-Servername

</td>

<td style="border:1px solid black;">


 

</td>

</tr>

</table>

Zuvor benötigte lösungsdefinierte Konfigurationseinstellungen
In der folgenden Tabelle werden Einstellungen aufgeführt, die nur dann geändert werden müssen, wenn ein bestimmter Grund vorliegt. Vergewissern Sie sich, dass die Auswirkungen und Abhängigkeiten durch Änderungen vollkommen klar sind und eingeplant werden, bevor Parameter geändert werden. Dies schließt auch Änderungen an Skripts ein, die möglicherweise erforderlich sind.

**Tabelle 18. Lösungsdefinierte Konfigurationseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Konfigurationselement

</th>

<th style="border:1px solid black;">

Einstellung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory zum Steuern der Bereitstellung von 802.1X-Benutzerauthentifizierungszertifikaten

</td>

<td style="border:1px solid black;">


AutoEnroll Client Authentication – User Certificate

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory zum Steuern der Bereitstellung von 802.1X-Computerauthentifizierungszertifikaten

</td>

<td style="border:1px solid black;">


AutoEnroll Client Authentication – Computer Certificate

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory, die die IAS-Server enthält, die 802.1X Authentifizierungszertifikate erfordern

</td>

<td style="border:1px solid black;">


AutoEnroll RAS und IAS Server Authentication Certificate

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory, die die Benutzer enthält, die auf das drahtlose Netzwerk zugreifen dürfen

</td>

<td style="border:1px solid black;">


RAS-Richtlinie Drahtlose Benutzer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory, die die Computer enthält, die auf das drahtlose Netzwerk zugreifen dürfen

</td>

<td style="border:1px solid black;">


RAS-Richtlinie Drahtlose Computer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Universelle Gruppe in Active Directory, die sowohl die Gruppe „Drahtlose Benutzer“ als auch „Drahtlose Computer“ enthält

</td>

<td style="border:1px solid black;">


RAS-Richtlinie Drahtloser Zugriff

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Gruppe in Active Directory, die die Computer enthält, für die die Konfiguration der Eigenschaften des drahtlosen Netzwerks erforderlich ist

</td>

<td style="border:1px solid black;">


Drahtlosnetzwerkrichtlinie Computer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zertifikatvorlage zum Erzeugen der Zertifikate für die Benutzerclientauthentifizierung

</td>

<td style="border:1px solid black;">


Clientauthentifizierung Benutzer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zertifikatvorlage zum Erzeugen der Zertifikate für die Computerclientauthentifizierung

</td>

<td style="border:1px solid black;">


Clientauthentifizierung Computer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zertifikatvorlage zum Erzeugen der Serverauthentifizierungszertifikate für IAS

</td>

<td style="border:1px solid black;">


RAS und IAS Server Authentication

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad für Installationsskripts

</td>

<td style="border:1px solid black;">


C:\MSSScripts

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad für Konfigurationssicherungsdateien

</td>

<td style="border:1px solid black;">


D:\IASConfig

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Pfad für IAS-Authentifizierungs- und Überwachungsprotokolle

</td>

<td style="border:1px solid black;">


D:\IASLogs

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Richtlinienname

</td>

<td style="border:1px solid black;">


Drahtlosen Zugriff zulassen

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Name des Gruppenrichtlinienobjekts in Active Directory

</td>

<td style="border:1px solid black;">


Drahtlosnetzwerkrichtlinie

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Richtlinie für drahtloses Netzwerk innerhalb des obigen Gruppenrichtlinienobjekts

</td>

<td style="border:1px solid black;">


Client-Computer drahtlose Konfiguration

</td>

</tr>

</table>

Erstellen der erforderlichen Active Directory-Gruppen für WLAN-Zugriff
Das folgende Skript muss mit einem Konto ausgeführt werden, das über die Berechtigung zum Erstellen von Active Directory-Sicherheitsgruppen verfügt, da es die erforderlichen Gruppen zum Implementieren der Registrierung für drahtlose Authentifizierungszertifikate, der RAS-Richtlinie und der Gruppenrichtlinie für drahtlose Netzwerke erstellt:
Cscript //job:CreateWirelessGroups C:\MSSScripts\wl_tools.wsf
**Hinweis**   In Gesamtstrukturumgebungen mit mehreren Domänen sollten die Gruppen in derselben Domäne wie die Drahtlosbenutzer erstellt werden.
Überprüfen der DHCP-Einstellungen
Um drahtlose Netzwerke zu unterstützen, sollten die DHCP-Server mit spezifischen Bereichen für die Drahtlostechnologie und einer Leasedauer für IP-Adressen konfiguriert werden, die kürzer als bei anderen drahtgebundenen Clients sind. Klären Sie dies mit den DHCP-Serveradministratoren, um sicherzustellen, dass DHCP ordnungsgemäß konfiguriert wurde. Weitere Informationen zur DHCP-Planung für WLANs finden Sie im [Windows Server 2003-Bereitstellungskit](http://www.microsoft.com/windowsserver2003/techinfo/reskit/deploykit.mspx) unter www.microsoft.com/windowsserver2003/techinfo/reskit/deploykit.mspx.

Konfigurieren der WLAN-Authentifizierungszertifikate

Zum Implementieren der EAP-TLS-basierten WLAN-Sicherheit gemäß Beschreibung in diesem Handbuch müssen die folgenden Typen von Zertifikaten erstellt und bereitgestellt werden:
* Clientauthentifizierung Computer

* Clientauthentifizierung Benutzer

* RAS und IAS Server Authentication

Erstellen einer Zertifikatvorlage für die IAS-Serverauthentifizierung
IAS-Server benötigen ein Serverzertifikat zum Authentifizieren von Computern für Clients während des EAP-TLS-Protokollhandshakes. Der Administrator der Zertifikatsdienste muss die folgenden Schritte ausführen, um eine Zertifikatvorlage für die Serverauthentifizierung für die Verwendung durch die IAS-Server zu erstellen.

**So erstellen Sie eine Zertifikatvorlage für die Serverauthentifizierung**
* Melden Sie sich an der ausstellenden Zertifizierungsstelle mit einem Konto der administrativen Gruppe der Zertifizierungsstelle an, und führen Sie die MMC für Zertifikatvorlagen aus.

* Erstellen Sie ein Duplikat der RAS- und IAS-Server-Zertifikatvorlage. Geben Sie auf der Registerkarte **Allgemein** der Eigenschaften für die neue Vorlage im Feld **Vorlagenanzeigename** den Namen **RAS und IAS Server Authentication** ein.

* Vergewissern Sie sich auf der Registerkarte **Erweiterungen**, dass die Ausstellungsrichtlinien nur die Serverauthentifizierung (OID 1.3.6.1.5.5.7.3.1) umfassen.

* Bearbeiten Sie ebenfalls auf der Registerkarte **Erweiterungen** die Ausstellungsrichtlinien zum Hinzufügen der Richtlinie „Mittlere Zusicherung“.

* Wählen Sie auf der Registerkarte **Antragstellername** die Option **Aus diesen Informationen in Active Directory erstellen** aus. Stellen Sie auch sicher, dass für **Format des Antragstellernamen** die Einstellung **Allgemeiner Name** ausgewählt wurde und dass nur **DNS-Name** unter **Informationen im alternativen Antragstellernamen****einbeziehen** ausgewählt wurde.

* Klicken Sie auf der Registerkarte **Anforderungsverarbeitung** auf die Schaltfläche **Kryptografiedienstanbieter**, stellen Sie sicher, dass **Einen der folgenden Kryptografiedienstanbieter verwenden** ausgewählt wurde und dass ausschließlich **Microsoft RSA SChannel Cryptographic Provider** ausgewählt ist.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe **AutoEnroll RAS und IAS Server Authentication Certificate** mit den Berechtigungen Lesen, Registrieren und Autoregistrierung hinzu, und entfernen Sie alle anderen Gruppen, die möglicherweise Berechtigungen zum manuellen oder automatischen Registrieren dieser Zertifikatvorlage haben.

**Hinweis**   Es könnte vorteilhaft sein, für dieses Zertifikat die Genehmigung durch die Zertifikatsverwaltung zu erfordern, da es einen relativ hohen Sicherheitswert aufweist. Durch Aktivieren dieses Werts wird dazu beigetragen, dass ein riskanter IAS-Server nicht registriert wird, sondern manuelle Genehmigung erfordert, nachdem die Zertifikate ausgestellt und automatisch vom IAS-Server gesendet wurden.

Erstellen einer Zertifikatvorlage für die Benutzerauthentifizierung
Endbenutzer benötigen Benutzerzertifikate für die Authentifizierung am IAS-Server während des EAP-TLS-Handshakeprozesses. Wiederum sollten die folgenden Schritte von einem Konto aus durchgeführt werden, das über Administratorrechte für Zertifikatsdienste verfügt.

**So erstellen Sie eine Zertifikatvorlage für die Benutzerauthentifizierung**
* Starten Sie das MMC-Snap-In für Zertifikatvorlagen auf dem Server für die ausstellende Zertifizierungsstelle.

* Erstellen Sie ein Duplikat der Vorlage „Authentifizierte Sitzung“, und geben Sie auf der Registerkarte **Allgemein** der neuen Vorlage im Feld **Vorlagenanzeigename** den Namen **Clientauthentifizierung – Benutzer** ein.

* Klicken Sie auf der Registerkarte **Anforderungsverarbeitung** auf die Schaltfläche **Kryptografiedienstanbieter**, und deaktivieren Sie die Kontrollkästchen **Microsoft Base DSS** **Cryptographic Provider.**  

* Stellen Sie sicher, dass auf der Registerkarte **Antragstellername** die Einstellung **Aus diesen Informationen in Active Directory erstellen** ausgewählt ist. Wählen Sie unter **Format des Antragstellernamen** die Einstellung **Allgemeiner Name** aus. Vergewissern Sie sich, dass **Benutzerprinzipalname** **(UPN)** als einzige Option unter **Informationen im alternativen Antragstellernamen einbeziehen** ausgewählt ist.

* Stellen Sie sicher, dass auf der Registerkarte **Erweiterungen** nur **Clientauthentifizierung (OID 1.3.6.1.5.5.7.3.2)** in **Anwendungsrichtlinien** enthalten ist. Bearbeiten Sie auch die Ausstellungsrichtlinien, und fügen Sie die Richtlinie **Niedrige Zusicherung** hinzu.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe **AutoEnroll Client Authentication – User Certificate** mit den Berechtigungen Lesen, Registrieren und Autoregistrierung hinzu. Außerdem sollten alle anderen Gruppen entfernt werden, die über Berechtigungen zum Registrieren oder automatischen Registrieren verfügen.

Erstellen einer Zertifikatvorlage für die Computerauthentifizierung
Dieses Zertifikat wird von Computern beim Authentifizieren mit dem IAS-Server während des EAP-TLS-Handshakes verwendet. Wieder sollte der Administrator für Zertifikatsdienste die folgenden Aufgaben ausführen.

**So erstellen Sie eine Zertifikatvorlage für die Computerauthentifizierung**
* Starten Sie das MMC-Snap-In für Zertifikatvorlagen auf der ausstellenden Zertifizierungsstelle.

* Erstellen Sie ein Duplikat der Vorlage „Arbeitsstationsauthentifizierung“. Geben Sie auf der Registerkarte **Allgemein** der neuen Vorlage im Feld **Vorlagenanzeigename** den Namen **Clientauthentifizierung Computer** ein.

* Stellen Sie sicher, dass auf der Registerkarte **Antragstellername** die Einstellung **Aus diesen Informationen in Active Directory erstellen** ausgewählt ist. Wählen Sie unter **Format des Antragstellernamen** die Einstellung **Allgemeiner Name** aus. Vergewissern Sie sich, dass **DNS-Name** als einzige Option unter **Informationen im alternativen Antragstellernamen einbeziehen** ausgewählt ist.

* Bearbeiten Sie auf der Registerkarte **Erweiterungen** die Anwendungsrichtlinien, und stellen Sie sicher, dass nur **Clientauthentifizierung (OID 1.3.6.1.5.5.7.3.2)** enthalten ist. Bearbeiten Sie auch die **Ausstellungsrichtlinien**, und fügen Sie die Richtlinie **Niedrige Zusicherung** hinzu.

* Fügen Sie auf der Registerkarte **Sicherheit** die Sicherheitsgruppe **AutoEnroll Client Authentication – Computer Certificate** mit den Berechtigungen Lesen, Registrieren und Autoregistrierung hinzu. Alle anderen Gruppen mit Berechtigungen sollten entfernt werden.

Hinzufügen von WLAN-Authentifizierungszertifikaten zur Zertifizierungsstelle
Nachdem nun die Zertifikatvorlagen konfiguriert wurden, müssen sie zur Zertifizierungsstelle hinzugefügt werden, um die Registrierung zu ermöglichen. Hierzu muss der Administrator für die Zertifikatsdienste die folgenden Aufgaben ausführen.

**So fügen Sie Zertifikatvorlagen zur Zertifizierungsstelle hinzu**
* Starten Sie auf der ausstellenden Zertifizierungsstelle das MMC-Snap-In für die Zertifizierungsstelle, und klicken Sie mit der rechten Maustaste auf den Ordner **Zertifikatvorlagen.**   Klicken Sie auf **Neu**, und klicken Sie dann auf **Auszustellende Zertifikatvorlage.**   Wählen Sie die folgenden Zertifikate aus, und klicken Sie dann auf **OK**:
* Clientauthentifizierung Computer

* Clientauthentifizierung Benutzer

* RAS und IAS Server Authentication


Registrieren für das IAS-Serverzertifikat
Das Bereitstellen der Serverauthentifizierungszertifikate für IAS-Server ist ein relativ einfacher und automatisierter Vorgang.

**So registrieren Sie einen IAS-Server**
* Starten Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer, und fügen Sie die IAS-Computerkonten zur Sicherheitsgruppe „AutoEnroll RAS und IAS Server Authentication Certificate“ hinzu.

* Starten Sie den IAS-Server neu, und melden Sie sich als Mitglied der lokalen Administratorgruppe an.

* Führen Sie an einer Eingabeaufforderung GPUPDATE /force aus.

* Öffnen Sie die MMC, und fügen Sie dann das Snap-In für Zertifikate hinzu. Wählen Sie bei der entsprechenden Abfrage die Option „Computerkonto“ aus, und wählen Sie dann „Lokaler Computer“ aus.

* Wählen Sie in der Konsolenstruktur **Zertifikate (Lokaler Computer)** aus, klicken Sie im Menü **Aktion** auf **Alle Tasks**, und klicken Sie dann auf **Zertifikate automatisch registrieren.**  

**Hinweis**   Wenn die Option zum Erfordern der Genehmigung durch die Zertifikatsverwaltung aktiviert war, muss der Administrator der Zertifizierungsstelle die Gültigkeit dieser Anforderung überprüfen und das Zertifikat ausstellen.

Hinzufügen von Benutzern und Computern zu Gruppen für die Autoregistrierung
Benutzer und Computer, die WLAN-Konnektivität verwenden möchten, benötigen Benutzer- und Computerzertifikate, bevor sie eine Authentifizierung am Netzwerk über eine drahtlose Verbindung ausführen und auf das Netzwerk zugreifen können. Der Prozess zum Ausstellen und Erneuern dieser Zertifikate ist für den Endbenutzer transparent, da zuvor Autoregistrierungsgruppen eingerichtet wurden.

Zum Hinzufügen von Benutzern und deren Computern zu den Autoregistrierungsgruppen verwenden Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer, um die Benutzerkonten zur Gruppe „AutoEnroll Client Authentication – User Certificate“ hinzuzufügen und deren Computer zur Gruppe „AutoEnroll Client Authentication – Computer Certificate“ hinzuzufügen. Nachdem dies erfolgt ist, erhalten die entsprechenden Benutzer ihre Benutzer- und Computerzertifikate, nachdem sie ihre Computer neu starten und sich wieder am Netzwerk anmelden.

**Hinweis**   Bei dieser Lösung werden benutzerdefinierte Gruppen verwendet, um zu steuern, welche Benutzer und Computer Zertifikate erhalten können. Wenn die Umgebung erfordert, dass alle Benutzer und Computer Zertifikate benötigen, fügen Sie einfach die Domänenbenutzer zur Gruppe „AutoEnroll Client Authentication – User Certificate“ und die Domänencomputer zur Gruppe „AutoEnroll Client Authentication – Computer Certificate“ hinzu.

Konfigurieren der Infrastruktur für den WLAN-Zugriff

Der primäre IAS-Server muss mit einer RAS-Richtlinie und Einstellungen für Verbindungsanforderungen konfiguriert werden, die die Authentifizierung und Autorisierung von drahtlosen Clients für das WLAN bestimmen. Diese Einstellungen müssen dann auf die anderen IAS-Server repliziert werden. Danach muss jeder IAS-Server einzeln konfiguriert werden, um Verbindungen von RADIUS-Clients wie drahtlosen Zugriffspunkten zu akzeptieren. Danach müssen die drahtlosen Zugriffspunkte konfiguriert werden, um den IAS-Server als Authentifizierungs- und Autorisierungsquelle für das drahtlose 802.1X-Netzwerk zu verwenden.
Erstellen einer IAS RAS-Richtlinie für WLANs
Verwenden Sie das MMC-Snap-In für den Internetauthentifizierungsdienst auf dem primären IAS-Server, um IAS wie folgt mit einer RAS-Richtlinie zu konfigurieren.

**So erstellen Sie eine RAS-Richtlinie**
* Klicken Sie mit der rechten Maustaste auf den Ordner **RAS-Richtlinien**, und klicken Sie dann auf **Neue RAS-Richtlinie erstellen.**  

* Nennen Sie die neue Richtlinie **Drahtlosen Zugriff zulassen**, und legen Sie im Assistenten die Einstellung **Typische Richtlinie für ein allgemeines Szenario** fest.

* Wählen Sie als Zugriffsmethode **Drahtlos** aus.

* Gewähren Sie Zugriff basierend auf Gruppen, und verwenden Sie die Sicherheitsgruppe „RAS-Richtlinie Drahtloser Zugriff“.

* Wählen Sie **Smartcard oder anderes Zertifikat für das Extensible Authentication Protocol (EAP)**, und wählen Sie dann das für IAS installierte Serverauthentifizierungszertifikat aus.

* Beenden Sie den Assistenten.

* Öffnen Sie die Eigenschaften der Richtlinie „Drahtlosen Zugriff zulassen“, und klicken Sie dann auf **Profil bearbeiten.**  

* Fügen Sie auf der Registerkarte **Erweitert** das Attribut **Ignore-User-Dialin-Properties** hinzu, legen Sie dafür den Wert **Wahr** fest, und fügen Sie dann das Attribut **Termination-Action** hinzu, und legen Sie dafür den Wert **RADIUS-Anforderung** fest.

**Hinweis**   Die Richtlinie „Drahtlosen Zugriff zulassen“ kann gleichzeitig mit anderen, von Benutzern erstellten Richtlinien oder den standardmäßigen Zugriffsrichtlinien verwendet werden. Die standardmäßige RAS-Richtlinie muss jedoch erst nach der Richtlinie „Drahtlosen Zugriff zulassen“ im Ordner mit den RAS-Richtlinien aufgeführt werden, um ordnungsgemäß zu funktionieren.

Hinzufügen von RADIUS-Clients zu IAS
Drahtlose Zugriffspunkte und RADIUS-Proxys müssen zu IAS als RADIUS-Clients hinzugefügt werden, damit sie die Authentifizierungs- und Kontoführungsdienste über das RADIUS-Protokoll verwenden können.

**So fügen Sie RADIUS-Clients zu IAS hinzu**
* Starten Sie das MMC-Snap-In für den Internetauthentifizierungsserver.

* Klicken Sie mit der rechten Maustaste auf den Ordner **RADIUS-Clients**, und klicken Sie dann auf **Neuer RADIUS-Client.**  

* Geben Sie den Anzeigenamen und die IP-Adresse des drahtlosen Zugriffspunkts ein.

* Wählen Sie „RADIUS Standard“ als Herstellerattribut des Clients, und geben Sie den gemeinsamen geheimen Schlüssel für den spezifischen drahtlosen Zugriffspunkt ein. Wählen Sie dann das Attribut **Anforderung muss das Attribut „Message Authenticator“ enthalten** aus.

**Hinweis**   Dieser Prozess sollte auf jedem IAS-Server wiederholt werden, um sicherzustellen, dass jeder Server über eine eindeutige Sammlung von drahtlosen Zugriffspunktclients und gemeinsamen geheimen Schlüsseln verfügt. Um diesen Prozess zu vereinfachen, enthält dieses Handbuch ein Skript, das zum Erzeugen gemeinsamer geheimer Schlüssel verwendet werden kann. Diese können dann an einem sicheren Ort gespeichert werden, falls eine Systemwiederherstellung erforderlich ist. Geben Sie zum Verwenden dieses Skripts folgenden Befehl an einer Eingabeaufforderung ein:
Cscript //job:GenPWD C:\MSSScripts\wl_tools.wsf /client:ClientName

Bereitstellen von Konfigurationen für mehrere IAS-Server

Nachdem die folgenden Elemente auf dem primären IAS-Server konfiguriert sind, können sie mit dem Befehl **netsh** in Textdateien exportiert werden. Nach dem Export können diese Textdateien dann auf jeden IAS-Server importiert werden, der eine ähnliche Funktion innerhalb der Umgebung ausführt. Dadurch wird sichergestellt, dass eine gemeinsame Konfiguration in der gesamten Umgebung vorhanden ist.

Zu den exportierbaren Konfigurationseinstellungen zählen:
* Servereinstellungen

* Protokollierungskonfiguration

* RAS-Richtlinien

* RADIUS-Clients

* Vollständige Konfiguration


Jeder IAS-Server sollte seine eigene eindeutige Liste mit RADIUS-Clients und gemeinsamen geheimen Schlüsseln aufweisen. Daher muss diese Information individuell auf jedem Server konfiguriert und einzeln gesichert werden. Außerdem enthält ein vollständiges Konfigurationsabbild höchst vertrauliche Informationen, die sorgfältig gesichert werden müssen, da diese Informationen bei einem Diebstahl für den Zugriff auf das drahtlose Netzwerk verwendet werden können.
Exportieren der Konfiguration des primären IAS-Servers
Die folgenden Typen von Einstellungen sollten in Textdateien exportiert werden, um auf andere IAS-Server repliziert zu werden.
* Serverkonfiguration

* Protokollierungseinstellungen

* RAS-Richtlinie

* Richtlinien für Verbindungsanforderungen


Um diesen Prozess zu vereinfachen, sind diesem Handbuch Batchdateien beigefügt, die die Befehle **netsh** enthalten. Dieser Befehl kann die gemeinsamen Konfigurationsinformationen in Textdateien im Verzeichnis „D:\IASConfig“ exportieren. Hierzu muss folgender Befehl an einer Eingabeaufforderung eingegeben werden:
C:\MSSScripts\IASExport.batImportieren von Konfigurationsinformationen vom primären IAS-Server
Wie zuvor erwähnt, verwendet IAS den Befehl **netsh** zum Übertragen von Konfigurationszuständen zwischen Servern. Dieser Prozess gestaltet die Bereitstellung effizienter und verringert zugleich die Gefahr von Fehlern während des Konfigurationsprozesses. Nachdem nun die Konfigurationsinformationen des primären IAS-Servers exportiert wurden, können die sekundären IAS-Server den Konfigurationszustand importieren.

**So importieren Sie den Konfigurationszustand des primären IAS-Servers auf andere IAS-Server**
* Kopieren Sie alle Konfigurationsdateien aus dem Verzeichnis „D:\IASConfig“ auf dem primären IAS-Server in das entsprechende Verzeichnis „D:\IASConfig“ auf anderen IAS-Servern.

* Verwenden Sie die folgende Batchdatei (diesem Handbuch beigefügt) an einer Eingabeaufforderung auf den sekundären Servern, um den Konfigurationszustand zu importieren:
C:\MSSScripts\IASImport.bat

Drahtlose Zugriffspunkte und Clients

Das Verfahren zum Konfigurieren drahtloser Zugriffspunkte kann sich je nach Marke und Modell des betreffenden Geräts stark unterscheiden. Allerdings stellen die Anbieter drahtloser Zugriffspunkte im Allgemeinen detaillierte Anweisungen zum Konfigurieren der Geräte mit den folgenden notwendigen Details zur Verfügung:
* 802.1X-Netzwerkeinstellungen

* Konfigurieren der primären RADIUS-Serveradresse

* Konfigurieren der sekundären RADIUS-Serveradresse

* Gemeinsamer geheimer RADIUS-Schlüssel für primären RADIUS-Server

* Gemeinsamer geheimer RADIUS-Schlüssel für sekundären RADIUS-Server


Anweisungen zum Konfigurieren von drahtloser Ausrüstung einer bestimmten Marke oder eines bestimmten Modells finden Sie in den Anweisungen des Herstellers oder der Website für Support.

Bereitstellen von WLAN-Authentifizierungszertifikaten

Dieser Abschnitt beschreibt einige wichtige Konfigurationsaufgaben, die erforderlich sind, um die automatische Zertifikatregistrierung für Windows XP-basierte Clients zu aktivieren. Obwohl sich frühere Abschnitte mit den zugrunde liegenden Richtlinien und Vorlagen für die Unterstützung der automatischen Zertifikatregistrierung in der Infrastruktur für Zertifikate beschäftigt haben, ist die Unterstützung von Windows XP für diese Funktionalität standardmäßig deaktiviert. Um die Unterstützung für die automatische Zertifikatregistrierung zu aktivieren, müssen die richtigen Einstellungen mit einer Gruppenrichtlinie konfiguriert werden. Durch die Verwendung von Sicherheitsgruppen zum Steuern der automatischen Registrierung kann diese Funktion für alle Benutzer und Computer in einer Domäne aktiviert werden. Mit den Sicherheitsgruppen kann bestimmt werden, wer die Zertifikate der einzelnen Typen erhält.

**So aktivieren Sie die automatische Registrierung für alle Benutzer und Computer in einer Domäne**
* Melden Sie sich mit einem Konto an, das über Berechtigungen zum Erstellen von Gruppenrichtlinienobjekten verfügt, und verknüpfen Sie Gruppenrichtlinienobjekte mit der Domäne.

* Wählen Sie in Active Directory-Benutzer und -Computer das Domänenobjekt durch Klicken mit der rechten Maustaste aus, und klicken Sie dann auf „Eigenschaften“.

* Klicken Sie auf der Registerkarte **Gruppenrichtlinie** auf **Neu**, und geben Sie dann einen Namen für das Gruppenrichtlinienobjekt ein (beispielsweise „Domain PKI Policies“).

* Klicken Sie auf **Bearbeiten**, und wechseln Sie dann zu **Richtlinien öffentlicher Schlüssel** unter Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen.

* Doppelklicken Sie im Bereich **Details** auf **Einstellung für die automatische Registrierung.**  

* Vergewissern Sie sich, dass die folgenden Einstellungen ausgewählt sind:
* Zertifikate automatisch registrieren

* Abgelaufene Zertifikate erneuern, ausstehende Zertifikate aktualisieren und gesperrte Zertifikate entfernen

* Zertifikate aktualisieren, die Zertifikatvorlagen verwenden


* Wiederholen Sie die Schritte 5 und 6 für die Einstellung zur automatischen Registrierung unter Benutzerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Richtlinien öffentlicher Schlüssel.

* Schließen Sie das Gruppenrichtlinienobjekt.

* Vergewissern Sie sich, dass das Gruppenrichtlinienobjekt über eine höhere Priorität als das standardmäßige Gruppenrichtlinienobjekt für Domänenrichtlinien verfügt.

* Wiederholen Sie dieses Verfahren für jede Domäne, in der die automatische Zertifikatregistrierung aktiviert wird, wenn eine Gesamtstruktur mit mehreren Domänen vorliegt.

**Hinweis**   Wenn Benutzer keine Roamingprofile verwenden und die automatische Registrierung universell erlaubt ist, werden Zertifikate an jedem Computer für Benutzer ausgestellt, an dem sie sich anmelden. Dies könnte unerwünscht sein, wenn sich administrative Benutzer an Servern anmelden. Um dies zu verhindern, wird empfohlen, ein Gruppenrichtlinienobjekt für Server zu erstellen, um die automatische Registrierung zu deaktivieren. Wenn die automatische Registrierung für alle Benutzer Nachteile mit sich bringt, kann ein Gruppenrichtlinienobjekt mit OUs verknüpft werden, das die Untergruppe von Benutzern enthält, die automatische Registrierung benötigen.


Aktivieren des WLAN-Zugriffs für Benutzer und Computer

Die endgültigen Schritte zum Aktivieren von Benutzern und Computern für den sicheren WLAN-Zugriff umfassen einige Aktionen, die für Active Directory-Objekte ausgeführt werden müssen. Diese Aktionen umfassen das Ändern von Kontoberechtigungen, Gruppenberechtigungen und Implementieren von WLAN-Gruppenrichtlinieneinstellungen.
Hinzufügen von Benutzern zu RAS-Richtliniengruppen
Die IAS RAS-Richtlinie verwendet Active Directory-basierte Sicherheitsgruppen zum Bestimmen, ob Benutzer und Computer zum Aufbauen von Verbindungen mit dem WLAN autorisiert sind. Die folgenden Sicherheitsgruppen wurden bereits in früheren Abschnitten erstellt:
* RAS-Richtlinie Drahtlose Benutzer

* RAS-Richtlinie Drahtlose Computer

* RAS-Richtlinie Drahtloser Zugriff


**So fügen Sie Benutzer und Computer zu den WLAN-Zugriffsgruppen hinzu**
* Öffnen Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer.

* Fügen Sie die Gruppe „RAS-Richtlinie Drahtlose Benutzer“ und die Gruppe „RAS-Richtlinie Drahtlose Computer“ zur Gruppe „RAS-Richtlinie – Drahtloser Zugriff“ hinzu.

* Fügen Sie Benutzer, die zum Zugriff auf das WLAN berechtigt sind, zur Gruppe „RAS-Richtlinie Drahtlose Benutzer“ hinzu.

* Fügen Sie Computer hinzu, die zum Zugriff auf das WLAN berechtigt sind, zur Gruppe „RAS-Richtlinie Drahtlose Computer“ hinzu.

**Hinweis**   Wenn beschlossen wird, dass standardmäßig allen Benutzern und Computern der Zugriff auf das WLAN eingeräumt werden soll, können die Gruppen „Domänenbenutzer“ und „Domänencomputer“ zu ihren jeweiligen Richtliniengruppen hinzugefügt werden, um die Verwaltung zu vereinfachen.

Erstellen der WLAN-Gruppenrichtlinie für Active Directory
Gruppenrichtlinien können verwendet werden, um die WLAN-Konfigurationseinstellungen für Clientcomputer zu automatisieren und durchzusetzen, da die MMC für Gruppenrichtlinien in Windows Server 2003 Richtlinieneinstellungen für drahtlose Netzwerke enthält, die auf den Standards 802.1X und 802.11 beruhen.

**So erstellen Sie eine Gruppenrichtlinie für drahtlose Netzwerke**
* Öffnen Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer auf einem Windows Server 2003-basierten Server oder einer Arbeitsstation, auf der die Verwaltungstools von Windows Server 2003 installiert sind.

* Wählen Sie die Eigenschaften des Domänenobjekts auf der Registerkarte **Gruppenrichtlinie** aus, klicken Sie auf **Neu**, und nennen Sie das Gruppenrichtlinienobjekt dann „Drahtlosnetzwerkrichtlinie“.

* Klicken Sie auf die Schaltfläche **Eigenschaften**, und gewähren Sie auf der Registerkarte **Sicherheit** der Sicherheitsgruppe „Drahtlosnetzwerkrichtlinie Computersicherheit“ die Gruppenrichtlinienberechtigungen zum Lesen und Übernehmen. Entfernen Sie zudem beim Gruppenrichtlinienobjekt aus „Authentifizierte Benutzer“ die Berechtigungen zum Übernehmen der Gruppenrichtlinie.

* Wählen Sie auf der Registerkarte **Allgemein** die Einstellung **Benutzerdefinierte Konfigurationseinstellungen deaktivieren** für das Richtlinienobjekt, und klicken Sie bei allen angezeigten Warnmeldungen auf **Ja.**   Übernehmen Sie die Änderungen, und schließen Sie das Fenster.

* Klicken Sie auf die Schaltfläche **Bearbeiten**, und wechseln Sie zu \Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Richtlinien für Drahtlosnetzwerke (IEEE 802.11).

* Wählen Sie das Objekt „Richtlinien für Drahtlosnetzwerke (IEEE 802.11)“ im Navigationsfenster aus, und klicken Sie dann im Menü **Aktion** auf **Drahtlosnetzwerkrichtlinie erstellen.**   Verwenden Sie den Assistenten, um die Richtlinie **Drahtloskonfiguration für Clientcomputer** zu nennen. Lassen Sie die Option **Eigenschaften bearbeiten** ausgewählt, und klicken Sie dann auf **Fertig stellen**, um den Assistenten zu schließen.

* Wählen Sie in der Richtlinie **Drahtloskonfiguration der Clientcomputer** die Registerkarte **Bevorzugte Netzwerke** aus, klicken Sie auf **Hinzufügen**, und geben Sie dann den Netzwerknamen oder die SSID (Service Set ID) des drahtlosen Netzwerks ein.

* Klicken Sie auf die Registerkarte **IEEE 802.1X**, und öffnen Sie dann die Einstellungen für **Smartcard oder anderes Zertifikat für das Extensible Authentication Protocol (EAP).**   Wählen Sie unter **Vertrauenswürdige Ursprungszertifizierungsagenturen** das Zertifikat der Stammzertifizierungsstelle für die PKI aus, in der die IAS-Serverzertifikate ausgestellt wurden.

* Schließen Sie die Eigenschaften für die Drahtloskonfiguration der Clientcomputer und den Gruppenrichtlinienobjekt-Editor.

**Hinweis**   WPA2 kann derzeit nicht mithilfe von Gruppenrichtlinienobjekten angewendet werden. Allerdings ist die Unterstützung durch Gruppenrichtlinienobjekte für WPA2 mit der Veröffentlichung von Windows Vista und Longhorn geplant. Zudem werden Updates verfügbar sein, um auch die Unterstützung für die aktuellen Windows-Versionen anzubieten.

Hinzufügen von Computern zu Sicherheitsgruppen für die WLAN-Gruppenrichtlinie
Active Directory-basierte Sicherheitsgruppen werden verwendet, um zu bestimmen, auf welche Computer Richtlinien für drahtlose Netzwerke angewendet werden, um automatisch die erforderlichen 802.11- und 802.1X-Einstellungen zu konfigurieren. Diese Einstellungen sollten bereitgestellt werden, bevor die 802.1X-Einstellungen auf drahtlosen Zugriffspunkten konfiguriert werden und das WLAN aktiviert wird. Dieser Ansatz stellt sicher, dass die Clientcomputer über ausreichende Möglichkeiten verfügen, um die computerbasierte Gruppenrichtlinie herunterzuladen und zu übernehmen, selbst wenn sie selten eine Verbindung mit dem drahtgebundenen Netzwerk herstellen.

Die Gruppenrichtlinieneinstellungen können sogar vor der Installation eines WLAN-Schnittstellenadapters (NIC) installiert werden, da automatisch die richtigen Gruppenrichtlinieneinstellungen für Netzwerke abgerufen und übernommen werden.

Um Computer zu den Gruppen für die Gruppenrichtlinie für drahtlose Netzwerke hinzufügen, verwenden Sie das MMC-Snap-In für Active Directory-Benutzer und -Computer, um die autorisierten Computerobjekte zur Gruppe „Drahtlosnetzwerkrichtlinie Computer“ hinzuzufügen.

**Hinweis**   Die Gruppenrichtlinieneinstellungen für drahtlose Netzwerke werden auf den Clientcomputern während des nächsten Aktualisierungsintervalls für Computergruppenrichtlinien aktualisiert. Um eine Aktualisierung zu erzwingen, geben Sie den Befehl GPUPDATE /force ein.

WPA2-Clientanforderungen

Die in diesem Handbuch skizzierte Lösung wurde für Clientcomputer mit Unterstützung für Drahtlostechnologie entworfen, die Windows XP Professional mit SP2 oder Windows XP Tablet Edition als Betriebssystem verwenden. Diese Versionen von Windows bieten integrierte Unterstützung für 802.1X und WLAN. Außerdem stellen Clients auf der Grundlage von Windows XP die Funktionalität für automatische Registrierung und Erneuerung von Zertifikaten bereit, was eine zertifikatbasierte Lösung wie diese besonders dann sehr kostengünstig gestaltet, wenn sie an eine Infrastruktur für Zertifikate angebunden ist.

Wenngleich Windows XP SP2 integrierte Unterstützung für WPA aufweist, muss ein zusätzliches Update installiert werden, um die Unterstützung für IEEE 802.11i WPA2 auf Windows XP SP2-basierten Clients zu ermöglichen. Weitere Informationen über dieses zusätzliche Update sowie Downloadanweisungen finden Sie unter [Wi-Fi Protected Access 2 (WPA2)/Wireless Provisioning Service Information Element (WPS IE) update for Windows XP with Service Pack 2](http://support.microsoft.com/default.aspx?scid=kb;en-us;893357) (Update für Windows XP mit Service Pack 2 und WPA2/WPS IE; in englischer Sprache) unter http://support.microsoft.com/default.aspx?scid=kb;en-us;893357.
[Zum Seitenanfang](#mainsection)  



### Zusammenfassung

Nach Prüfung der zahllosen verfügbaren Lösungen zum Beheben der allseits bekannten Probleme bei älteren Drahtlosnetzwerk-Sicherheitsstandards sowie der Industriestandards, mit denen diese Problembehebungen überflüssig gemacht wurden, ist nun klar, welche Lösung zum Verbessern der Sicherheit von drahtlosen Netzwerken in mittelgroßen Unternehmen verwendet werden soll. Nun können mittelgroße Unternehmen auf effiziente Weise diese wertvolle Technologie implementieren, um die großen Produktivitätsverbesserungen zu nutzen, ohne auf Zuverlässigkeit und Sicherheit verzichten zu müssen. Hierzu findet die Lösung mit WPA- oder WPA2-EAP-TLS mit Zertifikatsdiensten Verwendung, die in diesem Handbuch vorgestellt wird. Nachdem die detaillierten Schritte in diesem Dokument befolgt und die bereitgestellten Tools verwendet wurden, kann ein mittelgroßes Unternehmen eine zuverlässige und sichere Drahtloslösung einsetzen, die nicht nur die Produktivität steigert, sondern auch den ununterbrochenen Betrieb für die Netzwerkendbenutzer sicherstellt.
 

**Download**  


[Dokument „Sichere Konfiguration von drahtlosen Zugriffspunkten“ herunterladen](http://go.microsoft.com/fwlink/?linkid=71716)
 
[Zum Seitenanfang](#mainsection)




