---
Title: Kapitel 4 - Die Richtlinie für die Mitgliedsserver-Baseline
TOCTitle: Kapitel 4 - Die Richtlinie für die Mitgliedsserver-Baseline
ms:assetid: 7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443725(v=TechNet.10)
ms:contentKeyID: 20075668
---


# Windows Server 2003-Sicherheitshandbuch



### Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline
Aktualisiert: 27.12.2005
 

#### Auf dieser Seite

[Überblick](#ekaa)  
[Baseline-Richtlinie für Windows Server 2003](#ejaa)  
[Überwachungsrichtlinie](#eiaa)  
[Zuweisen von Benutzerrechten](#ehaa)  
[Sicherheitsoptionen](#egaa)  
[Ereignisprotokoll](#efaa)  
[Zusätzliche Registrierungseinträge](#eeaa)  
[Eingeschränkte Gruppen](#edaa)  
[Sichern des Dateisystems](#ecaa)  
[Zusätzliche Sicherheitseinstellungen](#ebaa)  
[Zusammenfassung](#eaaa)  



### Überblick

In diesem Kapitel werden die Konfigurationsanforderungen behandelt, die zum Verwalten einer Baseline-Sicherheitsvorlage für alle Server unter Microsoft® Windows Server™ 2003 mit Service Pack 1 (SP1) erforderlich sind. Das Kapitel bietet auch Verwaltungsanweisungen für die Einrichtung und Konfiguration eines sicheren Windows Server 2003 SP1-Systems in drei unterschiedlichen Umgebungen. Die Konfigurationsanforderungen in diesem Kapitel bilden die Grundlage für alle Verfahren, die in späteren Kapiteln dieses Handbuchs beschrieben werden. In diesen Kapiteln wird die Absicherung spezifischer Serverrollen beschrieben.

Die Einstellungsempfehlungen in diesem Kapitel unterstützen Sie bei der Errichtung einer sicheren Grundlage für Geschäftsanwendungsserver in einer Unternehmensumgebung. Vor der Implementierung in der Produktionsumgebung müssen Sie jedoch sorgfältig testen, wie diese Sicherheitskonfigurationen zusammen mit den Geschäftsanwendungen Ihrer Organisation funktionieren.

Die Empfehlungen in diesem Kapitel eignen sich für die meisten Organisationen und können sowohl auf vorhandene als auch auf neue Computer angewendet werden, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die Standardsicherheitskonfigurationen in Windows Server 2003 mit SP1 wurden von den Verfassern dieses Handbuchs untersucht, geprüft und getestet. Informationen zu sämtlichen Standardeinstellungen und eine ausführliche Erläuterung der einzelnen Einstellungen, die in diesem Kapitel diskutiert werden, finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)), das unter [http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) heruntergeladen werden kann. Im Allgemeinen bieten die meisten der folgenden Konfigurationsempfehlungen größere Sicherheit als die Standardeinstellungen.

Die Sicherheitseinstellungen, die in diesem Kapitel diskutiert werden, beziehen sich auf folgende drei Umgebungen:
* **Älterer Client (LC).** Diese Umgebung beinhaltet Computer unter Windows NT® 4.0 und Microsoft Windows® 98, bei denen es sich um *ältere Betriebssysteme* handelt. Obwohl diese Umgebung angemessene Sicherheit bietet, gilt sie als die unsicherste der drei in diesem Handbuch definierten Umgebungen. Zur Erhöhung der Sicherheit können sich Organisationen für eine Migration zur sichereren Unternehmensclient-Umgebung entscheiden. Neben den erwähnten älteren Betriebssystemen verfügt die Umgebung mit älteren Clients auch über Arbeitsstationen mit Windows 2000 Professional und Windows XP. Diese Umgebung enthält nur Domänencontroller unter Windows 2000 oder Windows Server 2003. Windows NT 4.0-Domänencontroller werden in dieser Umgebung nicht verwendet. Es können aber Windows NT-Mitgliedsserver vorhanden sein.

* **Unternehmensclient (EC).** Diese Umgebung bietet solide Sicherheit und wurde für neuere Versionen des Windows-Betriebssystems konzipiert. Die Unternehmensclient-Umgebung umfasst Clientcomputer, auf denen Windows 2000 Professional bzw. Windows XP Professional ausgeführt werden. Der Großteil der Arbeit bei der Migration von einer Umgebung mit älteren Clients zur Unternehmensclient-Umgebung liegt im Aktualisieren der älteren Systeme, wie z. B. Windows 98- und Windows NT 4.0-Arbeitsstationen, auf Windows 2000 oder Windows XP. Alle Domänencontroller und Mitgliedsserver in dieser Umgebung werden unter Windows 2000 Server oder Windows Server 2003 ausgeführt.

* **Hochsicher (SSLF).** Diese Umgebung bietet viel höherer Sicherheit als die Unternehmensclient-Umgebung. Die Migration von der Unternehmensclient-Umgebung zur Hochsicherheitsumgebung erfordert die Einhaltung strenger Sicherheitsrichtlinien im Hinblick auf Clientcomputer und Server. Diese Umgebung enthält Clientcomputer mit Windows 2000 Professional oder Windows XP Professional sowie Domänencontroller unter Windows 2000 Server oder Windows Server 2003. In der Hochsicherheitsumgebung sind die Sicherheitsaspekte so wichtig, dass ein Verlust an Funktionalität und Verwaltbarkeit als akzeptabler Kompromiss angesehen wird, um eine möglichst hohe Sicherheit zu erreichen. Mitgliedsserver in dieser Umgebung werden unter Windows 2000 Server oder Windows Server 2003 ausgeführt.

 

In vielen Fällen wird in der Hochsicherheitsumgebung explizit die Standardeinstellung ausgewählt. Sie müssen damit rechnen, dass sich diese Konfiguration auf die Kompatibilität auswirkt, da es aufgrund des lokalen Anpassens einiger Einstellungen zu Anwendungsfehlern kommen kann. Einige Anwendungen müssen z. B. Zuweisungen von Benutzerrechten anpassen, damit ihrem Dienstkonto zusätzliche Berechtigungen erteilt werden. Da Gruppenrichtlinien Vorrang vor Richtlinien für lokale Computer haben, schlagen diese Vorgänge oft fehl. Sie sollten sämtliche Anwendungen gründlich prüfen, bevor Sie die empfohlenen Einstellungen auf Ihren Produktionscomputern bereitstellen. Dies trifft insbesondere auf Einstellungen für Hochsicherheitsumgebungen zu.

In der folgenden Abbildung werden die drei Sicherheitsumgebungen und die darin jeweils unterstützten Clients aufgezeigt.

![](images/dd443725.sgfg0401(de-de,technet.10).gif)

**Abbildung 4.1: Bestehende und geplante Sicherheitsumgebungen**
 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443725.sgfg0401_big(de-de,technet.10).gif)
Organisationen, die einen auf mehreren Phasen beruhenden Ansatz für die Sicherung ihrer Umgebungen verwenden möchten, können auf der Ebene von Umgebungen mit älteren Clients beginnen und dann schrittweise zu Umgebungen mit höherer Sicherheit übergehen, wenn ihre Anwendungen und Clientcomputer aktualisiert und mit strengeren Sicherheitseinstellungen getestet werden.

Die folgende Abbildung zeigt, wie die INF-Sicherheitsvorlagen als Grundlage für die Mitgliedsserver-Baseline-Richtlinie (MSBP) der Unternehmensclient-Umgebung verwendet werden. In der Abbildung wird auch eine Möglichkeit aufgezeigt, wie diese Richtlinie verknüpft und auf alle Server in einer Organisation angewendet werden kann.

Windows Server 2003 mit SP1 wird mit Standardeinstellungswerten geliefert, deren Konfiguration eine sichere Umgebung gewährleistet. In vielen Fällen werden in diesem Kapitel Einstellungen empfohlen, die sich von den Standardwerten unterscheiden. Es werden in diesem Kapitel auch bestimmte Standardwerte für alle drei Umgebungen erzwungen. Informationen zu sämtlichen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx.


![](images/dd443725.sgfg0402(de-de,technet.10).gif)

**Abbildung 4.2: Die Sicherheitsvorlage Unternehmensclient-Mitgliedsserver-Baseline.inf wird in die Richtlinie für die Mitgliedsserver-Baseline importiert, die dann mit der Mitgliedsserver-Organisationseinheit verknüpft wird.**
 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443725.sgfg0402_big(de-de,technet.10).gif)  
Verfahren zur Absicherung bestimmter Serverrollen werden in den übrigen Kapiteln dieses Handbuchs definiert. Die wichtigsten in diesem Handbuch erläuterten Serverrollen sind folgende:
* Domänencontroller, die DNS-Dienste beinhalten

* Infrastrukturserver, die WINS- und DHCP-Dienste beinhalten

* Dateiserver

* Druckserver

* Webserver, auf denen Internet Information Services (IIS) ausgeführt werden

* Microsoft Internet Authentication Server (IAS)-Server

* Zertifikatdienste (CA)-Server

* Bastion-Hosts

 

Viele der folgenden Einstellungen in der Mitgliedsserver-Baselinie-Richtlinie für die Unternehmensclient-Umgebung gelten auch für die Serverrollen in den drei in diesem Handbuch definierten Umgebungen. Die Sicherheitsvorlagen werden speziell für die Sicherheitsanforderungen der jeweiligen Umgebung zugewiesen. Die folgende Tabelle enthält die Namen der Baseline-Sicherheitsvorlagen für die drei Umgebungen.

**Tabelle 4.1: Baseline-Sicherheitsvorlagen für alle drei Umgebungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Älterer Client - Mitgliedsserver-Baseline.inf

</td>

<td style="border:1px solid black;">


Unternehmensclient - Mitgliedsserver-Baseline.inf

</td>

<td style="border:1px solid black;">


Hochsicher - Mitgliedsserver-Baseline.inf

</td>

</tr>

</table>


Die auf alle drei Umgebungen und daher alle Sicherheitsvorlagen für die **Mitgliedsserver-Baseline** zutreffenden Sicherheitseinstellungen werden im übrigen Teil des Kapitels erläutert.

Die Baseline-Sicherheitsvorlagen bilden auch die Grundlage für die Domänencontroller-Sicherheitsvorlagen, die in Kapitel 5, „Richtlinie für die Domänencontroller-Baseline“, definiert sind. Die Sicherheitsvorlagen für die **Domänencontrollerrolle** umfassen Baseline-Einstellungen für das Gruppenrichtlinienobjekt der Domänencontrollergruppenrichtlinie, das in allen drei Umgebungen mit der Domänencontroller-Organisationseinheit verknüpft ist. Eine ausführliche Anleitung zum Erstellen der Organisationseinheiten und Gruppenrichtlinien und zum anschließenden Importieren der entsprechenden Sicherheitsvorlage in das jeweiligen Gruppenrichtlinienobjekt wird in Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, bereitgestellt.

**Hinweis**: Einige Verfahren zum Absichern von Servern können nicht anhand von Gruppenrichtlinien automatisiert werden. Diese Verfahren werden in diesem Kapitel im Abschnitt „Zusätzliche Sicherheitseinstellungen“ beschrieben.  

[Zum Seitenanfanq](#mainsection)  

### Baseline-Richtlinie für Windows Server 2003

Einstellungen auf der Mitgliedsserver-Organisationseinheitsebene legen die gemeinsamen Einstellungen für alle in diesem Handbuch erläuterten Mitgliedsserverrollen fest. Zum Anwenden dieser Einstellungen können Sie ein Gruppenrichtlinienobjekt erstellen, das mit der Mitgliedsserver-Organisationseinheit, der so genannten Baseline-Richtlinie, verknüpft ist. Durch das Gruppenrichtlinienobjekt wird die Konfiguration von spezifischen Sicherheitseinstellungen auf jedem Server automatisiert. Je nach der Rolle der einzelnen Server ist es erforderlich, die Serverkonten in die entsprechende untergeordnete Organisationseinheit der Mitgliedsserver-Organisationseinheit zu verschieben.

Die folgenden Einstellungen werden in der Reihenfolge beschrieben, in der sie in der Benutzeroberfläche des Sicherheitskonfigurations-Editor-Snap-Ins (SCE) der Microsoft Management Console (MMC) erscheinen.  

[Zum Seitenanfanq](#mainsection)  
### Überwachungsrichtlinie

Administratoren sollten eine Überwachungsrichtlinie erstellen, in der festgelegt wird, welche Sicherheitsereignisse gemeldet und welche Benutzer- oder Computeraktivitäten in festgelegten Ereigniskategorien aufgezeichnet werden sollen. Die Administratoren können dann die sicherheitsrelevanten Aktivitäten überwachen. Dazu gehört z. B. die Überwachung der für Objektzugriffe verwendeten Konten, der An- und Abmeldezeiten der Benutzer sowie der Änderungen, die an den Einstellungen der Überwachungsrichtlinien vorgenommen werden.

Vor dem Implementieren einer Überwachungsrichtlinie müssen Sie entscheiden, welche Ereigniskategorien in Ihrer Umgebung überwacht werden sollen. Die vom Administrator für die Ereigniskategorien ausgewählten Überwachungseinstellungen legen die Überwachungsrichtlinie der Organisation fest. Beim Definieren von Überwachungseinstellungen für bestimmte Ereigniskategorien können Administratoren eine den Sicherheitsanforderungen der Organisation entsprechende Überwachungsrichtlinie erstellen.

Wenn keine Überwachungsrichtlinie festgelegt wurde, ist es schwierig oder unmöglich, die genauen Umstände einer Sicherheitsverletzung zu bestimmen. Sind die Überwachungseinstellungen jedoch so konfiguriert, dass für eine Vielzahl autorisierter Aktivitäten Ereignisse produziert werden, sind die Sicherheitsereignisprotokolle schnell mit unnötigen Daten überfüllt. Die folgenden Empfehlungen und Einstellungsbeschreibungen sollen Ihnen dabei helfen zu bestimmen, was überwacht werden soll, damit die gesammelten Daten relevant sind.

Das Protokollieren fehlgeschlagener Ereignisse bietet häufig wertvollere Informationen als das Protokollieren erfolgreich ausgeführter Ereignisse, da fehlgeschlagene Ereignisse normalerweise auf Fehler hinweisen. Wenn sich ein Benutzer z. B. erfolgreich beim System anmeldet, wird dies in der Regel als normaler Vorgang angesehen. Wenn sich jedoch ein Benutzer mehrfach ohne Erfolg beim System anzumelden versucht, kann dies darauf hinweisen, dass sich ein Angreifer mit den Kontoanmeldeinformationen einer anderen Person unerlaubten Zugriff auf den Computer verschaffen möchte. In den Ereignisprotokollen werden die Ereignisse auf dem Computer aufgezeichnet. Microsoft Windows-Betriebssysteme verfügen über separate Ereignisprotokolle für Anwendungen, Sicherheitsereignisse und Systemereignisse. Im Sicherheitsprotokoll werden Überwachungsereignisse aufgezeichnet. Der Ereignisprotokoll-Container der Gruppenrichtlinie dient zum Definieren von Attributen für die Anwendungs-, Sicherheits- und Systemereignisprotokolle, z. B. maximale Protokollgröße, Zugriffsrechte für jedes Protokoll sowie Einstellungen für die Dauer und Methode der Aufbewahrung.

Vor der Implementierung von Überwachungsprozessen müssen Organisationen entscheiden, wie die Daten erfasst, strukturiert und analysiert werden sollen. Große Mengen von Überwachungsdaten sind nur von Nutzen, wenn ihre Verwendung zuvor geplant wurde. Zudem kann beim Überwachen von Computernetzwerken die Leistung beeinträchtigt werden. Während eine bestimmte Kombination von Einstellungen sich u. U. nur geringfügig auf einen Endbenutzercomputer auswirkt, kann dieselbe Kombination erhebliche Auswirkungen auf einen Server mit hoher Auslastung haben. Daher sollten Sie testen, ob die Leistung beeinträchtigt ist, bevor neue Überwachungseinstellungen in der Produktionsumgebung bereitgestellt werden.

Die folgende Tabelle enthält die empfohlenen Überwachungsrichtlinieneinstellungen für die drei in diesem Handbuch definierten Umgebungen. Die Einstellungen der meisten Werte sind für alle drei Umgebungen ähnlich. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.

Die Überwachungsrichtlinieneinstellungen können in Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien**  
**\Überwachungsrichtlinie**

Eine Zusammenfassung der in diesem Abschnitt beschriebenen Einstellungen finden Sie in der Microsoft Excel®-Arbeitsmappe „Sicherheitseinstellungen unter Windows Server 2003“, die gemeinsam mit dem Handbuch heruntergeladen werden kann. Weitere Informationen zu den Standardeinstellungen und eine ausführliche Erläuterung der einzelnen Einstellungen, die in diesem Abschnitt diskutiert werden, finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)), das unter [http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) heruntergeladen werden kann.

**Tabelle 4.2: Einstellungen für Überwachungsrichtlinien**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldeversuche überwachen

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg Fehler

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kontenverwaltung überwachen

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg Fehler

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldeereignisse überwachen

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg Fehler

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Objektzugriffsversuche überwachen

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Fehler

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Richtlinienänderungen überwachen

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Rechteverwendung überwachen

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Fehler

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Prozessverfolgung überwachen

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

<td style="border:1px solid black;">


Keine Überwachung

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Systemereignisse überwachen

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

<td style="border:1px solid black;">


Erfolg

</td>

</tr>

</table>



#### Anmeldeversuche überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob jede Instanz eines Benutzers, der sich von einem anderen für die Überprüfung des Kontos zuständigen Computer an- oder abmeldet, überwacht werden soll. Durch die Authentifizierung eines Domänenbenutzerkontos auf einem Domänencontroller wird ein Kontoanmeldeereignis erzeugt, das im Sicherheitsprotokoll des Domänencontrollers erfasst wird. Durch die Authentifizierung eines lokalen Benutzers auf einem lokalen Computer wird ein Anmeldeereignis erzeugt, das im lokalen Sicherheitsprotokoll erfasst wird. Abmeldungen werden nicht erfasst.

Die Einstellung **Anmeldeversuche überwachen** ist für die Baseline-Richtlinien für ältere Clients und Unternehmensclients auf den Wert **Erfolg** und für die Hochsicherheitsumgebung sowohl auf **Erfolg** als auch auf **Fehler** gesetzt.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse aufgeführt, die von der Richtlinieneinstellung im Sicherheitsprotokoll erfasst werden. Diese Ereigniskennungen können nützlich sein, wenn Sie benutzerdefinierte Warnmeldungen zum Überwachen beliebigen Softwaresammlung, wie z. B. Microsoft Operations Manager (MOM), erstellen möchten.

**Tabelle 4.3: Ereignisse zu Anmeldeversuchen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


672

</td>

<td style="border:1px solid black;">


Ein AS-Ticket (Authentifizierungsdienstticket) wurde erfolgreich ausgestellt und bestätigt. Unter Windows Server 2003 mit SP1 lautet dieser Ereignistyp für erfolgreiche Anforderungen „Erfolgsüberwachung“ und für fehlgeschlagene Anforderungen „Fehlerüberwachung“.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


673

</td>

<td style="border:1px solid black;">


Ein TGS-Ticket (Ticket-Granting Service, Ticket-genehmigender Dienst) wurde genehmigt. Ein TGS-Ticket wird vom Kerberos Version 5-TGS ausgestellt, der es Benutzern erlaubt, sich bei einem bestimmten Dienst in der Domäne zu authentifizieren. Windows Server 2003 mit SP1 erfasst Erfolge und Fehler für diesen Ereignistyp.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


674

</td>

<td style="border:1px solid black;">


Ein Sicherheitsprinzipal hat ein AS-Ticket oder TGS-Ticket erneuert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


675

</td>

<td style="border:1px solid black;">


Die Vorbestätigung ist fehlgeschlagen. Dieses Ereignis wird in einem Schlüsselverteilungscenter (Key Distribution Center, KDC) erzeugt, wenn ein Benutzer ein falsches Kennwort eingibt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


676

</td>

<td style="border:1px solid black;">


Fehlgeschlagene Anfrage für Authentifizierungsticket. Dieses Ereignis wird von Windows Server 2003 mit SP1 nicht erzeugt. Andere Windows-Versionen zeigen mit diesem Ereignis einen Authentifizierungsfehler an, der nicht auf falsche Anmeldeinformationen zurückzuführen ist.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


677

</td>

<td style="border:1px solid black;">


Ein TGS-Ticket wurde nicht genehmigt. Dieses Ereignis wird unter Windows Server 2003 mit SP1 nicht erzeugt. Für diesen Fall wird ein Fehlerüberwachungsereignis mit der Kennung 672 verwendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


678

</td>

<td style="border:1px solid black;">


Ein Konto wurde erfolgreich einem Domänenkonto zugeordnet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


681

</td>

<td style="border:1px solid black;">


Anmeldefehler. Ein Anmeldeversuch mit einem Domänenkonto wurde unternommen. Dieses Ereignis wird nur von Domänencontrollern erzeugt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


682

</td>

<td style="border:1px solid black;">


Ein Benutzer hat die Verbindung zu einer getrennten Terminalserversitzung wiederhergestellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


683

</td>

<td style="border:1px solid black;">


Ein Benutzer hat eine Terminalserversitzung getrennt, sich jedoch nicht abgemeldet.

</td>

</tr>

</table>



#### Kontenverwaltung überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob jedes Kontenverwaltungsereignis auf einem Computer überwacht werden soll. Beispiele für Kontenverwaltungsereignisse:
* Erstellen, Ändern oder Löschen eines Benutzerkontos oder einer Gruppe

* Umbenennen, Deaktivieren oder Aktivieren eines Benutzerkontos

* Festlegen oder Ändern eines Kennworts

 

Organisationen müssen feststellen können, wer Domänenkonten und lokale Konten erstellt, ändert oder löscht. Nicht autorisierte Änderungen können auf falsche Änderungen durch einen Administrator, der die Richtlinien der Organisation nicht versteht oder befolgt, oder auf absichtliche Angriffe hinweisen.

Kontenverwaltungs-Fehlerereignisse weisen z. B. häufig darauf hin, dass ein Administrator auf niedrigerer Ebene oder ein Angreifer, der sich Zugang zum Konto eines Administrators auf niedrigerer Ebene verschafft hat, versucht, seine Berechtigungen zu erhöhen. Mithilfe der Protokolle können Sie feststellen, welche Konten ein Angreifer geändert und erstellt hat.

Die Einstellung **Kontenverwaltung überwachen** ist für die Baseline-Richtlinien für ältere Clients und Unternehmensclients auf **Erfolg** und für die Baseline-Richtlinie für die Hochsicherheitsumgebung sowohl auf **Erfolg** als auch auf **Fehler** gesetzt.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Richtlinieneinstellung im Sicherheitsprotokoll aufgezeichnet werden. Diese Ereigniskennungen können nützlich sein, wenn Sie benutzerdefinierte Warnmeldungen zum Überwachen einer beliebigen Softwaresammlung, wie z. B. MOM, erstellen möchten. Der Großteil der Betriebsverwaltungssoftware kann mit Skripts so angepasst werden, dass auf diesen Sicherheitskennungen beruhende Ereignisse erfasst oder gekennzeichnet werden.

**Tabelle 4.4: Ereignisse zur Kontoverwaltung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


624

</td>

<td style="border:1px solid black;">


Ein Benutzerkonto wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


627

</td>

<td style="border:1px solid black;">


Ein Benutzerkennwort wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


628

</td>

<td style="border:1px solid black;">


Ein Benutzerkennwort wurde festgelegt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


630

</td>

<td style="border:1px solid black;">


Ein Benutzerkonto wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


631

</td>

<td style="border:1px solid black;">


Eine globale Gruppe wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


632

</td>

<td style="border:1px solid black;">


Einer globalen Gruppe wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


633

</td>

<td style="border:1px solid black;">


Aus einer globalen Gruppe wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


634

</td>

<td style="border:1px solid black;">


Eine globale Gruppe wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


635

</td>

<td style="border:1px solid black;">


Eine neue lokale Gruppe wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


636

</td>

<td style="border:1px solid black;">


Einer lokalen Gruppe wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


637

</td>

<td style="border:1px solid black;">


Aus einer lokalen Gruppe wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


638

</td>

<td style="border:1px solid black;">


Eine lokale Gruppe wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


639

</td>

<td style="border:1px solid black;">


Das Konto einer lokalen Gruppe wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


641

</td>

<td style="border:1px solid black;">


Das Konto einer globalen Gruppe wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


642

</td>

<td style="border:1px solid black;">


Ein Benutzerkonto wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


643

</td>

<td style="border:1px solid black;">


Eine Domänenrichtlinie wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


644

</td>

<td style="border:1px solid black;">


Ein Benutzerkonto wurde automatisch gesperrt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


645

</td>

<td style="border:1px solid black;">


Ein Computerkonto wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


646

</td>

<td style="border:1px solid black;">


Ein Computerkonto wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


647

</td>

<td style="border:1px solid black;">


Ein Computerkonto wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


648    

</td>

<td style="border:1px solid black;">


Es wurde eine lokale Sicherheitsgruppe mit deaktivierter Sicherheit erstellt.

**Hinweis**: SECURITY_DISABLED im formalen Namen bedeutet, dass mit dieser Gruppe keine Berechtigungen für Zugriffsprüfungen erteilt werden können.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


649

</td>

<td style="border:1px solid black;">


Es wurde eine lokale Sicherheitsgruppe mit deaktivierter Sicherheit geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


650

</td>

<td style="border:1px solid black;">


Einer lokalen Sicherheitsgruppe mit deaktivierter Sicherheit wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


651

</td>

<td style="border:1px solid black;">


Aus einer lokalen Sicherheitsgruppe mit deaktivierter Sicherheit wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


652

</td>

<td style="border:1px solid black;">


Eine lokale Gruppe mit deaktivierter Sicherheit wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


653

</td>

<td style="border:1px solid black;">


Eine globale Gruppe mit deaktivierter Sicherheit wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


654

</td>

<td style="border:1px solid black;">


Eine globale Gruppe mit deaktivierter Sicherheit wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


655

</td>

<td style="border:1px solid black;">


Einer globalen Gruppe mit deaktivierter Sicherheit wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


656

</td>

<td style="border:1px solid black;">


Aus einer globalen Gruppe mit deaktivierter Sicherheit wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


657

</td>

<td style="border:1px solid black;">


Eine globale Gruppe mit deaktivierter Sicherheit wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


658

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit aktivierter Sicherheit wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


659

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit aktivierter Sicherheit wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


660

</td>

<td style="border:1px solid black;">


Einer universellen Gruppe mit aktivierter Sicherheit wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


661

</td>

<td style="border:1px solid black;">


Aus einer universellen Gruppe mit aktivierter Sicherheit wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


662

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit aktivierter Sicherheit wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


663

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit deaktivierter Sicherheit wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


664

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit deaktivierter Sicherheit wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


665

</td>

<td style="border:1px solid black;">


Einer universellen Gruppe mit deaktivierter Sicherheit wurde ein Mitglied hinzugefügt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


666

</td>

<td style="border:1px solid black;">


Aus einer universellen Gruppe mit deaktivierter Sicherheit wurde ein Mitglied entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


667

</td>

<td style="border:1px solid black;">


Eine universelle Gruppe mit deaktivierter Sicherheit wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


668

</td>

<td style="border:1px solid black;">


Ein Gruppentyp wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


684    

</td>

<td style="border:1px solid black;">


Der Sicherheitsdeskriptor für administrative Gruppenmitglieder wurde festgelegt.

**Hinweis**: Auf einem Domänencontroller sucht ein Hintergrundthread alle 60 Minuten alle Mitglieder administrativer Gruppen (wie Domänen-, Unternehmens- und Schema-Administratoren) und wendet einen festen Sicherheitsdeskriptor auf sie an. Dieses Ereignis wird protokolliert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


685

</td>

<td style="border:1px solid black;">


Der Name eines Kontos wurde geändert.

</td>

</tr>

</table>



#### Anmeldeereignisse überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob sämtliche An- und Abmeldeereignisse von einem Computer überwacht werden sollen. Die Einstellung **Anmeldeereignisse überwachen** erzeugt auf Domänencontrollern und auf lokalen Computern Einträge zur Überwachung der Domänenkontenaktivitäten bzw. Aktivitäten für lokale Konten.

Wenn Sie die Einstellung **Anmeldeereignisse überwachen** auf **Keine Überwachung** setzen, ist es schwierig oder unmöglich festzustellen, welche Benutzer die Anmeldung bzw. einen Anmeldeversuch bei den Computern in der Organisation vorgenommen haben. Wenn Sie für einem Domänenmitglied den Wert **Erfolg** für die Option **Anmeldeereignisse überwachen** aktivieren, wird immer dann, wenn sich jemand beim Netzwerk anmeldet, ein Ereignis erzeugt, unabhängig davon, wo sich die Konten auf dem Netzwerk befinden. Wenn sich der Benutzer bei einem lokalen Konto anmeldet und **Anmeldeversuche überwachen** auf **Aktiviert** gesetzt ist, werden durch die Anmeldung zwei Ereignisse erzeugt.

Selbst wenn Sie die Standardwerte für diese Richtlinieneinstellung nicht ändern, ist nach einer Sicherheitsverletzung kein Überwachungseintrag als Beweis zur Analyse verfügbar. Die Einstellung **Anmeldeereignisse überwachen** ist in den Baseline-Richtlinien für ältere Clients und Unternehmensclients auf die Werte **Erfolg** und in der Baseline-Richtlinie für die Hochsicherheitsumgebung sowohl auf **Erfolg** als auch auf **Fehler** gesetzt.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Richtlinieneinstellung im Sicherheitsprotokoll aufgezeichnet werden.

**Tabelle 4.5: Ereignisse zur Anmeldeüberwachung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


528

</td>

<td style="border:1px solid black;">


Ein Benutzer hat sich erfolgreich bei einem Computer angemeldet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


529

</td>

<td style="border:1px solid black;">


Anmeldefehler. Es wurde eine Anmeldung mit einem unbekannten Benutzernamen oder einem bekannten Benutzernamen mit einem falschen Kennwort versucht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


530

</td>

<td style="border:1px solid black;">


Anmeldefehler. Ein Anmeldeversuch wurde außerhalb der zulässigen Zeit unternommen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


531

</td>

<td style="border:1px solid black;">


Anmeldefehler. Ein Anmeldeversuch mit einem deaktivierten Konto wurde unternommen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


532

</td>

<td style="border:1px solid black;">


Anmeldefehler. Ein Anmeldeversuch mit einem abgelaufenen Konto wurde unternommen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


533

</td>

<td style="border:1px solid black;">


Anmeldefehler. Ein Benutzer, dem die Anmeldung bei dem entsprechenden Computer nicht erlaubt ist, hat versucht sich anzumelden.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


534

</td>

<td style="border:1px solid black;">


Anmeldefehler. Der Benutzer hat versucht, sich mit einem unzulässigen Kennworttyp anzumelden.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


535

</td>

<td style="border:1px solid black;">


Anmeldefehler. Das Kennwort für das angegebene Konto ist abgelaufen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


536

</td>

<td style="border:1px solid black;">


Anmeldefehler. Der Anmeldedienst ist nicht aktiv.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


537    

</td>

<td style="border:1px solid black;">


Anmeldefehler. Der Anmeldeversuch ist aus anderen Gründen fehlgeschlagen.

**Hinweis**: In einigen Fällen ist der Grund für die fehlgeschlagene Anmeldung möglicherweise nicht bekannt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


538

</td>

<td style="border:1px solid black;">


Die Abmeldung eines Benutzers wurde abgeschlossen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


539

</td>

<td style="border:1px solid black;">


Anmeldefehler. Das Konto wurde beim Anmeldeversuch gesperrt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


540

</td>

<td style="border:1px solid black;">


Ein Benutzer hat sich erfolgreich bei einem Netzwerk angemeldet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


541

</td>

<td style="border:1px solid black;">


Die Internetschlüsselaustausch-Authentifizierung im Hauptmodus zwischen dem lokalen Computer und der aufgeführten Peeridentität wurde abgeschlossen (und eine Sicherheitszuordnung erstellt), oder der Schnellmodus hat einen Datenkanal aufgebaut.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


542

</td>

<td style="border:1px solid black;">


Ein Datenkanal wurde beendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


543    

</td>

<td style="border:1px solid black;">


Der Hauptmodus wurde beendet.

**Hinweis**: Gründe können die zeitliche Beschränkung der Sicherheitszuordnung (die Standardeinstellung lautet acht Stunden) sowie Richtlinienänderungen oder eine Peerbeendigung sein.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


544

</td>

<td style="border:1px solid black;">


Die Authentifizierung im Hauptmodus schlug fehl, da der Peer kein gültiges Zertifikat zur Verfügung stellte oder die Signatur nicht überprüft wurde.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


545

</td>

<td style="border:1px solid black;">


Die Authentifizierung im Hauptmodus schlug aufgrund eines Fehlers des Kerberos-Authentifizierungsprotokolls oder eines ungültigen Kennworts fehl.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


546

</td>

<td style="border:1px solid black;">


Die IKE-Sicherheitszuordnung konnte nicht festgelegt werden, da der Peer einen ungültigen Vorschlag sendete. Es wurde ein Paket empfangen, das ungültige Daten enthielt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


547

</td>

<td style="border:1px solid black;">


Bei einem IKE-Handshake ist ein Fehler aufgetreten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


548

</td>

<td style="border:1px solid black;">


Anmeldefehler. Die Sicherheitskennung (SID) einer vertrauenswürdigen Domäne stimmt nicht mit der SID der Kontendomäne des Clients überein.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


549

</td>

<td style="border:1px solid black;">


Anmeldefehler. Alle SIDs nicht vertrauenswürdiger Namespaces wurden bei einer Authentifizierung der Gesamtstruktur herausgefiltert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


550

</td>

<td style="border:1px solid black;">


Benachrichtigung, die auf einen möglichen DoS-Angriff hinweisen könnte.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


551

</td>

<td style="border:1px solid black;">


Ein Benutzer hat die Abmeldung initiiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


552

</td>

<td style="border:1px solid black;">


Ein Benutzer hat sich erfolgreich mit expliziten Anmeldeinformationen bei einem Computer angemeldet, obwohl er bereits als ein anderer Benutzer angemeldet war.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


682

</td>

<td style="border:1px solid black;">


Ein Benutzer hat die Verbindung zu einer getrennten Terminalserversitzung wieder hergestellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


683    

</td>

<td style="border:1px solid black;">


Ein Benutzer hat eine Terminalserversitzung getrennt, sich jedoch nicht abgemeldet.

**Hinweis**: Dieses Ereignis wird erzeugt, wenn ein Benutzer über das Netzwerk mit einer Terminalserversitzung verbunden ist. Das Ereignis wird auf dem Terminalserver angezeigt.

</td>

</tr>

</table>



#### Objektzugriffsversuche überwachen

Diese Richtlinieneinstellung allein führt nicht zur Überwachung von Ereignissen. Durch die Einstellung **Objektzugriffsversuche überwachen** wird festgelegt, ob Benutzerzugriffe auf Objekte (z. B. Dateien, Ordner, Registrierungsschlüssel, Drucker) mit definierter Systemzugriffssteuerungsliste (SACL) überwacht werden sollen.

Eine SACL besteht aus Zugriffssteuerungseinträgen (ACE). Jeder ACE enthält drei Informationen:
* Den zu überwachenden Sicherheitsprinzipal (Benutzer, Computer oder Gruppe)

* Den zu überwachenden Zugriffstyp (bezeichnet als Zugriffsmaske)

* Ein Flag, das angibt, ob fehlgeschlagene Zugriffsereignisse, erfolgreiche Zugriffsereignisse oder beide Ereignistypen überwacht werden sollen

 

Wenn Sie die Einstellung **Objektzugriffsversuche überwachen** für die Erfassung von **Erfolg**-Werten konfigurieren, wird jedes Mal ein Überwachungseintrag generiert, wenn ein Benutzer erfolgreich auf ein Objekt mit definierter SACL zugreift. Wenn Sie diese Richtlinieneinstellung für die Erfassung von **Fehler**-Werten konfigurieren, wird jedes Mal ein Überwachungseintrag generiert, wenn ein Benutzer erfolglos auf ein Objekt mit definierter SACL zugreift.

Organisationen sollten beim Konfigurieren von SACLs nur jene Aktionen definieren, die aktiviert sein sollen. Es kann z. B. sein, dass Sie die Überwachungseinstellung **Daten schreiben und Daten anhängen** für ausführbare Dateien aktivieren möchten, um Ersetzungen oder Änderungen dieser Dateien zu überwachen, weil Viren, Würmer und Trojaner meist ausführbare Dateien angreifen. Ebenso können Sie Änderungen an wichtigen Dokumenten oder den Zugriff auf solche Dokumente überwachen.

Die Einstellung **Objektzugriffsversuche überwachen** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf den Standardwert **Keine Überwachung** gesetzt. Die Richtlinieneinstellung ist jedoch so konfiguriert, dass **Fehler**-Werte in der Baseline-Richtlinie für die Hochsicherheitsumgebung aufgezeichnet werden.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Richtlinieneinstellung im Sicherheitsprotokoll aufgezeichnet werden.

**Tabelle 4.6: Objektzugriffsereignisse**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


560

</td>

<td style="border:1px solid black;">


Der Zugriff auf ein bereits vorhandenes Objekt wurde gewährt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


562

</td>

<td style="border:1px solid black;">


Ein Handle zu einem Objekt wurde geschlossen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


563    

</td>

<td style="border:1px solid black;">


Es wurde versucht, ein Objekt zu öffnen mit der Absicht dieses zu löschen.

**Hinweis**: Dieses Ereignis wird von Dateisystemen verwendet, wenn das Flag FILE_DELETE_ON_CLOSE in Createfile() festgelegt wurde.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


564

</td>

<td style="border:1px solid black;">


Ein geschütztes Objekt wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


565

</td>

<td style="border:1px solid black;">


Der Zugriff auf einen bereits vorhandenen Objekttyp wurde gewährt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


567    

</td>

<td style="border:1px solid black;">


Es wurde eine mit einem Handle verknüpfte Berechtigung verwendet.

**Hinweis**: Ein Handle wird mit bestimmten Berechtigungen erstellt (wie etwa Lese- und Schreibzugriff). Bei Verwendung des Handles wird für jede verwendete Berechtigung eine Überwachung generiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


568

</td>

<td style="border:1px solid black;">


Es wurde versucht, eine feste Verknüpfung zu einer überwachten Datei zu erstellen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


569

</td>

<td style="border:1px solid black;">


Der Ressourcenmanager des Autorisierungs-Managers hat versucht, einen Clientkontext zu erstellen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


570    

</td>

<td style="border:1px solid black;">


Ein Client hat versucht, auf ein Objekt zuzugreifen.

**Hinweis**: Für jeden Versuch, eine Aktion mit dem Objekt durchzuführen, wird ein Ereignis generiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


571

</td>

<td style="border:1px solid black;">


Der Clientkontext wurde vom Autorisierungs-Manager gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


572

</td>

<td style="border:1px solid black;">


Der Administratormanager hat die Anwendung initialisiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


772

</td>

<td style="border:1px solid black;">


Die Zertifikatsverwaltung hat eine ausstehende Zertifikatsanforderung abgelehnt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


773

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine erneut gestellte Zertifikatanforderung erhalten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


774

</td>

<td style="border:1px solid black;">


Die Zertifikatsdienste haben ein Zertifikat gesperrt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


775

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine Anforderung zur Veröffentlichung der Zertifikatsperrliste erhalten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


776

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben die Zertifikatssperrliste veröffentlicht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


777

</td>

<td style="border:1px solid black;">


Eine Zertifikatsanforderungserweiterung wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


778

</td>

<td style="border:1px solid black;">


Ein oder mehrere Zertifikatanforderungsattribute wurden geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


779

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine Anforderung zum Herunterfahren erhalten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


780

</td>

<td style="border:1px solid black;">


Die Sicherung der Zertifikatdienste wurde gestartet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


781

</td>

<td style="border:1px solid black;">


Die Sicherung der Zertifikatdienste wurde beendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


782

</td>

<td style="border:1px solid black;">


Die Wiederherstellung der Zertifikatdienste wurde gestartet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


783

</td>

<td style="border:1px solid black;">


Die Wiederherstellung der Zertifikatdienste wurde beendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


784

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste wurden gestartet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


785

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste wurden beendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


786

</td>

<td style="border:1px solid black;">


Die Sicherheitsberechtigungen für Zertifikatdienste wurden geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


787

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben einen archivierten Schlüssel wiedergefunden.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


788

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben ein Zertifikat in die Datenbank importiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


789

</td>

<td style="border:1px solid black;">


Der Überwachungsfilter für Zertifikatdienste wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


790

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine Zertifikatanforderung erhalten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


791

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine Zertifikatanforderung genehmigt und ein Zertifikat ausgestellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


792

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben eine Zertifikatanforderung abgelehnt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


793

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben den Status einer Zertifikatanforderung auf "anstehend" festgelegt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


794

</td>

<td style="border:1px solid black;">


Die Zertifikatverwaltungseinstellungen für die Zertifikatdienste wurden geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


795

</td>

<td style="border:1px solid black;">


Es wurde ein Konfigurationseintrag in den Zertifikatdiensten geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


796

</td>

<td style="border:1px solid black;">


Eine Eigenschaft der Zertifikatdienste wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


797

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben einen Schlüssel archiviert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


798

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben einen Schlüssel importiert und archiviert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


799

</td>

<td style="border:1px solid black;">


Die Zertifikatdienste haben das Zertifizierungsstellenzertifikat (CA-Zertifikat) in Active Directory veröffentlicht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


800

</td>

<td style="border:1px solid black;">


Aus der Zertifikatdatenbank wurde mindestens eine Zeile gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


801

</td>

<td style="border:1px solid black;">


Rollentrennung aktiviert

</td>

</tr>

</table>



#### Richtlinienänderungen überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob jede Änderung in Richtlinien für die Zuweisung von Benutzerrechten, in Vertrauensrichtlinien oder in der Überwachungsrichtlinie selbst überwacht wird.

Wenn Sie die Einstellung **Richtlinienänderungen überwachen** für die Erfassung von **Erfolg**-Werten konfigurieren, wird für jede erfolgreiche Änderung in Richtlinien für die Zuweisung von Benutzerrechten, in Überwachungsrichtlinien oder in Vertrauensrichtlinien ein Überwachungseintrag generiert. Wenn Sie diese Richtlinieneinstellung für die Erfassung von **Fehler**-Werten konfigurieren, wird für jede fehlgeschlagene Änderung in Richtlinien für die Zuweisung von Benutzerrechten, in Überwachungsrichtlinien oder in Vertrauensrichtlinien ein Überwachungseintrag generiert.

Die empfohlenen Einstellungen ermöglichen die Anzeige aller Kontenberechtigungen, die ein Angreifer versucht zu erhöhen, indem er z. B. die Berechtigung **Debuggen von Programmen** oder die Berechtigung **Sichern von Dateien und Verzeichnissen** hinzuzufügen versucht.

Die Einstellung **Richtlinienänderungen überwachen** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen zur Erfassung von **Erfolg**-Werten konfiguriert. Derzeit werden bei einer Einstellung auf **Fehler**-Werte keine bedeutungsvollen Ereignisse erfasst.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Richtlinieneinstellung im Sicherheitsprotokoll aufgezeichnet werden.

**Tabelle 4.7: Ereignisse zur Überwachung von Richtlinienänderungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


608

</td>

<td style="border:1px solid black;">


Ein Benutzerrecht wurde zugewiesen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


609

</td>

<td style="border:1px solid black;">


Ein Benutzerrecht wurde entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


610

</td>

<td style="border:1px solid black;">


Eine Vertrauensstellung mit einer anderen Domäne wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


611

</td>

<td style="border:1px solid black;">


Eine Vertrauensstellung mit einer anderen Domäne wurde entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


612

</td>

<td style="border:1px solid black;">


Eine Überwachungsrichtlinie wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


613

</td>

<td style="border:1px solid black;">


Ein Richtlinienagent für die Internetprotokollsicherheit (IPSec) wurde gestartet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


614

</td>

<td style="border:1px solid black;">


Ein IPSsec-Richtlinienagent wurde deaktiviert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


615

</td>

<td style="border:1px solid black;">


Ein IPSec-Richtlinienagent wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


616

</td>

<td style="border:1px solid black;">


Ein IPSec-Richtlinienagent hat einen potenziell schwerwiegenden Fehler entdeckt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


617

</td>

<td style="border:1px solid black;">


Eine Richtlinie von Kerberos Version 5 wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


618

</td>

<td style="border:1px solid black;">


Die Richtlinie zur Wiederherstellung verschlüsselter Daten wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


620

</td>

<td style="border:1px solid black;">


Eine vertrauenswürdige Beziehung zu einer anderen Domäne wurde geändert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


621

</td>

<td style="border:1px solid black;">


Systemzugriff auf ein Konto wurde erteilt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


622

</td>

<td style="border:1px solid black;">


Systemzugriff auf ein Konto wurde entfernt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


623

</td>

<td style="border:1px solid black;">


Die Überwachungsrichtlinie wurde auf Einzelbenutzerbasis festgelegt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


625

</td>

<td style="border:1px solid black;">


Die Überwachungsrichtlinie wurde auf Einzelbenutzerbasis aktualisiert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


768    

</td>

<td style="border:1px solid black;">


Ein Konflikt zwischen einem Namespace-Element in einer Gesamtstruktur und einem Namespace-Element in einer anderen Gesamtstruktur wurde erkannt.  

**Hinweis**: Das Überlappen zweier in verschiedenen Strukturen befindlicher Namespace-Elemente kann zu Mehrdeutigkeiten bei der Namensauflösung für Namespace-Elemente führen. Diese Überlappung wird auch als Konflikt bezeichnet. Nicht alle Parameter sind für jeden Eintragstyp gültig. Felder wie DNS-Name, NetBIOS-Name und SID sind z. B. nicht gültig für einen Eintrag des Typs „TopLevelName“.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


769    

</td>

<td style="border:1px solid black;">


Es wurden vertrauenswürdige Strukturinformationen hinzugefügt.  

**Hinweis**: Diese Ereignisnachricht wird generiert, wenn vertrauenswürdige Strukturinformationen aktualisiert wurden und mindestens ein Eintrag hinzugefügt wurde. Für jeden hinzugefügten, gelöschten oder geänderten Eintrag wird eine Ereignisnachricht generiert. Werden bei einer einzelnen Aktualisierung der vertrauenswürdigen Strukturinformationen mehrere Einträge hinzugefügt, gelöscht oder geändert, wird allen generierten Ereignisnachrichten eine einzelne eindeutige Kennung, die so genannte Vorgangs-ID, zugewiesen. Durch diese Funktion können Sie erkennen, dass die mehrfach generierten Ereignisnachrichten auf einen einzigen Vorgang zurückzuführen sind. Nicht alle Parameter sind für jeden Eintragstyp gültig. Parameter wie DNS-Name, NetBIOS-Name und SID sind z. B. nicht gültig für einen Eintrag des Typs „TopLevelName“.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


770    

</td>

<td style="border:1px solid black;">


Es wurden vertrauenswürdige Strukturinformationen gelöscht.  

**Hinweis**: Siehe Ereignisbeschreibung für Ereignis 769.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


771    

</td>

<td style="border:1px solid black;">


Es wurden vertrauenswürdige Strukturinformationen geändert.  

**Hinweis**: Siehe Ereignisbeschreibung für Ereignis 769.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


805

</td>

<td style="border:1px solid black;">


Dieser Ereignisprotokolldienst hat die Sicherheitsprotokollkonfiguration für eine Sitzung gelesen.

</td>

</tr>

</table>



#### Rechteverwendung überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob jede Ausübung eines Benutzerrechts überwacht wird. Ist die Einstellung **Rechteverwendung überwachen** auf **Erfolg** gesetzt, wird bei jeder erfolgreichen Ausübung eines Benutzerrechts ein Überwachungseintrag generiert. Ist diese Richtlinieneinstellung auf **Fehler** gesetzt, wird bei jeder fehlgeschlagenen Ausübung eines Benutzerrechts ein Überwachungseintrag generiert.

Für die folgenden Benutzerrechte werden auch dann keine Überwachungseinträge generiert, wenn die Einstellung **Rechteverwendung überwachen** konfiguriert ist, da diese Benutzerrechte viele Ereignisse im Sicherheitsprotokoll erzeugen. Die Computerleistung wäre beeinträchtigt, wenn folgende Benutzerrechte überwacht würden:
* Auslassen der durchsuchenden Prüfung

* Debuggen von Programmen

* Erstellen eines Tokenobjekts

* Ersetzen eines Prozessebenentokens

* Generieren von Sicherheitsüberwachungen

* Sichern von Dateien und Verzeichnissen

* Wiederherstellen von Dateien und Verzeichnissen
 

**Hinweis**: Wenn Sie diese Benutzerberechtigungen überwachen möchten, müssen Sie die Sicherheitsoption **Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen** in der Gruppenrichtlinie aktivieren.

 

Die Einstellung **Rechteverwendung überwachen** wird in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf dem Standardwert **Keine Überwachung** belassen. Die Richtlinieneinstellung ist jedoch so konfiguriert, dass **Fehler**-Werte in der Baseline-Richtlinie für die Hochsicherheitsumgebung aufgezeichnet werden. Der fehlgeschlagene Einsatz eines Benutzerrechts weist auf ein globales Netzwerkproblem hin und ist häufig ein Anzeichen für eine versuchte Sicherheitsverletzung. Organisationen sollten **Rechteverwendung überwachen** nur dann auf **Aktivieren** setzen, wenn bestimmte geschäftliche Gründe dies erfordern.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Einstellung im Sicherheitsprotokoll aufgezeichnet werden.

**Tabelle 4.8: Rechteverwendungsereignisse**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


576    

</td>

<td style="border:1px solid black;">


Die angegebenen Rechte wurden dem Zugriffstoken eines Benutzers hinzugefügt.

**Hinweis**: Dieses Ereignis wird generiert, wenn sich der Benutzer anmeldet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


577

</td>

<td style="border:1px solid black;">


Ein Benutzer hat versucht, eine privilegierte Systemdienstoperation auszuführen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


578

</td>

<td style="border:1px solid black;">


Rechte wurden an einem bereits geöffneten Handle eines geschützten Objekts ausgeübt.

</td>

</tr>

</table>



#### Prozessverfolgung überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob detaillierte Überwachungsinformationen für Ereignisse wie Programmaktivierung, Prozessbeendigung, Handleduplizierung und indirekter Objektzugriff erfasst werden. Wenn Sie diese Richtlinieneinstellung auf **Erfolg** setzen, wird bei jedem erfolgreichen Durchführen eines überwachten Prozesses ein Überwachungseintrag generiert. Wenn Sie diese Richtlinieneinstellung auf **Fehler** setzen, wird bei jedem fehlgeschlagenen Durchführen eines überwachten Prozesses ein Überwachungseintrag generiert.

Die Einstellung **Prozessverfolgung überwachen** erzeugt eine große Anzahl von Ereignissen, sodass sie in der Regel auf **Keine Überwachung** gesetzt ist. Diese Einstellung wird auch für die Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen verwendet. Diese Richtlinieneinstellung kann sich jedoch bei einer Reaktion auf Zwischenfälle als sehr nützlich erweisen, da sie eine detaillierte Aufzeichnung der gestarteten Prozesse sowie des Startzeitpunkts bietet.

In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die von der Einstellung im Sicherheitsprotokoll aufgezeichnet werden.

**Tabelle 4.9: Prozessverfolgungsereignisse**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


592

</td>

<td style="border:1px solid black;">


Ein neuer Vorgang wurde erstellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


593

</td>

<td style="border:1px solid black;">


Ein Vorgang wurde beendet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


594

</td>

<td style="border:1px solid black;">


Ein Handle zu einem Objekt wurde dupliziert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


595

</td>

<td style="border:1px solid black;">


Indirekter Zugriff auf ein Objekt war erfolgreich.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


596    

</td>

<td style="border:1px solid black;">


Ein Datensicherungs-Hauptschlüssel wurde gesichert.

**Hinweis**: Der Hauptschlüssel wird von den Routinen „CryptProtectData“ und „CryptUnprotectData“ sowie dem verschlüsselnden Dateisystem (EFS) verwendet. Der Hauptschlüssel wird gesichert, sobald ein neuer Schlüssel erstellt wird. (Die Standardeinstellung beträgt 90 Tage.) Der Schlüssel wird in der Regel von einem Domänencontroller gesichert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


597

</td>

<td style="border:1px solid black;">


Ein Datensicherungs-Hauptschlüssel wurde von einem Wiederherstellungsserver wiederhergestellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


598

</td>

<td style="border:1px solid black;">


Überwachbare Daten wurden geschützt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


599

</td>

<td style="border:1px solid black;">


Überwachbare Daten waren nicht geschützt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


600

</td>

<td style="border:1px solid black;">


Einem Prozess wurde ein primärer Token zugewiesen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


601

</td>

<td style="border:1px solid black;">


Ein Benutzer hat versucht, einen Dienst zu installieren.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


602

</td>

<td style="border:1px solid black;">


Ein Zeitplanauftrag wurde erstellt.

</td>

</tr>

</table>



#### Systemereignisse überwachen

Durch diese Richtlinieneinstellung wird festgelegt, ob das Neustarten und Herunterfahren eines Computers bzw. Ereignisse, die Computersicherheit oder das Sicherheitsprotokoll betreffen, überwacht werden. Wenn Sie diese Richtlinieneinstellung auf **Erfolg** setzen, wird ein Überwachungseintrag generiert, wenn ein Systemereignis erfolgreich ausgeführt wurde. Wenn Sie diese Richtlinieneinstellung auf **Fehler** setzen, wird ein Überwachungseintrag generiert, wenn die Ausführung eines Systemereignisses fehlgeschlagen ist.

In der folgenden Tabelle sind die nützlichsten, erfolgreich ausgeführten Ereignisse für diese Einstellung aufgeführt.

**Tabelle 4.10: Systemereignismeldungen zum Überwachen von Systemereignissen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Ereigniskennung

</th>

<th style="border:1px solid black;">

Ereignisbeschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


512

</td>

<td style="border:1px solid black;">


Windows wird gestartet.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


513

</td>

<td style="border:1px solid black;">


Windows wird heruntergefahren.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


514

</td>

<td style="border:1px solid black;">


Ein Authentifizierungspaket wurde durch die lokale Sicherheitsinstanz geladen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


515

</td>

<td style="border:1px solid black;">


Ein vertrauenswürdiger Anmeldevorgang wurde bei der lokalen Sicherheitsinstanz registriert.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


516

</td>

<td style="border:1px solid black;">


Die für die Warteschlangenverarbeitung von Sicherheitsereignismeldungen reservierten internen Ressourcen sind ausgelastet. Der Verlust von einigen Sicherheitsereignismeldungen ist eingetreten.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


517

</td>

<td style="border:1px solid black;">


Das Überwachungsprotokoll wurde gelöscht.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


518

</td>

<td style="border:1px solid black;">


Die Sicherheitskontenverwaltung hat ein Benachrichtigungspaket geladen.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


519

</td>

<td style="border:1px solid black;">


Ein Prozess verwendet einen ungültigen Port für den Lokalprozeduraufruf (LPC) und versucht, die Identität eines Clients anzunehmen und einen Clientadressraum zu lesen oder darauf zu antworten oder zu schreiben.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


520    

</td>

<td style="border:1px solid black;">


Die Systemzeit wurde geändert.

**Hinweis**: Diese Überwachung wird in der Regel zweimal durchgeführt.

</td>

</tr>

</table>

[Zum Seitenanfanq](#mainsection)  



### Zuweisen von Benutzerrechten

Die Einstellungen für die Zuweisung von Benutzerrechten versorgen Benutzer und Gruppen mit Anmelderechten oder Berechtigungen für die Computer in der Organisation. Ein Beispiel für ein Anmelderecht ist das Recht, sich an einem Computer interaktiv anzumelden. Ein Beispiel für eine Berechtigung ist das Recht, einen Computer herunterzufahren. Beide Arten werden Benutzern oder Gruppen durch Administratoren als Teil der Sicherheitseinstellungen eines Computers zugewiesen.

**Hinweis**: In diesem Abschnitt gilt „Nicht definiert“ nur für Benutzer. Administratoren besitzen weiterhin das Benutzerrecht. Lokale Administratoren können Änderungen vornehmen, alle domänenbasierten Gruppenrichtlinieneinstellungen haben jedoch Vorrang, wenn diese aktualisiert oder erneut angewendet werden.

Die Einstellungen für die Zuweisung von Benutzerrechten können in Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien**  
**\Zuweisen von Benutzerrechten**

Für die verschiedenen Servertypen in der Organisation gelten unterschiedliche Standardeinstellungen für die Zuweisung von Benutzerrechten. Windows Server 2003 weist z. B. vordefinierten Gruppen auf Mitgliedsservern und Domänencontrollern unterschiedliche Rechte zu. (Ähnlichkeiten zwischen vordefinierten Gruppen auf verschiedenen Servertypen sind in der folgenden Liste nicht dokumentiert.)
* **Mitgliedsserver**
    - **Hauptbenutzer.**   Besitzen mit einigen Einschränkungen die meisten Verwaltungsrechte. Hauptbenutzer können neben Anwendungen, die für Windows Server 2003 mit SP1 oder Windows XP zertifiziert sind, auch ältere Anwendungen ausführen.

    - **Hilfedienstgruppe.**   Die Gruppe für das Hilfe- und Supportcenter. Support_388945a0 ist standardmäßig ein Mitglied dieser Gruppe.

    - **Telnet-Clients.**   Mitglieder dieser Gruppe haben Zugriff auf den Telnet-Server im Netzwerk.


* **Domänencontroller**
    - **Server-Operatoren.**   Mitglieder dieser Gruppen können Domänenserver verwalten.

    - **Terminalserver-Lizenzserver.**   Mitglieder dieser Gruppe haben Zugriff auf Terminalserver-Lizenzserver im Netzwerk.

    - **Windows-Autorisierungszugriffsgruppe.**  Mitglieder dieser Gruppe haben Zugriff auf das berechnete tokenGroupsGlobalAndUniversal-Attribut von Benutzerobjekten.



Die Gruppe **Gäste** und die Benutzerkonten „Gast“ und „Support_388945a0“ besitzen in unterschiedlichen Domänen jeweils eindeutige SIDs. Daher muss diese Gruppenrichtlinie für die Zuweisung von Benutzerrechten u. U. auf einem Computer geändert werden, auf dem nur die spezifische Zielgruppe vorhanden ist. Alternativ dazu können die Richtlinienvorlagen auch einzeln bearbeitet werden, um die entsprechenden Gruppen in die INF-Dateien einzuschließen. Eine Gruppenrichtlinie für Domänencontroller könnte z. B. auf einem Domänencontroller in einer Testumgebung erstellt werden.

**Hinweis**: Aufgrund der eindeutigen SIDs für Mitglieder der Gruppe **Gäste**, „Support_388945a0“ und „Gast“ können einige Einstellungen zum Absichern von Servern anhand der in diesem Handbuch enthaltenen Sicherheitsvorlagen nicht automatisiert werden. Diese Einstellungen werden im Abschnitt „Zusätzliche Sicherheitseinstellungen“ weiter unten in diesem Kapitel beschrieben.

Dieser Abschnitt enthält eine ausführliche Beschreibung der empfohlenen MSBP-Einstellungen für die Zuweisung von Benutzerrechten für alle drei in diesem Handbuch definierten Umgebungen. Eine Zusammenfassung der in diesem Abschnitt beschriebenen Einstellungen finden Sie in der Microsoft Excel-Arbeitsmappe „Sicherheitseinstellungen unter Windows Server 2003“, die gemeinsam mit dem Handbuch heruntergeladen werden kann. Informationen zu den Standardeinstellungen und ausführliche Erklärungen zu den in diesem Abschnitt beschriebenen Einstellungen finden Sie im Begleithandbuch *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server* *2003 und Windows* *XP.*

Die folgende Tabelle enthält die empfohlenen Einstellungen für die Zuweisung von Benutzerrechten für die drei in diesem Handbuch definierten Umgebungen. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.

**Tabelle 4.11: Empfehlungen zu den Einstellungen für die Zuweisung von Benutzerrechten**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Auf diesen Computer vom Netzwerk aus zugreifen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren, Authentifizierte Benutzer, Domänencontroller der Organisation

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Einsetzen als Teil des Betriebssystems

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anpassen von Speicherkontingenten für einen Prozess

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren, NETZWERKDIENST, LOKALER DIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokal anmelden zulassen

</td>

<td style="border:1px solid black;">


Administratoren, Sicherungs-Operatoren, Hauptbenutzer

</td>

<td style="border:1px solid black;">


Administratoren, Sicherungs-Operatoren, Hauptbenutzer

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldung über Terminaldienste zulassen

</td>

<td style="border:1px solid black;">


Administratoren und Remotedesktopbenutzer

</td>

<td style="border:1px solid black;">


Administratoren und Remotedesktopbenutzer

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Sichern von Dateien und Verzeichnissen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Auslassen der durchsuchenden Prüfung

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Authentifizierte Benutzer

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Ändern der Systemzeit

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Auslagerungsdatei erstellen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Erstellen eines Tokenobjekts

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Globale Objekte erstellen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren, DIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Permanente freigegebene Objekte erstellen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Debuggen von Programmen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Den Zugriff auf diesen Computer vom Netzwerk aus verweigern

</td>

<td style="border:1px solid black;">


ANONYME ANMELDUNG; Gäste; Support_388945a0;

Alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


ANONYME ANMELDUNG; Gäste; Support_388945a0;

Alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


ANONYME ANMELDUNG; Gäste; Support_388945a0;

Alle betriebssystemfremden Dienstkonten

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmelden als Batchauftrag verweigern

</td>

<td style="border:1px solid black;">


Gäste; Support_388945a0

</td>

<td style="border:1px solid black;">


Gäste; Support_388945a0

</td>

<td style="border:1px solid black;">


Gäste; Support_388945a0;

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldung als Dienst verweigern

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokale Anmeldung verweigern

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Gäste; Support_388945a0;

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldung über Terminaldienste verweigern

</td>

<td style="border:1px solid black;">


Gäste

</td>

<td style="border:1px solid black;">


Gäste

</td>

<td style="border:1px solid black;">


Gäste

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Computer und Benutzerkonten für Delegierungszwecke vertrauen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Erzwingen des Herunterfahrens von einem Remotesystem aus

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Generieren von Sicherheitsüberwachungen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


NETZWERKDIENST, LOKALER DIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Annehmen der Clientidentität nach Authentifizierung

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren, DIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anheben der Zeitplanungspriorität

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Laden und Entfernen von Gerätetreibern

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Seiten im Speicher sperren

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmelden als Stapelverarbeitungsauftrag

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Als Dienst anmelden

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


NETZWERKDIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Verwalten von Überwachungs- und Sicherheitsprotokoll

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Firmware-Umgebungsvariablen ändern

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Wartungsaufgaben für Speichermedien ausführen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Einzelprozessprofil erstellen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Erstellen eines Profils der Systemleistung

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Entfernen eines Computers aus der Dockingstation

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Ersetzen eines Prozessebenentokens

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


LOKALER DIENST, NETZWERKDIENST

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Wiederherstellen von Dateien und Verzeichnissen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


System herunterfahren

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Synchronisieren von Verzeichnisdienstdaten

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Niemand

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Übernehmen des Besitzes an Dateien und Objekten

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

</table>



#### Auf diesen Computer vom Netzwerk aus zugreifen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer und Gruppen eine Verbindung zu dem Computer über das Netzwerk herstellen dürfen. Sie ist für eine Reihe von Netzwerkprotokollen erforderlich. Hierzu zählen SMB-basierte Protokolle (Server Message Block), NetBIOS, CIFS (Common Internet File System), HTTP und COM+ (Component Object Model Plus).

Die Einstellung **Auf diesen Computer vom Netzwerk aus zugreifen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. Berechtigungen, die in Windows Server 2003 mit SP1 der Sicherheitsgruppe **Jeder** zugewiesen wurden, bieten anonymen Benutzern zwar keinen Zugriff mehr, aber Gastgruppen und -konten können weiterhin über die Sicherheitsgruppe **Jeder** Zugriff erhalten. Aus diesem Grund wird der Sicherheitsgruppe **Jeder** in der Hochsicherheitsumgebung das Benutzerrecht **Auf diesen Computer vom Netzwerk aus zugreifen** verweigert. Der Schutz vor Angriffen auf den Gastzugriff zur Domäne wird dadurch verbessert. In der Hochsicherheitsumgebung werden diese Benutzerrechte nur den Gruppen **Administratoren**, **Authentifizierte Benutzer** und **DOMÄNENCONTROLLER DER ORGANISATION** zugewiesen.


#### Einsetzen als Teil des Betriebssystems

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Prozess die Identität eines beliebigen Benutzers annehmen und dadurch Zugriff auf die dem Benutzer zugänglichen Ressourcen erlangen kann. Normalerweise erfordern nur einfache Authentifizierungsdienste dieses Benutzerrecht.

Das Benutzerrecht **Einsetzen als Teil des Betriebssystems** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung allerdings auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch wird dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto gewährt.


#### Anpassen von Speicherkontingenten für einen Prozess

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer das maximale Arbeitsspeicherkontingent, das für einen Prozess zur Verfügung steht, anpassen können. Sie ist bei Anpassung des Computers von Nutzen, kann allerdings missbraucht werden. Ein Angreifer könnte dieses Benutzerrecht ausnutzen, um eine DoS-Attacke zu starten.

Die Einstellung **Anpassen von Speicherkontingenten für einen Prozess** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur den Gruppen **Administrator**, NETZWERKDIENST und LOKALER DIENST zugewiesen.


#### Lokal anmelden zulassen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer sich interaktiv bei dem angegebenen Computer anmelden können. Der Benutzer benötigt dieses Benutzerrecht, um sich durch Drücken der Tastenkombination STRG+ALT+ENTF anmelden zu können. Jedes Konto mit diesem Benutzerrecht kann zur Anmeldung an der lokalen Konsole des Computers verwendet werden.

Das Benutzerrecht **Lokal anmelden zulassen** ist in Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf die Gruppen **Administratoren**, **Sicherungs-Operatoren** und **Hauptbenutzer** beschränkt. Dadurch wird verhindert, dass sich unautorisierte Benutzer anmelden können, die ihre Berechtigungsebene erhöhen oder Viren in die Umgebung einschleusen möchten. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen.


#### Anmeldung über Terminaldienste zulassen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer oder Gruppen sich als Terminaldiensteclients anmelden können.

Für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen ist das Benutzerrecht **Anmeldung über Terminaldienste zulassen** auf die Gruppen **Administratoren** und **Remotedesktopbenutzer** beschränkt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur Mitgliedern der Gruppe **Administratoren** zugeteilt.


#### Sichern von Dateien und Verzeichnissen

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer Berechtigungen für Dateien und Verzeichnisse umgehen können, um den Computer zu sichern. Sie wird nur verwendet, wenn eine Anwendung versucht, über das NTFS-Sicherungs-API Zugriff zu erlangen, z. B. mit einem Sicherungsprogramm wie NTBACKUP.EXE. Andernfalls gelten die normalen Berechtigungen für Dateien und Verzeichnisse.

Die Einstellung **Sichern von Dateien und Verzeichnissen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen.


#### Auslassen der durchsuchenden Prüfung

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer Ordner durchsuchen können, ohne dass bei der Navigation über einen Objektpfad im NTFS-Dateisystem oder in der Registrierung die spezielle Berechtigung „Ordner durchsehen“ überprüft wird. Das Benutzerrecht ermöglicht dem Benutzer nicht, den Inhalts eines Ordners anzuzeigen. Der Benutzer ist nur berechtigt, die entsprechenden Verzeichnisse zu passieren.

Die Einstellung **Auslassen der durchsuchenden Überprüfung** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Authentifizierte Benutzer** zugewiesen.


#### Ändern der Systemzeit

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Uhrzeit und das Datum der internen Uhr des Computers ändern können. Benutzer, denen dieses Benutzerrecht zugewiesen wird, können die Ausgabe der Ereignisprotokolle beeinflussen, die von der internen Uhr des Computers mit einem Zeitstempel versehen werden. Wenn die Zeit des Computers geändert wird, enthalten die Protokolle nicht die Zeit, zu der Ereignisse tatsächlich aufgetreten sind.

Die Einstellung **Ändern der Systemzeit** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen.

**Hinweis**: Abweichungen zwischen der Uhrzeit auf dem lokalen Computer und der Uhrzeit auf den Domänencontrollern können beim Kerberos-Authentifizierungsprotokoll Probleme verursachen. Dies kann dazu führen, dass Benutzer sich nicht mehr bei der Domäne anmelden können oder nach der Anmeldung nicht für den Zugriff auf Domänenressourcen autorisiert werden.


#### Auslagerungsdatei erstellen

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer eine Auslagerungsdatei erstellen und ihre Größe anpassen können. Dazu legt der Benutzer im Dialogfeld **Systemeigenschaften** auf der Registerkarte **Erweitert** im Feld **Leistungsoptionen** für bestimmte Laufwerke eine Auslagerungsdateigröße fest.

Die Einstellung **Auslagerungsdatei erstellen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen.


#### Erstellen eines Tokenobjekts

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Prozess ein Token erstellen kann. Wenn der Prozess NtCreateToken() oder andere APIs zur Tokenerstellung verwendet, kann anschließend mithilfe dieses Tokens auf alle lokalen Ressourcen zugegriffen werden.

Die Einstellung **Erstellen eines Tokenobjekts** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.


#### Globale Objekte erstellen

Diese Richtlinieneinstellung lässt zu, dass Benutzer globale Objekte erstellen, die in allen Sitzung zur Verfügung stehen. Benutzer haben auch ohne dieses Recht die Möglichkeit, für ihre Sitzungen spezifische Objekte zu erstellen.

Die Einstellung **Globale Objekte erstellen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt Für die Hochsicherheitsumgebung wird dieses Benutzerrecht nur den Gruppen **DIENST** und **Administratoren** zugewiesen.


#### Permanente freigegebene Objekte erstellen

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer Verzeichnisobjekte im Objekt-Manager erstellen können, also das Recht zur Erstellung von Ordnern, Druckern und anderen Objekten besitzen. Sie ist für Kernelmoduskomponenten von Nutzen, die den Objekt-Namespace erweitern. Diese Komponenten beinhalten dieses Benutzerrecht automatisch. Deshalb ist es in der Regel nicht erforderlich, dieses Benutzerrecht Benutzern ausdrücklich zuzuweisen.

Die Einstellung **Permanente freigegebene Objekte erstellen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.


#### Debuggen von Programmen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer einen Prozess oder den Kernel debuggen können. Sie bietet Zugriff auf wichtige Komponenten des Betriebssystems. In Produktionsumgebungen sollte nur in extremen Fällen ein Debugging stattfinden, z. B. zur Problembehandlung einer für das Geschäft notwendigen Anwendung, die in der Testumgebung nicht effektiv beurteilt werden kann.

Die Einstellung **Debuggen von Programmen** ist für die Umgebung mit älteren Clients auf **Nicht definiert** gesetzt. In der Unternehmensclient-Umgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.

**Hinweis**: Unter Windows Server 2003 mit SP1 kann das Entfernen des Benutzerrechts **Debuggen von Programmen** dazu führen, dass der Windows-Update-Dienst nicht verwendet werden kann. Patches können jedoch weiterhin manuell heruntergeladen und installiert oder auf anderen Wegen angewendet werden. Das Entfernen dieses Benutzerrechts kann auch den Clusterdienst beeinträchtigen. Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel [Anwenden strengerer Sicherheitseinstellungen auf einem Windows Server 2003-basierten Clusterserver](http://support.microsoft.com/kb/891597/en-us) (in englischer Sprache) unter [http://support.microsoft.com/kb/891597/en-us](http://support.microsoft.com/kb/891597/en-us).


#### Den Zugriff auf diesen Computer vom Netzwerk aus verweigern

**Hinweis**: Die Konten ANONYME ANMELDUNG, „Vordefinierter Administrator“, „Support_388945a0“ und „Gast“ sowie alle betriebssystemfremden Dienstkonten sind nicht in der INF-Sicherheitsvorlage enthalten. Diese Konten und Gruppen besitzen für jede Domäne in der Organisation eindeutige SIDs. Daher müssen sie manuell hinzugefügt werden. Weitere Informationen finden Sie im Abschnitt „Manuelle Absicherungsverfahren“ am Ende dieses Kapitels.

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer über das Netzwerk auf Computer zugreifen können. Dabei können eine Reihe von Netzwerkprotokollen, einschließlich SMB-basierter Protokolle, NetBIOS, CIFS, HTTP und COM+ nicht verwendet werden. Diese Richtlinieneinstellung ersetzt das Benutzerrecht **Auf diesen Computer vom Netzwerk aus zugreifen**, wenn ein Benutzerkonto beiden Einstellungen unterliegt.

Für alle drei in diesem Handbuch definierten Umgebungen wird das Benutzerrecht **Den Zugriff auf diesen Computer vom Netzwerk aus verweigern** den Gruppen **Gäste**, ANONYME ANMELDUNG und „Support_388945a0“ sowie allen Dienstkonten, die nicht Teil des Betriebssystems sind, zugewiesen.

Die Konfiguration dieser Richtlinieneinstellung für andere Gruppen kann dazu führen, dass die Möglichkeiten von Benutzern mit speziellen Administratorrollen in der Umgebung eingeschränkt sind. Sie müssen sicherstellen, dass dies keine negativen Auswirkungen auf delegierte Aufgaben hat.


#### Anmeldung als Batchauftrag verweigern

**Hinweis**: Die Konten ANONYME ANMELDUNG, „Vordefinierter Administrator“, „Support_388945a0“ und „Gast“ sowie alle betriebssystemfremden Dienstkonten sind nicht in der INF-Sicherheitsvorlage enthalten. Diese Konten und Gruppen besitzen für jede Domäne in der Organisation eindeutige SIDs. Daher müssen sie manuell hinzugefügt werden. Weitere Informationen finden Sie im Abschnitt „Manuelle Absicherungsverfahren“ am Ende dieses Kapitels.

Durch diese Richtlinieneinstellung wird festgelegt, welche Konten sich beim Computer nicht als Stapelverarbeitungsauftrag anmelden können. Ein Stapelverarbeitungsauftrag ist keine Batchdatei (BAT), sondern eine Batchwarteschlangeneinrichtung. Dieses Benutzerrecht wird von Konten benötigt, die den Taskplaner zum Planen von Aufgaben verwenden.

Das Benutzerrecht **Anmeldung als Batchauftrag verweigern** setzt das Benutzerrecht **Anmelden als Stapelverarbeitungsauftrag** außer Kraft, das das Planen von Aufträgen ermöglichen könnte, die extrem viel Systemressourcen verbrauchen. Dies könnte einen Denial-of-Service verursachen. Deshalb wird das Benutzerrecht **Anmeldung als Batchauftrag verweigern** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen der Gruppe **Gäste** und dem Benutzerkonto „Support_388945a0“ zugewiesen. Wenn Sie die Zuweisung des Benutzerrechts an die empfohlenen Konten unterlassen, kann dies ein Sicherheitsrisiko darstellen.


#### Anmeldung als Dienst verweigern

Durch diese Richtlinieneinstellung wird festgelegt, ob innerhalb des angegebenen Kontos Dienste gestartet werden können.

Die Einstellung **Anmeldung als Dienst verweigern** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.


#### Lokale Anmeldung verweigern

Durch diese Richtlinieneinstellung wird festgelegt, ob sich Benutzer direkt über die Computertastatur anmelden können.

Die Einstellung **Lokale Anmeldung verweigern** ist für Umgebungen mit älteren Clients oder Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. Dieses Benutzerrecht wird in der Hochsicherheitsumgebung jedoch nur der Gruppe **Gäste** und dem Benutzerkonto „Support_388945a0“ zugewiesen. Wenn Sie die Zuweisung des Benutzerrechts an die empfohlenen Konten unterlassen, kann dies ein Sicherheitsrisiko darstellen.


#### Anmeldung über Terminaldienste verweigern

**Hinweis**: Die Konten ANONYME ANMELDUNG, „Vordefinierter Administrator“, „Support_388945a0“ und „Gast“ sowie alle betriebssystemfremden Dienstkonten sind nicht in der INF-Sicherheitsvorlage enthalten. Diese Konten und Gruppen besitzen für jede Domäne in der Organisation eindeutige SIDs. Daher müssen sie manuell hinzugefügt werden. Weitere Informationen finden Sie im Abschnitt „Manuelle Absicherungsverfahren“ am Ende dieses Kapitels.

Durch diese Richtlinieneinstellung wird festgelegt, ob sich Benutzer als Terminaldiensteclients anmelden können. Nachdem Sie den Baseline-Mitgliedsserver einer Domänenumgebung hinzugefügt haben, müssen keine lokalen Konten für den Netzwerkzugriff auf den Server verwendet werden. Domänenkonten können zur Verwaltung und Endbenutzerverarbeitung auf den Server zugreifen.

Für alle drei in diesem Handbuch definierten Umgebungen wird der Gruppe **Gäste** das Benutzerrecht **Anmeldung über Terminaldienste verweigern** zugewiesen, damit eine Anmeldung über Terminaldienste nicht möglich ist.


#### Computer und Benutzerkonten für Delegierungszwecke vertrauen

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Einstellung **Für Delegierungszwecke vertraut** für einen Benutzer oder ein Computerobjekt in Active Directory ändern können. Benutzer oder Computer, denen dieses Benutzerrecht gewährt wird, müssen auch Schreibzugriff auf die Kontosteuerungsflags des Objekts haben. Der Missbrauch dieses Benutzerrechts kann dazu führen, dass nicht autorisierte Benutzer die Identität anderer Benutzer im Netzwerk annehmen.

Die Einstellung **Computer und Benutzerkonten für Delegierungszwecke vertrauen** ist für Umgebungen mit älteren Clients oder Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Erzwingen des Herunterfahrens von einem Remotesystem aus

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer einen Computer von einem Remotestandort im Netzwerk aus herunterfahren können. Jeder Benutzer, der einen Computer herunterfahren kann, könnte einen Denial-of-Service verursachen. Daher sollte dieses Benutzerrecht streng beschränkt werden.

Die Einstellung **Erzwingen des Herunterfahrens von einem Remotesystem aus** ist für Umgebungen mit älteren Clients oder Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur der Gruppe **Administratoren** zugewiesen.


#### Generieren von Sicherheitsüberwachungen

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Prozess Überwachungseinträge im Sicherheitsprotokoll erzeugen kann. Da das Sicherheitsprotokoll zum Verfolgen von unautorisiertem Systemzugriff dienen kann, könnten Konten mit Schreibzugriff auf das Sicherheitsprotokoll verwendet werden, um dieses Protokoll mit sinnlosen Ereignissen zu füllen. Wenn Sie den Computer zum bedarfsabhängigen Überschreiben von Ereignissen konfigurieren, kann ein Angreifer mit dieser Funktion Beweise für seine unautorisierten Aktivitäten entfernen. Wenn Sie den Computer so konfigurieren, dass er herunterfährt, wenn im Sicherheitsprotokoll keine Ereignisse erfasst werden können, kann ein Angreifer diese Funktion einsetzen, um einen Denial-of-Service zu verursachen.

Die Einstellung **Generieren von Sicherheitsüberwachungen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht nur den Konten NETZWERKDIENST und LOKALER DIENST zugewiesen.  


#### Annehmen der Clientidentität nach Authentifizierung

Durch diese Richtlinieneinstellung wird festgelegt, ob im Auftrag eines authentifizierten Benutzers ausgeführte Anwendungen die Identität von Clients annehmen können. Wenn dieses Benutzerrecht für diese Art von Identitätswechsel erforderlich ist, können unautorisierte Benutzer einen Client nicht dazu verleiten, eine Verbindung mit einem von ihnen erstellten Dienst herzustellen (z. B. durch einen Remoteprozeduraufruf oder durch Named Pipes), damit sie die Identität des Clients annehmen können. Der nicht autorisierte Benutzer könnte diese Möglichkeit zum Erhöhen seiner Berechtigungen auf Verwaltungs- oder Systemebene verwenden.

Die Einstellung **Annehmen der Clientidentität nach Authentifizierung** ist für die Umgebung mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** und dem Konto DIENST zugewiesen.


#### Anheben der Zeitplanungspriorität

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Basisprioritätsklasse eines Prozesses erhöhen können. Das Erhöhen der relativen Priorität innerhalb einer Prioritätsklasse ist keine privilegierter Vorgang. Die mit dem Betriebssystem gelieferten Verwaltungsprogramme erfordern dieses Benutzerrecht nicht, es ist jedoch u. U. für Softwareentwicklungstools erforderlich. Ein Benutzer, dem diese Benutzerrechte zugewiesen wurden, kann die Zeitplanungspriorität eines Prozesses in Echtzeit erhöhen und wenig Verarbeitungszeit für alle anderen Prozesse zur Verfügung stellen, wodurch ein Denial-of-Service verursacht werden kann.

Die Einstellung **Anheben der Zeitplanungspriorität** wird für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Laden und Entfernen von Gerätetreibern

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer Gerätetreiber dynamisch laden und entfernen können. Das Benutzerrecht ist nicht erforderlich, wenn ein signierter Treiber für die neue Hardware bereits in der Datei Driver.cab auf dem Computer vorhanden ist. Gerätetreiber werden als hoch privilegierter Code ausgeführt. Ein Benutzer, dem das Benutzerrecht **Laden und Entfernen von Gerätetreibern** zugewiesen wurde, kann unbeabsichtigt oder absichtlich schädlichen, als Gerätetreiber getarnten Code installieren. (Administratoren sollten vorsichtiger vorgehen und nur Treiber mit bestätigten digitalen Signaturen installieren.)

Die Einstellung **Laden und Entfernen von Gerätetreibern** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Seiten im Speicher sperren

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Prozess Daten im physischen Speicher ablegen kann, wodurch der Computer daran gehindert wird, die Daten in einen virtuellen Speicher auf der Festplatte auszulagern. Dies könnte die Leistung stark beeinträchtigen. Benutzer, denen dieses Benutzerrecht zugewiesen wurde, können mehreren Prozessen physischen Speicher zuweisen, wodurch wenig RAM (Random Access Memory) für andere Prozesse verbleibt und ein Denial-of-Service verursacht werden kann.

Die Einstellung **Seiten im Speicher sperren** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.


#### Als Dienst anmelden

Durch diese Richtlinieneinstellung wird festgelegt, ob sich ein Sicherheitsprinzipal als Dienst anmelden kann. Dienste können so konfiguriert werden, dass sie unter den Konten „Lokales System“, „Lokaler Dienst“ oder „Netzwerkdienst“ ausgeführt werden. Diese Konten haben vordefinierte Rechte zur Anmeldung als Dienst. Allen Diensten, die unter einem separaten Benutzerkonto ausgeführt werden, muss dieses Benutzerrecht zugewiesen werden.

Die Einstellung **Als Dienst anmelden** ist für die Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur dem Konto „Netzwerkdienst“ zugewiesen.


#### Verwalten von Überwachungs- und Sicherheitsprotokoll

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer Objektzugriff-Überwachungsoptionen für einzelne Ressourcen wie Dateien, Active Directory-Objekte und Registrierungsschlüssel festlegen können. Dieses Benutzerrecht ist sehr umfassend und sollte genau überwacht werden. Jede Person mit diesem Benutzerrecht kann das Sicherheitsprotokoll löschen und so möglicherweise wichtige Beweise für nicht autorisierte Aktivitäten beseitigen.

Die Einstellung **Verwalten von Überwachungs- und Sicherheitsprotokoll** wird für Umgebungen mit älteren Clients und Unternehmensclient auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.

**Wichtig**: Microsoft Exchange Server 2003 ändert dieses Benutzerrecht in der Standarddomänencontrollerrichtlinie während des Installationsprozesses. Ausführliche Informationen finden Sie im Artikel [Bereitstellung von Exchange Server 2003](http://www.microsoft.com/technet/prodtechnol/exchange/guides/e2k3adperm/110e37bf-a68c-47bb-b4d5-1cfd539d9cba.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/exchange/guides/E2k3ADPerm/110e37bf-a68c-47bb-b4d5-1cfd539d9cba.mspx](http://www.microsoft.com/technet/prodtechnol/exchange/guides/e2k3adperm/110e37bf-a68c-47bb-b4d5-1cfd539d9cba.mspx). Wird dieses Benutzerrecht nicht auf die Administratorgruppe beschränkt, dann zeichnet Exchange im Anwendungsereignisprotokoll häufig Fehlermeldungen auf. Wenn Sie Exchange Server 2003 verwenden, müssen Sie den Wert dieser Einstellung für die Domänencontroller anpassen. Wie bei allen in diesem Handbuch empfohlenen Einstellungen müssen Sie u. U. einige Anpassungen durchführen, damit die Anwendungen Ihrer Organisation ordnungsgemäß funktionieren.


#### Firmware-Umgebungsvariablen ändern

Durch diese Richtlinieneinstellung wird festgelegt, ob die Umgebungsvariablen des Computers entweder durch einen Prozess über eine API oder durch einen Benutzer über die **Systemeigenschaften** geändert werden kann. Jeder, der mit diesem Benutzerrecht ausgestattet ist, kann durch entsprechende Einstellungskonfiguration den Ausfall einer Hardwarekomponente verursachen. Die Folge wäre eine Beschädigung von Daten oder ein Denial-of-Service.

Die Einstellung **Firmware-Umgebungsvariablen ändern** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Wartungsaufgaben für Speichermedien ausführen

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Nicht-Administrator oder Remotebenutzer die Verwaltung von Datenträgern oder Festplatten übernehmen kann. Ein Benutzer mit diesem Benutzerrecht kann einen Datenträger löschen und dadurch Datenverluste oder einen Denial-of-Service verursachen.

Die Einstellung **Wartungsaufgaben für Speichermedien ausführen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Einzelprozessprofil erstellen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer Leistungsüberwachungsprogramme zur Überwachung der Leistung von systemfremden Prozessen verwenden können. Dieses Benutzerrecht stellt ein geringes Sicherheitsrisiko dar. Ein Angreifer mit diesem Recht kann die Leistung eines Computers überwachen und kritische Prozesse identifizieren, die er möglicherweise direkt angreifen möchte. Ein Angreifer könnte auch die auf dem Computer ausgeführten Prozesse und somit die zu umgehenden Gegenmaßnahmen identifizieren, z. B. Antivirensoftware, ein System zum Erkennen von Eindringversuchen oder andere am Computer angemeldete Benutzer.

Die Einstellung **Einzelprozessprofil erstellen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. Zur Erhöhung der Sicherheit sollten Sie sicherstellen, dass dieses Benutzerrecht in der Hochsicherheitsumgebung nicht der Gruppe **Hauptbenutzer** zugewiesen wurde. Nur Mitglieder der Gruppe **Administratoren** sollten in einer derartigen Umgebung über diese Funktion verfügen.


#### Erstellen eines Profils der Systemleistung

Diese Richtlinieneinstellung ähnelt der vorherigen Einstellung. Durch sie wird festgelegt, welche Benutzer die Leistung der Systemprozesse überwachen können. Dieses Benutzerrecht stellt ein geringes Sicherheitsrisiko dar. Ein Angreifer mit diesem Recht kann die Leistung eines Computers überwachen und kritische Prozesse identifizieren, die er möglicherweise direkt angreifen möchte. Ein Angreifer könnte auch die auf dem Computer ausgeführten Prozesse und somit die zu umgehenden Gegenmaßnahmen identifizieren, z. B. Antivirensoftware oder ein System zum Erkennen von Eindringversuchen.

Die Einstellung **Systemleistungsprofil erstellen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Entfernen eines Computers aus der Dockingstation

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer tragbarer Computer im Menü **Start** den Befehl **PC trennen** auswählen können, um die Computer abzudocken. Ein Benutzer, dem dieses Benutzerrecht zugewiesen wurde, kann einen tragbaren Computer aus der Dockingstation entfernen.

Die Einstellung **Entfernen eines Computers aus der Dockingstation** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Ersetzen eines Prozessebenentokens

Durch diese Richtlinieneinstellung wird festgelegt, ob ein übergeordneter Prozess das mit einem untergeordneten Prozess verknüpfte Zugriffstoken ersetzen kann.

Die Einstellung **Ersetzen eines Prozessebenentokens** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur den Konten LOKALER DIENST und NETZWERKDIENST zugewiesen.


#### Wiederherstellen von Dateien und Verzeichnissen

Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer beim Wiederherstellen gesicherter Dateien und Verzeichnisse Rechte für Dateien, Verzeichnisse, die Registrierung und andere ständige Objekte umgehen können. Dieses Recht bestimmt auch, welche Benutzer gültige Sicherheitsprinzipale als Besitzer eines Objekts festlegen können.

Die Einstellung **Wiederherstellen von Dateien und Verzeichnissen** ist für Umgebungen mit älteren Clients und Unternehmensclient auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen. Die Wiederherstellung von Dateien wird in der Regel von Administratoren oder Mitgliedern einer anderen speziell delegierten Sicherheitsgruppe ausgeführt. Dies gilt insbesondere für Server und Domänencontroller, die besonders gut geschützt werden müssen.


#### System herunterfahren

Durch diese Richtlinieneinstellung wird festgelegt, welche lokal angemeldeten Benutzer das Betriebssystem herunterfahren können, indem sie den Befehl **Herunterfahren** verwenden. Das Recht, Domänencontroller herunterzufahren, sollte auf eine kleine Gruppe vertrauenswürdiger Administratoren beschränkt werden, da ein Missbrauch einen Denial-of-Service verursachen kann. Obwohl das Herunterfahren voraussetzt, dass sich der Benutzer beim Server anmelden kann, sollten Sie die zum Herunterfahren eines Domänencontrollers berechtigten Konten und Gruppen besonders sorgfältig auswählen.

Die Einstellung **System herunterfahren** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung wird dieses Benutzerrecht jedoch nur der Gruppe **Administratoren** zugewiesen.


#### Synchronisieren von Verzeichnisdienstdaten

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Prozess alle Objekte und Eigenschaften im Verzeichnis unabhängig von den auf die Objekte und Eigenschaften angewendeten Schutzmaßnahmen lesen kann. Dieses Benutzerrecht ist für den Einsatz der LDAP-Verzeichnissynchronisierungsdienste (Dirsync) erforderlich.

Die Einstellung **Synchronisieren von Verzeichnisdienstdaten** ist standardmäßig auf **Nicht definiert** gesetzt, was für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen ausreichend ist. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf einen Nullwert oder einen leeren Wert gesetzt. Dadurch steht dieses Benutzerrecht keiner Sicherheitsgruppe bzw. keinem Konto zu.


#### Übernehmen des Besitzes an Dateien und Objekten

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer die Besitzrechte für ein zu sicherndes Objekt im Netzwerk übernehmen können. Hierzu zählen auch Active Directory-Objekte, Dateien im NTFS-Dateisystem (NTFS), Ordner, Drucker, Registrierungsschlüssel, Dienste, Prozesse und Threads.

Die Einstellung **Übernehmen des Besitzes an Dateien und Objekten** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung sollten Sie dieses Benutzerrecht jedoch nur der Gruppe der lokalen **Administratoren** zuweisen.  

[Zum Seitenanfanq](#mainsection)  

### Sicherheitsoptionen

Die Richtlinieneinstellungen im Abschnitt zu den Sicherheitsoptionen für Gruppenrichtlinien werden zum Aktivieren oder Deaktivieren von Funktionen und Merkmalen verwendet. Dazu gehören der Zugriff auf Disketten- und CD-ROM-Laufwerke und Anmeldeaufforderungen. Diese Richtlinieneinstellungen werden auch verwendet, um verschiedene andere Einstellungen (z. B. für das digitale Signieren von Daten), Namen von Administrator- und Gastkonten sowie die Funktionsweise der Treiberinstallation zu konfigurieren.

Die Sicherheitsoptionen können in Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien\**  
**Sicherheitsoptionen**

Nicht alle in diesem Abschnitt behandelten Einstellungen sind bei allen Computertypen vorhanden. Deshalb müssen die in diesem Abschnitt definierten Einstellungen, die den Abschnitt der Sicherheitsoptionen der Gruppenrichtlinien bilden, auf Computern, in denen diese Einstellungen vorhanden sind, möglicherweise manuell geändert werden, um sie vollständig funktionsfähig zu machen.

In den folgenden Abschnitten werden Informationen zu den empfohlenen Sicherheitsoptionen für die Mitgliedsserver-Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen bereitgestellt. Eine Zusammenfassung der empfohlenen Einstellungen finden Sie in der Microsoft Excel-Arbeitsmappe „Sicherheitseinstellungen unter Windows Server 2003“, die gemeinsam mit dem Handbuch heruntergeladen werden kann. Informationen zur Standardkonfiguration und eine detaillierte Erklärung der einzelnen Einstellungen finden Sie im Begleithandbuch *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server* *2003 und Windows* *XP*.

Die Tabellen in den folgenden Abschnitten fassen die empfohlenen Einstellungen für die verschiedenen Sicherheitsoptionen zusammen. Ausführliche Informationen zu den Einstellungen sind in den Unterabschnitten nach den einzelnen Tabellen angeführt.


#### Kontoeinstellungen

**Tabelle 4.12: Sicherheitsoptionen: Empfehlungen zu Kontoeinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Administratorkontostatus

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Gastkontenstatus

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Konten: Administratorkontostatus

Durch diese Richtlinieneinstellung wird das Administratorkonto während des normalen Betriebs aktiviert oder deaktiviert. Beim Starten eines Computers im abgesicherten Modus ist das Administratorkonto immer aktiviert, unabhängig von dieser Einstellung.

Die Einstellung **Konten: Administratorkontostatus** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** und für Hochsicherheitsumgebungen auf **Aktiviert** gesetzt.

##### Konten: Gastkontenstatus

Durch diese Richtlinieneinstellung wird festgelegt, ob das Gastkonto aktiviert oder deaktiviert ist. Dieses Konto ermöglicht es nicht authentifizierten Netzwerkbenutzern, sich als Gast anzumelden und auf den Computer zuzugreifen.

Die Einstellung **Konten: Gastkontenstatus** ist für alle drei in diesem Handbuch definierten Umgebungen in der Baseline-Richtlinie auf **Deaktiviert** gesetzt.

##### Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken

Durch diese Richtlinieneinstellung wird festgelegt, ob lokale Konten, die nicht durch ein Kennwort geschützt sind, sich von anderen Orten als der physischen Computerkonsole aus anmelden können. Ist diese Richtlinieneinstellung aktiviert, können sich lokale Konten mit nicht leeren Kennwörtern nicht von einem Remoteclient aus beim Netzwerk anmelden, während lokale Konten ohne Kennwortschutz die Anmeldung nur dann durchführen können, wenn eine Computertastatur zur Verfügung steht.

Die Einstellung **Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standardwert **Aktiviert** gesetzt.


#### Überwachungseinstellungen

**Tabelle 4.13: Sicherheitsoptionen: Empfehlungen zu Überwachungseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Zugriff auf globale Systemobjekte prüfen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Überwachung: Zugriff auf globale Systemobjekte prüfen

Durch diese Richtlinieneinstellung wird der Zugriff auf globale Systemobjekte überwacht. Wenn sowohl die Einstellung **Überwachung: Zugriff auf globale Systemobjekte prüfen** als auch die Einstellung **Objektzugriffsversuche überwachen** aktiviert sind, werden viele Überwachungsereignisse erzeugt.

Die Einstellung **Überwachung: Zugriff auf globale Systemobjekte prüfen** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standartwert **Deaktiviert** gesetzt.

**Hinweis**: Änderungen an der Konfiguration dieser Richtlinieneinstellung werden erst nach einem Neustart von Windows Server 2003 wirksam.

Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen

Durch diese Richtlinieneinstellung wird festgelegt, ob die Verwendung aller Benutzerrechte überwacht wird. Dies betrifft auch das Recht „Sichern und wiederherstellen“, wenn die Richtlinieneinstellung **Rechteverwendung überwachen** aktiviert ist. Bei Aktivierung dieser Richtlinieneinstellung kann eine große Anzahl von Sicherheitsereignissen generiert werden, wodurch die Serverreaktion verlangsamt wird und zahlreiche Ereignissen mit geringer Bedeutung im Sicherheitsereignisprotokoll erfasst werden.

Die Einstellung **Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standartwert **Deaktiviert** gesetzt.

**Hinweis**: Änderungen an der Konfiguration dieser Richtlinieneinstellung werden erst nach einem Neustart von Windows Server 2003 wirksam.

Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können

Durch diese Richtlinieneinstellung wird festgelegt, ob der Computer sofort heruntergefahren wird, wenn Sicherheitsereignisse nicht protokolliert werden können.

Der zur Aktivierung der Einstellung **Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können** erforderliche Verwaltungsaufwand wurde in Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen als zu groß erachtet. Diese Richtlinieneinstellung ist deshalb in der Baseline-Richtlinie für diese Umgebungen auf **Deaktiviert** gesetzt. In der Baseline-Richtlinie der Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt, da der Verwaltungsaufwand als annehmbar erachtet wurde, um das Löschen von Ereignissen aus dem Sicherheitsprotokoll zu verhindern, sofern es nicht von einem Administrator ausdrücklich befohlen wurde.


#### Geräteeinstellungen

**Tabelle 4.14: Sicherheitsoptionen: Empfehlungen zu Geräteeinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Entfernen ohne vorherige Anmeldung erlauben

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Formatieren und Auswerfen von Wechselmedien zulassen

</td>

<td style="border:1px solid black;">


Administratoren

</td>

<td style="border:1px solid black;">


Administratoren

</td>

<td style="border:1px solid black;">


Administratoren

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anwendern das Installieren von Druckertreibern nicht erlauben

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Verhalten bei der Installation von nichtsignierten Treibern

</td>

<td style="border:1px solid black;">


Warnen, aber Installation erlauben

</td>

<td style="border:1px solid black;">


Warnen, aber Installation erlauben

</td>

<td style="border:1px solid black;">


Warnen, aber Installation erlauben

</td>

</tr>

</table>


##### Geräte: Entfernen ohne vorherige Anmeldung erlauben

Durch diese Richtlinieneinstellung wird festgelegt, ob ein tragbarer Computer ohne Anmeldung des Benutzers vom Computer abgedockt werden kann. Sie können diese Richtlinieneinstellung aktivieren, damit die Anmeldeanforderung entfällt und der Computer über eine Schaltfläche zum Trennen externer Hardware abgedockt werden kann. Bei Deaktivierung dieser Richtlinieneinstellung muss ein nicht angemeldeter Benutzer das Benutzerrecht **Entfernen eines Computers aus der Dockingstation** erhalten.

Die Einstellung **Geräte: Entfernen ohne vorherige Anmeldung erlauben** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt.

##### Geräte: Formatieren und Auswerfen von Wechselmedien zulassen

Durch diese Richtlinieneinstellung wird festgelegt, wer Wechselmedien formatieren und auswerfen kann. Auf Servern sollte das Auswerfen von Wechselmedien nur Administratoren erlaubt sein.

Der empfohlene Wert für die Einstellung **Geräte: Formatieren und Auswerfen von Wechselmedien zulassen** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen der Standardwert **Administratoren.**  

##### Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben

Ein Computer kann nur auf einem Netzwerkdrucker drucken, wenn der Treiber für diesen Netzwerkdrucker installiert ist. Wenn Sie die Einstellung **Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben** aktivieren, sind nur Benutzer der Gruppe **Administratoren** bzw. **Hauptbenutzer** sowie Benutzer mit Serveroperatorberechtigungen befugt, Druckertreiber zu installieren und Netzwerkdrucker hinzuzufügen. Bei Deaktivierung dieser Richtlinieneinstellung kann jeder Benutzer einen Druckertreiber installieren.

Die Einstellung **Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken

Durch diese Richtlinieneinstellung wird festgelegt, ob ein CD-ROM-Laufwerk gleichzeitig für lokale Benutzer und Remotebenutzer zugänglich ist. Wenn diese Richtlinieneinstellung aktiviert ist, können nur interaktiv angemeldete Benutzer auf Wechselmedien im CD-ROM-Laufwerk zugreifen. Ist diese Richtlinieneinstellung aktiviert und kein Benutzer interaktiv angemeldet, kann über das Netzwerk auf das CD-ROM-Laufwerk zugegriffen werden.

Die Einstellung **Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Baseline-Richtlinie für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf **Deaktiviert** gesetzt.

##### Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken

Durch diese Richtlinieneinstellung wird festgelegt, ob Wechselmedien im Diskettenlaufwerk gleichzeitig für lokale Benutzer und Remotebenutzer zugänglich sind. Wenn diese Richtlinieneinstellung aktiviert ist, können nur interaktiv angemeldete Benutzer auf Wechselmedien im Diskettenlaufwerk zugreifen. Ist diese Richtlinieneinstellung aktiviert und kein Benutzer interaktiv angemeldet, ist die Diskette über das Netzwerk zugänglich.

Die Einstellung **Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Baseline-Richtlinie für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung auf **Deaktiviert** gesetzt.

##### Geräte: Verhalten bei der Installation von nicht signierten Treibern

Durch diese Richtlinieneinstellung wird festgelegt, was passiert, wenn ein Benutzer versucht, einen nicht genehmigten und nicht vom Windows Hardware Quality Lab (WHQL) signierten Gerätetreiber zu installieren (über die Setup-API). Je nach Konfiguration verhindert diese Richtlinieneinstellung die Installation von nicht signierten Treibern oder warnt den Administrator, wenn ein solcher Treiber installiert werden soll.

Die Einstellung **Geräte: Verhalten bei der Installation von nicht signierten Treibern** kann dazu verwendet werden, die Installation von Treibern zu verhindern, die nicht für Windows Server 2003 mit SP1 zertifiziert wurden. Diese Richtlinieneinstellung ist jedoch in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Warnen, aber Installation erlauben** gesetzt. Ein potenzielles Problem bei dieser Konfiguration liegt in der Ausführung von unbeaufsichtigten Installationsskripts, die bei der Installation von nicht signierten Treibern fehlschlagen.

#### Einstellungen für Domänenmitglieder

**Tabelle 4.15: Sicherheitsoptionen: Empfehlungen zu Einstellungen für Domänenmitglieder**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Daten des sicheren Kanals digital verschlüsseln (wenn möglich)

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Daten des sicheren Kanals digital signieren (wenn möglich)

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Änderungen von Computerkontenkennwörtern deaktivieren

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Maximalalter von Computerkontenkennwörtern

</td>

<td style="border:1px solid black;">


30 Tage

</td>

<td style="border:1px solid black;">


30 Tage

</td>

<td style="border:1px solid black;">


30 Tage

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Starker (Windows 2000, Windows XP oder Windows Server 2003) Sitzungsschlüssel erforderlich

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)

Durch diese Richtlinieneinstellung wird festgelegt, ob der gesamte Datenverkehr vom sicheren Kanal, der vom Domänenmitglied initiiert wird, signiert oder verschlüsselt werden muss. Wenn ein Computer so konfiguriert ist, dass Daten des sicheren Kanals immer verschlüsselt oder signiert werden, kann kein sicherer Kanal mit einem Domänencontroller hergestellt werden, der nicht in der Lage ist, den gesamten Verkehr durch den sicheren Kanal zu signieren oder zu verschlüsseln.

Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)** ist in der Baseline-Richtlinie für die Umgebung mit älteren Clients auf **Deaktiviert** und in der Basisrichtlinie für Umgebungen mit Unternehmensclients und Hochsicherheitsumgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Wenn Sie diese Einstellung auf Mitgliedsarbeitsstationen und Servern nutzen möchten, muss auf allen Domänencontrollern, die die Domäne des Mitglieds bilden, Windows NT 4.0 mit Service Pack 6a oder eine höhere Windows-Version ausgeführt werden. Diese Richtlinieneinstellung wird zudem in Clients mit Windows 98 Second Edition nicht unterstützt, wenn sie nicht DSClient installiert haben.

##### Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen kann, für den gesamten von ihm initiierten Verkehr über den sicheren Kanal die Verschlüsselung auszuhandeln. Wenn Sie diese Richtlinieneinstellung aktivieren, fordert das Domänenmitglied für den gesamten Verkehr über den sicheren Kanal eine Verschlüsselung an. Bei Deaktivierung dieser Richtlinieneinstellung ist das Domänenmitglied nicht zur Aushandlung einer Verschlüsselung für den sicheren Kanal berechtigt.

Deshalb ist die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)** in der Baseline-Richtlinie für die drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen kann, eine Signatur für den gesamten von ihm initiierten Verkehr über den sicheren Kanal auszuhandeln. Durch eine erforderliche Signatur wird verhindert, dass der Verkehr geändert wird, wenn er bei der Übertragung abgefangen wird.

Deshalb ist die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)** in der Baseline-Richtlinie für die drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied sein Computerkontenkennwort regelmäßig ändern kann. Bei Aktivierung dieser Richtlinieneinstellung kann das Domänenmitglied sein Computerkontenkennwort nicht ändern. Bei Deaktivierung dieser Richtlinieneinstellung kann das Domänenmitglied sein Computerkontenkennwort je nach Festlegung unter **Domänenmitglied: Maximalalter von Computerkennwörtern** ändern. Die Standardeinstellung beträgt alle 30 Tage.

Bei Computern, die ihre Kontenkennwörter nicht mehr automatisch ändern können, besteht die Gefahr eines Angriffs durch Personen, die das Kennwort für das Domänenkonto des Computers in Erfahrung gebracht haben. Die Einstellung **Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch aktivierten Umgebungen auf **Deaktiviert** gesetzt.

##### Domänenmitglied: Maximalalter von Computerkennwörtern

Durch diese Richtlinieneinstellung wird das maximal zulässige Alter für Computerkontenkennwörter festgelegt. Sie gilt auch für Computer mit Windows 2000, ist dort jedoch nicht über die Tools des Sicherheitskonfigurations-Managers verfügbar. Standardmäßig ändern Domänenmitglieder ihre Domänenkennwörter automatisch alle 30 Tage. Eine erhebliche Erhöhung dieses Intervalls oder die Einstellung auf 0, damit die Kennwörter von Computern nicht mehr geändert werden müssen, gibt Angreifern mehr Zeit, um über Brute-Force-Angriffe das Kennwort von Computerkonten zu erraten.

Die Einstellung **Domänenmitglied: Maximalalter von Computerkennwörtern** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch aktivierten Umgebungen auf **30 Tage** gesetzt.

##### Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)

Durch diese Richtlinieneinstellung wird festgelegt, ob eine 128-Bit-Schlüsselstärke für verschlüsselte Daten des sicheren Kanals erforderlich ist. Bei Aktivierung dieser Richtlinieneinstellung können sichere Kanäle nur mit einer 128-Bit-Verschlüsselung eingerichtet werden. Bei Deaktivierung dieser Richtlinieneinstellung müssen Domänenmitglieder die Schlüsselstärke mit dem Domänencontroller aushandeln. Sitzungsschlüssel, die zum Einrichten einer Kommunikation über einen sicheren Kanal zwischen Domänencontrollern und Mitgliedscomputern verwendet werden, sind in Windows 2000 viel stärker als in früheren Microsoft-Betriebssystemen.

Da die drei in diesem Handbuch beschriebenen Sicherheitsumgebungen Domänencontroller mit Windows 2000 oder höher enthalten, wird die Einstellung **Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)** in der Baseline-Richtlinie für alle drei Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Bei Aktivierung dieser Richtlinieneinstellung können keine Computer angeschlossen werden, auf denen Domänen unter Windows 2000 bis Windows NT 4.0 ausgeführt werden.


#### Einstellungen für die interaktive Anmeldung

**Tabelle 4.16: Sicherheitsoptionen: Empfehlungen zu Einstellungen für die interaktive Anmeldung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Benutzerinformationen bei gesperrter Sitzung anzeigen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Benutzeranzeigename, Domäne und Benutzernamen

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Letzten Benutzernamen nicht anzeigen

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kein STRG+ALT+ENTF erforderlich

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Nachricht für Benutzer, die sich anmelden wollen

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Nachrichtentitel für Benutzer, die sich anmelden wollen

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

<td style="border:1px solid black;">


(Wenden Sie sich an die zuständigen Personen Ihrer Organisation.)

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern

</td>

<td style="border:1px solid black;">


14 Tage

</td>

<td style="border:1px solid black;">


14 Tage

</td>

<td style="border:1px solid black;">


14 Tage

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Smartcard erforderlich

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Verhalten beim Entfernen von Smartcards

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Arbeitsstation sperren

</td>

<td style="border:1px solid black;">


Arbeitsstation sperren

</td>

</tr>

</table>


##### Interaktive Anmeldung: Benutzerinformationen bei gesperrter Sitzung anzeigen

Durch diese Richtlinieneinstellung wird festgelegt, ob der Kontoname des zuletzt auf den Clientcomputern Ihrer Organisation angemeldeten Benutzers auf dem Windows-Anmeldebildschirm jedes Computers angezeigt wird. Bei Aktivierung dieser Richtlinieneinstellung können Eindringlinge nicht die Kontonamen von den Bildschirmen der Desktop- oder Laptopcomputer in Ihrer Organisation ablesen.

Die Einstellung **Interaktive Anmeldung: Benutzerinformationen bei gesperrter Sitzung anzeigen** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Baseline-Serverrichtlinie für die Hochsicherheitsumgebung ist sie auf **Benutzeranzeigenamen****,****Domäne und Benutzernamen** gesetzt.

##### Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen

Durch diese Richtlinieneinstellung wird festgelegt, ob der Name des Benutzers, der sich zuletzt auf dem Computer angemeldet hat, auf dem Windows-Anmeldebildschirm angezeigt wird. Bei Aktivierung dieser Richtlinieneinstellung wird der Name des zuletzt angemeldeten Benutzers nicht im Dialogfeld **Windows-Anmeldung** angezeigt.

Die Einstellung **Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen** ist in der Baseline-Serverrichtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich

Durch diese Richtlinieneinstellung wird festgelegt, ob der Benutzer vor der Anmeldung STRG+ALT+ENTF drücken muss. Bei Deaktivierung dieser Richtlinieneinstellung müssen alle Benutzer STRG+ALT-ENTF drücken, bevor sie sich bei Windows anmelden können (es sei denn, sie verwenden für die Windows-Anmeldung eine Smartcard).

Die Einstellung **Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich** ist für alle drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt, um die Wahrscheinlichkeit zu verringern, dass ein Angreifer Benutzerkennwörter mittels eines Trojaners abfängt.

##### Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden wollen

Durch diese Richtlinieneinstellung wird eine Textmeldung festgelegt, die bei der Anmeldung eines Benutzers angezeigt wird. Dieser Text wird in der Regel aus rechtlichen Gründen verwendet, z. B. um Benutzer auf die Auswirkungen eines unautorisierten Zugriffs bzw. eines Missbrauchs von Firmeninformationen hinzuweisen oder um sie darüber zu informieren, dass ihre Aktionen überwacht werden.

Die empfohlene Sicherheitsoptionseinstellung ist **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten.**   Sie sollten mit den zuständigen Personen in Ihrer Organisation sprechen, um den Inhalt dieses Textes festzulegen.

**Hinweis**: Sowohl die Einstellung **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten** als auch die Einstellung **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** müssen aktiviert sein, damit jede für sich korrekt funktionieren kann.

##### Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten

Diese Richtlinieneinstellung ermöglicht das Festlegen eines Titels für die Titelleiste des Dialogfelds mit der interaktiven Anmeldung, das bei der Anmeldung am Computer angezeigt wird. Diese Richtlinieneinstellung wird aus denselben Gründen verwendet wie die Einstellung **Nachricht für Benutzer, die sich anmelden wollen.**  

Die empfohlene Einstellung ist deshalb **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten.**   Sie sollten mit den zuständigen Personen in Ihrer Organisation sprechen, um den Inhalt dieses Texts festzulegen.

**Hinweis**: Sowohl die Einstellung **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten** als auch die Einstellung **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** müssen aktiviert sein, damit jede für sich korrekt funktionieren kann.

Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)

Durch diese Richtlinieneinstellung wird festgelegt, ob sich ein Benutzer unter Verwendung von zwischengespeicherten Konteninformationen bei einer Windows-Domäne anmelden kann. Anmeldeinformationen für Domänenkonten können lokal zwischengespeichert werden, damit sich ein Benutzer selbst dann anmelden kann, wenn ein Domänencontroller bei späteren Anmeldungen nicht erreichbar ist. Aufgrund dieser Funktion können sich Benutzer möglicherweise anmelden, nachdem ihr Konto deaktiviert oder gelöscht wurde, weil die Arbeitsstation nicht mit dem Domänencontroller in Verbindung tritt. Durch diese Einstellung wird die Anzahl von eindeutigen Benutzern festgelegt, für die Anmeldeinformationen lokal zwischengespeichert werden. Wenn Sie für diese Richtlinieneinstellung den Wert 0 festlegen, ist der Anmeldecache deaktiviert.

Die Einstellung **Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)** ist in der Baseline-Richtlinie für die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung auf **0** gesetzt. In der Umgebung mit älteren Clients ist die Einstellung auf **1** gesetzt, um gültigen Clients Zugriff zu gewähren, wenn sie den Domänencontroller nicht kontaktieren können.

##### Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern

Durch diese Richtlinieneinstellung wird festgelegt, wie viele Tage im Voraus Benutzer auf den Ablauf ihrer Kennwörter hingewiesen werden. Im Abschnitt „Kontenrichtlinien“ in Kapitel 3 wird empfohlen, Benutzerkennwörter so zu konfigurieren, dass sie regelmäßig ablaufen. Wenn Benutzer nicht über den bevorstehenden Ablauf ihrer Kennwörter benachrichtigt werden, merken sie u. U. zu spät, dass sie abgelaufen sind. Dies könnte zu Problemen für lokale Benutzer führen, die Schwierigkeiten haben, ihr Kennwort zu ändern. Bei einem unerwarteten Ablauf des Kennworts können sich Remotebenutzer nicht mehr über eine Einwahlverbindung oder ein virtuelles privates Netzwerk (VPN-Verbindung) anmelden.

Deshalb ist die Einstellung **Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf die Standardeinstellung von 14 Tagen gesetzt.

##### Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich

Für Domänenkonten wird durch diese Richtlinieneinstellung festgelegt, ob zum Entsperren eines Computers ein Domänencontroller kontaktiert werden muss. Die Richtlinieneinstellung behebt eine potenzielle Sicherheitsanfälligkeit, die mit der Einstellung **Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)** vergleichbar ist. Ein Benutzer könnte das Netzwerkkabel des Servers trennen und den Server mit einem alten Kennwort entsperren, ohne sich zu authentifizieren.

Um dies zu verhindern, ist die Einstellung **Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

**Wichtig**: Diese Richtlinieneinstellung gilt für Computer mit Windows 2000, Windows XP und Windows Server 2003. Unter Windows 2000 ist sie jedoch nicht über die Tools des Sicherheitskonfigurations-Managers verfügbar.

##### Interaktive Anmeldung: Smartcard erforderlich

Durch diese Richtlinieneinstellung wird festgelegt, dass Benutzer sich mit einer Smartcard am Computer anmelden müssen. Die Sicherheit wird erhöht, wenn Benutzer lange, komplexe Kennwörter zur Authentifizierung verwenden müssen, insbesondere wenn sie gezwungen sind, diese häufig zu ändern. Dieser Ansatz verringert das Risiko, dass ein Angreifer das Kennwort eines Benutzers durch einen Brute-Force-Angriff erraten kann. Es ist jedoch schwierig, Benutzer zur Auswahl sicherer Kennwörter zu zwingen. Außerdem sind selbst sichere Kennwörter nicht vor Brute-Force-Angriffen geschützt.

Die Sicherheit verbessert sich erheblich, wenn anstelle von Kennwörtern Smartcards zur Authentifizierung verwendet werden, da es mit der derzeit verfügbaren Technologie für einen Angreifer nahezu unmöglich ist, eine Benutzeridentität vorzutäuschen. Smartcards, die die Eingabe einer PIN (Personal Identification Number) erfordern, dienen einer Authentifizierung mit zwei Faktoren: Der Benutzer muss die Smartcard besitzen und gleichzeitig die PIN kennen. Ein Angreifer, der den Datenverkehr zur Authentifizierung zwischen dem Computer des Benutzers und dem Domänencontroller aufzeichnet, wird große Schwierigkeiten haben, die Daten zu entschlüsseln. Selbst wenn dies gelingen sollte, wird bei der nächsten Netzwerkanmeldung des Benutzers ein neuer Sitzungsschlüssel zum Verschlüsseln des Datenverkehrs zwischen dem Benutzer und dem Domänencontroller erstellt.

Microsoft empfiehlt Organisationen, Smartcards oder andere starke Authentifizierungstechnologien zu verwenden. Sie sollten allerdings die Einstellung **Interaktive Anmeldung: Erfordern Smartcard erforderlich** nur dann aktivieren, wenn bereits Smartcards bereitgestellt sind. Aus diesem Grund ist die Richtlinieneinstellung in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Baseline-Richtlinie für die Hochsicherheitsumgebung ist die Richtlinieneinstellung auf **Deaktiviert** gesetzt.

##### Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards

Durch diese Richtlinieneinstellung wird festgelegt, was geschieht, wenn die Smartcard eines angemeldeten Benutzers aus dem Smartcard-Lesegerät entfernt wird. Wenn Sie diese Einstellung auf **Arbeitsstation sperren** setzen, ist die Arbeitsstation beim Entfernen der Smartcard gesperrt. Dadurch können Benutzer den Bereich verlassen und Ihre Smartcard mitnehmen. Wenn Sie diese Einstellung auf **Abmeldung erzwingen** setzen, wird der Benutzer beim Entfernen der Smartcard automatisch abgemeldet.

Die Einstellung **Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients auf **Nicht definiert** und für Umgebungen mit Unternehmensclients und die Hochsicherheitsumgebung auf **Arbeitsstation sperren** gesetzt.


#### Einstellungen für den Microsoft-Netzwerkclient

**Tabelle 4.17: Sicherheitsoptionen: Empfehlungen zu den Einstellungen für den Microsoft-Netzwerkclient**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Kommunikation digital signieren (immer)

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kommunikation digital signieren (wenn Server zustimmt)

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

</table>


##### Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)

Durch diese Richtlinieneinstellung wird festgelegt, ob die SMB-Clientkomponente die Signierung von Paketen erfordert. Wenn Sie diese Einstellung aktivieren, kann der Microsoft-Netzwerkclient nur dann mit einem Microsoft-Netzwerkserver kommunizieren, wenn der Server der SMB-Paketsignierung zustimmt. In gemischten Umgebungen mit älteren Clients sollte diese Option auf **Deaktiviert** gesetzt werden, da diese Clients sich nicht authentifizieren und nicht auf Domänencontroller zugreifen können. In Umgebungen mit Windows 2000, Windows XP und Windows Server 2003 kann diese Einstellung jedoch verwendet werden. Die in diesem Handbuch definierten Unternehmensclient- und Hochsicherheitsumgebungen enthalten nur Computer mit diesen Betriebssystemen, von denen alle digitale Signaturen unterstützen.

Zur Erhöhung der Sicherheit der Kommunikation zwischen Computern in dieser Umgebung, ist die Einstellung **Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)** deshalb in der Baseline-Richtlinie für Umgebungen mit Unternehmensclients und die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.

##### Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Server zustimmt)

Durch diese Richtlinieneinstellung wird festgelegt, ob der SMB-Client versucht, SMB-Paketsignaturen auszuhandeln. Durch die Implementierung digitaler Signaturen in Windows-Netzwerken trägt dazu bei, Sitzungsübernahmen zu verhindern. Bei Aktivierung dieser Richtlinieneinstellung fordert der Microsoft-Netzwerkclient auf Mitgliedsservern Signaturen nur an, wenn die Server, mit denen er kommuniziert, digital signierte Kommunikation akzeptieren.

Die Einstellung **Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Server zustimmt)** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden

Bei Aktivierung dieser Richtlinieneinstellung kann der SMB-Redirector Nur-Text-Kennwörter an Nicht-Microsoft-SMB-Server senden, die keine Kennwortverschlüsselung während der Authentifizierung unterstützen.

Die Einstellung **Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden** ist in der Baseline-Richtlinie für die drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt, sofern die Anwendungen geheime Kennwörter nicht unnötig machen.


#### Einstellungen für Microsoft-Netzwerkserver

**Tabelle 4.18: Sicherheitsoptionen: Empfehlungen zu den Einstellungen für den Microsoft-Netzwerkserver**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Leerlaufzeitspanne bis zum Anhalten der Sitzung

</td>

<td style="border:1px solid black;">


15 Minuten

</td>

<td style="border:1px solid black;">


15 Minuten

</td>

<td style="border:1px solid black;">


15 Minuten

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kommunikation digital signieren (immer)

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kommunikation digital signieren (wenn Server zustimmt)

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung

Durch diese Richtlinieneinstellung wird die durchgehende Leerlaufzeitspanne festgelegt, nach der eine SMB-Sitzung aufgrund von Inaktivität angehalten wird. Administratoren können mit dieser Richtlinieneinstellung steuern, zu welchem Zeitpunkt eine nicht aktive Sitzung vom Computer angehalten wird. Wenn der Client seine Aktivität wieder aufnimmt, wird die Sitzung automatisch wiederhergestellt.

Die Einstellung **Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **15 Minuten** gesetzt.

##### Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)

Mit dieser Richtlinie wird festgelegt, ob die SMB-Serverkomponente Paketsignierung erfordert, bevor weitere Kommunikation mit einem SMB-Client zugelassen wird. Windows 2000 Server, Windows 2000 Professional, Windows Server 2003 und Windows XP Professional enthalten SMB-Versionen, die gegenseitige Authentifizierung unterstützen. Diese Form der Authentifizierung verhindert Sitzungsübernahmen und unterstützt Nachrichtenauthentifizierung zur Verhinderung von Man-in-the-Middle-Angriffen. Die SMB-Signierung stellt diese Authentifizierung bereit, da sie in jedes SMB-Paket eine digitale Signatur einfügt, die anschließend vom Client und vom Server überprüft wird. Wenn Computer zum Ignorieren der gesamten nicht signierten SMB-Kommunikation konfiguriert sind, können ältere Anwendungen und Betriebssysteme keine Verbindung herstellen. Wenn die SMB-Signierung vollständig deaktiviert wird, sind Computer für Angriffe anfällig, die die Übernahme der Kommunikationssitzungen der Benutzer zum Ziel haben.

Die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients auf **Deaktiviert** und für die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.

##### Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Client zustimmt)

Durch diese Richtlinieneinstellung wird festgelegt, ob der SMB-Server mit Clients, die dies erfordern, SMB-Paketsignierung aushandelt. Windows 2000 Server, Windows 2000 Professional, Windows Server 2003 und Windows XP Professional enthalten SMB-Versionen, die gegenseitige Authentifizierung unterstützen. Diese Form der Authentifizierung verhindert Sitzungsübernahmen und unterstützt Nachrichtenauthentifizierung zur Verhinderung von Man-in-the-Middle-Angriffen. Die SMB-Signierung stellt diese Authentifizierung bereit, da sie in jedes SMB-Paket eine digitale Signatur einfügt, die anschließend vom Client und vom Server überprüft wird. Wenn Computer zum Ignorieren der gesamten nicht signierten SMB-Kommunikation konfiguriert sind, können ältere Anwendungen und Betriebssysteme keine Verbindung herstellen. Wenn die SMB-Signierung vollständig deaktiviert wird, sind Computer für Angriffe anfällig, die die Übernahme der Kommunikationssitzungen der Benutzer zum Ziel haben.

Die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Client zustimmt)** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird

Durch diese Richtlinieneinstellung wird festgelegt, ob Benutzer abgemeldet werden, die außerhalb der für ihr Benutzerkonto gültigen Anmeldezeiten beim Netzwerkcomputer angemeldet sind. Diese Richtlinieneinstellung betrifft die SMB-Komponente. Wenn in Ihrer Organisation Anmeldezeiten für Benutzer festgelegt wurden, sollte diese Richtlinieneinstellung aktiviert werden. Andernfalls können Benutzer, die außerhalb ihrer Anmeldezeiten keinen Zugriff auf das Netzwerk haben sollen, diese Ressourcen über während der zulässigen Verbindungszeit eingerichteten Sitzungen weiter verwenden.

Die Einstellung **Microsoft-Netzwerk (Server): Clientverbindungen aufheben, wenn die Anmeldezeit überschritten wird** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.


#### Netzwerkzugriffseinstellungen

**Tabelle 4.19: Sicherheitsoptionen: Empfehlungen zu Netzwerkzugriffseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Anonyme SID-/Namensübersetzung zulassen

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anonyme Aufzählung von SAM-Konten nicht erlauben

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Speicherung von Anmeldeinformationen oder.NET-Passports für die Netzwerkauthentifikation nicht erlauben

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Named Pipes, auf die anonym zugegriffen werden kann

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


COMNAP, COMNODE, SQL\QUERY, SPOOLSS, LLSRPC, netlogon, lsarpc, samr, browser

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann

</td>

<td style="border:1px solid black;">


System\CurrentControlSet\Control\ Product Options;

System\CurrentControlSet\Control\

Serveranwendungen;

Software\Microsoft\

Windows NT\Current

Version

</td>

<td style="border:1px solid black;">


System\CurrentControlSet\Control\ Product Options;

System\CurrentControlSet\Control\

Serveranwendungen;

Software\Microsoft\

Windows NT\Current

Version

</td>

<td style="border:1px solid black;">


System\CurrentControlSet\Control\ Product Options;

System\CurrentControlSet\Control\

Serveranwendungen;

Software\Microsoft\

Windows NT\Current

Version

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann

</td>

<td style="border:1px solid black;">


(Informationen zu den Einstellungen finden Sie im folgenden Unterabschnitt.)

</td>

<td style="border:1px solid black;">


(Informationen zu den Einstellungen finden Sie im folgenden Unterabschnitt.)

</td>

<td style="border:1px solid black;">


(Informationen zu den Einstellungen finden Sie im folgenden Unterabschnitt.)

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anonymen Zugriff auf Named Pipes und Freigaben einschränken

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Freigaben, auf die anonym zugegriffen werden kann

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Keine

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten

</td>

<td style="border:1px solid black;">


Klassisch – lokale Benutzer authentifizieren sich als sie selbst

</td>

<td style="border:1px solid black;">


Klassisch – lokale Benutzer authentifizieren sich als sie selbst

</td>

<td style="border:1px solid black;">


Klassisch – lokale Benutzer authentifizieren sich als sie selbst

</td>

</tr>

</table>


##### Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen

Durch diese Richtlinieneinstellung wird festgelegt, ob ein anonymer Benutzer die SID-Attribute für einen anderen Benutzer anfordern kann. Bei Aktivierung dieser Richtlinieneinstellung könnte ein Benutzer mit lokalem Zugriff die allgemein bekannte SID des Administrators verwenden, um den richtigen Namen für den vordefinierten Administratornamen zu ermitteln – auch nach einer Umbenennung des Kontos. Diese Person könnte mithilfe des Kontos das Kennwort erraten.

Die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** ist in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt. In der Baseline-Richtlinie für die Hochsicherheitsumgebung ist die Richtlinieneinstellung auf **Deaktiviert** gesetzt.

##### Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben

Durch diese Richtlinieneinstellung wird festgelegt, welche zusätzlichen Berechtigungen für anonyme Verbindungen zum Computer erteilt werden. Windows ermöglicht anonymen Benutzern die Ausführung bestimmter Aktivitäten, wie z. B. das Auflisten von Domänenkonten. Diese Funktion ist hilfreich, wenn z. B. ein Administrator den Benutzern in einer vertrauenswürdigen Domäne Zugriff gewähren möchte, die keine gegenseitige Vertrauensstellung unterhält. Selbst wenn diese Einstellung aktiviert ist, haben anonyme Benutzer weiterhin Zugriff auf alle Ressourcen mit Berechtigungen, in denen die vordefinierte Gruppe **ANONYMOUS-ANMELDUNG** explizit enthalten ist.

Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben

Durch diese Richtlinieneinstellung wird festgelegt, ob die anonyme Aufzählung von SAM-Konten und Freigaben zulässig ist.

Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten und Freigaben nicht erlauben** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

##### Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben

Durch diese Richtlinieneinstellung wird festgelegt, ob Einstellungen für **Gespeicherte Benutzernamen und Kennwörter** nach der Domänenauthentifizierung Kennwörter, Anmeldeinformationen oder Microsoft.NET-Passports zur späteren Verwendung speichern.

Die Einstellung **Netzwerkzugriff: Speicherung von Anmeldeinformationen oder.NET-Passports für die Netzwerkauthentifikation nicht erlauben** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Sicherheitsumgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Änderungen an der Konfiguration dieser Richtlinieneinstellung werden erst nach einem Neustart von Windows wirksam.

##### Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen

Durch diese Richtlinieneinstellung wird festgelegt, welche zusätzlichen Berechtigungen für anonyme Verbindungen zum Computer erteilt werden. Bei Aktivierung dieser Richtlinieneinstellung können anonyme Windows-Benutzer bestimmte Aktivitäten ausführen, wie z. B. das Auflisten von Domänenkonten und Netzwerkfreigaben. Ein nicht autorisierter Benutzer könnte Kontennamen und freigegebene Ressourcen anonym auflisten und anhand dieser Informationen Kennwörter erraten oder Social Engineering-Angriffe durchführen.

Die Einstellung **Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt.

**Hinweis**: Domänen, bei denen diese Einstellung aktiviert ist, können mit Windows NT 4.0-Domänen oder -Domänencontrollern keine Vertrauensstellungen herstellen oder aufrechterhalten.

##### Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann

Durch diese Richtlinieneinstellung wird festgelegt, welche Kommunikationssitzungen (Named Pipes) Attribute und Berechtigungen besitzen, die anonymen Zugriff zulassen.

Es empfiehlt sich, in der Hochsicherheitsumgebung für die Einstellung **Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann** die Standardwerte zu erzwingen. Die Standardwerte bestehen aus folgenden Named Pipes:
* COMNAP – Zugriff auf SNA-Sitzung

* COMNODE – Zugriff auf SNA-Sitzung

* SQL\QUERY – Zugriff auf SQL-Instanz

* SPOOLSS – Druckwarteschlangendienst

* LLSRPC – Lizenzprotokollierdienst

* Netlogon – Anmeldedienst

* Lsarpc – LSA-Zugriff

* Samr – SAM-Zugriff

* browser – Computerbrowserdienst
 

**Wichtig**: Wenn Sie diese Richtlinieneinstellung aktivieren müssen, stellen Sie sicher, dass Sie nur jene Named Pipes hinzufügen, die zur Unterstützung der Anwendungen in Ihrer Umgebung erforderlich sind. Wie alle empfohlenen Einstellungen in diesem Handbuch sollte diese Richtlinieneinstellung sorgfältig getestet werden, bevor Sie sie in der Produktionsumgebung bereitstellen.


##### Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann

Durch diese Richtlinieneinstellung wird festgelegt, auf welche Registrierungspfade über das Netzwerk zugegriffen werden kann.

Die Einstellung **Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann** ist in den Baseline-Sicherheitsvorlagen für alle drei in diesem Handbuch definierten Sicherheitsumgebungen auf ihren Standardwert gesetzt.

**Hinweis**: Selbst wenn Sie diese Richtlinieneinstellung aktivieren, muss der Remoteregistrierungs-Systemdienst gestartet werden, wenn autorisierte Benutzer über das Netzwerk auf die Registrierung zugreifen können sollen.

Netzwerkzugriff: Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann

Durch diese Richtlinieneinstellung wird festgelegt, auf welche Registrierungspfade und -unterpfade über das Netzwerk zugegriffen werden kann.

Für die Einstellung **Netzwerkzugriff: Registrierungspfade und -unterpfade, auf die von anderen Computern aus zugegriffen werden kann** werden in den Baseline-Sicherheitsvorlagen für alle drei in diesem Handbuch definierten Sicherheitsumgebungen die Standardwerte verwendet. Die Standardeinstellungen bestehen aus den folgenden Pfaden und Unterpfaden:
* System\CurrentControlSet\Control\Print\Printers

* System\CurrentControlSet\Services\Eventlog

* Software\Microsoft\OLAP Server

* Software\Microsoft\Windows NT\CurrentVersion\Print

* Software\Microsoft\Windows NT\CurrentVersion\Windows

* System\CurrentControlSet\Control\ContentIndex

* System\CurrentControlSet\Control\Terminal Server

* System\CurrentControlSet\Control\Terminal Server\UserConfig

* System\CurrentControlSet\Control\Terminal Server\DefaultUserConfiguration

* Software\Microsoft\Windows NT\CurrentVersion\Perflib

* System\CurrentControlSet\Services\SysmonLog


##### Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken

Mit dieser Richtlinieneinstellung kann in folgenden Einstellungen der anonyme Zugriff auf Freigaben und Named Pipes eingeschränkt werden:
* **Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann**

* **Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann**

 

Die Einstellung **Netzwerkzugriff: Anonymen Zugriff auf Named Pipes und Freigaben einschränken** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standardwert **Aktiviert** gesetzt.

##### Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann

Durch diese Richtlinieneinstellung werden die Netzwerkfreigaben festgelegt, auf die anonyme Benutzer zugreifen können. Die Standardkonfiguration für diese Option hat geringe Auswirkungen, da alle Benutzer authentifiziert werden müssen, bevor sie auf freigegebene Ressourcen auf dem Server zugreifen können.

Die Einstellung **Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann** ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Keine** gesetzt.

**Hinweis**: Diese Richtlinieneinstellung kann sehr gefährlich sein, weil alle aufgelisteten Netzwerkressourcen für jeden Netzwerkbenutzer zugänglich sind. Vertrauliche Daten könnten weitergegeben oder beschädigt werden, wenn diese Richtlinieneinstellung aktiviert ist.

##### Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten

Durch diese Richtlinieneinstellung wird festgelegt, wie Netzwerkanmeldungen über lokale Konten authentifiziert werden. Die Konfiguration **Klassisch** gestattet eine genaue Steuerung des Ressourcenzugriffs und ermöglicht verschiedenen Benutzern unterschiedliche Zugriffstypen für dieselbe Ressource. Die Einstellung **Nur Gast** ermöglicht es Ihnen, alle Benutzer gleich zu behandeln. In diesem Fall werden alle Benutzer als **Nur Gast** authentifiziert und haben dieselben Zugriffsrechte auf die jeweilige Ressource.

Die Einstellung **Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf die Standardkonfiguration **Klassisch** gesetzt.


#### Netzwerksicherheitseinstellungen

**Tabelle 4.20: Sicherheitsoptionen: Empfehlungen zu Netzwerksicherheitseinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


LAN Manager-Authentifizierungsebene

</td>

<td style="border:1px solid black;">


Nur NTLMv2-Antworten senden

</td>

<td style="border:1px solid black;">


Nur NTLMv2-Antworten senden\LM verweigern

</td>

<td style="border:1px solid black;">


Nur NTLMv2-Antworten senden\LM &amp; NTLM verweigern

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Signaturanforderungen für LDAP-Clients

</td>

<td style="border:1px solid black;">


Signatur aushandeln

</td>

<td style="border:1px solid black;">


Signatur aushandeln

</td>

<td style="border:1px solid black;">


Signatur aushandeln

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)

</td>

<td style="border:1px solid black;">


Kein Minimum

</td>

<td style="border:1px solid black;">


Alle Einstellungen aktiviert

</td>

<td style="border:1px solid black;">


Alle Einstellungen aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)

</td>

<td style="border:1px solid black;">


Kein Minimum

</td>

<td style="border:1px solid black;">


Alle Einstellungen aktiviert

</td>

<td style="border:1px solid black;">


Alle Einstellungen aktiviert

</td>

</tr>

</table>


##### Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern

Durch diese Richtlinieneinstellung wird festgelegt, ob die bei der Änderung von Kennwörtern vom LAN Manager (LM) erzeugten Hashwerte für das neue Kennwort gespeichert werden. LM-Hashwerte sind anfälliger für Angriffe, weil für ihre Erzeugung im Vergleich zu Windows NT-Hashwerten ein schwächerer kryptografischer Algorithmus verwendet wird.

Die Einstellung **Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Sehr alte Betriebssysteme und einige Anwendungen funktionieren möglicherweise nicht einwandfrei, wenn diese Einstellung aktiviert ist. Außerdem müssen Sie nach dem Aktivieren dieser Einstellung die Kennwörter sämtlicher Konten ändern.

##### Netzwerksicherheit: LAN Manager-Authentifizierungsebene

Durch diese Richtlinieneinstellung wird festgelegt, welches Anfrage/Antwort-Authentifizierungsprotokoll für Netzwerkanmeldungen verwendet wird. Diese Auswahl betrifft die von Clientcomputern verwendete Authentifizierungsprotokollebene, die ausgehandelte Sicherheitsebene und die von Servern akzeptierte Authentifizierungsebene wie im Folgenden beschrieben. Die Zahlen in der folgenden Tabelle sind die tatsächlichen Einstellungen für den Registrierungswert **LMCompatibilityLevel.**  

**Tabelle 4.21: Einstellungen für den Registrierungswert**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Wert

</th>

<th style="border:1px solid black;">

Protokoll

</th>

</tr>

<tr>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


Clients verwenden LAN Manager- und NTLM-Authentifizierung, jedoch nie die NTLMv2-Sitzungssicherheit.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


Clients verwenden LAN Manager- und NTLM-Authentifizierung sowie die NTLMv2-Sitzungssicherheit, wenn sie vom Server unterstützt wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


2

</td>

<td style="border:1px solid black;">


Clients verwenden nur die NTLM-Authentifizierung sowie die NTLMv2-Sitzungssicherheit, wenn sie vom Server unterstützt wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


3

</td>

<td style="border:1px solid black;">


Clients verwenden nur die NTLMv2-Authentifizierung sowie die NTLMv2-Sitzungssicherheit, wenn sie vom Server unterstützt wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


4

</td>

<td style="border:1px solid black;">


Clients verwenden nur die NTLM-Authentifizierung sowie die NTLMv2-Sitzungssicherheit, wenn sie vom Server unterstützt wird. Der Domänencontroller lehnt die LAN Manager-Authentifizierung durch ab.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


5

</td>

<td style="border:1px solid black;">


Clients verwenden nur die NTLMv2-Authentifizierung sowie die NTLMv2-Sitzungssicherheit, wenn sie vom Server unterstützt wird. Der Domänencontroller lehnt LAN Manager- und die NTLM-Authentifizierung ab und akzeptiert nur NTLMv2.

</td>

</tr>

</table>


Diese Richtlinieneinstellung sollte entsprechend den folgenden Richtlinien auf die höchste in der Umgebung zulässige Ebene eingestellt werden:

Setzen Sie diese Richtlinieneinstellung in einer Umgebung, die nur Windows NT 4.0 SP4, Windows 2000 und Windows XP Professional enthält, auf allen Clients auf **Nur NTLMv2-Antworten senden\LM &amp; NTLM verweigern** und anschließend, nachdem alle Clients konfiguriert wurden, auf allen Servern auf **Nur NTLMv2-Antworten senden\LM &amp; NTLM verweigern.**   Eine Ausnahme von dieser Empfehlung bilden Windows Server 2003 Routing- und RAS-Server, da diese bei einer höheren Einstellung als **Nur NTLMv2-Antworten senden\LM verweigern** nicht korrekt funktionieren.

Die Unternehmensclient-Umgebung muss u. U. Routing- und RAS-Server unterstützen. Deshalb ist die Einstellung **Netzwerksicherheit: LAN Manager-Authentifizierungsebene** in der Baseline-Richtlinie für diese Umgebung auf **Nur NTLMv2-Antworten senden\LM verweigern** gesetzt. Da Routing- und RAS-Server in der Hochsicherheitsumgebung nicht unterstützt werden, ist die Richtlinieneinstellung für diese Umgebung auf **Nur NTLMv2-Antworten senden\LM &amp; NTLM verweigern** gesetzt.

Wenn Sie mit Windows 9x-Clients arbeiten und auf diesen den DSClient installieren können, setzen Sie diese Richtlinieneinstellung auf Computern, auf denen Windows NT (Windows NT, Windows 2000 und Windows XP Professional) ausgeführt wird, auf **Nur NTLMv2-Antworten senden\LM &amp; NTLM verweigern.**   Auf Computern, die nicht Windows 9x ausführen, darf für die Baseline-Richtlinie keine höhere Einstellung als **Nur NTLMv2-Antworten senden** gewählt werden. Dies ist die Einstellung für die Umgebung mit älteren Clients.

Schlägt die Ausführung bestimmter Anwendungen bei Aktivierung dieser Richtlinieneinstellung fehl, probieren Sie schrittweise die jeweils niedrigere Einstellung aus, um die Fehlerquelle festzustellen. Auf allen Computern sollten Sie diese Richtlinieneinstellung in der Baseline-Richtlinie mindestens auf **LM- und NTLM-Antworten senden (NTLMv2-Sitzungssicherheit verwenden, wenn ausgehandelt)** setzen. In der Regel können Sie sie auf allen Computern der Umgebung auf **Nur NTLMv2-Antworten senden** setzen.

Netzwerksicherheit: Signaturanforderungen für LDAP-Clients

Durch diese Richtlinieneinstellung wird die Datensignaturebene festgelegt, die im Auftrag von Clients angefordert wird, wenn diese LDAP-BIND-Anforderungen ausgeben. Nicht signierter Netzwerkdatenverkehr ist Man-in-the-Middle-Angriffen ausgesetzt. Im Falle eines LDAP-Servers könnte ein Angreifer den Server veranlassen, Entscheidungen zu treffen, die auf falschen Anfragen vom LDAP-Client basieren.

Die Einstellung **Netzwerksicherheit: LDAP Client Unterzeichnung Bedingungen** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Signatur aushandeln** gesetzt.

Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)

Diese Richtlinieneinstellung ermöglicht es einem Client, die Aushandlung der Nachrichtenvertraulichkeit (Verschlüsselung), Nachrichtensignatur, 128-Bit-Verschlüsselung oder NTLMv2-Sitzungssicherheit (NTLM, Version 2) anzufordern. Setzen Sie diese Richtlinieneinstellung so hoch wie möglich, bedenken Sie aber, dass die Anwendungsfunktionalität auf dem Netzwerk nach wie vor gewährleistet sein muss. Eine korrekte Konfiguration dieser Richtlinieneinstellung trägt dazu bei, Netzwerkverkehr von NTLM-SSP-basierten Servern vor Man-in-the-Middle-Angriffen und der Offenlegung von Daten zu schützen.

Die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)** ist in der Baseline-Richtlinie für die Umgebung mit älteren Clients auf **Kein Minimum** gesetzt. Sämtliche Einstellungen sind für die Unternehmensclient- und die Hochsicherheitsumgebung aktiviert.

##### Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)

Diese Richtlinieneinstellung ermöglicht es einem Server, die Aushandlung von Nachrichtenvertraulichkeit (Verschlüsselung), Nachrichtenintegrität, 128-Bit-Verschlüsselung und NTLMv2-Sitzungssicherheit zu verlangen. Setzen Sie diese Richtlinieneinstellung so hoch wie möglich, bedenken Sie aber, dass die Anwendungsfunktionalität auf dem Netzwerk nach wie vor gewährleistet sein muss. Wie bei der vorherigen Richtlinieneinstellung wird trägt eine korrekte Konfiguration dieser Richtlinieneinstellung dazu bei, den Netzwerkverkehr von NTLM-SSP-basierten Clients vor Man-in-the-Middle-Angriffen und der Offenlegung von Daten zu schützen.

Die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)** ist in der Baseline-Richtlinie für die Umgebung mit älteren Clients auf **Kein Minimum** gesetzt. Sämtliche Einstellungen sind für die Unternehmensclient- und die Hochsicherheitsumgebung aktiviert.


#### Einstellungen für die Wiederherstellungskonsole

**Tabelle 4.22: Sicherheitsoptionen: Empfehlungen zu den Einstellungen für die Wiederherstellungskonsole**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Automatische administrative Anmeldungen zulassen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

</table>


##### Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen

Durch diese Richtlinieneinstellung wird festgelegt, ob das Kennwort für das Administratorkonto eingegeben werden muss, bevor Zugriff auf den Computer gewährt wird. Bei Aktivierung dieser Richtlinieneinstellung fordert die Wiederherstellungskonsole Sie nicht zur Eingabe eines Kennworts auf, und Sie werden automatisch beim System angemeldet. Die Wiederherstellungskonsole kann sehr nützlich sein, wenn Sie mit Computern arbeiten müssen, die Probleme beim Starten haben. Die Aktivierung dieser Einstellung kann jedoch problematisch sein, da jeder zum Server gehen, diesen durch Unterbrechen der Stromzufuhr herunterfahren und anschließende neu starten kann. Wählt dieser Benutzer dann im Menü **Neu starten** den Befehl **Wiederherstellungskonsole**, hat er Vollzugriff auf den Server.

Die Einstellung **Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf die Standardeinstellung **Deaktiviert** gesetzt. Bei Deaktivierung dieser Option muss der Benutzer, um auf das Wiederherstellungskonsolenkonto zugreifen und die Wiederherstellungskonsole verwenden zu können, einen Benutzernamen und ein Kennwort eingeben.

##### Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen

Sie können diese Richtlinieneinstellung aktivieren, um den Befehl **SET** der Wiederherstellungskonsole verfügbar zu machen, mit dem die folgenden Umgebungsvariablen der Wiederherstellungskonsole festgelegt werden können:
* **AllowWildCards.**   Aktiviert die Platzhalterunterstützung für einige Befehle (z. B. für den Befehl DEL).

* **AllowAllPaths.**   Ermöglicht den Zugriff auf alle Dateien und Ordner auf dem Computer.

* **AllowRemovableMedia.**   Ermöglicht das Kopieren von Dateien auf Wechselmedien wie Disketten.

* **NoCopyPrompt.**   Unterdrückt die Anzeige einer Eingabeaufforderung beim Überschreiben einer vorhandenen Datei.

 

Um maximale Sicherheit zu erreichen, ist die Einstellung **Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen** in der Baseline-Richtlinie für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt. Diese Richtlinieneinstellung ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Aktiviert** gesetzt.


#### Einstellungen für das Herunterfahren

**Tabelle 4.23: Sicherheitsoptionen: Empfehlungen zu den Einstellungen für das Herunterfahren**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Herunterfahren des Systems ohne Anmeldung zulassen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Auslagerungsdatei des virtuellen Arbeitspeichers löschen

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

</table>


##### Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen

Durch diese Richtlinieneinstellung wird festgelegt, ob ein Computer von einem Benutzer heruntergefahren werden kann, der sich nicht beim Windows-Betriebssystem anmelden muss. Benutzer mit Zugriff auf die Konsole könnten den Computer herunterfahren. Ein Angreifer oder unbedarfter Benutzer könnte über die Terminaldienste eine Verbindung mit dem Server herstellen und diesen herunterfahren oder neu starten, ohne sich identifizieren zu müssen.

Die Einstellung **Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen** ist deshalb in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf die Standardeinstellung **Deaktiviert** gesetzt.

##### Herunterfahren: Auslagerungsdatei des virtuellen Arbeitspeichers löschen

Durch diese Richtlinieneinstellung wird festgelegt, ob die Auslagerungsdatei des virtuellen Arbeitsspeichers beim Herunterfahren des Computers gelöscht wird. Wenn diese Richtlinieneinstellung aktiviert ist, wird die Auslagerungsdatei des Systems bei jedem fehlerfreien Herunterfahren des Computers gelöscht. Bei Aktivierung dieser Richtlinieneinstellung wird die Ruhezustanddatei (Hiberfil.sys) ebenfalls gelöscht, wenn die Ruhezustandfunktion auf einem tragbaren Computer deaktiviert ist. Das Herunterfahren und Neustarten des Servers dauert auf Servern mit großen Auslagerungsdateien länger und macht sich dort besonders bemerkbar.

Deshalb ist die Einstellung **Herunterfahren: Auslagerungsdatei des virtuellen Arbeitspeichers löschen** in allen drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt.

**Hinweis**: Ein Angreifer mit physischem Zugriff auf den Server kann diese Gegenmaßnahme umgehen, indem er einfach das Netzkabel des Servers herauszieht.


#### Einstellungen für die Systemkryptografie

**Tabelle 4.24: Sicherheitsoptionen: Empfehlungen zu den Einstellungen für die Systemkryptografie**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Starken Schlüsselschutz für auf dem Computer gespeicherte Benutzerschlüssel erzwingen

</td>

<td style="border:1px solid black;">


Benutzer wird zur Eingabe aufgefordert, wenn der Schlüssel zum ersten Mal verwendet wird

</td>

<td style="border:1px solid black;">


Benutzer wird zur Eingabe aufgefordert, wenn der Schlüssel zum ersten Mal verwendet wird

</td>

<td style="border:1px solid black;">


Benutzer müssen jedes Mal, wenn sie einen Schlüssel verwenden, ein Kennwort eingeben

</td>

</tr>

<tr>

<td style="border:1px solid black;">


FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Systemkryptografie: Starken Schlüsselschutz für auf dem Computer gespeicherte Benutzerschlüssel erzwingen

Durch diese Richtlinieneinstellung wird festgelegt, ob private Schlüssel des Benutzers (z. B. S-MIME-Schlüssel) die Verwendung eines Kennworts erfordern. Wird diese Richtlinieneinstellung so konfiguriert, dass Benutzer bei jeder Verwendung eines Schlüssels ein Kennwort eingeben müssen (nicht das Domänenkennwort), dann wird der Zugriff auf lokal gespeicherte Benutzerschlüssel für Angreifer auch dann erschwert, wenn der Angreifer Anmeldekennwörter aufdeckt.

Zum Zwecke der Benutzerfreundlichkeit ist die Einstellung **Systemkryptografie: Starken Schlüsselschutz für auf dem Computer gespeicherte Benutzerschlüssel erzwingen** in Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen in der Baseline-Richtlinie auf **Benutzer wird zur Eingabe aufgefordert, wenn der Schlüssel zum ersten Mal verwendet** gesetzt. Zur Erhöhung der Sicherheit ist diese Richtlinieneinstellung für die Hochsicherheitsumgebung auf **Benutzer müssen jedes Mal, wenn sie einen Schlüssel verwenden, ein Kennwort eingeben** gesetzt.

##### Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden

Durch diese Richtlinieneinstellung wird festgelegt, ob der TLS/SSL-Sicherheitsdienst nur die Verschlüsselungssammlung TLS_RSA_WITH_3DES_EDE_CBC_SHA unterstützt. Obwohl durch diese Richtlinieneinstellung die Sicherheit erhöht wird, werden diese Algorithmen von den meisten öffentlichen Websites, die mit TLS oder SSL gesichert sind, nicht unterstützt. Auch viele Clientcomputer sind nicht für die Unterstützung dieser Algorithmen konfiguriert.

Deshalb ist die Einstellung **Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung,Hashing,und Signatur verwenden** in der Baseline-Richtlinie für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Deaktiviert** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **Aktiviert** gesetzt.


#### Systemobjekteinstellungen

**Tabelle 4.25: Sicherheitsoptionen: Empfehlungen zu den Systemobjekteinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden

</td>

<td style="border:1px solid black;">


Objektersteller

</td>

<td style="border:1px solid black;">


Objektersteller

</td>

<td style="border:1px solid black;">


Objektersteller

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Standardberechtigungen interner Systemobjekte (z. B. symbolischer Verknüpfungen) verstärken

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Systemobjekte: Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden

Durch diese Richtlinieneinstellung wird festgelegt, ob die **Administratorengruppe** oder ein Objektersteller der Standardbesitzer aller erstellten Systemobjekte ist. Beim Erstellen von Systemobjekten spiegeln die Besitzrechte wider, von welchem Konto das Objekt erstellt wurde (anstelle der allgemeineren Gruppe **Administratoren**).

Die Einstellung **Systemobjekte: Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Objektersteller** gesetzt.

Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren

Durch diese Richtlinieneinstellung wird festgelegt, ob für alle Subsysteme das Ignorieren der Groß-/Kleinschreibung erzwungen wird. Für das Microsoft Win32®-Subsystem wird die Groß-/Kleinschreibung ignoriert. Der Kernel unterstützt jedoch die Beachtung der Groß-/Kleinschreibung für andere Subsysteme, z. B. POIX (Portable Operating System Interface für UNIX). Da unter Windows die Groß-/Kleinschreibung ignoriert wird und das POSIX-Subsystem die Groß-/Kleinschreibung beachtet, kann ein Benutzer des Subsystems bei Deaktivierung dieser Option durch Verwenden von Groß- und Kleinbuchstaben eine Datei mit einem bereits vorhandenen Namen erstellen. In diesem Fall kann ein anderer Benutzers möglicherweise nicht mit Win32-Tools auf diese Dateien zugreifen, da nur eine der Dateien verfügbar ist.

Zum Gewährleisten der Konsistenz von Dateinamen wird die Einstellung **Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

Systemobjekte: Standardberechtigungen interner Systemobjekte (z. B. symbolischer Verknüpfungen) verstärken

Diese Richtlinieneinstellung legt die Stärke der wahlfreien Zugriffssteuerungsliste (DACL) für Objekte fest und trägt zur Sicherung von Objekten bei, die gesucht und zwischen Prozessen freigegeben werden können. Zur Verstärkung der DACL können Sie den Standardwert **Aktiviert** verwenden. Nicht-Administratoren können dann freigegebene Objekte lesen, aber keine Objekte ändern, die sie nicht erstellt haben.

Die Einstellung **Systemobjekte: Standardberechtigungen interner Systemobjekte (z. B. symbolischer Verknüpfungen) verstärken** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standardwert **Aktiviert** gesetzt.


#### Systemeinstellungen

**Tabelle 4.26: Sicherheitsoptionen: Empfehlungen zu den Systemeinstellungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Systemeinstellungen: Optionale Subsysteme

</td>

<td style="border:1px solid black;">


Keine

</td>

<td style="border:1px solid black;">


Keine

</td>

<td style="border:1px solid black;">


Keine

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Systemeinstellungen: Zertifikatsregeln zur Durchsetzung von Softwareeinschränkungsrichtlinien auf Windows-Programme anwenden

</td>

<td style="border:1px solid black;">


Nicht definiert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


##### Systemeinstellungen: Optionale Subsysteme

Durch diese Richtlinieneinstellung wird festgelegt, welche Subsysteme zur Unterstützung von Anwendungen in der Umgebung verwendet werden. Unter Windows Server 2003 ist der Standardwert für diese Richtlinieneinstellung **POSIX.**  

Zum Deaktivieren des POSIX-Subsystems ist die Einstellung **Systemeinstellungen: Optionale Subsysteme** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Keine** gesetzt.

##### Systemeinstellungen: Zertifikatsregeln zur Durchsetzung von Softwareeinschränkungsrichtlinien auf Windows-Programme anwenden

Durch diese Richtlinieneinstellung wird festgelegt, ob digitale Zertifikate verarbeitet werden, wenn Richtlinien für Softwareeinschränkungen aktiviert sind und ein Benutzer oder Prozess versucht, Software mit einer EXE-Dateinamenerweiterung auszuführen. Durch sie werden Zertifikatsregeln (eine Art Richtlinienregeln für Softwareeinschränkungen) aktiviert bzw. deaktiviert. Mit Softwareeinschränkungsrichtlinien können Sie eine Zertifikatsregel erstellen, um das Ausführen von mit Authenticode®-Technologie signierter Software in Abhängigkeit vom digitalen Zertifikat der Software zuzulassen oder zu sperren. Damit die Zertifikatsregeln in Softwareeinschränkungsrichtlinien wirksam werden, müssen Sie diese Richtlinieneinstellung aktivieren.

Die Einstellung **Systemeinstellungen: Zertifikatsregeln zur Durchsetzung von Softwareeinschränkungsrichtlinien auf Windows-Programme anwenden** ist in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Aufgrund der potenziellen Beeinträchtigung der Leistung ist sie jedoch in der Umgebung mit älteren Clients auf **Deaktiviert** und in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt.

[Zum Seitenanfanq](#mainsection)  

### Ereignisprotokoll

Im Ereignisprotokoll werden Ereignisse auf dem Computer erfasst, während im Sicherheitsprotokoll Überwachungsereignisse aufgezeichnet werden. Der Ereignisprotokoll-Container der Gruppenrichtlinie dient zum Definieren von Attributen der Anwendungs-, Sicherheits- und Systemereignisprotokolle, z. B. maximale Protokollgröße, Zugriffsrechte für jedes Protokoll sowie Einstellungen für die Dauer und Methode der Aufbewahrung. Die Einstellungen für die Anwendungs-, Sicherheits- und Systemereignisprotokolle werden in der Mitgliedsserver-Baseline-Richtlinie konfiguriert und auf alle Mitgliedsserver in der Domäne angewendet.

Die Ereignisprotokolleinstellungen können in Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Ereignisprotokoll**

Dieser Abschnitt enthält eine ausführliche Beschreibung der empfohlenen MSBP-Ereignisprotokolleinstellungen für alle drei in diesem Handbuch definierten Umgebungen. Eine Zusammenfassung der in diesem Abschnitt beschriebenen Einstellungen finden Sie in der Microsoft Excel-Arbeitsmappe „Sicherheitseinstellungen unter Windows Server 2003“, die zusammen mit diesem Handbuch heruntergeladen werden kann. Informationen zur Standardkonfiguration und eine ausführliche Erläuterung der einzelnen Einstellungen finden Sie im Begleithandbuch *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server* *2003 und Windows* *XP*, das unter [http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) erhältlich ist.

In der folgenden Tabelle werden die Empfehlungen zu den Einstellungen für Ereignisprotokolle für die drei in diesem Handbuch definierten Umgebungen zusammengefasst. Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle.

**Tabelle 4.27: Empfehlungen zu den Einstellungen für Ereignisprotokolle**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Maximale Größe des Anwendungsprotokolls

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Maximale Größe des Sicherheitsprotokolls

</td>

<td style="border:1px solid black;">


81.920 KB

</td>

<td style="border:1px solid black;">


81.920 KB

</td>

<td style="border:1px solid black;">


81.920 KB

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Maximale Größe des Systemprotokolls

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

<td style="border:1px solid black;">


16.384 KB

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Lokalen Gastkontozugriff auf Systemprotokoll verhindern

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Aufbewahrungsmethode des Anwendungsprotokolls

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Aufbewahrungsmethode des Sicherheitsprotokolls

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Aufbewahrungsmethode des Systemprotokolls

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

<td style="border:1px solid black;">


Bei Bedarf

</td>

</tr>

</table>



#### Maximale Größe des Anwendungsprotokolls

Durch diese Richtlinieneinstellung wird die maximale Größe des Anwendungsereignisprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen an die Anwendungsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.

Die Einstellung **Maximale Größe des Anwendungsprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standardwert **16.384 KB** gesetzt.


#### Maximale Größe des Sicherheitsprotokolls

Durch diese Richtlinieneinstellung wird die maximale Größe des Sicherheitsprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Sie sollten das Sicherheitsprotokoll auf Domänencontrollern und eigenständigen Servern für mindestens 80 MB konfigurieren. Dies sollte ausreichen, um genügend Informationen zu Überwachungszwecken speichern zu können. Wie Sie diese Richtlinieneinstellung für andere Computer konfigurieren müssen, hängt z. B. von der Häufigkeit der Protokollüberprüfung und dem verfügbaren Festplattenspeicher ab.

Die Einstellung **Maximale Größe des Sicherheitsprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **81.920 KB** gesetzt.


#### Maximale Größe des Systemprotokolls

Durch diese Richtlinieneinstellung wird die maximale Größe des Systemprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen für die Systemprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen.

Die Einstellung **Maximale Größe des Systemprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf den Standardwert **16.384 KB** gesetzt.


#### Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern

Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Anwendungsereignisprotokoll zuzugreifen. Unter Windows Server 2003 mit SP1 ist der Gastzugriff standardmäßig auf sämtlichen Computern unzulässig. Daher hat diese Richtlinieneinstellung keine praktische Auswirkung auf Computer mit Standardkonfigurationen.

Da diese Konfiguration jedoch als Tiefenverteidigungsmaßnahme ohne unerwünschte Auswirkungen gilt, ist die Einstellung **Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Diese Einstellung wird im Objekt der lokalen Computerrichtlinie nicht angezeigt.


#### Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern

Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Sicherheitsereignisprotokoll zuzugreifen. Für den Zugriff auf das Sicherheitsprotokoll muss ein Benutzer das Recht **Verwalten von Überwachungs- und Sicherheitsprotokoll** besitzen. (Dieses Recht wird in diesem Handbuch nicht beschrieben.) Daher hat diese Richtlinieneinstellung keine praktische Auswirkung auf Computer mit Standardkonfigurationen.

Da diese Konfiguration jedoch als Tiefenverteidigungsmaßnahme ohne unerwünschte Auswirkungen gilt, ist die Einstellung **Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Diese Einstellung wird im Objekt der lokalen Computerrichtlinie nicht angezeigt.


#### Lokalen Gastkontozugriff auf Systemprotokoll verhindern

Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Systemereignisprotokoll zuzugreifen. Unter Windows Server 2003 mit SP1 ist der Gastzugriff standardmäßig auf sämtlichen Computern unzulässig. Daher hat diese Richtlinieneinstellung keine praktische Auswirkung auf Computer mit Standardkonfigurationen.

Da diese Konfiguration jedoch als Tiefenverteidigungsmaßnahme ohne unerwünschte Auswirkungen gilt, ist die Einstellung **Lokalen Gastkontozugriff auf Systemprotokoll verhindern** in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Diese Einstellung wird im Objekt der lokalen Computerrichtlinie nicht angezeigt.


#### Aufbewahrungsmethode des Anwendungsprotokolls

Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Anwendungsprotokoll festgelegt. Das Anwendungsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung benötigt werden. Wenn Ereignisse je nach Bedarf überschrieben werden, speichert das Protokoll immer die neuesten Ereignisse, obwohl diese Konfiguration zu einem Verlust von Verlaufsdaten führen könnte.

Die Einstellung **Aufbewahrungsmethode des Anwendungsprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Bei Bedarf** gesetzt.


#### Aufbewahrungsmethode des Sicherheitsprotokolls

Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Sicherheitsprotokoll festgelegt. Das Sicherheitsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung benötigt werden. Wenn Ereignisse je nach Bedarf überschrieben werden, speichert das Protokoll immer die neuesten Ereignisse, obwohl diese Konfiguration zu einem Verlust von Verlaufsdaten führen könnte.

Die Einstellung **Aufbewahrungsmethode des Sicherheitsprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Bei Bedarf** gesetzt.


#### Aufbewahrungsmethode des Systemprotokolls

Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Systemprotokoll festgelegt. Die Protokolle müssen regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung benötigt werden. Wenn Ereignisse je nach Bedarf überschrieben werden, speichert das Protokoll immer die neuesten Ereignisse, obwohl diese Konfiguration zu einem Verlust von Verlaufsdaten führen könnte.

Die Einstellung **Aufbewahrungsmethode des Systemprotokolls** ist in der Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Bei Bedarf** gesetzt.  

[Zum Seitenanfanq](#mainsection)  

### Zusätzliche Registrierungseinträge

Für die Baseline-Sicherheitsvorlagendateien wurden zusätzliche Registrierungseinträge (auch *Registrierungswerte* genannt) erstellt, die nicht in den standardmäßigen administrativen Vorlagen (ADM-Datei) für die drei in diesem Handbuch verwendeten Umgebungen definiert sind. In den ADM-Dateien werden die Richtlinien und Beschränkungen für die Desktop-, Shell- und Sicherheitseinstellungen für Windows Server 2003 definiert.

Diese Registrierungseinträge sind in den Sicherheitsvorlagen im Abschnitt „Sicherheitsoptionen“ eingebettet, um die Änderungen zu automatisieren. Wenn die Richtlinie entfernt wird, werden die Registrierungseinträge nicht automatisch mitgelöscht. Sie müssen manuell mit einem Programm zum Bearbeiten der Registrierung (wie Regedt32.exe) geändert werden. In allen drei Umgebungen werden dieselben Registrierungseinträge verwendet.

Dieses Handbuch enthält zusätzliche Registrierungseinträge, die dem Sicherheitskonfigurations-Editor (SCE) hinzugefügt wurden. Zum Hinzufügen dieser Registrierungseinträge müssen Sie die Datei Sceregvl.inf im Ordner **%windir%\inf** ändern und die Datei Scecli.dll erneut registrieren. Die ursprünglichen und die zusätzlichen Sicherheitseinträge sind in den zuvor in diesem Kapitel genannten Snap-Ins und Tools unter **Lokale Richtlinien\Sicherheit** aufgeführt. Auf Computern, auf denen die in diesem Handbuch beschriebenen Sicherheitsvorlagen und Gruppenrichtlinien bearbeitet werden, müssen Sie die Datei Sceregvl.inf aktualisieren und die Datei Scecli.dll neu registrieren. Ausführliche Informationen zum Aktualisieren dieser Dateien sind im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) enthalten, das unter [http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) zur Verfügung steht.

Dieser Abschnitt enthält nur eine Zusammenfassung der im Begleithandbuch vollständig beschriebenen zusätzlichen Registrierungseinträge. Informationen zu den Standardeinstellungen und eine ausführliche Erläuterung der in diesem Abschnitt erwähnten Einstellungen finden Sie unter *Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows* *Server* *2003 und Windows* *XP.*


#### Sicherheitshinweise für Netzwerkattacken

Bei DoS-Angriffen (Denial of Service) handelt es sich um Netzwerkangriffe, bei denen versucht wird, die Verfügbarkeit eines Computers oder eines bestimmten Dienstes auf einem Computer für Netzwerkbenutzer zu stören. Die Abwehr von DoS-Attacken kann schwierig sein.

Zum Schutz vor diesen Angriffe sollten Sie auf Ihrem Computer immer die neuesten Sicherheitspatches installieren und den TCP/IP-Protokollstapel auf jenen Computern absichern, auf denen Windows Server 2003 mit SP1 ausgeführt wird und die potenziellen Angriffen ausgesetzt sind. Die standardmäßige TCP/IP-Stapelkonfiguration wird zur Verarbeitung von Standardintranetverkehr angepasst. Wenn Sie einen Computer direkt mit dem Internet verbinden, empfiehlt Microsoft, den TCP/IP-Stapel gegen DoS-Attacken zu abzusichern.

Sie können die in der folgenden Tabelle aufgeführten Registrierungswerte der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\Tcpip\Parameters\**

hinzufügen.

**Tabelle 4.28: Empfehlungen zu den TCP/IP-Registrierungseinträgen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Registrierungseintrag

</th>

<th style="border:1px solid black;">

Format

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


EnableICMPRedirect

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


SynAttackProtect

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


EnableDeadGWDetect

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


KeepAliveTime

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


300.000

</td>

<td style="border:1px solid black;">


300.000

</td>

<td style="border:1px solid black;">


300.000

</td>

</tr>

<tr>

<td style="border:1px solid black;">


DisableIPSourceRouting

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


2

</td>

<td style="border:1px solid black;">


2

</td>

<td style="border:1px solid black;">


2

</td>

</tr>

<tr>

<td style="border:1px solid black;">


TcpMaxConnectResponseRetransmissions

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


2

</td>

<td style="border:1px solid black;">


2

</td>

<td style="border:1px solid black;">


2

</td>

</tr>

<tr>

<td style="border:1px solid black;">


TcpMaxDataRetransmissions

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


3

</td>

<td style="border:1px solid black;">


3

</td>

<td style="border:1px solid black;">


3

</td>

</tr>

<tr>

<td style="border:1px solid black;">


PerformRouterDiscovery

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

</table>



#### Sonstige Registrierungseinträge

Sonstige empfohlene, nicht TCP/IP-spezifische Registrierungseinträge sind in der folgenden Tabelle aufgelistet. Weitere Informationen zu jedem Eintrag finden Sie in den Unterabschnitten im Anschluss an die Tabelle.

**Tabelle 4.29: Empfehlungen zu sonstigen Registrierungseinträgen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Registrierungseintrag

</th>

<th style="border:1px solid black;">

Format

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (NoNameReleaseOnDemand) NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (NtfsDisable8dot3NameCreation) Erstellen der Dateinamen im 8.3-Format deaktivieren (empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (NoDriveTypeAutoRun) Autorun für alle Laufwerke deaktivieren (empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0xFF

</td>

<td style="border:1px solid black;">


0xFF

</td>

<td style="border:1px solid black;">


0xFF

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (ScreenSaverGracePeriod) Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner (empfohlen: 0)

</td>

<td style="border:1px solid black;">


Zeichenformat

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (WarningLevel) Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


90

</td>

<td style="border:1px solid black;">


90

</td>

<td style="border:1px solid black;">


90

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (SafeDllSearchMode) Sicheren DLL-Suchmodus aktivieren (empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (AutoReboot) Automatischen Neustart von Windows nach einem Systemabsturz zulassen (empfohlen mit Ausnahme von Hochsicherheitsumgebungen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (AutoAdminLogon) Automatische Anmeldung aktivieren (nicht empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (AutoShareWks) Verwaltungsfreigaben aktivieren (empfohlen mit Ausnahme von Hochsicherheitsumgebungen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


0

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (DisableSavePassword) Speichern des DFÜ-Kennworts nicht zulassen (empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

<td style="border:1px solid black;">


1

</td>

</tr>

<tr>

<td style="border:1px solid black;">


MSS: (NoDefaultExempt) NoDefaultExempt für IPSec-Filterung aktivieren (empfohlen)

</td>

<td style="border:1px solid black;">


DWORD

</td>

<td style="border:1px solid black;">


3

</td>

<td style="border:1px solid black;">


3

</td>

<td style="border:1px solid black;">


3

</td>

</tr>

</table>


##### Konfigurieren der NetBIOS-Namensfreigabesicherheit: NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoNameReleaseOnDemand) NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen** angezeigt.

„NetBIOS über TCP/IP“ ist ein Netzwerkprotokoll, das u. a. eine Möglichkeit zur einfachen Auflösung der auf Windows-basierten Computern registrierten NetBIOS-Namen in auf diesen Computern konfigurierte IP-Adressen bereitstellt. Durch diesen Wert wird festgelegt, ob der NetBIOS-Name des Computers beim Empfang einer Namensfreigabeanforderung freigegeben wird.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\Netbt\Parameters\**

hinzufügen.

##### Deaktivieren der automatischen Generierung von 8.3-Dateinamen: Erstellen der Dateinamen im 8.3-Format deaktivieren

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NtfsDisable8dot3NameCreation) Erstellen der Dateinamen im 8.3-Format deaktivieren (empfohlen)** angezeigt.

Windows Server 2003 unterstützt 8.3-Dateinamensformate zur Gewährleistung der Abwärtskompatibilität mit 16-Bit-Anwendungen. Die 8.3-Dateinamenkonvention lässt Dateinamen mit maximal acht Zeichen zu.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\FileSystem\**

hinzufügen.

##### Deaktivieren von Autorun: Autorun für alle Laufwerke deaktivieren

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoDriveTypeAutoRun) Autorun für alle Laufwerke deaktivieren (empfohlen)** angezeigt.

Bei Aktivierung von Autorun werden Daten unmittelbar nach dem Einlegen von Medien in ein Laufwerk gelesen. Infolgedessen werden die Setupdatei (für Programme) und die Wiedergabe (für Audioinhalte) sofort gestartet.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Explorer\**

hinzufügen.

Sofortige Anwendung des Bildschirmschoner-Kennwortschutzes: Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner (empfohlen: 0)

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (ScreenSaverGracePeriod) Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner (empfohlen: 0)** angezeigt.

Windows enthält einen Kulanzzeitraum zwischen dem Start des Bildschirmschoners und der tatsächlichen automatischen Sperrung der Konsole, wenn die Bildschirmschonersperre aktiviert wird.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\**  
**Winlogon\**

hinzufügen.

Speicherplatzwarnung für das Sicherheitsprotokoll: Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (WarningLevel) Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung** angezeigt.

Diese Option ist seit SP3 für Windows 2000 verfügbar. Durch sie wird beim Überschreiten eines benutzerdefinierten Schwellenwerts eine Sicherheitsüberwachung im Sicherheitsprotokoll erzeugt. Wenn Sie für diesen Registrierungseintrag z. B. den Wert 90 festlegen, wird ein Eintrag mit der Ereignis-ID 523 und dem Text „Das Sicherheitsprotokoll ist jetzt 90 % voll.“ angezeigt, wenn dies der Fall ist.

**Hinweis**: Wenn die Protokolleinstellungen auf **Ereignisse bei Bedarf überschreiben** oder **Ereignisse überschreiben, die älter sind als x Tage** gesetzt sind, wird dieses Ereignis nicht erzeugt.

Sie können diesen Registrierungswert der Sicherheitsvorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\ SYSTEM\CurrentControlSet\Services\Eventlog\Security\**

hinzufügen.

##### Aktivieren der sicheren DLL-Suchreihenfolge: Sicheren DLL-Suchmodus aktivieren (empfohlen)

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (SafeDllSearchMode) Sicheren DLL-Suchmodus aktivieren (empfohlen)** angezeigt.

Zum Konfigurieren der DLL-Suchreihenfolge für die Suche nach DLLs, die von laufenden Prozessen angefordert werden, stehen zwei Methoden zur Auswahl:
* Zuerst die im Systempfad angegebenen Ordner und dann den aktuellen Arbeitsordner durchsuchen.

* Zuerst den aktuellen Arbeitsordner und dann die im Systempfad angegebenen Ordner durchsuchen.

 

Der Registrierungswert ist auf 1 gesetzt. Bei dieser Konfiguration werden zuerst die im Systempfad angegebenen Ordner und anschließend der aktuelle Arbeitsordner durchsucht. Wenn Sie diesen Eintrag auf 0 setzen, werden zuerst der aktuelle Arbeitsordner und anschließend die im Systempfad angegebenen Ordner durchsucht.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\ SYSTEM\CurrentControlSet\Control\Session Manager\**

hinzufügen.

Automatischer Neustart: Automatischen Neustart von Windows nach einem Systemausfall zulassen

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (AutoReboot) Automatischen Neustart von Windows nach einem Systemausfall zulassen** **(empfohlen mit Ausnahme von Hochsicherheitsumgebungen)** angezeigt.

Bei Aktivierung dieses Eintrags kann ein Server nach einem schwerwiegendem Absturz automatisch neu gestartet werden. Dieser Eintrag ist standardmäßig aktiviert, was für Hochsicherheitsserver nicht zu empfehlen ist.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Control\CrashControl\**

hinzufügen.

Automatische Anmeldung: Automatische Anmeldung aktivieren

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (AutoAdminLogon) Automatische Anmeldung aktivieren** **(nicht empfohlen )** angezeigt. Dieser Eintrag ist standardmäßig nicht aktiviert und sollte unter nahezu keinen Umständen auf einem Server verwendet werden.

Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Aktivieren der automatischen Anmeldung in Windows XP](http://support.microsoft.com/kb/315231/de)“ unter [http://support.microsoft.com/default.aspx?kbid=315231](http://support.microsoft.com/kb/315231/de).

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\**  
**Winlogon\**

hinzufügen.    

##### Verwaltungsfreigaben: Verwaltungsfreigaben aktivieren

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (AutoShareWks) Verwaltungsfreigaben aktivieren**  **(empfohlen mit Ausnahme von Hochsicherheitsumgebungen)** angezeigt. Ist Windows Networking auf einem Server aktiv, dann erstellt Windows standardmäßig verborgene Verwaltungsfreigaben, was auf Hochsicherheitsservern nicht zu empfehlen ist.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\RasMan\Parameters\**

hinzufügen.

##### Deaktivieren gespeicherter Kennwörter: Speichern des DFÜ-Kennworts nicht zulassen

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (DisableSavePassword) Speichern des DFÜ-Kennworts nicht zulassen** **(empfohlen)** angezeigt. Standardmäßig steht in Windows die Option zur Verfügung, Kennwörter für DFÜ- und VPN-Verbindungen zu speichern, was auf einem Server nicht empfehlenswert ist.

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\LanmanServer\**  
**Parameters\**

hinzufügen.

##### Aktivieren von IPSec zum Schutz des Kerberos-RSVP-Verkehrs: NoDefaultExempt für IPSec-Filter aktivieren

Dieser Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoDefaultExempt) NoDefaultExempt für IPSec-Filter aktivieren** **(empfohlen)** angezeigt. Die Standardausnahmen zu IPSec-Richtlinienfiltern sind in der Microsoft Windows Server 2003-Onlinehilfe dokumentiert. Diese Filter ermöglichen die Funktion des gegenseitigen Schlüsselaustausches (Internet Key Exchange, IKE) und des Kerberos-Authentifizierungsprotokolls. Mithilfe der Filter kann das Netzwerk-QoS (Quality of Service) ausgegeben werden (RSVP), und zwar sowohl wenn der Datenverkehr durch IPSec gesichert wird als auch wenn dies nicht der Fall ist (z. B. bei Multicast- und Broadcastverkehr).

Sie können diesen Registrierungswert der Vorlagendatei unter dem Unterschlüssel

**HKEY_LOCAL_MACHINE\System\CurrentControlSet\Services\IPSEC\**

hinzufügen.  

[Zum Seitenanfanq](#mainsection)  

### Eingeschränkte Gruppen

Die Funktion „Eingeschränkten Gruppen“ ermöglicht es, die Gruppenmitgliedschaft mithilfe von Richtlinienmechanismen zu verwalten und eine absichtliche oder unabsichtliche Ausnutzung von Gruppen mit umfassenden Benutzerrechten zu verhindern. Sie sollen zunächst die Anforderungen Ihrer Organisation prüfen, bevor Sie die einzuschränkenden Gruppen festlegen.

Die Gruppen **Sicherungs-Operatoren** und **Hauptbenutzer** sind in allen drei Umgebungen in diesem Handbuch definierten Umgebungen eingeschränkt. Obwohl Mitglieder der Gruppen **Sicherungs-Operatoren** und **Hauptbenutzer** weniger Zugriffsrechte als Mitglieder der Gruppe **Administratoren** besitzen, sind ihre Berechtigungen dennoch sehr umfassend.

**Hinweis**: Wenn Ihre Organisation eine dieser Gruppen verwendet, sollten Sie deren Mitgliedschaft sorgfältig überprüfen und die Anleitung für die Einstellung „Eingeschränkte Gruppen“ nicht implementieren. Wenn Ihre Organisation der Gruppe „Hauptbenutzer“ Benutzer hinzufügt, sollten Sie die optionalen Dateisystemberechtigungen implementieren, die im folgenden Abschnitt „Sichern des Dateisystems“ beschrieben werden.

Die Einstellung für eingeschränkte Gruppen kann unter Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Eingeschränkte Gruppen\**

Administratoren können eingeschränkte Gruppen konfigurieren, indem sie die gewünschte Gruppe direkt der Richtlinie für die Mitgliedsserver-Baseline hinzufügen. Ist eine Gruppe eingeschränkt, können deren Mitglieder und andere Gruppen, denen sie angehört, festgelegt werden. Werden diese Gruppenmitglieder nicht festgelegt, bleibt die Gruppe vollkommen eingeschränkt.  

[Zum Seitenanfanq](#mainsection)  

### Sichern des Dateisystems

Das NTFS-Dateisystem wurde mit jeder neuen Microsoft Windows-Version verbessert, und die Standardberechtigungen für NTFS sind für die meisten Organisationen angemessen. Die in diesem Abschnitt beschriebenen Einstellungen können insbesondere von Organisationen genutzt werden, die keine eingeschränkten Gruppen verwenden, aber dennoch eine zusätzliche Absicherung auf ihren Servern benötigen.

Die Sicherheitseinstellungen für das Dateisystem können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Dateisystem**

**Hinweis**: An den Standardsicherheitseinstellungen des Dateisystems vorgenommene Änderungen sollten in einer Testumgebung gründlich geprüft werden, bevor sie in einer großen Organisation bereitgestellt werden. Es ist vorgekommen, dass Dateiberechtigungen derartig geändert wurden, dass die betroffenen Computer vollständig neu eingerichtet werden mussten.

Die standardmäßigen Dateiberechtigungen in Windows Server 2003 mit SP1 sind für die meisten Situationen ausreichend. Wenn Sie nicht vorhaben, die Mitgliedschaft in der Gruppe **Hauptbenutzer** mit der Funktion „Eingeschränkte Gruppen“ zu blockieren, oder wenn Sie beabsichtigen, die Einstellung **Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen** zu aktivieren, sollten u. U. Sie die im folgenden Absatz beschriebenen optionalen Berechtigungen anwenden. Diese sind sehr spezifisch und wenden zusätzliche Einschränkungen auf bestimmte ausführbare Tools an, mit denen ein Angreifer mit erhöhten Berechtigungen möglicherweise den Computer oder das Netzwerk beeinträchtigen kann.

Beachten Sie, dass diese Änderungen keine Auswirkungen auf mehrere Ordner oder das Stammverzeichnis des Systemlaufwerks haben. Berechtigungen auf diese Weise zu ändern, kann riskant sein und zu einer Instabilität des Computers führen. Alle folgenden Dateien befinden sich im Ordner **%SystemRoot%\System32\** und verfügen über die Berechtigungen **Administratoren: Vollzugriff** und **System: Vollzugriff.**
* regedit.exe

* arp.exe

* at.exe

* attrib.exe

* cacls.exe

* debug.exe

* edlin.exe

* eventcreate.exe

* eventtriggers.exe

* ftp.exe

* nbtstat.exe

* net.exe

* net1.exe

* netsh.exe

* netstat.exe

* nslookup.exe

* ntbackup.exe

* rcp.exe

* reg.exe

* regedt32.exe

* regini.exe

* regsvr32.exe

* rexec.exe

* route.exe

* rsh.exe

* sc.exe

* secedit.exe

* subst.exe

* systeminfo.exe

* telnet.exe

* tftp.exe

* tlntsvr.exe

 

Diese optionalen Berechtigungen sind bereits in einer Sicherheitsvorlage mit dem Namen **Optional-File-Permissions.inf** konfiguriert und können gemeinsam mit diesem Handbuch heruntergeladen werden.  

[Zum Seitenanfanq](#mainsection)  


### Zusätzliche Sicherheitseinstellungen

Obwohl die meisten Gegenmaßnahmen zum Absichern der in diesem Handbuch enthaltenen Baseline-Server mithilfe von Gruppenrichtlinien angewendet wurden, können einige Einstellungen nur schwer oder gar nicht mit Gruppenrichtlinien implementiert werden. Eine ausführliche Erläuterung der in diesem Abschnitt beschriebenen Gegenmaßnahmen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)), das unter [http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10)) verfügbar ist.


#### Manuelle Absicherungsverfahren

In diesem Abschnitt wird beschrieben, wie einige zusätzliche Gegenmaßnahmen (wie z. B. das Sichern von Konten) für die einzelnen in diesem Handbuch definierten Sicherheitsumgebungen manuell implementiert wurden.

Manuelles Hinzufügen von eindeutigen Sicherheitsgruppen zu den Zuweisungen von Benutzerrechten

Die meisten empfohlenen Sicherheitsgruppen für Zuweisungen von Benutzerrechten wurden innerhalb der Sicherheitsvorlagen konfiguriert, die diesem Handbuch angefügt sind. Einige Rechte können jedoch nicht in die Sicherheitsvorlagen eingeschlossen werden, da die SIDs spezifischer Sicherheitsgruppen in Bezug auf unterschiedliche Windows 2003-Domänen eindeutig sind. Das Problem besteht darin, dass die in der SID enthaltene RID (relative ID) eindeutig ist. Diese Rechte werden in der folgenden Tabelle aufgeführt.

**Warnung**: Die folgende Tabelle enthält Werte für „Vordefinierter Administrator“. Bei „Vordefinierter Administrator“ handelt sich um das vordefinierte Benutzerkonto, *nicht* um die Sicherheitsgruppe **Administratoren.**   Wenn die Sicherheitsgruppe **Administrator** einem der folgenden Benutzerrechte zugewiesen wird, die den Zugriff verweigern, müssen Sie sich lokal anmelden, um den Fehler zu beheben.

Das Konto „Vordefinierter Administrator“ kann einen neuen Namen aufweisen, wenn Sie die in diesem Handbuch enthaltene Empfehlung zur Umbenennung befolgt haben. Wenn Sie dieses Konto zu einem der Benutzerrechte hinzufügen, die den Zugriff verweigern, müssen Sie sicherstellen, dass Sie das umbenannte Administratorkonto auswählen.

**Tabelle 4.30: Manuell hinzugefügte Zuweisungen von Benutzerrechten**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Name der Einstellung in der Benutzeroberfläche

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Den Zugriff auf diesen Computer vom Netzwerk aus verweigern

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Support_388945a0;

Gast; alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Support_388945a0;

Gast; alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Support_388945a0;

Gast; alle betriebssystemfremden Dienstkonten

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldung als Batchauftrag verweigern

</td>

<td style="border:1px solid black;">


Support_388945a0 und Gast

</td>

<td style="border:1px solid black;">


Support_388945a0 und Gast

</td>

<td style="border:1px solid black;">


Support_388945a0 und Gast

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Anmeldung über Terminaldienste verweigern

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Gäste; Support_388945a0; Gast; alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Gäste; Support_388945a0; Gast; alle betriebssystemfremden Dienstkonten

</td>

<td style="border:1px solid black;">


Vordefinierter Administrator; Gäste; Support_388945a0; Gast, alle betriebssystemfremden Dienstkonten

</td>

</tr>

</table>


**Wichtig**: Alle betriebssystemfremden Dienstkonten sind Dienstkonten für spezifische Anwendungen in Ihrem Unternehmen. Nicht zu diesen Konten zählen die Konten LOKALES SYSTEM, LOKALER DIENST oder NETZWERKDIENST. Bei diesen handelt es sich um vordefinierte Konten für das Betriebssystem.

Zum manuellen Hinzufügen der aufgeführten Sicherheitsgruppen zur Unternehmensclient-Richtlinie für die Mitgliedsserver-Baseline führen Sie die folgenden Schritte durch.

**So fügen Sie den Zuweisungen von Benutzerrechten Sicherheitsgruppen hinzu**

1. Klicken Sie in Active Directory-Benutzer und -Computer mit der rechten Maustaste auf die Mitgliedsserver-Organisationseinheit, und wählen Sie anschließend **Eigenschaften** aus.

2. Wählen Sie auf der Registerkarte **Gruppenrichtlinie** die **Unternehmensclient-Richtlinie für die Mitgliedsserver-Baseline** aus, um das verknüpfte Gruppenrichtlinienobjekt zu bearbeiten.

3. Wählen Sie **Unternehmensclient-Richtlinie für die Mitgliedsserver-Baseline** aus, und klicken Sie auf **Bearbeiten.**

4. Klicken Sie im Fenster **Gruppenrichtlinie** auf **Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen\Lokale Richtlinien\Zuweisung von Benutzerrechten**, um die eindeutigen Sicherheitsgruppen aus der vorherigen Tabelle für jedes Recht hinzuzufügen.

5. Schließen Sie die geänderte Gruppenrichtlinie.

6. Schließen Sie das Eigenschaftsfenster der Mitgliedsserver-Organisationseinheit.

7. Führen Sie folgende Schritte aus, um die Replikation zwischen den Domänencontrollern zu erzwingen, sodass die Richtlinie auf alle Controller angewendet wird:

    a. Öffnen Sie eine Eingabeaufforderung, geben Sie **gpupdate /Force** ein, und drücken Sie die Eingabetaste, um den Server zum Aktualisieren der Richtlinie zu veranlassen.

    b. Starten Sie den Server neu.


8. Überprüfen Sie im Ereignisprotokoll, ob die Gruppenrichtlinie erfolgreich heruntergeladen wurde und der Server mit den anderen Domänencontrollern in der Domäne kommunizieren kann.


##### Sichern von bekannten Konten

Windows Server 2003 mit SP1 verfügt über eine ganze Reihe von vordefinierten Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.

Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Aus diesem Grund wird das vordefinierte Administratorkonto umbenannt und seine Beschreibung geändert, um Angriffen vorzubeugen, bei denen versucht wird, einen Remoteserver durch Nutzung dieses bekannten Kontos zu beeinträchtigen.

Der Wert dieser Konfigurationsänderung hat sich in den letzten Jahren verringert, weil Angriffstools entwickelt wurden, mit denen über die SID (Sicherheits-ID) des vordefinierten Administratorkontos dessen wahrer Name ermittelt und somit Zugang zum Server erlangt werden kann. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf das Administratorkonto überwachen, wenn Sie es mit einem eindeutigen Namen versehen.

Führen Sie die folgenden Schritte aus, um bekannte Konten auf Domänen und Servern zu sichern:
* Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie die zugehörigen Kennwörter zu langen und komplexen Werten.

* Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server mit dem gleichen Kontonamen und -kennwort zugreifen.

* Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.

* Notieren Sie die vorgenommenen Änderungen, und bewahren Sie diese Informationen an einem sicheren Ort auf.
  

**Hinweis**: Das vordefinierte Administratorkonto kann durch Gruppenrichtlinien umbenannt werden. Diese Einstellung wurde in der Baseline-Richtlinie nicht implementiert, weil jede Organisation einen eindeutigen Namen für dieses Konto auswählen sollte. Sie können jedoch die Einstellung **Konten: Administratorkonto umbenennen** so konfigurieren, dass Administratorkonten in den drei in diesem Handbuch definierten Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.


##### Sichern von Dienstkonten

Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx).

##### NTFS

NTFS-Partitionen unterstützen ACLs auf Datei- und Ordnerebene. Diese Unterstützung ist für die Dateizuordnungstabelle (FAT) und FAT32-Dateisysteme nicht verfügbar. FAT32 ist eine aktualisierte Version des FAT-Dateisystems, die nun erheblich kleinere Clustergrößen zulässt und Festplatten von bis zu 2 TB unterstützt. FAT32 ist in Windows 95 OSR2, Windows 98, Microsoft Windows Me, Windows 2000, Windows XP Professional und Windows Server 2003 enthalten.

Formatieren Sie alle Partitionen auf jedem Server mit NTFS. Verwenden Sie das Konvertierungsdienstprogramm, um alle FAT-Partitionen in NTFS zu konvertieren. Gehen Sie dabei vorsichtig vor, und denken Sie daran, dass das Konvertierungsdienstprogramm die Zugriffssteuerungslisten für das konvertierte Laufwerk auf **Jeder: Vollzugriff** setzt.

Wenden Sie auf Computer, auf denen Windows 2003 Server mit SP1 ausgeführt wird, lokal die folgenden zwei Sicherheitsvorlagen an, um die standardmäßigen Zugriffssteuerungslisten des Dateisystems für Mitgliedsserver und Domänencontroller zu konfigurieren:
* **%windir%\inf\defltsv.inf**

* **%windir%\inf\defltdc.inf**
 

    **Hinweis**: Die Standardsicherheitseinstellungen für Domänencontroller werden während der Heraufstufung eines Servers zu einem Domänencontroller angewendet.

Alle Partitionen auf Servern in den drei in diesem Handbuch definierten Umgebungen werden mit NTFS-Partitionen formatiert, um die Verwaltung der Datei- und Verzeichnissicherheit mittels Zugriffssteuerungslisten zu ermöglichen.

##### Einstellungen für Terminaldienste

Die Einstellung **Verschlüsselungsstufe der Clientverbindung festlegen** legt die Stufe der Verschlüsselung für Clientverbindungen von Terminaldiensten in der Umgebung fest. Die Einstellung **Höchste Stufe** verwendet eine 128-Bit-Verschlüsselung und verhindert, dass ein Angreifer mithilfe von Paketanalysen Lauschangriffe auf Terminaldienstesitzungen durchführen kann. Einige ältere Versionen des Terminaldiensteclients unterstützen diese hohe Stufe der Verschlüsselung nicht. Wenn Ihr Netzwerk über solche Clients verfügt, setzen Sie die Verschlüsselungsstufe der Verbindung auf die höchste Stufe, die von diesen Clients beim Senden und Empfangen von Daten unterstützt wird.

Diese Einstellung kann in der Gruppenrichtlinie in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\Windows-Komponenten\**  
**Terminaldienste\Verschlüsselung und Sicherheit**

**Tabelle 4.31: Empfehlung zur Einstellung Verschlüsselungsstufe der Clientverbindung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Name der Einstellung in der Benutzeroberfläche

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Verschlüsselungsstufe der Clientverbindung festlegen

</td>

<td style="border:1px solid black;">


Hoch

</td>

<td style="border:1px solid black;">


Hoch

</td>

<td style="border:1px solid black;">


Hoch

</td>

</tr>

</table>


Die drei verfügbaren Verschlüsselungsstufen werden in der folgenden Tabelle beschrieben:

**Tabelle 4.32: Verschlüsselungsstufe für Terminaldienste**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Verschlüsselungsstufe

</th>

<th style="border:1px solid black;">

Beschreibung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Höchste Stufe

</td>

<td style="border:1px solid black;">


Verschlüsselt die zwischen Client und Server übermittelten Daten mit einer leistungsfähigen 128-Bit-Verschlüsselung. Verwenden Sie diese Stufe, wenn der Terminalserver in einer Umgebung ausgeführt wird, die ausschließlich 128-Bit-Clients enthält (z. B. Clients mit Remotedesktopverbindung). Mit Clients, die diese Verschlüsselungsstufe nicht unterstützen, wird bei dieser Einstellung keine Verbindung hergestellt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Clientkompatibel

</td>

<td style="border:1px solid black;">


Verschlüsselt die zwischen Client und Server übermittelten Daten mit der höchsten vom Client unterstützten Schlüsselstufe. Verwenden Sie diese Stufe, wenn der Terminalserver in einer Umgebung ausgeführt wird, die unterschiedliche bzw. ältere Clients enthält.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Niedrige Stufe

</td>

<td style="border:1px solid black;">


Verschlüsselt die vom Client zum Server gesendeten Daten mit einer 56-Bit-Verschlüsselung.

**Wichtig**: Vom Server an den Client gesendete Daten werden nicht verschlüsselt.

</td>

</tr>

</table>



#### Fehlerberichterstattung

**Tabelle 4.33: Empfohlene Einstellungen für die Fehlerberichterstattung**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Windows-Fehlerberichterstattung deaktivieren

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

<td style="border:1px solid black;">


Aktiviert

</td>

</tr>

</table>


Dieser Dienst hilft Microsoft bei der Erfassung und Behebung von Fehlern. Sie können diesen Dienst konfigurieren, um Berichte über Betriebssystemfehler, Windows-Komponentenfehler oder Programmfehler zu generieren. Er ist nur in Windows XP Professional und Windows Server 2003 verfügbar.

Mit dem Dienst **Fehlerberichterstattung** können solche Fehler über das Internet oder über eine interne Datenfreigabe Microsoft gemeldet werden. Obwohl Fehlerberichte sicherheitsrelevante oder sogar vertrauliche Daten enthalten können, wird durch die Microsoft-Datenschutzrichtlinie für die Fehlerberichterstattung sichergestellt, dass derartige Daten von Microsoft nicht zweckentfremdet werden. Die als Klartext-HTTP-Verkehr übertragenen Daten können jedoch im Internet abgefangen und von Dritten angezeigt werden.

Mithilfe der Einstellung zum **Deaktivieren der Windows**-**Fehlerberichterstattung** kann festgelegt werden, ob der Fehlerberichterstattungsdienst Daten überträgt.

Diese Richtlinieneinstellung kann unter Windows Server 2003 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\Administrative Vorlagen\System\Internetkommunikationsmanagement\Internetkommunikationseinstellungen**

Setzen Sie die Einstellung zum Deaktivieren der **Windows**-**Fehlerberichterstattung** in der Domänencontroller-Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert.**  

Aktivieren manueller Speicherabbilder

Windows Server 2003 mit SP1 enthält ein Merkmal, das Sie zum Anhalten des Computers und Erstellen einer Memory.dmp-Datei verwenden können. Sie müssen diese Funktion, die möglicherweise nicht für alle Server Ihrer Organisation geeignet ist, ausdrücklich aktivieren. Wenn Sie feststellen, dass die Erfassung von Speicherabbildern auf einigen Servern sinnvoll wäre, können Sie die Anweisungen im Artikel [Ein Windows-Feature ermöglicht das Erzeugen einer Datei "Memory.dmp" mit der Tastatur](http://support.microsoft.com/default.aspx?kbid=244139) unter [http://support.microsoft.com/default.aspx?kbid=244139](http://support.microsoft.com/default.aspx?kbid=244139) befolgen.

**Wichtig**: Wenn Speicherinhalt entsprechend den Anweisungen in diesem Artikel auf eine Datenträger kopiert wird, können in der Memory.dmp-Datei vertrauliche Daten enthalten sein. Im Idealfall sind alle Server vor nicht autorisiertem physischem Zugriff geschützt. Beim Erstellen einer Speicherabbilddatei auf einem Server, der durch physische Angriffe beeinträchtigt werden könnte, müssen Sie die Abbilddatei nach Abschluss der Fehlerbehebung unbedingt löschen.


#### Erstellen der Baseline-Richtlinie mithilfe des SCW

Zur Bereitstellung der notwendigen Sicherheitseinstellungen müssen Sie zunächst eine Mitgliedsserver-Baseline-Richtlinie (MSBP) erstellen. Dazu sollten Sie den SCW (den Sicherheitskonfigurations-Assistenten) und die in der herunterladbaren Version dieses Handbuchs enthaltenen Sicherheitsvorlagen verwenden.

Achten Sie beim Erstellen Ihrer eigenen Richtlinie darauf, die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ zu überspringen. Diese Einstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den vom SCW konfigurierten Elementen haben.

Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie ähnliche Hardware wie in Ihrer Bereitstellungsumgebung verwenden, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.

Während der Erstellung der Mitgliedsserver-Baseline-Richtlinie werden Sie wahrscheinlich die Dateiserverrolle aus der Liste mit den erkannten Rollen entfernen. Diese Rolle wird häufig auf Servern konfiguriert, die sie nicht benötigen. Sie könnte als Sicherheitsrisiko betrachtet werden. Um die Dateiserverrolle für Server zu aktivieren, die sie benötigen, können Sie zu einem späteren Zeitpunkt eine zweite Richtlinie anwenden.

**So erstellen Sie die Richtlinie für die Mitgliedsserver-Baseline (MSBP)**
* Erstellen Sie auf einem neuen Referenzcomputer eine neue Installation von Windows Server 2003 mit SP1.

* Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.

* Treten Sie mit dem Computer der Domäne bei.

* Installieren und konfigurieren Sie nur die obligatorischen Anwendungen, die auf sämtlichen Servern Ihrer Umgebung benötigt werden. Dazu zählen beispielsweise Ihre Software- und Verwaltungsagenten, Bandsicherungsagenten und Antiviren- und Antispywaredienstprogramme.

* Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.

* Entfernen Sie die Dateiserverrolle aus der Liste mit den erkannten Rollen.

* Stellen Sie sicher, dass die ermittelten Serverrollen für Ihre Umgebung geeignet sind.

* Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.

* Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.

* Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.

* Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.

* Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter.**   Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.

* Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.

* Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.

* Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. Unternehmensclient-Mitgliedsserver-Baseline.inf).

* Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Mitgliedsserver-Baseline.xml).



#### Testen der Richtlinie mithilfe des SCW

Nach dem Erstellen und Speichern der Richtlinie empfiehlt es sich unbedingt, sie in Ihrer Testumgebung bereitzustellen. Im Idealfall werden Ihre Testserver die gleiche Hardware- und Softwarekonfiguration wie Ihre Produktionsserver aufweisen. Mit diesem Ansatz können Sie mögliche Probleme, wie etwa das Vorhandensein unerwarteter Dienste, die von bestimmten Hardwaregeräten benötigt werden, ermitteln und beheben.

Zum Testen der Richtlinie gibt es zwei Möglichkeiten. Sie können die standardmäßigen SCW-Bereitstellungsgeräte verwenden oder mithilfe eines Gruppenrichtlinienobjekts Richtlinien anwenden.

Beim Verfassen der Richtlinien sollten Sie zunächst die Verwendung der standardmäßigen SCW-Bereitstellungsgeräte in Betracht ziehen. Sie können eine Richtlinie mit dem SCW jeweils auf einen einzelnen Server oder mithilfe von Scwcmd auf eine ganze Servergruppe anwenden. Die standardmäßige Bereitstellungsmethode bietet den Vorteil, dass bereitgestellte Richtlinien leicht vom SCW aus zurückgenommen werden können. Dies erweist sich als außerordentlich nützlich, wenn Sie im Testverfahren mehrere Änderungen an Ihren Richtlinien vornehmen.

Die Richtlinie wird getestet, um sicherzustellen, dass ihre Anwendung auf den Zielservern keine negativen Auswirkungen auf wichtige Funktionen hat. Nach Übernahme der Konfigurationsänderungen müssen Sie zunächst die Kernfunktionalität des Computers überprüfen. Ist der Server z. B. als Zertifizierungsstelle (CA) konfiguriert, müssen Sie sicherstellen, dass Clients Zertifikate anfordern und erhalten bzw. eine Zertifikatsperrliste herunterladen können usw.

Wenn Sie mit der Konfiguration von Richtlinien vertraut sind, können Sie Scwcmd verwenden, um wie im folgenden Verfahren veranschaulicht die Richtlinien in Gruppenrichtlinienobjekte umzuwandeln.

Weitere Informationen zum Testen von SCW-Richtlinien finden Sie im [Dokumentation zum Sicherheitskonfigurations-Assistenten](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/scwdeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx">Bereitstellungshandbuch für den Sicherheitskonfigurations-Assistenten unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/SCWDeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/scwdeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx) sowie in der [http://go.microsoft.com/fwlink/?linkid=43450](http://go.microsoft.com/fwlink/?linkid=43450) unter 


#### Umwandeln und Bereitstellen der Richtlinie

Nachdem Sie die Richtlinie gründlich getestet haben, führen Sie folgende Schritte aus, um sie in ein Gruppenrichtlinienobjekt umzuwandeln und bereitzustellen:
* Geben Sie an der Eingabeaufforderung folgenden Befehl ein:
 


<CodeSnippet Language="" ContainsMarkup="false" DisplayLanguage="">scwcmd transform /p:&lt;PathToPolicy.xml&gt; /g:&lt;GPODisplayName&gt;</CodeSnippet>
und drücken Sie anschließend die Eingabetaste. Beispiel:
 


<CodeSnippet Language="" ContainsMarkup="false" DisplayLanguage="">scwcmd transform /p:"C:\Windows\Security\msscw\Policies\Member Server Baseline.xml" /g:"Member Server Baseline Policy"</CodeSnippet>
**Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.

* Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der jeweiligen Organisationseinheit.


Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall.**  

Anschließend sollten Sie eine endgültige Prüfung vornehmen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Einstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Einstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.  

[Zum Seitenanfanq](#mainsection)  

### Zusammenfassung

In diesem Kapitel wurden die Serverabsicherungsverfahren erläutert, die zu Beginn in den drei in diesem Handbuch definierten Umgebungen auf alle Server unter Windows Server 2003 mit SP1 angewendet wurden. Um die gewünschte Sicherheitsstufe zu erreichen, wurde im Zuge der meisten dieser Verfahren für jede Sicherheitsumgebung eine eindeutige Sicherheitsvorlage erstellt, die dann in ein Gruppenrichtlinienobjekt importiert wurde, das mit der übergeordneten Organisationseinheit des Mitgliedsservers verknüpft ist.

Einige dieser Absicherungsverfahren können jedoch nicht mittels Gruppenrichtlinien angewendet werden. Anweisungen zur manuellen Konfigurationen dieser Einstellungen wurden bereitgestellt. Für spezifische Serverrollen wurden zusätzliche Schritte unternommen, damit diese innerhalb ihrer Rollen so sicher wie möglich funktionieren.

Die zusätzlichen Schritte für Serverrollen umfassen sowohl zusätzliche Absicherungsverfahren als auch Verfahren zum Verringern der Sicherheitseinstellungen in der Baseline-Sicherheitsrichtlinie. Diese Änderungen werden in den folgenden Kapiteln dieses Handbuchs ausführlich behandelt.


#### Weitere Informationen

Die folgenden Links bieten zusätzliche Informationen zur Absicherung von Servern, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
* Weitere Informationen zu den Sicherheitseinstellungen von Windows Server 2003 finden Sie auf der Seite [Beschreibungen von Sicherheitseinstellungen](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/dd980ca3-f686-4ffc-a617-50c6240f5582.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/dd980ca3-f686-4ffc-a617-50c6240f5582.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/dd980ca3-f686-4ffc-a617-50c6240f5582.mspx).

* Weitere Informationen zur Sicherheit für Windows Server 2003 finden Sie im [Windows Server 2003-Sicherheitscenter](http://www.microsoft.com/technet/security/prodtech/windowsserver2003.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/security/prodtech/windowsserver2003.mspx](http://www.microsoft.com/technet/security/prodtech/windowsserver2003.mspx).

* Weitere Informationen zur Überwachungsrichtlinie für Windows Server 2003 finden Sie auf der Seite [Überwachungsrichtlinie](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/6847e72b-9c47-42ab-b3e3-691addac9f33.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/6847e72b-9c47-42ab-b3e3-691addac9f33.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/6847e72b-9c47-42ab-b3e3-691addac9f33.mspx).

* Weitere Informationen zu Microsoft Operations Manager (MOM) finden Sie auf der Seite [Microsoft Operations Manager](http://www.microsoft.com/germany/mom/) unter [http://www.microsoft.com/germany/mom/](http://www.microsoft.com/germany/mom/).

* Weitere Informationen zu Benutzerrechten in Windows Server 2003 finden Sie auf der Seite [Benutzerrechte](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/589980fb-1a83-490e-a745-357750ced3d9.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/589980fb-1a83-490e-a745-357750ced3d9.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/589980fb-1a83-490e-a745-357750ced3d9.mspx).

* Weitere Informationen zu den Standardsicherheitseinstellungen für Windows Server 2003, finden Sie auf der Seite [Unterschiede bei Standardsicherheitseinstellungen](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/1494bf2c-b596-4785-93bb-bc86f8e548d5.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/1494bf2c-b596-4785-93bb-bc86f8e548d5.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/1494bf2c-b596-4785-93bb-bc86f8e548d5.mspx).

* Weitere Informationen zum Sichern von Terminaldiensten unter Windows 2000 finden Sie im Abschnitt „[Sichern von Windows 2000-Terminaldiensten](http://www.microsoft.com/technet/prodtechnol/win2kts/maintain/optimize/secw2kts.mspx)“ (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/win2kts/maintain/optimize/secw2kts.mspx](http://www.microsoft.com/technet/prodtechnol/win2kts/maintain/optimize/secw2kts.mspx).

* Weitere Informationen zum Sichern des TCP/IP-Stapels unter Windows Server 2003 finden Sie im Microsoft Knowledge Base-Artikel „[Absichern des TCP/IP-Stapels gegen Dienstverweigerungsangriffe unter Windows Server 2003](http://support.microsoft.com/kb/324270/en-us)“ (in englischer Sprache) unter [http://support.microsoft.com/kb/324270/en-us](http://support.microsoft.com/kb/324270/en-us).

* Weitere Informationen zur Absicherung der Einstellungen für Windows Sockets-Anwendungen finden Sie im Microsoft Knowledge Base-Artikel „[Internetserver aufgrund von SYN-Angriffen nicht verfügbar](http://support.microsoft.com/?kbid=142641)“ (in englischer Sprache) unter [http://support.microsoft.com/?kbid=142641](http://support.microsoft.com/?kbid=142641).

* Weitere Informationen zum Speicherort von.adm-Dateien finden Sie im Microsoft Knowledge Base-Artikel „[Speicherort von ADM-Dateien (Administrative Vorlagen) in Windows](http://support.microsoft.com/kb/228460/de)“ unter [http://support.microsoft.com/kb/228460](http://support.microsoft.com/kb/228460/de).

* Weitere Informationen zum Anpassen der Benutzeroberfläche des Sicherheitskonfigurations-Editors finden Sie im Microsoft Knowledge Base-Artikel „[Hinzufügen benutzerdefinierter Registrierungseinstellungen zum Sicherheitskonfigurations-Editor](http://support.microsoft.com/?kbid=214752)“ unter [http://support.microsoft.com/?kbid=214752](http://support.microsoft.com/?kbid=214752).

* Weitere Informationen zum Erstellen benutzerdefinierter administrativer Vorlagendateien unter Windows finden Sie im Microsoft Knowledge Base-Artikel [SO WIRD'S GEMACHT: Erstellen von benutzerdefinierten administrativen Vorlagen in Windows 2000](http://support.microsoft.com/kb/323639/de) unter [http://support.microsoft.com/kb/323639](http://support.microsoft.com/kb/323639/de). Lesen Sie auch das Whitepaper „[Implementieren registrierungsbasierter Gruppenrichtlinien](http://www.microsoft.com/windows2000/techinfo/howitworks/management/rbppaper.asp)“ (in englischer Sprache) unter [http://www.microsoft.com/WINDOWS2000/techinfo/howitworks/management/rbppaper.asp](http://www.microsoft.com/windows2000/techinfo/howitworks/management/rbppaper.asp).

* Weitere Informationen dazu, wie sichergestellt werden kann, dass sicherere LAN Manager-Authentifizierungseinstellungen in gemischten Netzwerken mit Windows 2000- und Windows NT® 4.0-Computern funktionieren, finden Sie im Microsoft Knowledge Base-Artikel „[Authentifizierungsprobleme in Windows 2000 mit NTLM 2-Ebenen oberhalb von 2 in einer Windows NT 4.0-Domäne](http://support.microsoft.com/?kbid=305379)“ (in englischer Sprache) unter [http://support.microsoft.com/?kbid=305379](http://support.microsoft.com/?kbid=305379).

* Weitere Informationen zur NTLMv2-Authentifizierung finden Sie im Microsoft Knowledge Base-Artikel [Aktivieren der NTLM 2-Authentifizierung](http://support.microsoft.com/kb/239869/de) unter [http://support.microsoft.com/kb/239869](http://support.microsoft.com/kb/239869/de).

* Weitere Informationen zu den Standardeinstellungen für Dienste in Windows Server 2003 finden Sie auf der Seite [Standardeinstellungen für Dienste](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/2b1dc6cf-2e34-4681-9aa6-8d0ffba2d3e3.mspx) (in englischer Sprache) unter [http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/2b1dc6cf-2e34-4681-9aa6-8d0ffba2d3e3.mspx](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/2b1dc6cf-2e34-4681-9aa6-8d0ffba2d3e3.mspx).

* Weitere Informationen zur Bereitstellung von Smartcards finden Sie im Artikel [Get Smart! Steigern Sie mit Smart Cards die Leistungsfähigkeit Ihres Netzwerks](http://www.microsoft.com/technet/technetmag/issues/2005/01/smartcards/) (in englischer Sprache) unter [http://www.microsoft.com/technet/technetmag/issues/2005/01/SmartCards/default.aspx](http://www.microsoft.com/technet/technetmag/issues/2005/01/smartcards/).

* Weitere Informationen zum Registrierungswert „RestrictAnonymous“ in Verbindung mit Windows 2000 finden Sie im Microsoft Knowledge Base-Artikel [Registrierungswert „RestrictAnonymous“ kann Vertrauensstellung einer Windows 2000-Domäne aufheben](http://support.microsoft.com/?kbid=296405) (in englischer Sprache) unter [http://support.microsoft.com/?kbid=296405](http://support.microsoft.com/?kbid=296405).

* Weitere Informationen zur Fehlerberichterstattung finden Sie auf der Seite [Firmen-Fehlerberichterstattung](http://www.microsoft.com/resources/satech/cer/) (in englischer Sprache) unter [http://www.microsoft.com/resources/satech/cer/](http://www.microsoft.com/resources/satech/cer/).

* Informationen zu Netzwerkports, die von Microsoft-Anwendungen verwendet werden, finden Sie im Microsoft Knowledge Base-Artikel „[Dienste und Netzwerk-Port-Anforderungen für das Microsoft Windows-Serversystem](http://support.microsoft.com/zumkb/832017/de)“ (in englischer Sprache) unter [http://support.microsoft.com/kb/832017](http://support.microsoft.com/zumkb/832017/de).

 
[Zum Seitenanfanq](#mainsection)

In diesem Beitrag
* [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))
* [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))
* [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))
* [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))
* Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline
* [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))
* [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))
* [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))
* [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))
* [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))
* [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))
* [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))
* [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))
* [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))
* [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))
* [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))
* [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))
* [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))
* [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
 

**Download**  


[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&amp;clcid=0x409)

**Benachrichtigungen über Neuerungen**  


[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)

**Feedback**  


[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows server 2003 security guide)

 

<table style="border:1px solid black;">

<tr>

<td style="border:1px solid black;">

[Zum Seitenanfanq](#mainsection)

</td>

<td style="border:1px solid black;">

[![](https://technet.microsoft.com/de-de/Dd443725.pageLeft(de-de,TechNet.10).gif "Dd443725.pageLeft(de-de,TechNet.10).gif")](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))
5 von 19[![](https://technet.microsoft.com/de-de/Dd443725.pageRight(de-de,TechNet.10).gif "Dd443725.pageRight(de-de,TechNet.10).gif")](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))

</td>

</tr>

</table>