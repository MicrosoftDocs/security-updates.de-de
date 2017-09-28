---
TOCTitle: 'Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch'
Title: 'Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch'
ms:assetid: 'b0015e61-fe4e-4523-a875-ef8b971da55c'
ms:contentKeyID: 20075665
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443722(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch

Aktualisiert: 27.12.2005

##### Auf dieser Seite

[](#eiaa)[Überblick](#eiaa)
[](#ehaa)[Kurzzusammenfassung](#ehaa)
[](#egaa)[Zielgruppe](#egaa)
[](#efaa)[Themenumfang dieses Handbuchs](#efaa)
[](#eeaa)[Zusammenfassungen der Kapitel](#eeaa)
[](#edaa)[Fertigkeiten](#edaa)
[](#ecaa)[Softwareanforderungen](#ecaa)
[](#ebaa)[Typografische Elemente](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Willkommen beim *Windows* *Server* *2003-Sicherheitshandbuch*. Dieses Handbuch enthält grundlegende Informationen zur Beurteilung und Abwehrung von Sicherheitsrisiken in Ihrem Unternehmen, die Microsofts® Windows Server™ 2003 mit Service Pack 1 (SP1) betreffen. Die Kapitel in diesem Handbuch enthalten ausführliche Anleitungen zur Verbesserung der Konfigurationen und Funktionen der Sicherheitseinstellungen in Windows Server 2003 mit SP1, um erkannte Risiken in Ihrer Umgebung abzuwehren. Dieses Handbuch wurde für Systemtechniker, Berater und Netzwerkadministratoren zusammengestellt, die in einer Windows Server 2003-Umgebung mit SP1 arbeiten.

Dieses Handbuch wurde von Technikerteams, Berater, Supportmitarbeiter und Kunden sowie Partnern von Microsoft bearbeitet und genehmigt. Microsoft hat gemeinsam mit Beratern und Systemtechnikern, die Windows Server 2003, Windows® XP und Windows 2000 in verschiedenen Umgebungen implementiert haben, die neuesten empfohlenen Vorgehensweisen zum Schutz dieser Server und Clients erstellt. Diese Verfahrensweisen sind in diesem Handbuch ausführlich beschrieben.

Das Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) (verfügbar unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx) bietet einen umfassenden Überblick über die wichtigsten Sicherheitseinstellungen, die in Windows Server 2003 mit SP1 und Windows XP mit SP2 vorhanden sind. In den Kapiteln 2 bis 12 dieses Handbuchs sind schrittweise Sicherheitsanweisungen, -verfahren und -empfehlungen enthalten, die Ihnen eine Aufgabenliste bieten, mit deren Hilfe Sie eine erhöhte Sicherheitsstufe für Computer unter Windows Server 2003 mit SP1 in Ihrem Unternehmen erzielen. Ausführliche Erläuterungen der Konzepte, auf denen diese Informationen beruhen, finden Sie in den folgenden Ressourcen: *Microsoft Windows* *Server* *2003 Resource Kit*, *Microsoft Windows* *XP Resource Kit*, *Microsoft Windows* *2000 Security Resource Kit* und Microsoft TechNet.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Kurzzusammenfassung

Unabhängig von Ihrer Umgebung ist es unbedingt empfehlenswert, dem Thema Sicherheit oberste Priorität beizumessen. Viele Organisationen unterschätzen den Wert ihrer IT-Umgebung. Dies hängt oft damit zusammen, dass erhebliche indirekte Kosten nicht berücksichtigt werden. Ein schwerwiegender Angriff auf die Server Ihrer Umgebung kann einen beträchtlichen Schaden für die gesamte Organisation verursachen. Beispielsweise kann ein Angriff, der zu einem Zusammenbruch Ihrer Unternehmenswebsite und damit zu erheblichen finanziellen Einbußen oder einem verringerten Kundenvertrauen führt, die gesamte Wirtschaftlichkeit des Unternehmens aufs Spiel setzen. Bei der Bewertung von Sicherheitskosten sollten Sie daher die indirekten Kosten, die mit einem Angriff verbunden sind, sowie die durch einen Ausfall Ihrer IT-Funktionen verursachten Kosten in die Kalkulation einbeziehen.

Durch eine Analyse der Schwachstellen, der Risiken und der Angriffspunkte Ihrer Umgebung erhalten Sie eine Vorstellung von der Abwägung zwischen Sicherheit und Benutzerfreundlichkeit, die in einer Netzwerkumgebung für alle Computer erforderlich ist. In diesem Handbuch werden die wichtigsten Sicherheitsgegenmaßnahmen in Windows Server 2003 mit SP1, die entsprechenden Sicherheitsrisiken und ggf. mögliche negative Folgen der Implementierung der einzelnen Gegenmaßnahmen behandelt.

Das Handbuch gibt dann spezifische Empfehlungen zum Absichern dieser Systeme, auf denen Windows Server 2003 mit SP1 in drei verschiedenen Unternehmensumgebungen ausgeführt werden. Die Ältere Client-Umgebung muss ältere Betriebssysteme wie z. B. Windows 98 unterstützen. Die Unternehmensclient-Umgebung hat als erstes Betriebssystem Windows 2000 eingesetzt. Bei der dritten Umgebung wird der Sicherheit derart viel Bedeutung beigemessen, dass ein Verlust an Funktionalität und Verwaltbarkeit des Clients als akzeptabler Kompromiss im Streben nach höchster Sicherheit betrachtet wird. Diese dritte Umgebung ist die Hochsicher-Umgebung (SSLF). Es wurde großer Wert darauf gelegt, dass diese Informationen gut strukturiert und einfach abzurufen sind, damit Sie schnell bestimmen können, welche Einstellungen für die Computer in Ihrer Umgebung geeignet sind. Auch wenn sich dieses Handbuch an Kunden in Unternehmen richtet, sind viele der Informationen für Organisationen jeder Größe geeignet.

Zur optimalen Nutzung der Unterlagen empfiehlt es sich, das gesamte Handbuch zu lesen. Weitere Informationen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx.

Das für dieses Handbuch verantwortliche Team hofft, dass die vorliegenden Informationen für Sie hilfreich, informativ und interessant sind.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zielgruppe

Dieses Handbuch richtet sich in erster Linie an Berater, Sicherheitsexperten, Systemarchitekten und IT-Fachleute, die für die Planung der Anwendungs- bzw. Infrastrukturentwicklung und die Bereitstellung von Windows Server 2003 verantwortlich sind. Diese Rollen gelten für die folgenden allgemeinen Tätigkeitsbeschreibungen:

-   Systemarchitekten und -planer, die für die Entwicklung der Architektur von Clients in ihren Unternehmen verantwortlich sind

-   IT-Sicherheitsexperten, die sich ausschließlich mit plattformübergreifenden Sicherheitsaufgaben innerhalb ihres Unternehmens befassen

-   Unternehmensanalytiker und Entscheidungsträger in Unternehmen, in deren Verantwortungsbereich wichtige Unternehmensziele und -anforderungen fallen, die Clientunterstützung benötigen.

-   Berater von Microsoft Services und von Partnern, die detaillierte Ressourcen von relevanten und nützlichen Informationen für Partner und Unternehmenskunden suchen

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Themenumfang dieses Handbuchs

Dieses Handbuch befasst sich mit der Erstellung und Aufrechterhaltung einer sicheren Umgebung für Computer in Ihrem Unternehmen, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die Anleitungen beschreiben die verschiedenen Stufen des Schutzes der drei in diesem Handbuch definierten Umgebungen, und welche Auswirkungen jede vorgeschriebene Servereinstellung in Bezug auf Clientabhängigkeiten aufweist. Die drei Umgebungen bestehen aus folgenden Elementen:

-   Die Ältere Client-Umgebung besteht aus einer Domäne des Active Directory®-Verzeichnisdienstes mit Mitgliedsservern und Domänencontrollern, auf denen Windows Server 2003 ausgeführt wird, und Clientcomputern, auf denen Microsoft Windows 98 und Windows NT® 4.0 ausgeführt wird. Computer, auf denen Windows 98 ausgeführt wird, müssen die Active Directory Client Extension (DSCLient) installiert haben. Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[SO WIRD'S GEMACHT: Installieren von Active Directory Client Extension](http://support.microsoft.com/kb/288358)“ unter http://support.microsoft.com/kb/288358.

-   Die Unternehmensclient-Umgebung besteht aus einer Active Directory-Domäne mit Mitgliedsservern und Domänencontrollern, auf denen Windows Server 2003 mit SP1 ausgeführt wird, und Clientcomputern, auf denen Windows 2000 und Windows XP ausgeführt wird.

-   Die Hochsicher-Umgebung (SSLF) besteht ebenfalls aus einer Active Directory-Domäne mit Mitgliedsservern und Domänencontrollern, auf denen Windows Server 2003 mit SP1 ausgeführt wird, und Clientcomputern, auf denen Windows 2000 und Windows XP ausgeführt wird. Allerdings sind die Einstellungen der Hochsicher-Umgebung so eingeschränkt, dass viele Anwendungen nicht funktionstüchtig sind. Deshalb kann die Serverleistung beeinträchtigt werden, sodass die Verwaltung der Server eine Herausforderung darstellt.

    Außerdem können Clientcomputer, die nicht durch SSLF-Richtlinien geschützt sind, Kommunikationsprobleme mit durch SSLF-Richtlinien geschützten Clientcomputern und Servern aufweisen. Im *Windows XP-Sicherheitshandbuch* finden Sie Informationen zum Sichern von Clientcomputern mit SSLF-kompatiblen Einstellungen.

Hilfestellung bei der Absicherung von Computern in diesen drei Umgebungen werden für eine Gruppe verschiedener Serverrollen bereitgestellt. Bei den erläuterten Gegenmaßnahmen und bereitgestellten Tools wird vorausgesetzt, dass jeder Server eine einzelne Rolle aufweist. Wenn Sie Rollen für bestimmte Server der Umgebung kombinieren müssen, können Sie die im Download enthaltenen Sicherheitsvorlagen verwenden, um die entsprechende Kombination der Dienste und Sicherheitsoptionen zusammenzustellen. Zu den in diesem Handbuch erläuterten Rollen zählen Folgende:

-   Domänencontroller

-   Infrastrukturserver

-   Dateiserver

-   Druckserver

-   Internet Information Services (IIS)-Server

-   IAS-Server (Internet Authentication Services)

-   Zertifikatdienstserver

-   Bastion-Hosts

Die in diesem Handbuch empfohlenen Einstellungen wurden in Testumgebungen, bei denen die zuvor beschriebenen Umgebungen (Umgebung mit älteren Clients, Unternehmensclient-Umgebung und Hochsicherheitsumgebung) simuliert wurden, gründlich getestet. Die Funktion dieser Einstellungen wurde in den Testumgebungen geprüft, es ist jedoch wichtig, dass Ihr Unternehmen diese Einstellungen in einer eigenen Testumgebung prüft, die Ihre Produktionsumgebung genau widerspiegelt. Sie müssen wahrscheinlich einige Änderungen an den Sicherheitsvorlagen und den in diesem Handbuch beschriebenen manuellen Vorgehensweisen vornehmen, damit alle Geschäftsanwendungen weiterhin wie gewohnt ausgeführt werden können. Anhand der ausführlichen Informationen im Begleithandbuch *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server* *2003 und Windows* *XP*, können Sie jede spezielle Gegenmaßnahme beurteilen und entscheiden, welche dieser Maßnahmen für Ihre Unternehmensumgebung und Ihre Geschäftsanforderungen geeignet ist.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zusammenfassungen der Kapitel

Das *Windows* *Server* *2003-Sicherheitshandbuch* besteht aus 13 Kapiteln. Jedes Kapitel baut auf dem End-to-End-Lösungsprozess auf, der für das Implementieren und Schützen von Windows Server 2003 in Ihrer Umgebung erforderlich ist. In den ersten paar Kapiteln wird beschrieben, wie Sie eine Grundlage für die Absicherung der Server in Ihrem Unternehmen bilden, während in den verbleibenden Kapiteln die Verfahren vorgestellt werden, die in den einzelnen Serverrollen zur Anwendung kommen.

#### Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch

Dieses Kapitel enthält eine Einführung in das *Windows* *Server* *2003-Sicherheitshandbuch* und einen kurzen Überblick über die einzelnen Kapitel. In diesem Kapitel werden Ältere Client- (Legacy Client, LC), Unternehmensclient- (Enterprise Client, EC) und Hochsicher- (SSLF) Umgebungen, sowie die Computer, die darin ausgeführt werden, beschrieben.

#### Kapitel 2: Absicherungsmechanismen von Windows Server 2003

In diesem Kapitel wurde ein Überblick über die Hauptmechanismen gegeben, die zum Absichern von Windows Server 2003 SP1 in diesem Handbuch – dem Sicherheitskonfigurations-Assistenten (SCW) und der Active Directory-Gruppenrichtlinie – verwendet werden. In diesem Kapitel wird erläutert, wie der Sicherheitskonfigurations-Assistent ein interaktives Rahmenwerk zum Erstellen, Verwalten und Testen von Sicherheitsrichtlinien für Windows-Server bereitstellt, die unterschiedliche Rollen übernehmen. Außerdem werden die Funktionen des Sicherheitskonfigurations-Assistenten im Zusammenhang mit den drei in Kapitel 1 beschriebenen Umgebungen bewertet.

Im nächsten Teil dieses Kapitels werden der Active Directory-Entwurf, der Organisationseinheiten-Entwurf, die Gruppenrichtlinienobjekte (GPOs), der Entwurf administrativer Gruppen und die Domänenrichtlinie kurz umrissen. Diese Themen werden im Zusammenhang mit den drei in Kapitel 1 beschriebenen Umgebungen erläutert und haben eine ideale und sichere Endumgebung zum Ziel.

Das Kapitel endet mit einer ausführlichen Untersuchung darüber, wie die herausragenden Funktionen von SCW und herkömmliche gruppenrichtlinienobjektbasierte Ansätze im Hinblick auf eine Absicherung von Windows Server 2003 mit SP1 kombiniert werden können.

#### Kapitel 3: Die Domänenrichtlinie

In diesem Kapitel werden Einstellungen für Sicherheitsvorlagen und zusätzliche Gegenmaßnahmen für die Richtlinien auf Domänenebene in den drei in Kapitel 1 beschriebenen Umgebungen erläutert. Das Kapitel beschäftigt sich nicht mit spezifischen Serverrollen, sondern vielmehr mit bestimmten Richtlinien und Einstellungen, die für Domänenrichtlinien der obersten Ebene nützlich sind.

#### Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline

In diesem Kapitel werden Einstellungen für Sicherheitsvorlagen sowie zusätzliche Gegenmaßnahmen für die unterschiedlichen Serverrollen in den drei in Kapitel 1 beschriebenen Umgebungen erläutert. Das Kapitel befasst sich mit der Erstellung einer Richtlinie für die Mitgliedsserver-Baseline (MSBP) für die später im Handbuch erläuterten Serverrollen.

Die Empfehlungen in diesem Kapitel sind so konzipiert, dass sie es Unternehmen ermöglichen, Einstellungskonfigurationen für bestehende und neue Systeme von Windows Server 2003 mit SP1 bereitzustellen. Die Standardsicherheitskonfigurationen in Windows Server 2003 SP1 wurden erforscht und getestet. Die in diesem Kapitel abgegebenen Empfehlungen dienen der Erhöhung der Sicherheit im Vergleich zu den Standardeinstellungen des Betriebssystems. Gelegentlich wird eine weniger restriktive Einstellung als die in der Standardinstallation von Windows Server 2003 mit SP1 enthaltene vorgeschlagen, um den Support für Umgebungen mit älteren Systemen zu gewährleisten.

#### Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline

Die Serverrolle für den Domänencontroller ist eine der wichtigsten Rollen zur Absicherung einer Active Directory-Umgebung mit Computern, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Jeder Verlust oder jede Gefährdung eines Domänencontrollers kann ernsthafte Folgen für Clients, Server und Anwendungen haben, die für die Authentifizierung, für Gruppenrichtlinien und für ein zentrales LDAP-Verzeichnis (Lightweight Directory Access Protocol) auf Domänencontroller angewiesen sind.

In diesem Kapitel wird hervorgehoben, dass Domänencontroller immer an physisch sicheren Orten gespeichert werden sollten, zu denen nur qualifizierte Verwaltungsmitarbeiter Zugriff haben. Es werden die Gefahren von Domänencontrollern an ungesicherten Orten, wie z. B. Zweigstellen, besprochen und ein Großteil des Kapitels befasst sich mit den Sicherheitserwägungen, die der empfohlenen Gruppenrichtlinie für Domänencontroller zugrunde liegt.

Active Directory-Domänencontroller erfordern einen stabilen, ordnungsgemäß konfigurierten DNS-Dienst. Standardmäßig integriert Windows Server 2003 mit SP1 DNS-Zonen in Active Directory, sodass Domänencontroller den DNS-Dienst ausführen und DNS-Anforderungen nach Clients in der Active Directory-Domäne beantworten können. In diesem Kapitel wird davon ausgegangen, dass der Domänencontroller zudem DNS-Dienste anbietet, und es werden entsprechende Anleitungen geboten.

#### Kapitel 6: Die Infrastrukturserverrolle

Die Infrastrukturserverrolle ist in diesem Kapitel als DHCP-Server oder als WINS-Server definiert. Sie erhalten ausführliche Informationen dazu, wie die Infrastrukturserver mit Windows Server 2003 mit SP1 in Ihrer Umgebung von Sicherheitseinstellungen profitieren können, die nicht durch die Richtlinie für die Mitgliedsserver-Baseline (MSBP) angewendet werden. Dieses Kapitel enthält keine Informationen zur Konfiguration des DNS-Dienstes, der in der Domänencontrollerrolle enthalten ist.

#### Kapitel 7: Die Dateiserverrolle

Dieses Kapitel beschäftigt sich mit der Dateiserverrolle und den schwierigen Aspekten der Absicherung solcher Server. Für die wesentlichsten Dienste für Dateiserver ist die Verwendung von Windows-NetBIOS-Protokollen und SMB- und CIFS-Protokollen erforderlich. Das SMB (Server Message Block)- und das CIFS (Common Internet File System)-Protokoll werden in der Regel dazu benutzt, den Zugriff für authentifizierte Benutzer bereitzustellen. Sind diese jedoch nicht ordnungsgemäß abgesichert, können sie wichtige Informationen auch an nicht authentifizierte Benutzer oder Angreifer weitergeben. Aufgrund dieser Gefährdung sind diese Protokolle in Umgebungen mit hohen Sicherheitsanforderungen häufig deaktiviert. In diesem Kapital wird erläutert, wie Dateiserver, auf denen Windows Server 2003 mit SP1 ausgeführt wird, von Sicherheitseinstellungen profitieren können, die nicht von der Richtlinie für die Mitgliedsserver-Baseline angewendet werden.

#### Kapitel 8: Die Druckserverrolle

Der Schwerpunkt in diesem Kapitel liegt auf Druckservern. Wie für Dateiserver ist für die wesentlichsten Dienste für Druckserver der Einsatz von Windows-Netbios-Protokollen und SMB- und CIFS-Protokollen erforderlich. Wie bereits zuvor erläutert, sind diese Protokolle in Umgebungen mit hohen Sicherheitsanforderungen häufig deaktiviert. In diesem Kapitel wird beschrieben, wie Sicherheitseinstellungen für Druckserver in Windows Server 2003 mit SP1 besser abgesichert werden können und Möglichkeiten beinhalten, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

#### Kapitel 9: Die Webserverrolle

In diesem Kapitel wird erläutert, wie umfassende Sicherheit für Websites und Anwendungen einen gesamten IIS-Server erforderlich macht (einschließlich der einzelnen Websites und Anwendungen, die auf dem IIS-Server ausgeführt werden), der vor Clientcomputern in seiner Umgebung geschützt werden muss. Die Websites und Anwendungen müssen auch vor anderen Websites und Anwendungen geschützt werden, die auf dem gleichen IIS-Server ausgeführt werden. Vorgehensweisen zur Sicherstellung der Erfüllung dieser Maßnahmen über die IIS-Server, auf denen Windows Server 2003 mit SP1 in Ihrer Umgebung ausgeführt wird, werden in diesem Kapitel ausführlich erläutert.

IIS wird standardmäßig nicht auf Mitgliedern der Microsoft Windows Server System™-Familie installiert. Beim ersten Installieren wird IIS in einem hochsicheren, „gesperrten“ Modus installiert. Die Standardeinstellungen lassen nur zu, dass IIS statischen Inhalt verarbeitet. Die Features, wie z. B. Active Server Pages (ASP), ASP.NET, Serverseitige Includes, WebDAV-Veröffentlichung und Microsoft FrontPage®-Servererweiterungen müssen durch den Administrator über den Webdiensterweiterungsknoten im Internetinformationsdienst-Manager (Information Services Manager, IIS Manager) aktiviert werden.

In den Abschnitten dieses Kapitels werden ausführliche Informationen zu verschiedenen Einstellungen zur Absicherung der IIS-Server in Ihrer Umgebung geboten. Betont wird die Notwendigkeit einer Überwachung, Erkennung und Reaktion auf Sicherheitsrisiken um zu gewährleisten, dass die Server geschützt bleiben. Dieses Kapitel befasst sich mit IIS-Internetprotokollen und -anwendungen, wie etwa HTTP, enthält aber keine Anleitung zu den anderen Protokollen, die IIS bereitstellen kann, wie zum Beispiel SMTP, FTP und NNTP.

#### Kapitel 10: Die IAS-Serverrolle

Internetauthentifizierungsserver (IAS) bieten Remote Authentication Dial-In User Service (RADIUS), ein auf Standards basierendes Authentifizierungsprotokoll, das zur Überprüfung der Identität von Kunden entworfen wurde, die von einem Remotestandort auf das Netzwerk zugreifen. In diesem Kapital werden Möglichkeiten erläutert, bei denen IAS-Server mit Windows Server 2003 mit SP1 von Sicherheitseinstellungen profitieren können, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

#### Kapitel 11: Die Zertifikatdienstserverrolle

Die Zertifikatdienste stellen die Verschlüsselungs- und Zertifikatverwaltungsdienste zur Verfügung, die für das Erstellen einer Infrastruktur öffentlicher Schlüssel (PKI) in Ihrer Serverumgebung erforderlich sind. In diesem Kapital werden Möglichkeiten erläutert, bei denen Zertifikatdienstserver mit Windows Server 2003 mit SP1 von Sicherheitseinstellungen profitieren, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

#### Kapitel 12: Die Bastion-Hostrolle

Auf Bastion-Hostserver können Clientcomputer über das Internet zugreifen. In diesem Kapitel wird erklärt, weshalb diese öffentlich zugänglichen Computer für Angriffe von einer großen Anzahl an Benutzern anfällig sind, die, wenn sie möchten, vollständig anonym bleiben können. Viele Unternehmen weiten ihre Domäneninfrastruktur nicht auf das Internet aus. Aus diesem Grund enthält dieses Kapitel v. a. Informationen zur besseren Absicherung eigenständiger Computer. Sie erhalten ausführliche Informationen dazu, wie Bastion-Hosts, auf denen Windows Server 2003 mit SP1 ausgeführt wird, bei Computern, die keine Mitglieder einer Active Directory-basierten Domäne sind, von den Sicherheitsempfehlungen in diesem Handbuch profitieren können.

#### Kapitel 13: Zusammenfassung

Das letzte Kapitel dieses Handbuchs bietet einen Überblick über die wichtigsten Punkte des in den vorangehenden Kapiteln präsentierten Materials.

#### Anhang A: Sicherheitstools und Formate

Obwohl sich dieses Handbuch mit dem Einsatz von SCW zur Erstellung von Richtlinien beschäftigt, die anschließend in Sicherheitsvorlagen und Gruppenrichtlinienobjekte umgewandelt werden, gibt es eine ganze Reihe anderer Tools und Dateiformate, die zur Verbesserung oder Veränderung dieser Methoden eingesetzt werden können. In diesem Anhang wird eine kurze Liste dieser Tools und Formate bereitgestellt.

#### Anhang B: Zu berücksichtigende Schlüsseleinstellungen

In diesem Handbuch wird eine Vielzahl an Sicherheitsgegenmaßnahmen und Sicherheitseinstellungen erläutert. Dabei ist es jedoch wichtig zu wissen, welche davon von besonderer Bedeutung sind. In diesem Anhang werden die Einstellungen erörtert, die sich am stärksten auf die Sicherheit der Computer auswirken, auf denen Windows Server 2003 mit SP1 ausgeführt wird.

#### Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen

In diesem Anhang wird die Microsoft Excel®-Arbeitsmappe „Sicherheitshandbucheinstellungen für Windows Server 2003“ eingeführt, die mit den Tools und Vorlagen in der [Download-Version](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409) dieses Handbuchs unter http://go.microsoft.com/fwlink/?LinkId=14846&clcid=0x409 enthalten ist. Diese Excel-Tabelle bietet in kompakter, übersichtlicher Form einen umfassenden Überblick über alle empfohlenen Einstellungen für die drei in diesem Handbuch definierten Umgebungen.

#### Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs

Dieses Handbuch befasst sich in erster Linie mit der Absicherung von Servern, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Der Leser wird jedoch ständig darauf hingewiesen, alle Einstellung vor ihrer Implementierung in einer Produktionsumgebung zu testen und zu prüfen.

Dieser Anhang enthält Anweisungen zum Erstellen einer geeigneten Testumgebung, mit deren Hilfe die erfolgreiche Implementierung der empfohlenen Einstellungen in einer Produktionsumgebung sichergestellt werden kann. Dadurch können Benutzer die notwendige Überprüfung durchführen, und die dafür erforderlichen Ressourcen werden verringert.

#### Tools und Vorlagen

Eine Sammlung der Sicherheitsvorlagen, Skripts und zusätzlichen Tools ist in der Online-Version dieses Handbuchs enthalten und steht als Download zur Verfügung, damit Ihr Unternehmen die empfohlenen Gegenmaßnahmen bewerten, testen und implementieren kann. Bei den Sicherheitsvorlagen handelt es sich um Textdateien, die in domänenbasierte Gruppenrichtlinien importiert oder lokal mit dem Snap-In „Sicherheitskonfiguration und -analyse“ der Microsoft Management Console (MMC) angewendet werden können. Diese Verfahren werden in Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, ausführlich erläutert. Zu den in diesem Handbuch enthaltenen Skripts zählen Skripts zum Erstellen und Verknüpfen von Gruppenrichtlinienobjekten sowie Testskripts zum Testen der empfohlenen Gegenmaßnahmen. Ebenfalls enthalten ist die Excel-Arbeitsmappe, in der die Sicherheitsvorlageneinstellungen zusammengefasst werden, auf die zuvor im „Anhang C“ hingewiesen wurde.

Die mit diesem Handbuch verfügbaren Dateien werden in ihrer Gesamtheit als Tools und Vorlagen bezeichnet. Sie sind in einer MSI-Datei in dem selbstextrahierenden WinZip-Archiv enthalten, das im Microsoft Download Center unter http://go.microsoft.com/fwlink/?LinkId=14846&clcid=0x409 zur Verfügung steht. Bei Ausführung der MSI-Datei wird im gewünschten Verzeichnis folgende Ordnerstruktur erstellt:

-   **Windows Server 2003-Sicherheitshandbuch Tools und Vorlagen\\Sicherheitsvorlagen**. Dieser Ordner enthält alle Sicherheitsvorlagen, die im Handbuch erläutert werden.

-   **Windows Server 2003-Sicherheitshandbuch Tools und Vorlagen\\Testtools**. Dieser Ordner enthält verschiedene Dateien und Tools in Zusammenhang mit „Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs“.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Fertigkeiten

IT-Fachleute, die Installationen von Windows Server 2003 und Windows XP in einer Unternehmensumgebung entwickeln, bereitstellen und schützen, sollten folgende Kenntnisse und Fertigkeiten besitzen:

-   MCSE 2000- oder 2003-Zertifizierung mit mehr als zwei Jahren Erfahrung im Bereich Sicherheit.

-   Fundierte Kenntnisse von Domänen- und Active Directory-Umgebungen in Unternehmen.

-   Erfahrung im Umgang mit Verwaltungstools einschließlich der Microsoft Management Console (MMC), Secedit, Gpupdate und Gpresult.

-   Erfahrung im Verwalten von Gruppenrichtlinien.

-   Erfahrung bei der Bereitstellung von Anwendungen und Arbeitsstationscomputern in Unternehmensumgebungen.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Softwareanforderungen

Für den Einsatz der in diesem Handbuch genannten Tools und Vorlagen gelten die folgenden Softwareanforderungen:

-   Windows Server 2003 Standard Edition mit SP1, Windows Server 2003 Enterprise Edition mit SP1 oder Windows Server 2003 Datacenter Edition mit SP1.

-   Eine Windows Server 2003–basierte Active Directory-Domäne.

-   Microsoft Excel 2000 oder höher.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Typografische Elemente

In diesem Leitfaden werden folgende typografische Elemente verwendet.

**Tabelle 1.1: Typografische Elemente**

 
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
<td style="border:1px solid black;">Bedeutet, dass Zeichen dem Wortlaut nach angezeigt werden, einschließlich Befehle, Optionen und Dateinamen. Elemente der Benutzeroberfläche werden fett dargestellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><em>Kursiv</em></td>
<td style="border:1px solid black;">Titel von Büchern und andere wesentliche Veröffentlichungen werden kursiv dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><em>&lt;Kursiv&gt;</em></td>
<td style="border:1px solid black;">Platzhalter in Kursiv und Dreiecksklammern <em>&lt;Dateiname&gt;</em> stellen Variable dar.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Monospace-Schriftart</td>
<td style="border:1px solid black;">So werden Code- und Skriptbeispiele dargestellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><strong>Hinweis:</strong></td>
<td style="border:1px solid black;">Weist den Leser auf zusätzliche Informationen hin.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Wichtig</strong></td>
<td style="border:1px solid black;">Weist den Leser auf wesentliche Zusatzinformationen hin.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusammenfassung
  
Dieses Kapitel bietet einen Überblick über die Hauptfaktoren zum Schutz von Computern, auf denen Windows Server 2003 mit SP1 ausgeführt wird, die ausführlicher im Rest des Handbuchs berücksichtigt und erläutert werden. Nachdem Ihnen der Aufbau dieses Handbuchs dargelegt wurde, können Sie entscheiden, welche Abschnitte besonders interessant für Sie sind oder ob Sie es in seiner Gesamtheit lesen möchten.
  
Bedenken Sie dabei jedoch, dass effektive und erfolgreiche Sicherheitsabläufe Verbesserungen in allen hier behandelten Bereichen erfordern, nicht nur in einigen wenigen. Aus diesem Grund empfiehlt Microsoft, dass Sie das komplette Handbuch lesen, um die hierin enthaltenen Informationen zum Schutz von Computern unter Windows Server 2003 mit SP1 in Ihrem Unternehmen voll zu nutzen.
  
#### Weitere Informationen
  
Unter den folgenden Links erhalten Sie zusätzliche Informationen zum Thema Sicherheit und Windows Server 2003 mit SP1.
  
-   Weitere Informationen zur Sicherheit bei Microsoft finden Sie auf der Seite [Vertrauenswürdiges Programmieren](http://www.microsoft.com/germany/sicherheit/twc/default.mspx) unter www.microsoft.com/germany/sicherheit/twc/default.mspx.
  
-   Weitere Informationen dazu, wie MOF in Ihrem Unternehmen eingesetzt werden kann, finden Sie auf der Seite [Microsoft Operations Framework](http://www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/itsolutions/cits/mo/mof/default.mspx.
  
-   Informationen zu Sicherheitsbenachrichtigungen von Microsoft finden Sie auf der Seite [Microsoft Security Bulletins](http://www.microsoft.com/germany/technet/sicherheit/bulletins/default.mspx) unter www.microsoft.com/germany/technet/sicherheit/bulletins/default.mspx
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))  
-   Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))  
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))  
-   [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))  
-   [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))  
-   [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))  
-   [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))  
-   [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))  
-   [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))  
-   [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))  
-   [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))  
-   [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))  
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))  
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))  
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))  
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10)"><img src="images/Dd443722.pageLeft(de-de,TechNet.10).gif" /></a> 2 von 19 <a href="https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10)"><img src="images/Dd443722.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
