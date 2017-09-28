---
TOCTitle: 'Windows Vista-Sicherheitshandbuch – Übersicht'
Title: 'Windows Vista-Sicherheitshandbuch – Übersicht'
ms:assetid: 'cf32d9c1-61ca-433e-bb3f-b4b20767e9da'
ms:contentKeyID: 20075688
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443745(v=TechNet.10)'
---

Windows Vista-Sicherheitshandbuch
=================================

### Übersicht

Veröffentlicht: 08. Nov 2006

Willkommen beim *Windows Vista-Sicherheitshandbuch*. Dieses Handbuch stellt Ihnen Anweisungen und Empfehlungen bereit, um die Sicherheit der Desktop- und Laptopcomputer zu optimieren, auf denen Windows Vista™ in einer Domäne mit dem Active Directory®-Verzeichnisdienst ausgeführt wird.

Zusätzlich zu den im *Windows Vista-Sicherheitshandbuch* empfohlenen Lösungen enthält das Handbuch Tools, schrittweise Verfahren, Empfehlungen und Prozesse, mit denen der Bereitstellungsvorgang spürbar vereinfacht werden kann. Das Handbuch stellt Ihnen nicht nur einen Leitfaden für wirksame Sicherheitseinstellungen zur Verfügung, sondern bietet auch eine reproduzierbare Methode zum Umsetzen des Leitfadens in Test- und Produktionsumgebungen.

Das wichtigste Tool, das Ihnen vom *Windows Vista-Sicherheitshandbuch* bereitgestellt wird, ist das Skript „GPOAccelerator.wsf“. Mit diesem Tool können Sie ein Skript ausführen, mit dem automatisch alle Gruppenrichtlinienobjekte (GPOs) erstellt werden, die Sie zum Umsetzen dieses Sicherheitsleitfadens benötigen. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.

Entwicklungsteams, Berater, Supporttechniker, Partner und Kunden von Microsoft haben die Informationen in diesem Handbuch geprüft. Daher erfüllt es die folgenden Anforderungen:

-   **Bewährt**. Auf Erfahrungen aus der Praxis beruhend.

-   **Zuverlässig**. Mit aktuellen und nützlichen Informationen.

-   **Präzise**. Technisch geprüft und getestet.

-   **Umsetzbar**. Mit den zur erfolgreichen Umsetzung erforderlichen Schritten.

-   **Relevant**. Sicherheitsprobleme aus der Praxis werden behandelt.

Berater und Systemtechniker entwickeln Best Practices für die Implementierung von Windows Vista, Microsoft® Windows® XP Professional, Windows Server® 2003 und Windows 2000 in einer Vielzahl von Umgebungen. Wenn Sie Windows Vista für Ihre Umgebung bewerten, kann [Windows Vista Readiness Assessment](http://go.microsoft.com/fwlink/?linkid=74708) (VRA) mittelständische Unternehmen dabei unterstützen, die Bereitschaft ihrer Computer für Windows Vista zu bestimmen. VRA erstellt rasch Bestandsaufnahmen von Computern, identifiziert die unterstützten Features von Windows Vista und empfiehlt die geeigneten spezifischen Hardwareupgrades.

Microsoft hat Handbücher für Windows XP mit Service Pack 1 (SP1) und Windows XP mit SP2 veröffentlicht. Dieses Handbuch beschreibt die beträchtlichen Sicherheitsverbesserungen in Windows Vista. Das Handbuch wurde mit Computern entwickelt und getestet, auf denen Windows Vista ausgeführt wird. Dabei wurden sowohl Computer verwendet, die Mitglied einer Domäne mit Active Directory sind, als auch eigenständige Computer.

**Hinweis:**   Alle Verweise auf Windows XP in diesem Handbuch beziehen sich auf Windows XP mit SP2, sofern nicht anders angegeben.

##### Auf dieser Seite

[](#egaa)[Kurzzusammenfassung](#egaa)
[](#efaa)[Zielgruppe dieses Leitfadens](#efaa)
[](#eeaa)[Zusammenfassung der Kapitel](#eeaa)
[](#edaa)[Leitfaden und Tools](#edaa)
[](#ecaa)[Typografische Elemente](#ecaa)
[](#ebaa)[Weitere Informationen](#ebaa)
[](#eaaa)[Danksagungen](#eaaa)

### Kurzzusammenfassung

Unabhängig von Ihrer Umgebung wird dringend empfohlen, dass Sie Sicherheitsfragen ernst nehmen. Viele Unternehmen unterschätzen den Wert von Informationstechnologie (IT). Ein schwerwiegender Angriff auf die Server Ihrer Umgebung kann einen beträchtlichen Schaden für die gesamte Organisation verursachen. Wenn beispielsweise die Clientcomputer in Ihrem Netzwerk mit Malware infiziert werden, könnte Ihr Unternehmen proprietäre Daten verlieren und beträchtliche Kosten aufwenden müssen, um die Clientcomputer wieder in einen sicheren Zustand zu versetzen. Falls in Folge eines Angriffs Ihre Website nicht mehr verfügbar ist, könnte dies zu größeren Einnahmeverlusten und deutlich geringerem Vertrauen der Kunden in Ihr Unternehmen führen.

Durch eine Analyse, bei der Sicherheitsanfälligkeiten, Risiken und Gefährdungsgrad ermittelt werden, können Sie sich darüber informieren, wie es um die Kompromisse zwischen Sicherheit und Funktionalität bestellt ist, die alle Computersysteme in einer vernetzten Umgebung eingehen müssen. Dieses Handbuch beschreibt die wichtigsten sicherheitsbezogenen Gegenmaßnahmen, die in Windows Vista verfügbar sind, die Sicherheitsanfälligkeiten, denen diese Maßnahmen entgegen wirken sollen, sowie die potenziellen negativen Folgen (soweit vorhanden) beim Implementieren der jeweiligen Gegenmaßnahme.

Dieses Handbuch baut auf dem [*Windows XP-Sicherheitshandbuch*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) auf, das spezielle Empfehlungen zum Absichern von Computern enthält, auf denen Windows XP mit SP2 ausgeführt wird. Das *Windows Vista-Sicherheitshandbuch* stellt Empfehlungen zum Absichern von Computern mit einer jeweils spezifischen Sicherheitsbasis für die folgenden zwei Umgebungen bereit:

-   **Unternehmensclient (EC)**. Clientcomputer in dieser Umgebung befinden sich in einer Domäne, die Active Directory verwendet. Sie müssen lediglich mit Systemen kommunizieren, auf denen Windows Server 2003 ausgeführt wird. Die Clientcomputer in dieser Umgebung sind gemischt und führen teilweise Windows Vista und teilweise Windows XP aus. Anweisungen zum Testen und Bereitstellen der Unternehmensclient-Umgebung finden Sie in Kapitel 1, „Implementieren der Sicherheitsbasis“. Informationen zu den grundlegenden Sicherheitseinstellungen, die in dieser Umgebung verwendet werden, finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

-   **Hochsicherheit (SSLF)**. Sicherheit spielt in dieser Umgebung eine so wichtige Rolle, dass ein beträchtlicher Verlust an Funktionalität und Verwaltbarkeit akzeptabel ist. Beispielsweise werden Computer bei militärischen oder nachrichtendienstlichen Einrichtungen in dieser Art von Umgebung betrieben. Auf den Clientcomputern in dieser Umgebung wird nur Windows Vista ausgeführt. Anweisungen zum Testen und Bereitstellen der Hochsicherheitsumgebung finden Sie in Kapitel 5, „Hochsicherheit (SSLF)“. Informationen zu den SSLF-Einstellungen, die in dieser Umgebung verwendet werden, finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

    ![](images/Dd443745.warning(de-de,TechNet.10).gif)**Achtung:**

    Die SSLF-Sicherheitseinstellungen sind nicht für die Mehrzahl der Unternehmen vorgesehen. Die Konfiguration für diese Einstellungen wurde für Organisationen entwickelt, in denen Sicherheit wichtiger als Funktionalität ist.

Der Aufbau des Handbuchs ermöglicht Ihnen das rasche Auffinden der benötigten Informationen. Das Handbuch und die zugehörigen Tools unterstützen Sie bei Folgendem:

-   Bereitstellen und Aktivieren einer Sicherheitsbasis in Ihrer Netzwerkumgebung

-   Identifizieren und Verwenden von Sicherheitsfunktionen in Windows Vista für häufige Sicherheitsszenarien

-   Identifizieren des Zwecks der einzelnen Einstellungen in der jeweiligen Sicherheitsbasis und Verstehen ihrer jeweiligen Bedeutung

Obwohl dieses Handbuch für Unternehmenskunden entworfen wurde, können die meisten Anweisungen für Organisationen jeder Größe angewendet werden. Zur optimalen Nutzung dieser Unterlagen empfiehlt es sich, das gesamte Handbuch zu lesen. Allerdings ist es möglich, einzelne Abschnitte des Handbuchs zu lesen, um bestimmte Ziele zu erreichen. Der Abschnitt „Zusammenfassung der Kapitel“ in diesem Überblick enthält eine knappe Einführung in den Inhalt des Handbuchs. Weitere Informationen zu Sicherheitsthemen und -einstellungen für Windows XP finden Sie im [*Windows XP-Sicherheitshandbuch*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) und dem zugehörigen Handbuch mit der Bezeichnung [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10)).

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zielgruppe dieses Leitfadens

Das *Windows* *Vista-Sicherheitshandbuch* ist in erster Line für Allroundtalente im IT-Bereich, Sicherheitsspezialisten, Netwerkarchitekten und andere IT-Experten und -Berater vorgesehen, welche die Entwicklung von Anwendungen oder Infrastruktur sowie die Bereitstellung von Windows Vista auf Desktop- und Laptopclientcomputern in einer Unternehmensumgebung planen. Das Handbuch ist nicht für Heimanwender vorgesehen. Dieses Handbuch richtet sich an Personen, die folgende Tätigkeiten ausführen:

-   **Allroundtalent im IT**-**Bereich**. Benutzer in dieser Rolle kümmern sich um alle Fragen der Sicherheit in Unternehmen mit 50 bis 500 Clientcomputern. Für Allroundtalente im IT-Bereich ist es besonders wichtig, dass sie die Computer, für die sie zuständig sind, schnell und einfach sichern können.

-   **Sicherheitsspezialist**. Benutzer in dieser Rolle beschäftigen sich schwerpunktmäßig damit, innerhalb eines Unternehmens plattformübergreifende Sicherheit zu gewährleisten. Sicherheitsspezialisten benötigen ein zuverlässiges Referenzhandbuch, das die Sicherheitsanforderungen auf jeder Stufe des Unternehmens behandelt. Zudem müssen dort Best Practices zum Implementieren von Sicherheitsmaßnahmen bereitgestellt werden. Sicherheitsspezialisten identifizieren Sicherheitsfunktionen und -einstellungen und stellen ihren Kunden dann Empfehlungen zu deren optimaler Verwendung in Hochrisiko-Umgebungen zur Verfügung.

-   **Für IT-Abläufe,** **Helpdeskund Bereitstellung zuständige Mitarbeiter**. Mitarbeiter im Bereich der IT-Abläufe kümmern sich vor allem um die Integration von Sicherheitsfunktionen und die Steuerung von Änderungen beim Bereitstellungsprozess, während sich das Bereitstellungspersonal in erster Linie mit dem schnellen Verwalten von Sicherheitsupdates beschäftigt. Benutzer in diesen Rollen beheben auch Sicherheitsprobleme, die auf Anwendungen zurückzuführen sind. Diese Tätigkeit umfasst das Installieren, Konfigurieren und Verbessern der Verwendbarkeit und Verwaltbarkeit von Software. Zudem überwachten diese Personen die verschiedenen Problemtypen, um messbare Sicherheitsverbesserungen und möglichst geringe Auswirkungen auf wichtige Unternehmensanwendungen zu gewährleisten.

-   **Netzwerkarchitekt- und -planer**. Benutzer in diesen Rollen beschäftigen sich mit der Netzwerkarchitektur für die Computer in ihren Unternehmen.

-   **Berater**. Benutzer in dieser Rolle arbeiten in Unternehmen mit einer Größe von 50 bis 5.000 oder mehr Clientcomputern. IT-Berater kennen sich mit vielen Arten von Sicherheitsszenarien aus, die alle Geschäftsebenen eines Unternehmens umfassen. IT-Berater sowohl von Microsoft Services als auch von Partner nutzen Tools zur Wissensvermittlung für Partner und Unternehmenskunden.

-   **Wirtschaftsanalytiker und Geschäftsführer (BDM)**. Benutzer in diesen Rollen haben wichtige Unternehmensziele und -anforderungen, die IT-Desktop- oder Laptopsupport benötigen.

**Hinweis**:   Benutzer, die die Anleitungen in diesem Handbuch anwenden möchten, müssen mindestens die Schritte zum Einrichten der Unternehmensclient-Umgebung in Kapitel 1, „Implementieren der Sicherheitsbasis“, lesen und ausführen.

#### Fähigkeiten und Bereitschaft

Für die Zielgruppe dieses Handbuchs, also Personen, die unter Windows Vista ausgeführte Clientcomputer in Unternehmen entwickeln, bereitstellen und sichern, sind die folgenden Kenntnisse und Fähigkeiten erforderlich:

-   MCSE zu Windows Server 2003 oder eine höhere Zertifizierung sowie zwei oder mehr Jahre Erfahrung mit sicherheitsbezogenen Aufgaben oder gleichwertige Kenntnisse

-   Eingehende Kenntnisse über die Domänen- und Active Directory-Umgebungen des Unternehmens

-   Erfahrung mit der Gruppenrichtlinien-Verwaltungskonsole (GPMC)

-   Erfahrung mit der Verwaltung von Gruppenrichtlinien mithilfe der GPMC, die eine zentrale Lösung für das Verwalten aller Aufgaben in Zusammenhang mit Gruppenrichtlinien zur Verfügung stellt

-   Erfahrung mit der Verwendung von Verwaltungstools einschließlich der Microsoft Management Console (MMC) sowie von Gpupdate und Gpresult

-   Erfahrung im Bereitstellen von Anwendungen und Clientcomputern in Unternehmensumgebungen

#### Zweck des Handbuchs

Das Handbuch soll Ihnen in erster Linie Folgendes ermöglichen:

-   Verwenden der Anleitung zum effizienten Erstellen und Anwenden von getesteten Konfigurationen für die Sicherheitsbasis mithilfe von Gruppenrichtlinien.

-   Verstehen der Gründe für empfohlene Sicherheitseinstellungen in den Konfigurationen der Sicherheitsbasis in diesem Handbuch und deren Auswirkungen.

-   Identifizieren und Berücksichtigen häufiger Sicherheitsszenarien und Verwenden spezifischer Sicherheitsfunktionen in Windows Vista, um Sie bei deren Verwaltung in Ihrer Umgebung zu unterstützen.

Das Handbuch ist so aufgebaut, dass Sie die Möglichkeit haben, nur die Teile zu nutzen, die für die Sicherheitsanforderungen Ihres Unternehmens relevant sind. Allerdings empfiehlt es sich, das gesamte Handbuch zu lesen, um optimal davon profitieren zu können.

#### Umfang des Handbuchs

Dieses Handbuch beschäftigt sich mit dem Erstellen und Verwalten einer sicheren Umgebung für Desktop- und Laptopcomputer, auf denen Windows Vista ausgeführt wird. Das Handbuch erklärt die verschiedenen Phasen bei der Absicherung zweier verschiedener Umgebungen sowie den Zweck jeder einzelnen Sicherheitseinstellung für die Desktop- und Laptopcomputer, die in der jeweiligen Umgebung bereitgestellt werden. Darüber hinaus stellt das Handbuch Anweisungen und Sicherheitsempfehlungen zur Verfügung.

Auf den Clientcomputern in der Unternehmensclient-Umgebung kann entweder Windows XP oder Windows Vista ausgeführt werden. Allerdings muss auf den Computern, die diese Clientcomputer im Netzwerk verwalten, Windows Server 2003 R2 oder Windows Server 2003 mit SP1 ausgeführt werden. Auf den Clientcomputern in der Hochsicherheitsumgebung darf nur Windows Vista ausgeführt werden.

Das Handbuch umfasst lediglich die Sicherheitseinstellungen, die im empfohlenen Betriebssystem verfügbar sind. Eine gründliche Besprechung aller Sicherheitseinstellungen in Windows Vista finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10)).

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zusammenfassung der Kapitel

Das *Windows* *Vista-Sicherheitshandbuch* besteht aus fünf Kapiteln und einem Anhang, in dem Sie Beschreibungen von Einstellungen, Überlegungen und Werte finden. Die Datei „Windows Vista Security Guide Settings.xls“, die diesem Handbuch beigefügt ist, ermöglicht Ihnen zudem das Vergleichen von Einstellungswerten. Die folgende Abbildung zeigt die Struktur des Handbuchs. Sie soll Ihnen helfen, sich über die optimale Vorgehensweise zur Implementierung und Bereitstellung der hier enthaltenen Anleitungen zu informieren.

![](images/Dd443745.VSGOver(de-de,TechNet.10).gif)
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443745.vsgover_big(de-de,technet.10).gif)

#### Übersicht

In diesem Überblick erhalten Sie Informationen zu Zweck und Umfang des Handbuchs sowie zur Zielgruppe. Außerdem wird der Aufbau des Handbuchs beschrieben, damit Sie rasch die benötigten Informationen finden. Zudem werden die zum Handbuch gehörenden Tools und Vorlagen beschrieben sowie die Voraussetzungen, die Benutzer zur Durchführung der Anleitungen erfüllen sollten. Es folgen kurze Beschreibungen der einzelnen Kapitel und des Anhangs.

#### Kapitel 1: Implementieren der Sicherheitsbasis

In diesem Kapitel werden die Vorteile beschrieben, die Unternehmen durch das Erstellen und Bereitstellen einer Sicherheitsbasis nutzen können. Das Kapitel umfasst Anweisungen und Prozesse zum Implementieren der Einstellungen für die EC-Sicherheitsbasis sowie Sicherheitsanweisungen.

Zu diesem Zweck enthält das Kapitel Anweisungen, in denen die Verwendung des Skripts „GPOAccelerator.wsf“ in Verbindung mit der Gruppenrichtlinien-Verwaltungskonsole (GPMC) zum Erstellen, Testen und Bereitstellen von Organisationseinheiten (OUs) und Gruppenrichtlinienobjekten (GPOs) beschrieben wird, um diese Umgebung einzurichten. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.

#### Kapitel 2: Schutz gegen Malware

Dieses Kapitel stellt Empfehlungen zur Nutzung von neuen und verbesserten Sicherheitsfunktionen in Windows Vista bereit, um Clientcomputer und Unternehmensressourcen besser vor Malware zu schützen, etwa vor Viren, Würmern und trojanischen Pferden. Das Kapitel enthält Informationen zur effizientesten Nutzung der folgenden Technologien im Betriebssystem:

-   Benutzerkontensteuerung (UAC)

-   Windows Defender

-   Windows-Firewall

-   Windows-Sicherheitscenter

-   Tool zum Entfernen bösartiger Software

-   Richtlinien für Softwareeinschränkungen

Außerdem enthält das Kapitel die folgenden Informationen zu Sicherheitstechnologien in Internet Explorer 7:

-   Geschützter Modus von Internet Explorer

-   ActiveX-Auswahlmöglichkeit

-   Schutz vor domänenübergreifenden Skriptangriffen

-   Sicherheitsstatusleiste

-   Phishingfilter

-   Zusätzliche Sicherheitsfunktionen

#### Kapitel 3: Schutz von vertraulichen Daten

Dieses Kapitel stellt Empfehlungen und Informationen zu Best Practices dazu bereit, wie Computer mit Verschlüsselungs- und Zugriffssteuerungstechnologien in Windows Vista besser geschützt werden können. Diese Technologien sind besonders für Umgebungen mit mobilen Computern wichtig, in denen die Gefahr größer ist, dass ein Gerät mit Windows Vista verloren geht oder gestohlen wird.

Das Kapitel enthält Informationen zur effizientesten Nutzung der folgenden Technologien in Windows Vista:

-   BitLocker™-Laufwerkverschlüsselung

-   Verschlüsselndes Dateisystem (EFS)

-   Dienste für die Windows-Rechteverwaltung (RMS)

-   Gerätesteuerung

#### Kapitel 4: Anwendungskompatibilität

Dieses Kapitel enthält Empfehlungen zur Verwendungsweise der neuen und verbesserten Sicherheitsfunktionen und -einstellungen in Windows Vista, ohne dass dadurch die Funktionalität vorhandener Anwendungen in Ihrer Umgebung beeinträchtigt wird. Das Kapitel umfasst die folgenden Inhalte:

-   Überblick über potenzielle Probleme mit der Anwendungskompatibilität

-   Bereitstellen von zwei einfachen Testverfahren für die Anwendungskompatibilität mit Windows Vista

-   Bereitstellen von potenziellen Strategien zur Verminderung von Kompatibilitätsproblemen, Konfigurationen und Anweisungen

-   Verweis auf andere Ressourcen, die Sie zum weiteren Bestimmen der Anwendungskompatibilität mit Windows Vista heranziehen können

#### Kapitel 5: Hochsicherheit (SSLF)

Dieses Kapitel enthält eine Erklärung der Hochsicherheitsumgebung und der großen Unterschiede zwischen dieser Umgebung und der Unternehmensclient-Umgebung. Das Kapitel stellt Anweisungen und Prozesse zum Implementieren der Einstellungen für die SSLF-Sicherheitsbasis sowie Sicherheitsanweisungen bereit. Es enthält Anweisungen, in denen erläutert wird, wie Sie die Gruppenrichtlinien-Verwaltungskonsole mithilfe eines Skripts optimal einsetzen können, um zum Einrichten dieser Umgebung Organisationseinheiten und Gruppenrichtlinienobjekte zu erstellen, zu testen und bereitzustellen.

![](images/Dd443745.warning(de-de,TechNet.10).gif)**Achtung:**

Die Anleitungen in diesem Kapitel ermöglichen Ihnen die Einrichtung der Hochsicherheitsumgebung, die sich grundlegend von der Unternehmensclient-Umgebung unterscheidet, die in Kapitel 1, „Implementieren der Sicherheitsbasis“, beschrieben wird. Die Anleitungen in diesem Kapitel sind nur für Hochsicherheitsumgebungen vorgesehen und stellen keine Ergänzung zu den Anleitungen in Kapitel 1 dar.

#### Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen

Der Anhang enthält Beschreibungen und Tabellen, in denen die vorgeschriebenen Einstellungen für die jeweilige EC- und SSLF-Sicherheitsbasis für das Handbuch beschrieben werden. Der Anhang beschreibt jede Einstellung und den Grund für deren Konfiguration oder Wert. Der Anhang enthält zudem Informationen zu Unterschieden bei den Einstellungen zwischen Windows Vista und Windows XP.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Leitfaden und Tools

Dieser Solution Accelerator enthält mehrere Dateien wie „Windows Vista Security Guide.doc“, Anhang A von „Windows Vista Security Guide.doc“, „Windows Vista Security Guide Settings.xls“ und das Tool GPOAccelerator, um Sie bei der einfachen Implementierung dieses Leitfadens zu unterstützen. Nachdem Sie die englische Version des [*Windows Vista Security Guide*](http://go.microsoft.com/fwlink/?linkid=74028) im Microsoft Download Center heruntergeladen haben, installieren Sie diese Ressourcen mit der MSI-Datei (Microsoft Windows Installer) im gewünschten Verzeichnis auf Ihrem Computer.

**Hinweis**:   Wenn Sie die Installation des *Windows Vista-Sicherheitshandbuchs* starten, wird das Tool GPOAccelerator standardmäßig mit den anderen Leitfäden für die Installation ausgewählt, die diesem Tool beigefügt sind. Für die Verwendung des Tools sind Administratorrechte erforderlich. Der Solution Accelerator wird standardmäßig im Ordner „Dokumente“ gespeichert. Bei der Installation wird eine Verknüpfung mit dem Handbuch erstellt, die den Ordner mit dem Windows Vista-Sicherheitshandbuch öffnet.

Sie können die Tools und Vorlagen für beide in diesem Handbuch definierten Sicherheitsbasiskonfigurationen mithilfe der Gruppenrichtlinien-Verwaltungskonsole (GPMC) anwenden. Die Kapitel „Implementieren der Sicherheitsbasis“ und „Hochsicherheit (SSLF)“ beschreiben die Verfahren, die zum Ausführen dieser Aufgaben erforderlich sind.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Typografische Elemente

In diesem Handbuch werden die folgenden typografischen Konventionen verwendet.

**Tabelle 1.1 Typografische Konventionen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Element</th>
<th>Bedeutung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Fett</strong></td>
<td style="border:1px solid black;">Dies bedeutet, dass Zeichen genau wie dargestellt eingegeben werden, einschließlich Befehle, Switches und Dateinamen. Elemente der Benutzeroberfläche werden fett dargestellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>Kursiv</em></td>
<td style="border:1px solid black;">Titel von Büchern und anderen maßgeblichen Veröffentlichungen werden <em>kursiv</em> dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>&lt;Kursiv&gt;</em></td>
<td style="border:1px solid black;">Kursiv dargestellte und in spitze Klammern gesetzte Platzhalter &lt; <em>Dateiname</em>&gt; stellen Variablen dar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Schriftart mit fester Breite</td>
<td style="border:1px solid black;">So werden Code- und Skriptbeispiele dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Hinweis</strong></td>
<td style="border:1px solid black;">Weist den Leser auf zusätzliche Informationen hin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Wichtig</strong></td>
<td style="border:1px solid black;">Ein wichtiger Hinweis enthält Informationen, die für die Ausführung einer Aufgabe von hoher Bedeutung sind.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"> 
<img src="images/Dd443745.warning(de-de,TechNet.10).gif" /><strong>Achtung:</strong></td>
<td style="border:1px solid black;">Der Leser wird auf wichtige ergänzende Informationen hingewiesen, die nicht ignoriert werden sollten.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">‡</td>
<td style="border:1px solid black;">Dieses Symbol bezeichnet spezielle Änderungen von Gruppenrichtlinieneinstellungen oder Empfehlungen hierzu.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">§</td>
<td style="border:1px solid black;">Dieses Symbol bezeichnet Gruppenrichtlinieneinstellungen, die in Windows Vista neu sind.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Weitere Informationen
  
Die folgenden Links stellen zusätzliche Informationen zu Sicherheitsthemen sowie eine eingehende Behandlung der Konzepte und Sicherheitsvorgaben in diesem Handbuch zur Verfügung:
  
-   [*Microsoft Windows Sicherheit - Die technische Referenz*](http://www.edv-buchversand.de/mspress/product.asp?cnt=product&id=ms-981&lng=0)
  
-   [*Microsoft Windows Server 2003 - Die technische Referenz*](http://www.edv-buchversand.de/mspress/product.asp?cnt=product&id=ms-936&lng=0)
  
-   [Microsoft TechNet – Sicherheitsthemen](http://www.microsoft.com/germany/technet/sicherheit/themen/default.mspx)
  
-   [*Bedrohungen und Gegenmaßnahmen*](https://technet.microsoft.com/de-de/library/5289ecb9-b6a3-4c58-8832-3774bdb04053(v=TechNet.10))
  
-   [*Windows Server 2003-Sicherheitshandbuch*](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))
  
-   [Windows Vista Readiness Assessment](http://go.microsoft.com/fwlink/?linkid=74708) (engl.)
  
-   [*Windows XP Professional Resource Kit*](http://www.microsoft.com/germany/technet/prodtechnol/winxppro/reskit/default.mspx)
  
-   [*Windows XP-Sicherheitshandbuch*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))
  
#### Support und Feedback
  
Das SASC-Team (Solution Accelerators – Security and Compliance) würde sich über Ihre Rückmeldung zu diesem und anderen Solution Accelerators freuen.
  
Bitte tragen Sie Ihre Anmerkungen in der Newsgroup [Discussions in Security](http://windowshelp.microsoft.com/communities/newsgroups/en-us/default.mspx?dg=microsoft.public.windows.vista.security&lang=en&cr=us&r=9dcac6a3-b8e7-4ba3-aa06-4e38b8ee9f35) (Diskussionen zur Sicherheit, nur in englischer Sprache verfügbar) auf der Windows Vista-Website für Hilfe und Support ein.
  
Sie können Ihr Feedback auch per E-Mail an folgende Adresse senden: [secwish@microsoft.com](mailto:secwish@microsoft.com?subject=windows%20vista%20security%20guide).
  
Wir freuen uns auf Ihre Rückmeldung.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Danksagungen
  
Das SASC-Team (Solution Accelerators – Security and Compliance) möchte dem für die Entwicklung des *Windows Vista-Sicherheitshandbuch* zuständigen Team danken. Die folgenden Personen waren entweder unmittelbar beteiligt oder lieferten wichtige Beiträge zum Erstellen, Entwickeln und Testen dieser Lösung.
  
#### Entwicklungsteam
  
**Autoren und Experten**
  
José Maldonado
  
Mike Danseglio
  
Michael Tan
  
Richard Harrison, *Content Master Ltd*
  
David Coombes, *Content Master Ltd*
  
Jim Captainino, *Content Master Ltd*
  
Richard Hicks, *QinetiQ*
  
**Tester**
  
Gaurav Bora
  
Vikrant Minhas, *Infosys Technologies Ltd*
  
Sumit Parikh, *Infosys Technologies Ltd*
  
Dharani Mohanam, *Infosys Technologies Ltd*
  
Swapna Jagannathan, *Infosys Technologies Ltd*
  
Prashant Japkar, *Infosys Technologies Ltd*
  
**Redakteure**
  
John Cobb, *Wadeware LLC*
  
Jennifer Kerns, *Wadeware LLC*
  
Steve Wacker, *Wadeware LLC*
  
**Programm-Manager**
  
Kelly Hengesteg
  
Audrey Centola, *Volt Information Sciences*
  
Neil Bufton, *Content Master Ltd*
  
**Produktmanager**
  
Jim Stewart
  
Alain Meeus
  
Tony Bailey
  
Kevin Leo, *Excell Data Corporation*
  
**Release-Manager**
  
Karina Larson
  
Gareth Jones
  
#### Autoren und Reviewer
  
**Microsoft**
  
Charles Denny, Ross Carter,
  
Derick Campbell, Chase Carpenter
  
Karl Grunwald, Mike Smith-Lonergan
  
Don Armstrong, Bob Drake
  
Eric Fitzgerald, Emily Hill
  
George Roussos, David Abzarian
  
Darren Canavor, Nils Dussart
  
Peter Waxman, Russ Humphries
  
Sarah Wahlert, Tariq Sharif
  
Ned Pyle, Bomani Siwatu
  
Kiyoshi Watanabe, Eric Lawrence
  
David Abzarian, Chas Jeffries
  
Vijay Bharadwaj, Marc Silbey
  
Sean Lyndersay, Chris Corio
  
Matt Clapham, Tom Daemen
  
Sanjay Pandit, Jeff Williams
  
Alex Heaton, Mike Chan
  
Bill Sisk, Jason Joyce
  
**Extern**
  
Mehul Mediwala, *Infosys Technologies Ltd*
  
**Hinweise**  
Auf Anregung von Microsoft beteiligte sich das National Security Agency Information Assurance Directorate an der Prüfung dieses Microsoft-Sicherheitshandbuchs und stellte Anmerkungen zur Verfügung, die in die veröffentlichte Version aufgenommen wurden.  
Das United States Department of Commerce National Institute of Standards and Technology (NIST) beteiligt sich ebenfalls an der Prüfung dieses Microsoft-Sicherheitshandbuchs und stellte Anmerkungen zur Verfügung, die in die veröffentlichte Version aufgenommen wurden.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
##### In diesem Beitrag
  
-   Übersicht  
-   [Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)  
-   [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)  
-   [Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)  
-   [Kapitel 4: Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)  
-   [Kapitel 5: Hochsicherheit (SSLF)](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx)  
-   [Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/security_group_policy_settings.mspx)
  
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
<td style="border:1px solid black;">1 von 7 <a href="http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx"><img src="images/Dd443745.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
