---
TOCTitle: 'Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP'
Title: 'Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP'
ms:assetid: '4eddb4e4-fd7b-444c-8484-bb8ee220c0e1'
ms:contentKeyID: 20072361
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc163069(v=TechNet.10)'
---

Windows XP-Sicherheitshandbuch
==============================

### Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP

Aktualisiert: 20.10.2005

##### Auf dieser Seite

[](#ehaa)[Überblick](#ehaa)  
[](#egaa)[Kurzzusammenfassung](#egaa)  
[](#efaa)[Zielgruppe](#efaa)  
[](#eeaa)[Themenumfang dieses Handbuchs](#eeaa)  
[](#edaa)[Kapitelüberblick](#edaa)  
[](#ecaa)[Inhalt des Downloads](#ecaa)  
[](#ebaa)[Typografische Elemente](#ebaa)  
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Willkommen beim *Sicherheitshandbuch für Windows XP*. Dieses Handbuch bietet die aktuell verfügbaren Informationen zur Beurteilung und Abwehr von Sicherheitsrisiken, die in Ihrer Umgebung für Microsofts® Windows® XP Professional mit Service Pack 2 (SP2) bestehen. Die Kapitel in diesem Handbuch enthalten ausführliche Informationen zur Konfiguration erweiterter Sicherheitseinstellungen und -funktionen in Windows XP zur Abwehr von erkannten Risiken in Ihrer Umgebung. Dieses Handbuch wurde insbesondere für Berater, Designer oder Systemtechniker konzipiert, die in einer Windows XP-Umgebung arbeiten.

Entwicklungsteams, Berater, Supporttechniker, Partner und Kunden von Microsoft haben die Informationen in diesem Handbuch geprüft. Das Handbuch ist deshalb:

-   **Bewährt**. Auf Erfahrungen aus der Praxis beruhend.

-   **Zuverlässig**. Mit aktuellen und nützlichen Informationen.

-   **Korrekt**. Technisch geprüft und getestet.

-   **Nachvollziehbar**. Mit den zur erfolgreichen Umsetzung erforderlichen Schritten.

-   **Relevant**. Sicherheitsprobleme aus der Praxis werden behandelt.

Berater und Systemtechniker, die Windows XP Professional, Microsoft Windows Server™ 2003 und Windows 2000 in einer Vielzahl von Umgebungen implementiert haben, haben empfohlene Vorgehensweisen entwickelt, um sowohl Client- als auch Servercomputer abzusichern. Außerdem werden schrittweise Sicherheitsanweisungen, -verfahren und -empfehlungen bereitgestellt, mit denen Sie die Sicherheit für Computer in Ihrer Organisation maximieren können, auf denen Windows XP Professional mit SP2 ausgeführt wird.

Ausführliche Erläuterungen der Konzepte, auf denen diese Informationen beruhen, finden Sie in: *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server 2003 und Windows* *XP*, im *Microsoft Windows* *XP Resource Kit*, im *Microsoft Windows* *Server 2003 Resource Kit*, im *Microsoft Windows Security Resource Kit* und in Microsoft TechNet.

Dieses Handbuch wurde ursprünglich für Windows XP mit SP1 erstellt. Diese aktualisierte Version spiegelt die bedeutenden Sicherheitsverbesserungen wider, die Windows XP mit SP2 bietet. Sie wurde mit Computern geprüft und entwickelt, auf denen Windows XP Professional mit SP2 ausgeführt wird. Alle Verweise auf Windows XP in diesem Handbuch beziehen sich, wenn nicht anders angegeben, auf Windows XP mit SP2.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Kurzzusammenfassung

Unabhängig von Ihrer Arbeitsumgebung müssen Sicherheitsangelegenheiten unbedingt ernst genommen werden. Viele Organisationen unterschätzen den Wert ihrer IT-Umgebung. Dies hängt oft damit zusammen, dass erhebliche indirekte Kosten nicht berücksichtigt werden. Ein schwerwiegender Angriff auf die Server Ihrer Umgebung kann einen beträchtlichen Schaden für die gesamte Organisation verursachen. Ein Angriff, aufgrund dessen z. B. Ihre Website nicht mehr verfügbar ist und der dadurch zu erheblichen finanziellen Einbußen oder einem verringerten Kundenvertrauen führt, kann u. U. die gesamte Wirtschaftlichkeit des Unternehmens aufs Spiel setzen. Bei der Bewertung von Sicherheitskosten sollten Sie daher die indirekten Kosten, die mit einem Angriff verbunden sind, sowie die durch einen Ausfall Ihrer IT-Funktionen verursachten Kosten in die Kalkulation einbeziehen.

Durch eine Analyse der Schwachstellen, der Risiken und der Angriffspunkte Ihrer Umgebung erhalten Sie eine Vorstellung von der Abwägung zwischen Sicherheit und Benutzerfreundlichkeit, die in einer Netzwerkumgebung für alle Computersysteme erforderlich ist. In diesem Handbuch werden die wichtigsten sicherheitsbezogenen Gegenmaßnahmen in Windows XP mit SP2, die entsprechenden Sicherheitsrisiken und ggf. mögliche negative Folgen der Implementierung der einzelnen Gegenmaßnahmen behandelt.

Das Handbuch bietet spezifische Empfehlungen zum Absichern von Computern, auf denen Windows XP mit SP2 in drei häufig anzutreffenden Umgebungen ausgeführt wird:

-   **Unternehmensclient (EC).** Clientcomputer in dieser Umgebung befinden sich in einer Active Directory®-Verzeichnisdienstdomäne und müssen nur mit Systemen kommunizieren, auf denen Windows 2000 oder spätere Versionen des Windows-Betriebssystems ausgeführt werden.

-   **Eigenständig (SA).** Clientcomputer in dieser Umgebung sind nicht Mitglied einer Active Directory-Domäne und müssen ggf. mit Systemen kommunizieren, auf denen Windows NT® 4.0 ausgeführt wird.

-   **Hochsicher (SSLF).** In dieser Umgebung ist die Sicherheit so wichtig, dass ein Verlust an Funktionalität und Handhabbarkeit des Systems akzeptabel ist. Zum Beispiel werden Computer des Militärs und des Nachrichtendienstes in dieser Art Umgebung betrieben.

Die Gliederung dieses Handbuchs ermöglicht den einfachen und schnellen Zugriff auf wichtige Informationen zum Bestimmen der Einstellungen, die für die Computer in Ihrer Organisation geeignet sind, auf denen Windows XP mit SP2 ausgeführt wird. Auch wenn diese Anleitung für Kunden in Unternehmen gedacht ist, sind viele der Informationen für Organisationen jeder Größe geeignet.

Zur optimalen Nutzung dieser Unterlagen empfiehlt es sich, das gesamte Handbuch zu lesen. Das für dieses Handbuch verantwortliche Team hofft, dass die vorliegenden Informationen für Sie hilfreich, informativ und interessant sind. Weitere Informationen finden Sie außerdem im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx heruntergeladen werden kann.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Zielgruppe

Dieses Handbuch richtet sich in erster Linie an Berater, Sicherheitsspezialisten, Systemarchitekten und IT-Fachleute, die für die Planungsphasen der Anwendungs- bzw. Infrastrukturentwicklung und -bereitstellung von Windows XP-Arbeitsstationen in einer Unternehmensumgebung verantwortlich sind. Dieses Handbuch ist nicht für den privaten Benutzer gedacht. Das vorliegende Handbuch ist für Personen mit den folgenden Aufgabenbereichen ausgelegt:

-   Systemarchitekten und -planer, die für die Entwicklung der Architektur von Computern in ihren Unternehmen verantwortlich sind.

-   IT-Sicherheitsspezialisten, die mit plattformübergreifenden Sicherheitsaufgaben innerhalb einer Organisation befasst sind.

-   Unternehmensanalysten und geschäftliche Entscheidungsträger, in deren Verantwortungsbereich wichtige Unternehmensziele und -anforderungen fallen, die IT-Desktop- oder Laptopsupport benötigen.

-   Berater von Microsoft Services und von Partnern, die Tools zur Wissensvermittlung für Partner und Unternehmenskunden suchen.

#### Fertigkeiten

Die folgenden Kenntnisse und Fertigkeiten sind eine Grundvoraussetzung für Administratoren oder Systemarchitekten, die für die Entwicklung, Bereitstellung und den Schutz von Windows XP-Clientcomputern in einem Unternehmen verantwortlich sind.

-   MCSE 2000-Zertifizierung (Microsoft Certified Systems Engineer) oder höher mit mehr als 2 Jahren Erfahrung im Bereich Sicherheit (oder gleichwertig).

-   Fundierte Kenntnisse von Domänen- und Active Directory-Umgebungen in der Organisation.

-   Erfahrung im Umgang mit Verwaltungstools einschließlich MMC, Secedit, Gpupdate und Gpresult.

-   Erfahrung im Verwalten von Gruppenrichtlinien.

-   Erfahrung im Bereitstellen von Anwendungen und Clientcomputern in Unternehmensumgebungen.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Themenumfang dieses Handbuchs

Dieses Handbuch konzentriert sich auf die Erstellung und Verwaltung einer sicheren Umgebung für Desktops und Laptops, auf denen Windows XP Professional mit SP2 ausgeführt wird. Im Handbuch werden die verschiedenen Stufen der Sicherung von drei unterschiedlichen Umgebungen sowie die Auswirkungen jeder Einstellung auf die Desktop- und Laptopcomputer in der jeweiligen Umgebung erläutert. Die bereitgestellten Informationen betreffen die Umgebungen Unternehmensclient (EC), Eigenständig (SA) und Hochsicher (SSLF).

Einstellungen, die nicht ausdrücklich als Teil dieses Handbuchs empfohlen sind, sind nicht dokumentiert. Eine ausführliche Erläuterung aller Sicherheitseinstellungen in Windows XP finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx) unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx.

#### Unternehmensclient

Die Unternehmensclientumgebung besteht aus einer Active Directory-Domäne unter Windows 2000 oder Windows Server 2003. Die Clientcomputer in dieser Umgebung werden mithilfe von Gruppenrichtlinien verwaltet, die auf Sites, Domänen und Organisationseinheiten angewendet werden. Gruppenrichtlinien stellen eine zentralisierte Methode zum Verwalten von Sicherheitsrichtlinien in der gesamten Umgebung dar.

#### Umgebung mit eigenständigen Clients

Die Umgebung mit eigenständigen Clients enthält Clientcomputer, die nicht zu einer Domäne oder Computern hinzugefügt werden können, die Mitglied einer Windows NT 4.0-Domäne sind. Diese Clientcomputer müssen mithilfe von lokalen Richtlinieneinstellungen konfiguriert werden. Die Verwaltung eigenständiger Computer kann eine beträchtlich größere Herausforderung darstellen als die Verwaltung von Benutzerkonten und -richtlinien in einer Active Directory-Domäne.

#### Hochsicher (SSLF)

Die Hochsicherheitsumgebung bietet erhöhte Sicherheitseinstellungen für Clientcomputer. Wenn diese Einstellungen für Sicherheitsrichtlinien angewendet werden, kann die Benutzerfunktionalität deutlich verringert sein, da sie auf die spezifischen Funktionen beschränkt ist, die für die notwendigen Aufgaben erforderlich sind. Der Zugriff wird auf genehmigte Anwendungen, Dienste und Infrastrukturumgebungen beschränkt. Die Einstellungen für Sicherheitsrichtlinien für die Hochsicherheitsumgebung gelten nur für ein paar Systeme in einer sehr geringen Anzahl von Organisationen, z. B. das Militär und Nachrichtendienste. Bei diesen Einstellungen hat die Sicherheit Vorrang vor Verwaltbarkeit und Benutzerfreundlichkeit. Sie sollten nur auf Computern verwendet werden, deren Kompromittierung einen beträchtlichen finanziellen Verlust oder den Verlust von Menschenleben verursachen könnte. In anderen Worten: die Hochsicherheitseinstellungen sind für die meisten Organisationen keine gute Wahl.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Kapitelüberblick

Windows XP mit SP2 stellt bislang die zuverlässigste Version eines Windows-Clientbetriebssystems mit verbesserten Sicherheits- und Datenschutzfeatures dar. Die allgemeine Sicherheit wurde in Windows XP verbessert, um Ihrer Organisation die Arbeit in einer sicheren Computerumgebung zu ermöglichen. Das *Windows* *XP-Sicherheitshandbuch* umfasst sieben Kapitel. In den Kapiteln zwei bis sechs werden die Vorgehensweisen erläutert, die zum Erstellen einer solchen Umgebung erforderlich sind. Jedes dieser Kapitel basiert auf einem abgeschlossenen Verfahren, mit dem auf Windows XP basierende Computer geschützt werden sollen.

#### Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP

Dieses Kapitel enthält einen Überblick über das Handbuch, einschließlich einer Beschreibung der Zielgruppe, der im Handbuch beschriebenen Probleme und der allgemeinen Zielsetzung.

#### Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory

Zur Verwaltung von Benutzer- und Computerumgebungen in Windows Server 2003- und Windows 2000-Domänen können Gruppenrichtlinien verwendet werden. Gruppenrichtlinien sind ein wesentliches Tool für die Sicherheit von Windows XP und können zum zentralen Anwenden und Verwalten einheitlicher Sicherheitsrichtlinien für das gesamte Netzwerk verwendet werden. In diesem Kapitel werden die vorbereitenden Schritte erläutert, die in Ihrer Domäne durchgeführt werden müssen, bevor Sie Gruppenrichtlinien auf Ihre Windows XP-Clientcomputer anwenden.

Die Gruppenrichtlinieneinstellungen werden in Gruppenrichtlinienobjekten (GPOs) auf Domänencontrollern gespeichert. Gruppenrichtlinienobjekte sind mit Sites, Domänen und Organisationseinheiten innerhalb der Active Directory-Struktur verknüpft. Da Gruppenrichtlinien eng in Active Directory integriert sind, ist vor ihrer Implementierung eine grundlegende Kenntnis der Active Directory-Struktur und der Sicherheitsimplikationen erforderlich.

#### Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients

In diesem Kapitel werden die Sicherheitseinstellungen für Windows XP-Clientcomputer beschrieben, die in einer Windows 2000 oder Windows Server 2003 Active Directory-Domäne mithilfe von Gruppenrichtlinien eingerichtet werden können. Nicht für alle verfügbaren Einstellungen werden Anleitungen bereitgestellt – es werden nur solche Einstellungen angeboten, die eine Umgebung vor den meisten aktuellen Bedrohungen schützen. Die Anleitung erlaubt Benutzern auch, weiterhin typische Aufgabenfunktionen auf ihren Computern durchzuführen. Die konfigurierten Einstellungen sollten auf den Sicherheitszielen ihrer Organisation basieren.

#### Kapitel 4: Administrative Vorlagen für Windows XP

In diesem Kapitel werden die Einstellungen beschrieben, die mithilfe von administrativen Vorlagen zu Windows XP hinzugefügt werden können. Administrative Vorlagen sind Unicode-Dateien zum Konfigurieren der registrierungsbasierten Einstellungen, die das Verhalten von vielen Diensten, Anwendungen und Betriebssystemkomponenten steuern. Es gibt viele administrative Vorlagen, die in Windows XP verwendet werden können. Sie enthalten hunderte von Einstellungen.

#### Kapitel 5: Schützen eigenständiger Windows XP-Clients

Obwohl sich der Großteil dieses Handbuchs mit Unternehmensclient- (EC) und Hochsicherheitsumgebungen (SSLF) befasst, wird in diesem Kapitel auch die Konfiguration eigenständiger Windows XP-Clientcomputer erörtert. Microsoft empfiehlt, Windows XP in einer Active Directory-Domäneninfrastruktur bereitzustellen, ist sich jedoch dessen bewusst, dass dies nicht immer möglich ist. Dieses Kapitel enthält Anweisungen zum Anwenden der empfohlenen Konfigurationen auf Clientcomputern mit Windows XP mit SP2, die nicht Mitglied einer Windows 2000- oder Windows Server 2003-Domäne sind.

#### Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients

Dieses Kapitel bietet einen grundlegenden Überblick über Richtlinien für Softwareeinschränkungen. Diese stellen Administratoren einen auf Richtlinien beruhenden Mechanismus zur Verfügung, mit dem sie die Software identifizieren und einschränken können, die in ihrer Domäne ausgeführt werden kann. Mit einer Richtlinie für Softwareeinschränkungen können Administratoren verhindern, dass unerwünschte Programme ausgeführt werden und dass sich Viren, trojanische Pferde und schädlicher Code ausbreiten. Richtlinien für Softwareeinschränkungen passen sich vollständig in Active Directory und die Gruppenrichtlinien ein. Sie können auch in einer Umgebung ohne Windows Server 2003-Domäneninfrastruktur verwendet werden, wenn sie nur auf den lokalen Computer angewendet werden.

#### Kapitel 7: Zusammenfassung

Im letzten Kapitel werden alle Gesichtspunkte des Handbuchs in einem Überblick zusammengefasst.

#### Anhang A: Zu berücksichtigende Schlüsseleinstellungen

In diesem Handbuch werden viele Sicherheitsgegenmaßnahmen und Sicherheitseinstellungen erörtert, von denen einige besonders wichtig ist. In diesem Anhang werden die Einstellungen erörtert, die sich am stärksten auf die Sicherheit der Computer auswirken, auf denen Windows XP mit SP2 ausgeführt wird.

#### Anhang B: Testen des Sicherheitshandbuchs für Windows XP

In diesem Anhang wird erklärt, wie das *Windows* *XP-Sicherheitshandbuch* in einer Testumgebung geprüft wurde. Dadurch soll sichergestellt werden, dass die Anleitung wie erwartet funktioniert.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Inhalt des Downloads

Dieses Handbuch enthält eine Sammlung von Sicherheitsvorlagen, Skripts und zusätzlichen Dateien, um Ihrer Organisation die Beurteilung, das Testen und die Implementierung der empfohlenen Gegenmaßnahmen zu erleichtern.

Bei den Sicherheitsvorlagen handelt es sich um Textdateien, die in domänenbasierte Gruppenrichtlinien importiert oder lokal mit dem Snap-In „Sicherheitskonfiguration und -analyse“ der Microsoft Management Console (MMC) angewendet werden können. In Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, wird beschrieben, wie diese Aufgaben erledigt werden können. Sie können die in diesem Handbuch enthaltenen Skripts verwenden, um die empfohlenen Gegenmaßnahmen auf eigenständigen Arbeitsstationen zu implementieren.

Ebenfalls im Download enthalten ist die Microsoft Excel®-Arbeitsmappe „Sicherheitseinstellungen für Windows XP“. Darin sind die Einstellungen dokumentiert, die in jeder Sicherheitsvorlage enthalten sind.

Die mit diesem Handbuch verfügbaren Dateien werden in ihrer Gesamtheit als Tools und Vorlagen bezeichnet. Diese Dateien befinden sich in einer MSI-Datei innerhalb des selbstextrahierenden WinZip-Archivs, das dieses Handbuch enthält und das im Microsoft Download Center unter http://go.microsoft.com/fwlink/?Linkid=14840&clcid=0x409 zur Verfügung steht. Wenn Sie die MSI-Datei ausführen, wird an dem angegebenen Speicherort folgende Ordnerstruktur erstellt:

-   **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\Sicherheitsvorlagen**. Dieser Ordner enthält alle Sicherheitsvorlagen, die in den Kapiteln 2 und 3 des Handbuchs besprochen werden. Er enthält außerdem eine Excel-Kalkulationstabelle, in der alle Empfehlungen im Handbuch zusammengefasst sind.

-   **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\SCE Update**. Dieser Ordner enthält Skripts und Datendateien, um die Benutzeroberfläche für den Sicherheitskonfigurations-Editor wie in Kapitel 3 des Handbuchs beschrieben automatisch zu aktualisieren.

-   **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\Eigenständige Clients**. Dieser Ordner enthält alle Beispielskripts und -vorlagen, mit denen eigenständige Computer abgesichert werden. Diese werden in Kapitel 5 des Handbuchs behandelt.

-   **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\Testtools**. Dieser Ordner enthält Tools, die sich auf „Anhang B: Testen des Sicherheitshandbuchs für Windows XP“ beziehen.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Typografische Elemente

In diesem Handbuch werden folgende typografische Elemente verwendet.

**Tabelle 1.1: Typografische Elemente**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Element</th>
<th style="border:1px solid black;" >Bedeutung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Fett</strong></td>
<td style="border:1px solid black;">Dies bedeutet, dass Zeichen genau wie dargestellt eingegeben werden, einschließlich Befehle, Switches und Dateinamen. Elemente der Benutzeroberfläche werden fett dargestellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>Kursiv</em></td>
<td style="border:1px solid black;">Titel von Büchern und andere wesentliche Veröffentlichungen werden <em>kursiv</em> dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>&lt;Kursiv&gt;</em></td>
<td style="border:1px solid black;">Kursiv dargestellte und in spitze Klammern gesetzte Platzhalter &lt; <em>Dateiname</em>&gt; stellen Variablen dar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><pre><code>Monospace font</code></pre></td>
<td style="border:1px solid black;">So werden Code- und Skriptbeispiele dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Hinweis:</strong></td>
<td style="border:1px solid black;">Weist den Leser auf zusätzliche Informationen hin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wichtig</td>
<td style="border:1px solid black;">Weist den Leser auf wesentliche Zusatzinformationen hin.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurde das *Windows* *XP-Sicherheitshandbuch* vorgestellt und der Inhalt der einzelnen Kapitel zusammengefasst. Nachdem Sie sich über den Aufbau dieses Handbuchs informiert haben, sind Sie in der Lage, die in Windows XP mit SP2 integrierten Sicherheitsoptionen optimal zu nutzen.
  
Eine effektive, erfolgreiche Sicherheitsverwaltung erfordert Anstrengungen in allen in diesem Handbuch behandelten Bereichen und nicht nur Verbesserungen auf einem einzigen Gebiet. Aus diesem Grund wird dringend empfohlen, die für Ihre Organisation geeigneten Empfehlungen in diesem Handbuch als Teil einer weiter gefassten, tief greifenden Sicherheitsarchitektur zu implementieren.
  
#### Weitere Informationen
  
Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen hinsichtlich Windows XP Professional.
  
-   Weitere Informationen zu Sicherheitseinstellungen, die unter Microsoft Windows XP konfiguriert werden können, finden Sie im Begleithandbuch [*Bedrohungen und die Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx verfügbar ist.
  
-   Weitere Informationen zum Gewährleisten der Sicherheit auf Servern in einer Art und Weise, die der in diesem Handbuch dargelegten entspricht, finden Sie im [*Windows Server 2003-Sicherheitshandbuch*](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/sgch00.mspx). Die Empfehlungen in diesem Handbuch sind für Server konzipiert, die Windows XP-Clientcomputer unterstützen müssen und die wie in den verbleibenden Kapiteln beschrieben konfiguriert sind. Dieses Handbuch ist online unter http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/sgch00.mspx verfügbar.
  
-   Weitere Informationen zum wirksameren Implementieren des Sicherheitsrisikomanagements in Ihrer Organisation finden Sie im [Leitfaden zum Sicherheitsrisikomanagement](http://go.microsoft.com/fwlink/?linkid=30794) unter http://go.microsoft.com/fwlink/?LinkID=30794.
  
-   Weitere Informationen zum Minimieren der Auswirkungen schädlicher Software finden Sie im [Leitfaden zur erfolgreichen Virenabwehr](http://go.microsoft.com/fwlink/?linkid=28732) unter http://go.microsoft.com/fwlink/?LinkId=28732.
  
-   Weitere Informationen zum Minimieren der Abhängigkeit von Kennwörtern für die Authentifizierung in Ihrer Organisation finden Sie im [Planungshandbuch für sicheren Zugriff unter Verwendung von Smartcards](http://www.microsoft.com/germany/technet/datenbank/articles/900380.mspx) unter http://www.microsoft.com/germany/technet/datenbank/articles/900380.mspx.
  
-   Weitere Informationen zum effektiveren Überwachen von und Reagieren auf potenzielle Sicherheitsverletzungen in Ihrer Organisation finden Sie im [Planungshandbuch für die Sicherheitsüberwachung und Angriffserkennung](http://www.microsoft.com/germany/technet/datenbank/articles/900370.mspx) unter http://www.microsoft.com/germany/technet/datenbank/articles/900370.mspx.
  
-   Ausführlichere Informationen dazu, wie das [Microsoft Operations Framework (MOF)](http://www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx) Sie in Ihrer Organisation unterstützen kann, finden Sie (in englischer Sprache) unter www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx.
  
-   Weitere Informationen zur [Sicherheit](http://www.microsoft.com/germany/sicherheit//) unter Microsoft Windows finden Sie (in englischer Sprache) unter www.microsoft.com/germany/sicherheit/.
  
-   Weitere Informationen zum [Microsoft-Sicherheitsbenachrichtigungsdienst](http://www.microsoft.com/germany/sicherheit/alerts.mspx) finden Sie unter www.microsoft.com/germany/sicherheit/alerts.mspx.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/default.mspx)  
-   Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP  
-   [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch02.mspx)  
-   [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch03.mspx)  
-   [Kapitel 4: Administrative Vorlagen für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch04.mspx)  
-   [Kapitel 5: Schützen eigenständiger Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch05.mspx)  
-   [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch06.mspx)  
-   [Kapitel 7: Zusammenfassung](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch07.mspx)  
-   [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)  
-   [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxa.mspx)  
-   [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxb.mspx)  
-   [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgack.mspx)
  
##### Download
  
[![](images/Cc163069.icon_exe(de-de,TechNet.10).gif)Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)