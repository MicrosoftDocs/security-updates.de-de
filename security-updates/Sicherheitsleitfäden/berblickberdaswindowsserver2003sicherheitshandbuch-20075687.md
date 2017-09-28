---
TOCTitle: 'Überblick über das Windows Server 2003-Sicherheitshandbuch'
Title: 'Überblick über das Windows Server 2003-Sicherheitshandbuch'
ms:assetid: '303c53d5-6b76-46e1-8ee3-7d8c99891129'
ms:contentKeyID: 20075687
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443744(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Überblick

Aktualisiert: 27.12.2005

Das aktualisierte *Windows Server 2003-Sicherheitshandbuch* gibt spezifische Empfehlungen zum Absichern von Computern unter Windows® Server™ 2003 mit SP1 in drei verschiedenen Unternehmensumgebungen: eine Umgebung, in der ältere Betriebssysteme wie z. B. Windows NT® 4.0 und Windows® 98 unterstützt werden müssen, eine Umgebung, in der Windows 2000 die früheste Windows-Betriebssystemversion ist, und eine Umgebung, in der die Sicherheitsanforderungen so hoch sind, dass ein Verlust an Funktionalität und Verwaltbarkeit des Clients als akzeptabler Kompromiss im Streben nach höchster Sicherheit betrachtet wird. Diese drei Umgebungen werden in diesem Handbuch jeweils als Umgebung mit älteren Clients, Unternehmensclient-Umgebung und Hochsicherheitsumgebung bezeichnet.

Anweisungen zur Absicherung von Computern in diesen drei Umgebungen werden für eine Reihe unterschiedlicher Serverrollen bereitgestellt. Bei den erläuterten Gegenmaßnahmen und bereitgestellten Tools wird vorausgesetzt, dass jeder Server eine einzelne Rolle aufweist. Wenn Sie Rollen für bestimmte Server der Umgebung kombinieren müssen, können Sie die in der herunterladbaren Version dieses Handbuchs enthaltenen Sicherheitsvorlagen verwenden, um die entsprechende Kombination von Diensten und Sicherheitsoptionen zusammenzustellen. Zu den Serverrollen, auf die in diesem Handbuch verwiesen wird, zählen folgende:

-   Domänencontroller, die auch DNS-Dienste bereitstellen

-   Infrastrukturserver, die WINS- und DHCP-Dienste bereitstellen

-   Dateiserver

-   Druckserver

-   Webserver, auf denen Microsoft Internet Information Services (IIS) ausgeführt wird

-   IAS-Server (Internet Authentication Services)

-   Zertifikatdienstserver

-   Bastion-Hosts

Wir haben uns bemüht, dieses Handbuch übersichtlich zu gestalten, damit Sie die gewünschten Informationen schnell finden und dann bestimmen können, welche Einstellungen für die Computer in Ihrer Organisation geeignet sind. Die Informationen in diesem Handbuch richten sich zwar an Unternehmenskunden, sind aber für Organisationen jeglicher Größe geeignet.

Zur optimalen Nutzung dieser Unterlagen empfiehlt es sich, das gesamte Handbuch zu lesen. Es empfiehlt sich außerdem, das Begleithandbuch [Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) zu lesen, das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx heruntergeladen werden kann.

##### Auf dieser Seite

[](#eeaa)[Zielgruppe](#eeaa)
[](#edaa)[Überblick über den Leitfaden](#edaa)
[](#ecaa)[Verwandte Themen](#ecaa)
[](#ebaa)[Senden Sie uns Ihr Feedback](#ebaa)
[](#eaaa)[Consulting- und Supportdienstleistungen](#eaaa)

### Zielgruppe

Dieses Handbuch richtet sich in erster Linie an Berater, Sicherheitsspezialisten, Systemarchitekten und IT-Fachleute, die für die Planung der Anwendungs- bzw. Infrastrukturentwicklung und der Bereitstellung von Windows Server 2003 verantwortlich sind. Dieses Handbuch ist nicht für den privaten Benutzer gedacht.

Sicherheitsfachleute und IT-Architekten benötigen u. U. ausführlichere Informationen zu den in diesem Handbuch erläuterten Sicherheitseinstellungen. Weitere Informationen finden Sie im Begleithandbuch [Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Überblick über den Leitfaden

### Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch

In diesem Kapitel wird eine Kurzzusammenfassung über das *Windows Server 2003-Sicherheitshandbuch* sowie eine kurze Übersicht über die einzelnen Kapitel geboten. Außerdem werden die Umgebung mit älteren Clients, die Unternehmensclient-Umgebung, die Hochsicherheitsumgebung sowie die Computer, die in diesen Umgebungen ausgeführt werden, beschrieben.

### Kapitel 2: Absicherungsmechanismen von Windows Server 2003

In diesem Kapitel wird ein Überblick über die Hauptmechanismen gegeben, die in diesem Handbuch zum Absichern von Windows Server 2003 mit SP1 verwendet werden: den Sicherheitskonfigurations-Assistenten (SCW) und die Active Directory-Gruppenrichtlinie. Es wird erläutert, wie SCW ein interaktives Rahmenwerk zum Erstellen, Verwalten und Testen von Sicherheitsrichtlinien für Windows Server 2003-basierte Computer bereitstellt, die unterschiedliche Rollen übernehmen. Außerdem werden die Funktionen des Sicherheitskonfigurations-Assistenten im Zusammenhang mit den drei in Kapitel 1 beschriebenen Umgebungen bewertet.

Im nächsten Teil dieses Kapitels werden der Active Directory-Entwurf, der Organisationseinheiten-Entwurf, die Gruppenrichtlinienobjekte (GPOs), der Entwurf administrativer Gruppen und die Domänenrichtlinie kurz umrissen. Diese Themen werden im Zusammenhang mit den drei in Kapitel 1 beschriebenen Umgebungen erläutert und haben eine ideale und sichere Endumgebung zum Ziel.

Das Kapitel endet mit einer ausführlichen Untersuchung darüber, wie die herausragenden Funktionen von SCW und herkömmliche gruppenrichtlinienobjektbasierte Ansätze im Hinblick auf eine Absicherung von Windows Server 2003 mit SP1 kombiniert werden können.

### Kapitel 3: Die Domänenrichtlinie

In diesem Kapitel werden Einstellungen für Sicherheitsvorlagen und zusätzliche Gegenmaßnahmen für die Richtlinien auf Domänenebene in den drei in Kapitel 1 beschriebenen Umgebungen erläutert. Das Kapitel beschäftigt sich nicht mit spezifischen Serverrollen, sondern vielmehr mit bestimmten Richtlinien und Einstellungen, die für Domänenrichtlinien der obersten Ebene nützlich sind.

### Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline

Dieses Kapitel befasst sich mit der Erstellung einer Richtlinie für die Mitgliedsserver-Baseline (MSBP) für die später im Handbuch erläuterten Serverrollen.

### Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline

Die Serverrolle für den Domänencontroller ist eine der wichtigsten Rollen zur Absicherung einer Active Directory-Umgebung mit Computern, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Jeder Verlust oder jede Gefährdung eines Domänencontrollers kann ernsthafte Folgen für Clients, Server und Anwendungen haben, die für die Authentifizierung, für Gruppenrichtlinien und für ein zentrales LDAP-Verzeichnis (Lightweight Directory Access Protocol) auf Domänencontroller angewiesen sind. In den drei im Handbuch definierten Umgebungen stellen die Domänencontroller auch DNS-Dienste bereit.

### Kapitel 6: Die Infrastrukturserverrolle

In diesem Kapitel stellt die Infrastrukturserverrolle die DHCP- oder WINS-Dienste bereit. Sie erhalten ausführliche Informationen dazu, wie die Infrastrukturserver mit Windows Server 2003 mit SP1 in Ihrer Umgebung von Sicherheitseinstellungen profitieren können, die nicht durch die Richtlinie für die Mitgliedsserver-Baseline (MSBP) angewendet werden.

### Kapitel 7: Die Dateiserverrolle

Dieses Kapitel behandelt die Absicherung von Computern, die als Dateiserver fungieren, sowie die dabei bestehenden Probleme. Für die wesentlichen von Dateiservern bereitgestellten Dienste ist die Verwendung von Windows-NetBIOS-Protokollen sowie SMB (Server Message Block)- und CIFS (Common Internet File System)-Protokollen erforderlich. Das SMB- und das CIFS-Protokoll werden in der Regel dazu benutzt, den Zugriff für authentifizierte Benutzer bereitzustellen. Sind sie jedoch nicht ordnungsgemäß abgesichert, können sie wichtige Informationen auch an nicht authentifizierte Benutzer oder Angreifer weitergeben. Aufgrund dieser Gefährdung sind diese Protokolle in Umgebungen mit hohen Sicherheitsanforderungen häufig deaktiviert. In diesem Kapital wird erläutert, wie Dateiserver, auf denen Windows Server 2003 mit SP1 ausgeführt wird, von Sicherheitseinstellungen profitieren können, die nicht von der Richtlinie für die Mitgliedsserver-Baseline angewendet werden.

### Kapitel 8: Die Druckserverrolle

Der Schwerpunkt in diesem Kapitel liegt auf Druckservern. Wie bei Dateiservern sind auch für die wesentlichen von Druckservern bereitgestellten Dienste Windows-NetBIOS-Protokolle sowie das SMB- und das CIFS-Protokoll erforderlich. Wie bereits zuvor erwähnt, sind das SMB- und das CIFS-Protokoll in Hochsicherheitsumgebungen häufig deaktiviert. In diesem Kapitel wird beschrieben, wie Sicherheitseinstellungen für Druckserver in Windows Server 2003 mit SP1 besser abgesichert werden können und Möglichkeiten beinhalten, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

### Kapitel 9: Die Webserverrolle

In diesem Kapitel wird erläutert, wie umfassende Sicherheit für Websites und Anwendungen einen gesamten IIS-Server erforderlich macht (einschließlich der einzelnen Websites und Anwendungen, die auf dem IIS-Server ausgeführt werden), der vor Clientcomputern in seiner Umgebung geschützt werden muss. Die Websites und Anwendungen müssen auch vor anderen Websites und Anwendungen geschützt werden, die auf dem gleichen IIS-Server ausgeführt werden. Vorgehensweisen zur Sicherstellung der Erfüllung dieser Anforderungen auf IIS-Servern in Ihrer Umgebung, auf denen Windows Server 2003 mit SP1 ausgeführt wird, werden in diesem Kapitel erläutert.

### Kapitel 10: Die IAS-Serverrolle

Internetauthentifizierungsserver (IAS) bieten Remote Authentication Dial-In User Service (RADIUS), ein auf Standards basierendes Authentifizierungsprotokoll, das zur Überprüfung der Identität von Kunden entworfen wurde, die von einem Remotestandort auf das Netzwerk zugreifen. In diesem Kapital werden Möglichkeiten erläutert, bei denen IAS-Server mit Windows Server 2003 mit SP1 von Sicherheitseinstellungen profitieren können, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

### Kapitel 11: Die Zertifikatdienstserverrolle

Die Zertifikatdienste stellen die Verschlüsselungs- und Zertifikatverwaltungsdienste zur Verfügung, die für das Erstellen einer Infrastruktur öffentlicher Schlüssel (PKI) in Ihrer Serverumgebung erforderlich sind. In diesem Kapital werden Möglichkeiten erläutert, bei denen Zertifikatdienstserver mit Windows Server 2003 mit SP1 von Sicherheitseinstellungen profitieren, die durch die Richtlinie für die Mitgliedsserver-Baseline nicht angewendet werden.

### Kapitel 12: Die Bastion-Hostrolle

Auf Bastion-Hostserver können Clientcomputer über das Internet zugreifen. In diesem Kapitel wird erklärt, weshalb diese öffentlich zugänglichen Systeme für Angriffe von einer großen Anzahl an Benutzern anfällig sind, die je nach Belieben vollständig anonym bleiben können. Da viele Organisationen ihre Domäneninfrastruktur nicht auf das Internet erweitern, wird in diesem Kapitel in erster Linie die Absicherung von eigenständigen Computern behandelt, auf denen Windows Server 2003 mit SP1 ausgeführt wird, die aber keiner Active Directory-basierten Domäne angehören.

### Kapitel 13: Zusammenfassung

Das letzte Kapitel dieses Handbuchs bietet eine kurze Zusammenfassung des in den vorangehenden Kapiteln präsentierten Materials.

### Anhang A: Sicherheitstools und Formate

Obwohl sich das *Windows Server 2003-Sicherheitshandbuch* mit dem Einsatz des SCW zur Erstellung von Richtlinien beschäftigt, die anschließend in Sicherheitsvorlagen und Gruppenrichtlinienobjekte umgewandelt werden, gibt es eine ganze Reihe anderer Tools und Datenformate, die zur Verbesserung oder Veränderung dieser Methoden eingesetzt werden können. In diesem Anhang wird eine kurze Liste dieser Tools und Formate bereitgestellt.

### Anhang B: Zu berücksichtigende Schlüsseleinstellungen

Im *Windows Server 2003-Sicherheitshandbuch* wird eine Vielzahl an Sicherheitsgegenmaßnahmen und Sicherheitseinstellungen erläutert. Dabei ist es jedoch wichtig zu wissen, welche davon von besonderer Bedeutung sind. In diesem Anhang werden die Einstellungen erörtert, die sich am stärksten auf die Sicherheit der Computer auswirken, auf denen Windows Server 2003 mit SP1 ausgeführt wird.

### Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen

In diesem Anhang wird die [Microsoft Excel®-Arbeitsmappe zu den im Windows Server 2003-Sicherheitshandbuch beschriebenen Einstellungen](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409) vorgestellt. Diese Arbeitsmappe ist in den Tools und Vorlagen der unter http://go.microsoft.com/fwlink/?LinkId=14846&clcid=0x409 [herunterladbaren Version](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409) des Handbuchs enthalten. Diese Arbeitsmappe bietet in kompakter, übersichtlicher Form einen umfassenden Überblick über alle empfohlenen Einstellungen für die drei im Handbuch definierten Umgebungen.

### Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs

Das *Windows Server 2003-Sicherheitshandbuch* befasst sich in erster Linie mit der Absicherung von Servern, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Der Leser wird jedoch ständig darauf hingewiesen, alle Einstellungen vor deren Implementierung in einer Produktionsumgebung zu testen und zu prüfen.

Dieser Anhang enthält Anweisungen zum Erstellen einer geeigneten Testumgebung, mit deren Hilfe die erfolgreiche Implementierung der empfohlenen Einstellungen in einer Produktionsumgebung sichergestellt werden kann. Dadurch können Benutzer die notwendige Überprüfung durchführen, und die dafür erforderlichen Ressourcen werden verringert.

### Tools und Vorlagen

Eine Sammlung der Sicherheitsvorlagen, Skripts und zusätzlichen Tools ist in der Online-Version dieses Handbuchs enthalten und steht zum Herunterladen zur Verfügung, damit Ihre Organisation die empfohlenen Gegenmaßnahmen leichter bewerten, testen und implementieren kann. Bei den Sicherheitsvorlagen handelt es sich um Textdateien, die in domänenbasierte Gruppenrichtlinien importiert oder lokal mit dem Snap-In „Sicherheitskonfiguration und -analyse“ der Microsoft Management Console (MMC) angewendet werden können. Diese Verfahren werden in Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, ausführlich erläutert. Zu den in diesem Handbuch enthaltenen Skripts zählen Skripts zum Erstellen und Verknüpfen von Gruppenrichtlinienobjekten sowie Testskripts zum Testen der empfohlenen Gegenmaßnahmen.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Verwandte Themen

Weitere Informationen zu den in diesem Handbuch vorgeschriebenen Sicherheitseinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://go.microsoft.com/fwlink/?linkid=15160&clcid=0x409), das Sie unter http://go.microsoft.com/fwlink/?LinkId=15160&clcid=0x409 herunterladen können, sowie im [*Windows XP-Sicherheitshandbuch*](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409), das unter http://go.microsoft.com/fwlink/?Linkid=14840&clcid=0x409 heruntergeladen werden kann (jeweils in englischer Sprache). Informationen zu [anderen Sicherheitslösungen](http://www.microsoft.com/technet/community/columns/sectip/st0805.mspx) des MSSC-Teams (Microsoft Solutions for Security and Compliance) sind (in englischer Sprache) unter www.microsoft.com/technet/community/columns/sectip/st0805.mspx verfügbar.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Senden Sie uns Ihr Feedback

Das MSSC-Team (Microsoft Solutions for Security and Compliance) legt großen Wert auf Ihr Feedback zu dieser und anderen Sicherheitslösungen.

Wie lautet Ihre Meinung? Teilen Sie uns Ihre Meinung über das [Security Solutions Blog](http://blogs.technet.com/secguide) für IT-Fachleute mit.

Sie können Ihr Feedback auch an die folgende E-Mail-Adresse senden: [SecWish@microsoft.com.](mailto:secwish@microsoft.com?subject=windows%20server%202003%20security%20guide) Wir reagieren häufig auf Feedback, das an diese Adresse gesendet wird.

Wir danken Ihnen schon jetzt für Ihre Unterstützung.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Consulting- und Supportdienstleistungen

Es stehen viele Dienste zur Verfügung, die Unternehmen und Organisationen bei der Optimierung ihrer Sicherheitsstrategie unterstützen. Verwenden Sie die folgenden Links, um auf die gewünschten Dienste zuzugreifen:

Informationen zu Microsoft Gold Certified Partnern, Microsoft Certified Technical Education Centers (CTEC) und Microsoft Certified Partnern sowie zu Produkten von unabhängigen Softwareanbietern (Independent Software Vendors, ISV), die Microsoft-Technologie einsetzen, finden Sie im [Microsoft-Ressourcenverzeichnis](http://go.microsoft.com/fwlink/?linkid=43094) unter http://go.microsoft.com/fwlink/?LinkId=43094.

Informationen zu Consulting- und Supportdienstleistungen, die für Ihre Organisation relevant sind, finden Sie im Bereich für [Microsoft Services](http://support.microsoft.com/msservices) unter http://support.microsoft.com/msservices.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### In diesem Beitrag

-   Überblick
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))
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

<p> </p>
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
<td style="border:1px solid black;">1 von 19<a href="https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10)"><img src="images/Dd443744.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
