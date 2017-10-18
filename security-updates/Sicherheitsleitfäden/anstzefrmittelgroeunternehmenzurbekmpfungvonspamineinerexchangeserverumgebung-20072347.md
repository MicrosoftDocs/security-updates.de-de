---
TOCTitle: 'Ansätze für mittelgroße Unternehmen zur Bekämpfung von Spam in einer Exchange Server-Umgebung'
Title: 'Ansätze für mittelgroße Unternehmen zur Bekämpfung von Spam in einer Exchange Server-Umgebung'
ms:assetid: '3eed9be9-ffd4-4138-9384-d8d849ad979c'
ms:contentKeyID: 20072347
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc875815(v=TechNet.10)'
---

Ansätze zur Bekämpfung von Spam in einer Exchange Server-Umgebung
=================================================================

Veröffentlicht: 18. Aug 2006

##### Auf dieser Seite

[](#efaa)[Einführung](#efaa)  
[](#eeaa)[Definition](#eeaa)  
[](#edaa)[Herausforderungen](#edaa)  
[](#ecaa)[Lösungen](#ecaa)  
[](#ebaa)[Zusammenfassung](#ebaa)  
[](#eaaa)[Referenzen](#eaaa)

### Einführung

Willkommen bei diesem Dokument aus der Reihe der Sicherheitsleitfäden für mittelgroße Unternehmen. Microsoft hofft, dass Ihnen die folgenden Informationen beim Erstellen einer sichereren und produktiveren Computerumgebung helfen werden.

#### Kurzzusammenfassung

Unerwünschte E-Mail-Nachrichten, auch als Junk-E-Mails oder Spam bekannt, sind Nachrichten, die aus einer einzelnen Quelle stammen und vorsätzlich an viele Postfächer auf einmal gesendet werden. Spamversender (Spammer) möchten erreichen, dass die Endbenutzer, denen sie ihre E-Mails schicken, tatsächlich auf die Nachrichten eingehen und den Spammern in irgendeiner Form zu finanziellem Gewinn verhelfen. Es gibt selbstverständlich viele verschiedene Techniken, mit denen Nachrichten in Grauzonen verbreiten werden, in denen sie auf der Gatewayebene nicht leicht als Spam zu erkennen sind.

Nach Schätzungen der IT-Branche handelt es sich bei mindestens 40 Prozent aller eingehenden E-Mails um Spam. Diese steigende Zahl der Junk-E-Mails ist für mittelgroße Unternehmen eine ständige Herausforderung. Solche Nachrichten sind nicht nur lästig, sondern unter Umständen auch kostspielig, wenn man den potenziellen Produktivitätsverlust und den Mehraufwand zu dessen Bewältigung in Betracht zieht.

Deshalb ist eine praktische Lösung zur Bekämpfung von Spam notwendig.

Microsoft® Exchange Server 2003 mit Service Pack 2 (SP2) bietet ein Framework, das verschiedene Methoden zur Bekämpfung von Spam in Umgebungen mit einem oder mehreren Exchange-Servern kombiniert. Dieses Framework wird als Exchange Server 2003 Antispam-Framework bezeichnet und ermöglicht eine Filterung von Spamnachrichten auf Verbindungs-, Protokoll- und Inhaltsebene.

Mit den Methoden dieses Frameworks haben sowohl Administratoren als auch Endbenutzer die Möglichkeit, potenzielle Spam-E-Mails präzise zu filtern und zu kategorisieren und dann selbst zu entscheiden, ob es sich um Spam oder legitime Geschäfts-E-Mails handelt.

Das Hauptziel dieses Frameworks ist es, Administratoren und Benutzern Lösungen zur Verfügung zu stellen, die so flexibel sind, dass sie auf der Serverseite ebenso angewendet werden können wie auf der Clientseite. Im vorliegenden Dokument werden diese Methoden ausführlich beschrieben. Dabei wird sowohl die Funktionsweise der einzelnen Methoden innerhalb des Frameworks als auch ihre gemeinsame Wirkungsweise beschrieben. Im Abschnitt „Bereitstellung und Verwaltung“ finden Sie Bewertungs- und Entwicklungspläne sowie eine Schritt-für-Schritt-Anleitung.

**Hinweis**   Microsoft bietet außerdem einen wichtigen Dienst zur Bekämpfung von Spam an. Dieser Dienst wird als EHS (Exchange Hosted Services) bezeichnet. EHS besteht im Grunde aus vier einzelnen Diensten, die einem Unternehmen helfen, sich vor E-Mail-gestützter Malware zu schützen, Aufbewahrungsbestimmungen zu erfüllen, Daten zur Wahrung der Vertraulichkeit zu verschlüsseln und auch während und nach Notsituationen E-Mail-Zugriff zu ermöglichen.  
Das Herzstück von EHS ist ein verteiltes Netzwerk von Datenzentren an Schlüsselstandorten entlang des Internet-Backbones. Jedes Datenzentrum enthält fehlertolerante Server, bei denen ein Lastenausgleich zwischen mehreren Standorten und Servern stattfindet.
Eine ausführliche Beschreibung dieses Dienstes würde den Rahmen dieses Leitfadens sprengen. Weitere Informationen finden Sie jedoch im Whitepaper [Microsoft Exchange – Übersicht über gehostete Dienste](http://www.microsoft.com/exchange/services/services.mspx) (möglicherweise in englischer Sprache) unter www.microsoft.com/exchange/services/services.mspx.

#### Übersicht

Das vorliegende Dokument, in denen die Optionen und Lösungen zur Bekämpfung von Spam in der Exchange Server-Umgebung behandelt werden, gliedert sich in vier Hauptabschnitte: Einführung, Definition, Herausforderungen und Lösungen.

##### Einführung

Dieser Abschnitt enthält eine Kurzzusammenfassung dieses Dokuments sowie eine Übersicht über seine Struktur und Informationen zur Zielgruppe.

##### Definition

In diesem Abschnitt finden Sie Detailinformationen und eine Übersicht über das Antispam-Framework von Exchange Server 2003. Diese Informationen sind für das Verständnis der in diesem Dokument behandelten Lösungen von Nutzen.

##### Herausforderungen

In diesem Abschnitt werden einige der Herausforderungen beschrieben, vor denen mittelgroße Unternehmen stehen, wenn es darum geht, Spam auf den verschiedenen Ebenen des Antispam-Frameworks herauszufiltern.

##### Lösungen

In diesem Abschnitt werden praktische Möglichkeiten zur Lösung des Problems unerwünschter E-Mails behandelt. Dabei werden Ansätze und Entwicklungspläne zur Bewältigung der Herausforderungen sowie Schritt-für-Schritt-Informationen zur Bereitstellung und Verwaltung der folgenden Methoden vorgestellt:

-   Schutz auf Verbindungsebene

    -   IP-Verbindungsfilterung

    -   Echtzeit-Sperrlisten

-   Schutz auf Protokollebene

    -   Empfänger- und Absenderblockierung

    -   Sender ID

-   Schutz auf Inhaltsebene

    -   Intelligenter Nachrichtenfilter für Exchange

    -   Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

Das Problembewusstsein der Benutzer ist zur Bekämpfung von Spam in Exchange Server-Umgebungen nicht weniger wichtig als das Antispam-Framework von Exchange Server 2003. Hierauf wird am Ende des Abschnitts „Bereitstellung und Verwaltung“ eingegangen.

#### Zielgruppe dieses Leitfadens

Dieses Dokument richtet sich in erster Linie an IT-Experten und Führungskräfte, die für die Planung und Implementierung von Spambekämpfungsmethoden in einer Exchange Server-Umgebung für mittelgroße Unternehmen zuständig sind. Im Einzelnen kann es sich dabei um folgende Fachkräfte handeln:

-   **Systemarchitekten**. Mitarbeiter, die für die Gestaltung der gesamten Serverinfrastruktur, die Entwicklung von Serverbereitstellungsstrategien und -richtlinien, die Systemabsicherung und die Netzwerkkonnektivitätsstruktur verantwortlich sind.

-   **IT-Manager**. Mitarbeiter, die technikbezogene Entscheidungen treffen und das IT-Personal verwalten, das für die Infrastruktur, für die Desktop- und die Serverbereitstellung, für die Exchange Server-Verwaltung und für standortübergreifende Betriebsprozesse verantwortlich ist.

-   **Systemadministratoren**. Mitarbeiter, die für die Planung und Bereitstellung von Technologie auf den verschiedenen Microsoft Exchange-Servern sowie für die Beurteilung und Empfehlung neuer technologischer Lösungen verantwortlich sind.

-   **Exchange Messaging-Administratoren**. Mitarbeiter, die für die Implementierung und Verwaltung der unternehmensinternen Nachrichtenübermittlung zuständig sind.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Definition

Das Antispam-Framework von Exchange Server 2003 ist eine Funktion zur Bekämpfung von Spam innerhalb der Exchange Server-Umgebung. Exchange Server 2003 SP2 bringt eine Verbesserung des Frameworks durch Einbeziehung einer als Industriestandard anerkannten E-Mail-Authentifizierungstechnologie, die als Sender ID-Filterung bezeichnet wird. Diese Technologie hilft Ihnen, die Menge an Spam zu verringern, die im Posteingang des Benutzers ankommt.

In diesem Abschnitt wird das Antispam-Framework von Exchange Server 2003 ausführlich beschrieben.

#### Antispam-Framework von Exchange Server 2003

Exchange Server 2003 bietet Spamschutz auf drei verschiedenen Ebenen: auf der Verbindungs-, der Protokoll und der Inhaltsebene (siehe folgende Abbildung):

![](images/Cc875815.AFSESE01(de-de,TechNet.10).gif)

**Abbildung 1. Die drei Ebenen des Spamschutzes**

Beim Schutz auf Verbindungsebene wird der verbindende SMTP-Host analysiert, beim Schutz auf Protokollebene der Absender und der Empfänger der Nachricht und beim Schutz auf Inhaltsebene der Inhalt der Nachricht. Jede dieser Spamschutzmethoden wird in den folgenden Unterabschnitten ausführlicher beschrieben.

##### Schutz auf Verbindungsebene

Der Schutz auf Verbindungsebene ist eine der vorteilhaftesten Schutzschichten zur Vermeidung von Spam. Er verhindert, dass eine Spamnachricht überhaupt in das mittelgroße Unternehmen gelangt. Wie aus der folgenden Abbildung hervorgeht, wird beim Schutz auf Verbindungsebene jede eingehende SMTP-Verbindung hinsichtlich der Wahrscheinlichkeit geprüft, dass sie eine Spamquelle darstellt.

![](images/Cc875815.AFSESE02(de-de,TechNet.10).gif)

**Abbildung 2. Schutz auf Verbindungsebene**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese02_big(de-de,technet.10).gif)  
Wenn der verbindende SMTP-Host als Host identifiziert wird, der Spam sendet oder normalerweise keine SMTP-Nachrichten sendet, kann die Verbindung abgelehnt werden, wodurch eine aufwändige Prüfung der eingehenden Nachricht auf Spam entfällt. Hierzu stehen in Exchange Server 2003 zwei Arten der Filterung auf Verbindungsebene zur Verfügung.

###### IP-Verbindungsfilterung

In Exchange Server 2003 können Sie SMTP-Verbindungen anhand ihrer IP-Adresse explizit verweigern. Dieser Ansatz ist eine weniger elegante Methode zum Schutz eines Exchange-Servers, da die Verbindungsfilterlisten manuell verwaltet werden. Wenn Sie aus einem bestimmten Grund eingehende SMTP-Verbindungen von einem konkreten Host verweigern möchten (z. B. weil es sich wahrscheinlich um eine Spamquelle handelt), werden die Verbindungen bereits auf dieser Ebene verweigert.

SMTP-Verbindungen können explizit zugelassen werden. Wenn Sie E-Mail von einem blockierten SMTP-Host empfangen möchten, der als Spamquelle identifiziert wurde, können Sie festlegen, dass normalerweise verweigerte Nachrichten von diesem SMTP-Host zugelassen werden.

###### Echtzeit-Sperrlisten

Eine dynamischere Möglichkeit, Schutz auf Verbindungsebene zu gewährleisten, stellen Echtzeit-Sperrlisten (Real-Time Block Lists, RBL) dar. Sperrlisten sind Listen mit IP-Adressen, bei denen es sich um bekannte Spamquellen, offene Relays oder Teile eines IP-Bereichs handelt, die keinen SMTP-Host enthalten sollten, beispielsweise eine IP-Adresse aus dem Microsoft MSN®-DFÜ-Pool.

Bei Sperrlisten von Drittanbietern werden IP-Adressen gesammelt, die den einzelnen Profilen entsprechen. Wenn ein sendender Host eine SMTP-Sitzung mit einem Abonnenten des Sperrlistendiensts initiiert, sendet der Abonnent eine DNS-artige Abfrage mit der IP-Adresse des verbindenden Hosts an den Sperrlistenanbieter. Der Sperrlistenanbieter antwortet darauf mit einem Code, aus dem hervorgeht, ob der verbindende Host auf einer Liste steht. Aus dem Code kann auch hervorgehen, auf welcher Liste sich der verbindende SMTP-Host befindet.

Die Echtzeit-Sperrlistenfilterung läuft folgendermaßen ab (siehe nachstehende Abbildung):

1.  Ein SMTP-Host stellt über den TCP-Port 25 eine Verbindung zum Exchange Server 2003-Server her.

2.  Der Exchange Server 2003 fragt den Anbieter der konfigurierten Sperrliste ab, um sicherzugehen, dass der verbindende SMTP-Host nicht auf der Sperrliste steht.

3.  Steht der Host nicht auf der Sperrliste, wird die Verbindung zugelassen. Steht er auf der Sperrliste, so wird die Verbindung abgebrochen.

![](images/Cc875815.AFSESE03(de-de,TechNet.10).gif)

**Abbildung 3. Funktionsweise der Echtzeit-Sperrlistenfilterung**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese03_big(de-de,technet.10).gif)

Vor Exchange Server 2003 SP2 stand die Verbindungsfilterfunktion nicht zur Verfügung, wenn Firewalls oder SMTP-Zwischenhosts zwischen Exchange und der sendenden Identität vorhanden waren (Exchange befindet sich hinter dem Umkreisnetzwerk), da früher nur der verbindende Host berücksichtigt wurde. Wenn ein Zwischenhost (etwa eine Firewall oder ein anderes SMTP-Gerät) zwischen dem sendenden Host und Exchange vorhanden ist, wird nur der Zwischenhost berücksichtigt.

Seit Exchange Server 2003 SP2 kann der Exchange-Server an jeder Stelle des mittelgroßen Unternehmens positioniert werden und Verbindungen trotzdem korrekt filtern. Dies wird durch Umkreis-IP-Listen und eine interne IP-Bereichskonfiguration in Exchange-System-Manager ermöglicht. Auf diese Weise wird durch die Sender ID- und die Echtzeit-Sperrlistenfunktionalität die IP-Adresse analysiert, die eine Verbindung zu Ihrem SMTP-Zwischenhost (z. B. zu einer Firewall) herstellt.

##### Schutz auf Protokollebene

![](images/Cc875815.AFSESE04(de-de,TechNet.10).gif)

**Abbildung 4. Schutz auf Protokollebene**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese04_big(de-de,technet.10).gif)

Nachdem die SMTP-Nachricht den Schutz auf Verbindungsebene durchlaufen hat, trifft sie auf der SMTP-Protokollebene auf die nächste Schutzschicht. Hier wird der SMTP-Dialog zwischen dem sendenden SMTP-Host und dem empfangenden SMTP-Host analysiert, um festzustellen, ob Absender und Empfänger zugelassen sind, und um den SMTP-Domänennamen des Absenders zu ermitteln.

###### Empfänger- und Absenderblockierung

Eine andere Möglichkeit, Spam manuell zu verringern, besteht darin, einzelne Absender oder Domänen zu definieren, von denen keine Nachrichten angenommen werden sollen. Mit der Absenderblockierung können Sie einzelne SMTP-Adressen oder Domänen angeben, die blockiert werden sollen. In Exchange Server 2003 können Sie auch Nachrichten zurückweisen, die keine Absenderadresse aufweisen, und gefilterte Nachrichten archivieren.

Mit der Empfängerfilterung können Sie Nachrichten filtern, die an einen bestimmten Empfänger gesendet wurden. Sie können auch Empfänger herausfiltern, die nicht im Verzeichnis aufgelistet sind. Die Aktivierung der Filterung von Empfängern, die nicht im Verzeichnis enthalten sind, kann Ihr Unternehmen jedoch anfällig für Angriffe zum Auslesen von SMTP-E-Mail-Adressen (Directory Harvesting Attack, DHA) machen. In dieser Situation werden die Antworten des Exchange-Servers auf *RFC2821 RCPT TO:*-Befehle hinsichtlich gültiger SMTP-Adressen analysiert. Das SMTP-Protokoll bestätigt akzeptable Empfänger während einer SMTP-Sitzung, indem es eine *250 2.1.5*-Antwort sendet. Wenn eine E-Mail an einen nicht existenten Empfänger gesendet wird, gibt der Exchange-Server den Fehler *550 5.1.1 User unknown* (Benutzer unbekannt) zurück. Somit kann ein Spammer ein automatisiertes Programm schreiben, das mithilfe gängiger Namen oder Begriffe aus Wörterbüchern E-Mail-Adressen an eine bestimmte Domäne konstruiert. Das Programm kann dann alle E-Mail-Adressen erfassen, die *250 2.1.5 to RCPT TO: SMTP* zurückgeben, und alle E-Mail-Adressen verwerfen, die die Fehlermeldung *550 5.1.1 User unknown* verursachen. Anschließend kann der Spammer die gültigen E-Mail-Adressen verkaufen oder als Empfänger für unerwünschte Mail verwenden.

Dieser Gefahr kann mit dem so genannten *Teergrubenverfahren* entgegengewirkt werden. Mithilfe der SMTP-Teergrubenfunktion von Microsoft Windows Server™ 2003 SP1 kann ein Administrator eine konfigurierbare Verzögerung einfügen, bevor entsprechende SMTP-Protokollantworten gesendet werden. Der angreifende Host wartet nicht lange genug, um diese Antworten zu erhalten.

Weitere Informationen hierzu finden Sie im Microsoft Knowledge Base-Artikel [SMTP-Teergrubenfunktion für Microsoft Windows Server 2003](http://support.microsoft.com/?kbid=842851) (möglicherweise in englischer Sprache) unter http://support.microsoft.com/?kbid=842851.

###### Sender ID

Eine der neuesten Antispam-Funktionen von Exchange Server 2003 ist die Sender ID-Filterung. Diese Funktion in Exchange Server 2003 SP2 versucht zu überprüfen, ob der sendende SMTP-Host berechtigt ist, Nachrichten aus der Domäne zu versenden, die in der Absender-E-Mail-Adresse angegeben ist. Viele Spamnachrichten sind gefälscht, so dass sie scheinbar von legitimen E-Mail-Adressen stammen. Indem eine vertrauenswürdige Absenderadresse vorgetäuscht wird (Bank, Kundendienst o. Ä.), lassen sich die Empfänger oftmals dazu verleiten, wichtige persönliche Daten preiszugeben, die dann leicht missbraucht werden können. Mit der Sender ID wird versucht, den Empfang gefälschter Nachrichten zu verhindern.  

Die Sender ID muss zwei Bestandteile aufweisen, damit das System funktioniert. Der erste Teil ist ein DNS-Datensatz, der als SPF-Datensatz (SPF = Sender Policy Framework) bezeichnet wird. In diesem Datensatz ist definiert, welche Server zum Versenden von SMTP-Adressen für Ihre Domäne berechtigt sind. Für das Vorhandensein eines SPF-Datensatzes muss die Sender ID nicht konfiguriert sein. Der zweite Teil ist ein SMTP-Host, der die Sender ID unterstützt, zum Beispiel Exchange Server 2003 SP2.

Der SPF-Datensatz wird zur DNS-Zone hinzugefügt, so dass andere Organisationen mit Sender ID überprüfen können, ob die scheinbar von Ihnen versendeten Nachrichten tatsächlich von den Servern stammen, die Sie in Ihrem SPF-Datensatz autorisiert haben. Die folgenden Schritte und Abbildungen verdeutlichen den Prozess, zuerst ohne und dann mit SPF-Datensatz.

1.  An den Exchange Server 2003-Server wird vom Spamming-SMTP-Host fabrikam.com eine Nachricht mit aktivierter Sender ID gesendet. Die Absenderadresse lautet susanf@nwtraders.com.

2.  Der Exchange-Server fragt beim DNS nach dem SPF-Datensatz für nwtraders.com (Northwind Traders).

3.  Da nwtraders.com keinen SPF-Datensatz hat, kann die Nachricht die Sender ID-Überprüfung passieren.

![](images/Cc875815.AFSESE05(de-de,TechNet.10).gif)

**Abbildung 5. Spam ohne Sender ID bzw. SPF-Datensatz dringt in ein Unternehmen ein**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese05_big(de-de,technet.10).gif)

Anschließend fügt Northwind Traders den SPF-Datensatz der DNS-Zone von nwtraders.com folgendermaßen hinzu:

1.  An den Exchange Server 2003-Server wird vom Spamming-SMTP-Host fabrikam.com eine Nachricht mit aktivierter Sender ID gesendet. Die Absenderadresse lautet susanf@nwtraders.com.

2.  Der Exchange-Server fragt beim DNS nach dem SPF-Datensatz für nwtraders.com (Northwind Traders).

3.  Da die Absender-IP-Adresse (208.217.184.82) nicht in der Liste der IP-Adressen enthalten ist, die laut SPF eine E-Mail für nwtraders.com senden dürfen (131.107.76.156), wird die Nachricht durch den Sender ID-Schutz ausgesondert.

![](images/Cc875815.AFSESE06(de-de,TechNet.10).gif)

**Abbildung 6. In einem Unternehmen erkannter Spam mit Sender ID bzw. SPF-Datensatz**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese06_big(de-de,technet.10).gif)

Durch das Implementieren einer Sender ID können Sie die Menge an Spam, die vorgetäuschterweise von Domänen mit einem SPF-Datensatz stammen, weitgehend reduzieren. Sie sollten jedoch wissen, dass der Sender ID-Schutz nur funktioniert, wenn die jeweiligen Domäneninhaber tatsächlich SPF-Datensätze bereitstellen.

Bei Microsoft.com werden 59 Prozent der eingehenden Nachrichten, die die Filterung auf Verbindungsebene passieren, durch die Filterung auf Protokollebene blockiert.

##### Schutz auf Inhaltsebene

![](images/Cc875815.AFSESE07(de-de,TechNet.10).gif)

**Abbildung 7. Schutz auf Inhaltsebene**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese07_big(de-de,technet.10).gif)

Nachdem durch die Filterung auf Verbindungs- und Protokollebene bestimmt wurde, ob eine eingehende Nachricht Spam ist, besteht die nächste Verteidigungslinie in der Analyse des Nachrichteninhalts hinsichtlich typischer Merkmale, die auf unerwünschte E-Mail hinweisen. Spammer versuchen ständig neue Methoden zu erfinden, mit denen sich Inhaltsfilter überlisten lassen, so dass die Nachrichten in den Posteingang der Benutzer gelangen.

###### Intelligenter Nachrichtenfilter für Exchange

Der intelligente Nachrichtenfilter (Intelligent Message Filter, IMF) ist ein speziell für Exchange entwickelter Inhaltsfilter. Er basiert auf patentierter maschineller Lerntechnologie von Microsoft Research, die als Microsoft SmartScreen®-Technologie bekannt ist. SmartScreen wird derzeit von MSN, Microsoft Hotmail®, Microsoft Office Outlook® 2003 und Exchange verwendet. IMF hat die Aufgabe, anhand von Millionen von Nachrichten zwischen Merkmalen legitimer E-Mail-Nachrichten und Merkmalen von Spam zu unterscheiden. IMF beurteilt die Wahrscheinlichkeit, dass es sich bei einer eingehenden E-Mail um eine legitime Nachricht oder aber um Spam handelt. Im Unterschied zu vielen anderen Filtertechnologien orientiert sich IMF an Merkmalen aus einem statistisch soliden Pool von E-Mail-Nachrichten. Dadurch, dass in diesem Pool auch legitime Beispielnachrichten als Proben vorhanden sind, verringert sich die Wahrscheinlichkeit von Fehlern. Da IMF die Merkmale von legitimen ebenso wie von unerwünschten Nachrichten erkennt, kann er zwischen diesen beiden Nachrichten relativ zuverlässig unterscheiden.

IMF wird auf Exchange-Servern installiert, die eingehende SMTP-Nachrichten aus dem Internet akzeptieren. Wenn ein externer Benutzer E-Mails an einen Exchange-Server mit IMF sendet, wertet IMF den Textinhalt der Nachrichten aus und weist jeder Nachricht eine Bewertungsstufe zu, aus der die Wahrscheinlichkeit hervorgeht, dass es sich um Spam handelt. Die Bewertungsskala reicht von 1 bis 9 und wird in Form einer Nachrichteneigenschaft gespeichert, die als Spamvertrauensstufe (SCL) bezeichnet wird. Diese Bewertung bleibt in der Nachricht erhalten, wenn sie an andere Exchange-Server gesendet wird. Die folgende Abbildung zeigt den Gesamtprozess.

![](images/Cc875815.AFSESE08(de-de,TechNet.10).gif)

**Abbildung 8. Intelligente Nachrichtenfilterung mit Exchange**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese08_big(de-de,technet.10).gif)

Nachdem IMF der Nachricht eine SCL-Bewertung zugewiesen hat, wird die Nachricht mit zwei vom Administrator konfigurierten Schwellenwerten verglichen:

1.  **Gateway: Blockierungskonfiguration: Nachrichten blockieren, deren SCL-Bewertung größer oder gleich folgendem Wert ist**. Wenn die SCL-Bewertung einer Nachricht mindestens so hoch wie der festgelegte Schwellenwert ist, können folgende Aktionen in Bezug auf die Nachricht durchgeführt werden:

    -  Archivieren

    -  Löschen

    -  Keine Aktion

    -  Ablehnen

2.  **Junk-E-Mail-Konfiguration für Informationsspeicher: Nachrichten verschieben, deren SCL-Bewertung größer oder gleich folgendem Wert ist**. Wenn die SCL-Bewertung der Nachricht größer als der festgelegte Schwellenwert ist, wird die Nachricht in den Junk-E-Mail-Ordner des Benutzerposteingangs gesendet, es sei denn, der Absender ist beim Benutzer auf der Liste der sicheren Absender angegeben.

###### Anti-Phishing

Phishing ist eine Art von betrügerischen Mails, mit deren Hilfe sich die Absender Ihr Identitätsprofil aneignen. Durch Phishing versuchen Datendiebe, Opfern unter Vortäuschung falscher Tatsachen wichtige persönliche Daten wie Kreditkartennummern, Kennwörter oder Kontodaten zu entlocken (etwa durch E-Mails, in denen Sie zum Bestätigen von Kontodaten aufgefordert werden).

Mit Exchange Server 2003 SP2 wird der IMF um Anti-Phishing-Technologie erweitert, so dass auch Phishing-Nachrichten mit einer entsprechenden SCL-Bewertung versehen und entsprechend behandelt werden.

###### Benutzerdefinierte Gewichtung

Exchange Server 2003 SP2 bietet auch eine Funktion zur benutzerdefinierten Gewichtung, mit der Administratoren das Verhalten des IMF individuell auf bestimmte Zeichenfolgen im Text der E-Mail und/oder in ihrer Betreffzeile abstimmen können.

Die benutzerdefinierte Gewichtung wird durch Einfügen der XML-Datei MSExchange.UceContentFilter.xml in dasselbe Verzeichnis implementiert, in dem sich auch die Dateien MSExchange.UceContentFilter.dll und .dat auf dem Server befinden, auf dem der IMF installiert ist. Wenn der virtuelle SMTP-Server gestartet und der IMF initialisiert werden, wird die XML-Datei geladen.

In der XML-Datei ist definiert, welche Zeichenfolgen der IMF besonders stark oder gering gewichten soll. Auf diese Weise können Sie den IMF individuell anpassen, wenn es aus geschäftlichen Gründen erforderlich ist, Nachrichten mit bestimmten Zeichenfolgen anzunehmen, die der IMF im Normalfall mit einer anderen SCL-Bewertung versehen würde.

Bei Microsoft.com werden 38 Prozent der eingehenden Nachrichten, die die Filterung auf Verbindungs- und Protokollebene passieren, durch den IMF blockiert.

###### Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

Wenn eine Nachricht die serverbasierten Spamschutzfunktionen erfolgreich durchlaufen hat, kann der Outlook 2003-Client bei Nachrichten aktiv werden, die einen SCL-Wert aufweisen, der größer oder gleich dem im IMF eingestellten Wert für die Speicherung von Junk-E-Mail ist. Nachrichten, die diesen Wert erreichen, werden in den Junk-E-Mail-Ordner des Posteingangs von Outlook 2003 gesendet.

In Outlook 2003 und Outlook Web Access für Exchange Server 2003 haben Benutzer außerdem die Möglichkeit, eine Liste mit sicheren Absendern zu erstellen, von denen alle E-Mails angenommen werden sollen, sowie eine Liste mit blockierten Absendern, von denen alle E-Mails abgelehnt werden sollen. Am Postfachspeicher befördert Exchange unabhängig von der SCL-Bewertung, die der Nachricht zugewiesen wurde, alle Nachrichten von sicheren Absendern in den Posteingang des Benutzers und alle Nachrichten von blockierten Absendern in den Junk-E-Mail-Ordner des Benutzers. Wurde die E-Mail jedoch durch den Gatewayschwellenwert blockiert, so gelangt sie nicht in den Posteingang des Benutzers, da sie im Postfachspeicher gar nicht erst ankommt.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Herausforderungen

Die Flut unangeforderter, oftmals anstößiger und mitunter betrügerischer unerwünschter kommerzieller E-Mails, allgemein Spam genannt, schränkt die Möglichkeiten aller Benutzer ein, E-Mails als Kanal für Kommunikation und legitimen E-Commerce zu verwenden.

Für viele Einzelbenutzer und Regionen ist Spam zu einem so großen Problem geworden, dass der Posteingang kein sinnvoller Kommunikationsspeicherbereich mehr ist, da legitime Geschäfts-E-Mails in einem Meer von Spam einfach untergehen. In mittelgroßen Unternehmen treibt Spam aufgrund der Beanspruchung des Servers und des Netzwerks sowie der höheren Datenträgerauslastung auch die Kosten für das Messaging in die Höhe.

Mittelgroße Unternehmen stehen somit vor der Herausforderung, legitime E-Mails zuzulassen und Spam-E-Mails zu blockieren. Sie benötigen Methoden zur Bekämpfung von Spam in einer Exchange Server-Umgebung.

Microsoft Exchange Server 2003 mit SP2 verwendet mehrere Filtermethoden zur Verringerung der Spam-Flut. Diese Methoden sind die schichtweise aufgebauten Antispam-Lösungen zum Schutz auf Verbindungs-, Protokoll- und Inhaltsebene, die bereits weiter oben erwähnt wurden. Diese Methoden sind flexibel. Wenn die Wirkungsweise der einzelnen Methoden verstanden wird, können IT-Administratoren und Benutzer die Spamschutzstufe individuell einstellen. Mittelgroße Unternehmen haben damit die Möglichkeit, eine sinnvolle Balance zwischen E-Mail-Zugriff und Spamfilterung zu gewährleisten.

Es ist wichtig, dass Exchange-Administratoren und -Implementierer verstehen, wie die einzelnen Methoden funktionieren und zusammenwirken, um die Gesamtmenge an Spam zu verringern, die im Posteingang eines Benutzers ankommt. Die folgende Abbildung zeigt das Schichtenmodell zum Schutz vor Spam.

![](images/Cc875815.AFSESE09(de-de,TechNet.10).gif)

**Abbildung 9. Antispam-Framework von Exchange Server 2003**  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese09_big(de-de,technet.10).gif)

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Lösungen

In diesem Abschnitt werden die Voraussetzungen, die Entwicklung, die Bereitstellung und die Verwaltung von Microsoft Exchange Server 2003 Antispam-Framework-Lösungen zum Kampf gegen Spam in mittelgroßen Unternehmen behandelt.

#### Leistungsnachweise

Für eine wirksame Spambekämpfung muss zunächst die Gesamtsstruktur des Exchange Server 2003-E-Mail-Systems bewertet werden. Dabei muss festgestellt werden, welche Tools verfügbar sind und wie diese Tools effektiv eingesetzt werden können. Eine sorgfältige Beurteilung der Umgebung muss im Rahmen der Risikobewertungsstrategie vorgenommen werden.

Das Antispam-Framework von Microsoft Exchange Server 2003 besteht aus einer Kombination mehrerer Methoden, nämlich Verbindungsfilterung, Protokollfilterung und Inhaltsfilterung. Ein Verständnis dessen, wie diese Methoden funktionieren und wie sie zusammenwirken, ist von entscheidender Bedeutung. Zudem lassen sich die Chancen einer erfolgreichen Implementierung und Verwaltung dieser Technologien erhöhen, wenn ein entsprechendes Benutzerbewusstsein vorhanden ist.

Dabei sollten die folgenden Fragen berücksichtigt werden:

1.  Ist Exchange Server 2003 installiert?

    Damit die Vorteile des Antispam-Frameworks von Exchange Server 2003 genutzt werden können, muss Exchange Server 2003 auf der entsprechenden Windows-Plattform installiert sein.

    **Hinweis**   Microsoft Exchange Server 2003 kann unter Windows 2003 oder Windows 2000 mit SP3 oder höher installiert werden. Eine detaillierte Auflistung der Voraussetzungen für Exchange Server würde den Rahmen dieses Dokuments sprengen. Entsprechende Informationen finden Sie auf der Seite [Installieren von neuen Exchange 2003-Servern](http://www.microsoft.com/technet/prodtechnol/exchange/guides/ex2k3depguide/a3318f57-3536-4e65-9309-9300cda23c73.mspx?mfr=true) (möglicherweise in englischer Sprache) im Microsoft TechNet unter www.microsoft.com/technet/prodtechnol/exchange/guides/Ex2k3DepGuide/a3318f57-3536-4e65-9309-9300cda23c73.mspx?mfr=true.

2.  Wurde Exchange Server bereits mit Exchange 2003 SP2 ausgestattet?

    Exchange Server 2003 SP2 ist ein kumulatives Update, das für das Messaging von Exchange Server 2003 folgende Verbesserungen bringt:

    -   E-Mail-Verbesserungen im Mobilbereich

    -   Optimierungen des Postfachs

    -   Besserer Schutz vor Spam

    SP2 ermöglicht besseren Schutz vor Spam (siehe oben), um eine sicherere und zuverlässigere Messagingumgebung zu schaffen. Es umfasst folgende verbesserte Schutzfunktionen:

    -   Einen aktualisierten und integrierten intelligenten Nachrichtenfilter für Exchange auf der Basis der von Microsoft Research entwickelten und patentierten SmartScreen-Filtertechnologie.

    -   Neue Unterstützung des Sender ID-Authentifizierungsprotokolls für E-Mails, wodurch Phishing- und Spoofingangriffe wirksamer abgewehrt werden können.

3.  Ist der virtuelle SMTP-Standardserver im Exchange-System-Manager aktiviert?

    Empfängerfilterung, intelligente Filterung, Sender ID-Filterung und Verbindungsfilterung werden über die globalen Einstellungen konfiguriert und müssen auch auf SMTP-Ebene aktiviert sein. Deshalb muss SMTP bereits aktiviert sein, bevor Sie Änderungen an diesen Diensten vornehmen.

4.  Ist auf den Clientarbeitsstationen Outlook 2003 installiert?

    Die Server sind möglicherweise korrekt konfiguriert. Wenn jedoch die Clients mit älteren Outlook-Versionen arbeiten, können sie nicht von den Vorteilen profitieren, die das Antispam-Framework von Microsoft Exchange Server 2003 bietet.

    Wenn alle notwendigen Voraussetzungen bei Exchange Server 2003 und den Clients erfüllt sind, können die folgenden Methoden bereitgestellt werden:

    -  Schutz auf Verbindungsebene

        IP-Verbindungsfilterung

        Echtzeit-Sperrlisten

    -  Schutz auf Protokollebene

        Empfänger- und Absenderblockierung

        Sender ID

    -  Schutz auf Inhaltsebene

        Intelligenter Nachrichtenfilter für Exchange

        Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

#### Entwicklung

Im Abschnitt „Leistungsnachweise“ wurden einige Fragen zu Exchange Server 2003 und zu Clientvoraussetzungen für die Nutzung des Antispam-Frameworks von Microsoft Exchange Server 2003 formuliert und beantwortet.

Bei den Lösungen zur Bekämpfung von Spam in Exchange-Umgebungen geht es jedoch auch um Clientsicherheit und die Schulung der Benutzer. Für eine erfolgreiche Spambekämpfung sollten alle diese Ansätze in der Exchange-Umgebung miteinander kombiniert werden.

Alle Spamschutzmethoden des Antispam-Frameworks von Microsoft Exchange Server 2003 können implementiert werden, wenn folgende Voraussetzungen gegeben sind:

-   Exchange Server 2003 wurde auf den entsprechenden Windows-Plattformen installiert.

-   Outlook 2003 und Outlook Web Access wurden eingerichtet und konfiguriert.

-   Die neuesten empfohlenen Updates und Patches wurden angewendet, darunter auch Service Pack 2.

Je besser Sie die Funktionsweise der einzelnen Methoden und deren Interaktion verstehen, desto erfolgreicher können Sie sie anwenden. Nachdem die Methoden bereits oben kurz vorgestellt wurden, wird nun in diesem Abschnitt genauer auf die Voraussetzungen eingegangen, die für die Bereitstellung und Verwaltung der Methoden erfüllt sein müssen.

##### Schutz auf Verbindungsebene

Exchange Server 2003 SP2 bietet die Möglichkeit der Verbindungsfilterung, bei der die IP-Adresse des verbindenden Servers mit einer Liste der verweigerten IP-Adressen (der Echtzeit-Sperrliste) verglichen wird. Der Vergleich von IP-Adressen erfolgt sofort nach dem Initiieren der SMTP-Sitzung. Somit kann das Unternehmen die Verbindungen bereits zu Beginn der Nachrichtenübermittlung blockieren. Noch bevor ein auf der Echtzeit-Sperrliste aufgeführter Server Nachrichten senden kann, wird die Verbindung abgebrochen. Mit diesem Ansatz lassen sich Leistungsverluste sowohl auf der Messaging- als auch auf der Netzwerkebene verhindern.

Mittelgroße Unternehmen können die Verbindungsfilterung in Exchange Server 2003 SP2 entweder durch die manuelle Erstellung einer globalen Verweigerungsliste und einer globalen Annahmeliste oder über von Drittanbietern verwaltete Datenbanken bekannter blockierter IP-Adressen erzielen.

Die Mehrheit der Exchange Server 2003 SP2-Server befindet sich hinter dem Umkreis eines Unternehmens und greift nicht direkt auf das Internet zu. In dieser Anordnung ist die Verbindungsfilterung weniger effektiv, da es bei dieser Funktion darauf ankommt, dass die IP-Adresse des ursprünglichen Absenders abgerufen wird, um eine DNS-Abfrage ausführen zu können. In SP2 wird dieser Mangel durch einen Headeranalyse-Algorithmus ausgeglichen, mit dem die Ursprungs-IP-Adressen abgerufen werden. Exchange Server 2003 SP2 mit Verbindungsfilterung kann an jeder Stelle des Unternehmens positioniert werden und die Filterung in der gleichen Weise wie im Umkreis durchführen.

###### IP-Verbindungsfilterung

Ein mittelgroßes Unternehmen kann eine eigene statische Liste mit verweigerten IP-Adressen erstellen. Wie der Name schon sagt, enthält die globale Verweigerungsliste bestimmte IP-Adressen und Netzwerke, von denen ein Unternehmen niemals E-Mails annehmen möchte. Ebenso kann ein mittelgroßes Unternehmen auch eine globale Annahmeliste erstellen – eine Liste mit IP-Adressen und Netzwerken, deren E-Mails niemals blockiert oder in die Filterung einbezogen werden sollen. Die globale Annahmeliste kann beispielsweise IP-Adressen von Tochterunternehmen oder Handelspartnern enthalten, zu denen das Unternehmen ein Vertrauensverhältnis hat. In diesem Fall möchte das Unternehmen keine falschen Verdächtigungen riskieren und trägt deshalb die vertrauenswürdigen IP-Adressen der E-Mail-Server des Absenders in seine globale Annahmeliste ein.

###### Echtzeit-Sperrlisten

Eine Echtzeit-Sperrliste ist eine DNS-basierte Datenbank mit IP-Adressen bekannter, nachgewiesener Spamquellen. Echtzeit-Sperrlisten sind erhältlich bei Firmen, die sich auf die fortlaufende Überwachung des Internets und die Verfolgung bekannter Spamquellen spezialisiert haben. Wenn unerwünschte IP-Adressen erkannt werden, so werden sie zu einer Echtzeit-Sperrlisten-Datenbank hinzugefügt. Solche Listen sind häufig kostenlos erhältlich oder werden gegen eine Gebühr bereitgestellt, wenn Messagingadministratoren einen umfangreicheren Dienst wünschen.

Exchange Server 2003 SP2 bietet die Möglichkeit, solche Echtzeit-Sperrlisten von Drittanbietern zu nutzen. Wenn der Exchange Server 2003 mit SP2 für die Nutzung einer Echtzeit-Sperrliste konfiguriert wurde, vergleicht er die IP-Adresse des sendenden Servers mit der Echtzeit-Sperrlisten-Datenbank und verweigert die Verbindung, wenn die Adresse auf der Liste steht.

Da die Filterung bei Echtzeit-Sperrlisten anhand der IP-Adresse des sendenden Servers und nicht anhand des Inhalts der Nachrichten erfolgt, fallen Echtzeit-Sperrlisten im Bereich der Antispam-Software von Drittanbietern technisch gesehen in eine eigene Kategorie. Die Echtzeit-Sperrliste agiert gewissermaßen als Türsteher, indem sie verhindert, dass Nachrichten von bekannten bösartigen oder fragwürdigen Servern in die Computerumgebung des Unternehmens eindringen. Eine Nachricht, die die Echtzeit-Sperrliste unbeschadet passiert, ist dem Eindringen in das Netzwerk einen Schritt näher, allerdings nur so lange, bis ihr Inhalt von der nächsten Schicht des Messagingschutzes, etwa durch den intelligenten Nachrichtenfilter, genauer überprüft wird.

Aufgrund der Menge an DNS-Abfragen (mehrere Zehnmillionen) in Verbindung mit Echtzeit-Sperrlisten, die die IT-Abteilung von Microsoft (Microsoft IT) Tag für Tag durchführt, überträgt Microsoft IT in vorab definierten, regelmäßigen Abständen (meist mehrmals am Tag) eine exakte Kopie der Echtzeit-Sperrliste an seine lokalen DNS-Server. Die meisten Anbieter benötigen lokale Kopien der Echtzeit-Sperrlisten für Größenordnungen von mehr als 250.000 Abfragen pro Tag. Die Übertragung einer Kopie der Echtzeit-Sperrliste wird als Zonentransfer vom Listenanbieter bezeichnet. Microsoft IT hat seine Exchange Server 2003 SP2-Gateways so konfiguriert, dass DNS-Abfragen in Verbindung mit Echtzeit-Sperrlisten in Bezug auf diese DNS-Server durchgeführt werden.

##### Schutz auf Protokollebene

Nachdem die SMTP-Nachricht den Schutz auf Verbindungsebene durchlaufen hat, trifft sie auf der SMTP-Protokollebene auf die nächste Schutzschicht. Hier wird der SMTP-Dialog zwischen dem sendenden SMTP-Host und dem empfangenden SMTP-Host analysiert, um festzustellen, ob Absender und Empfänger zugelassen sind, und um den SMTP-Domänennamen des Absenders zu ermitteln.

###### Empfänger- und Absenderblockierung

Mit der Empfängerfilterung von Exchange Server 2003 SP2 sind mittelgroße Unternehmen in der Lage, sich vor zielgerichtetem Mailbombing zu schützen oder dessen Auswirkungen zumindest abzumildern. Oftmals brauchen die Empfänger, die zum Ziel solcher Angriffe werden, gar keine Nachrichten aus dem Internet zu empfangen. Die Empfängerfilterung lehnt Nachrichten anhand bestimmter Kriterien wie dem beabsichtigten Empfänger der Nachricht bereits auf der Gateway-Ebene ab.

Obwohl die Empfängerfilterung bei der Bekämpfung von Echtzeit-Spamgefahren nicht so effektiv ist wie Echtzeit-Antispam-Lösungen, kann sie bei der Verringerung der Risiken von Mailbombing-Angriffen äußerst wichtige Dienste leisten. Vor kurzem war Microsoft IT dank der Empfängerfilterung in der Lage, Millionen von Nachrichten zu blockieren, die an einem einzigen Tag an nur wenige Empfänger gesendet wurden.

###### Sender ID

Das Sender ID-Framework ist ein E-Mail-Authentifizierungsprotokoll, mit dem sich Spoofing und Phishing dadurch abwehren lassen, dass der Name der Domäne überprüft wird, von der aus die E-Mail gesendet wird. Sender ID überprüft den Ursprung von E-Mails, indem die IP-Adresse des Absenders mit dem angeblichen Inhaber der sendenden Domäne verglichen wird.

Dabei wird zu überprüfen versucht, ob jede E-Mail von der Internet-Domäne stammt, von der sie angeblich gesendet wurde. Diese Überprüfung wird dadurch erreicht, dass die Adresse des Servers, der die E-Mail sendet, mit einer Liste registrierter Server verglichen wird, die der Domäneninhaber zum Versenden von E-Mail autorisiert hat. Diese Überprüfung wird automatisch vom Internetdienstanbieter (ISP) oder vom Mailserver des Empfängers vorgenommen, bevor die E-Mail dem Benutzer zugestellt wird. Das Ergebnis der Sender ID-Überprüfung kann als zusätzliche Eingabe für die vom Server bereits angewendeten Filterungsfunktionen genutzt werden. Wenn der Absender authentifiziert wurde, kann der Mailserver frühere Verhaltensweisen, Datenverkehrsmuster und Absenderreputationen sowie konventionelle Inhaltsfilter berücksichtigen, wenn es zu entscheiden gilt, ob die Mail dem Empfänger zugestellt werden soll.

##### Schutz auf Inhaltsebene

Im Idealfall sollte Spam niemals die Clients erreichen. In der Realität gelangen jedoch immer auch einige Spamnachrichten auf die Desktopcomputer der Benutzer. Einer der Hauptgründe hierfür ist die Tatsache, dass einige legitime E-Mails, wie etwa Newsletter, oftmals bestimmte Spammerkmale aufweisen, weshalb es nicht sinnvoll ist, den Filterungsschwellenwert so einzustellen, dass alle verdächtigen Nachrichten gelöscht werden. Zudem haben möglicherweise einige Benutzer individuelle Präferenzen, denen unternehmensweit einheitliche Einstellungen nicht gerecht werden können.

###### Intelligenter Nachrichtenfilter für Exchange

Der erste Filter, den eingehende E-Mail-Nachrichten aus dem Internet durchlaufen müssen, ist der intelligente Nachrichtenfilter, der auf den Exchange Server 2003 SP2-Gatewayservern am äußersten Rand der Messagingumgebung ausgeführt wird. Der intelligente Nachrichtenfilter verwendet SCL, PCL (Phishing-Vertrauensstufe, einer der Faktoren beim Zuweisen von SCL-Bewertungen) und das in Exchange Server 2003 SP2 integrierte Sender ID-Framework. Der Filter kategorisiert bestimmte Teile der Nachricht, führt eine heuristikbasierte Nachrichtenanalyse durch und weist jeder geprüften Nachricht eine SCL-Bewertung von 0 bis 9 zu. Je höher die Bewertung ist, die eine Nachricht erhält, desto größer ist die Wahrscheinlichkeit, dass es sich um Spam handelt.

Exchange Server 2003 SP2 bezieht die neuesten Daten und Updates in den intelligenten Nachrichtenfilter ein. Verbesserungen am IMF und Updates in zweiwöchigen Zeitabständen sorgen für ständige Fortschritte beim Identifizieren von Spam und beim Vermeiden von falschen Verdächtigungen. Zu diesen Verbesserungen gehören neue Möglichkeiten der Spambekämpfung, beispielsweise die Blockierung von Phishing-Szenarios. Bei Phishing-Szenarios wird durch Vortäuschung einer legitimen E-Mail versucht, vertrauliche persönliche Informationen zu erlangen.

Die Exchange Server 2003 SP2-Umgebung kann so konfiguriert werden, dass Filteraktionen an Nachrichten durchgeführt werden, die eine SCL-Bewertung aufweisen, die über dem vom Administrator festgelegten Schwellenwert liegt. Der intelligente Nachrichtenfilter verwendet zwei Schwellenwerte, die in Exchange Server 2003 SP2 festgelegt werden: den Gatewayschwellenwert und den Speicherschwellenwert.

###### Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

-   **Junk-E-Mail-Filter**. Mithilfe modernster, von Microsoft Research entwickelter Technologie entscheidet Outlook 2003, ob eine Nachricht als Junk-E-Mail zu behandeln ist. Diese Entscheidung erfolgt anhand mehrerer Faktoren, etwa anhand des Zeitpunkts, zu dem die Nachricht abgesendet wurde, sowie anhand des Inhalts und der Struktur der Nachricht. Der Filter sondert keinen bestimmten Absender oder E-Mail-Typ aus. Vielmehr bestimmt er durch ein hoch entwickeltes Analyseverfahren, wie groß die Wahrscheinlichkeit ist, dass der Empfänger die Nachricht als Junk-E-Mail einstufen würde.

    Dieser Filter ist standardmäßig auf einen geringen Wert eingestellt, so dass zumindest die offensichtlichsten Junk-E-Mails herausgefiltert werden. Die herausgefilterten Nachrichten werden in einen speziellen Junk-E-Mail-Ordner verschoben, so dass später auf sie zugegriffen werden kann. Auf Wunsch können Sie den Filter rigoroser einstellen (wodurch eventuell auch mehr legitime Nachrichten ausgesondert werden) oder sogar Outlook 2003 so einstellen, dass eingehende Junk-E-Mails sofort unwiederbringlich gelöscht werden. Erfahren Sie Näheres über den Junk-E-Mail-Filter.

-   **Liste sicherer Absender**. Wenn eine E-Mail-Nachricht vom Filter versehentlich als Junk-E-Mail gekennzeichnet wird, können Sie den Absender dieser Nachricht mühelos Ihrer Liste sicherer Absender hinzufügen. E-Mails von Adressen und Domänennamen, die auf der Liste sicherer Absender stehen, werden niemals als Junk-E-Mail behandelt, unabhängig von ihrem Inhalt. Die entsprechenden Kontakte werden standardmäßig als vertrauenswürdig betrachtet, und von ihnen stammende Nachrichten werden niemals als Junk-E-Mail betrachtet. Wenn in Ihrem Unternehmen Microsoft Exchange Server verwendet wird, werden auch Nachrichten, die aus dem Unternehmen selbst stammen, niemals als Junk-E-Mail behandelt. Sie können Outlook 2003 so konfigurieren, dass nur Nachrichten aus der Liste sicherer Absender angenommen werden. Dadurch haben Sie volle Kontrolle darüber, welche Nachrichten Sie empfangen.

-   **Liste blockierter Absender**. E-Mail-Nachrichten von bestimmten E-Mail-Adressen oder Domänennamen können Sie einfach blockieren, indem Sie die Absender Ihrer Liste blockierter Absender hinzufügen. Nachrichten von Personen oder Domänennamen auf Ihrer Liste blockierter Absender werden unabhängig von ihrem Inhalt immer als Junk-E-Mail behandelt.

-   **Liste sicherer Empfänger**. Eine E-Mail-Liste oder -Gruppe, der Sie selbst angehören, können Sie Ihrer Liste sicherer Empfänger hinzufügen. Nachrichten, die an die E-Mail-Adressen oder Domänennamen gesendet werden, die auf dieser Liste stehen, werden nicht als Junk-E-Mail behandelt, und zwar unabhängig vom Absender und vom Inhalt der Nachrichten.

-   **AutoUpdate**. Sie können Ihren Junk-E-Mail-Filter regelmäßig mit Updates von Microsoft aktualisieren, damit Ihnen stets die neuesten Methoden zum Blockieren unerwünschter Nachrichten zur Verfügung stehen. Microsoft stellt regelmäßig Updates des Junk-E-Mail-Filters bereit.

#### Bereitstellung und Verwaltung

Das Hauptziel des Antispam-Frameworks von Microsoft Exchange Server 2003 ist es, ein Bewusstsein dafür zu entwickeln, wie die einzelnen Methoden dieses Frameworks funktionieren und wie sie einander ergänzen. Wenn das Gesamtkonzept dieses Frameworks verstanden wird, sind mittelgroße Unternehmen bei korrekter Bereitstellung und Verwaltung dieser Technologien in der Lage, Spam in Microsoft Exchange Server-Umgebungen wirksam zu bekämpfen. Zur Unterstützung des Kampfes gegen Spam sollten die Benutzer über gewisse Grundkenntnisse auf diesem Gebiet verfügen, um den richtigen Umgang mit den Clientcomputern in ihrer Umgebung zu gewährleisten. Darüber hinaus wird die Überwachung und Problembehandlung der intelligenten Nachrichtenfilterung im Rahmen der fortlaufenden Verwaltung behandelt.

Die unten genannten Funktionen müssen sowohl in den globalen Einstellungen als auch auf der SMTP-Ebene konfiguriert werden. Auf das Bewusstsein der Benutzer wird am Ende dieses Abschnitts noch näher eingegangen.

In diesem Abschnitt werden die folgenden Verfahren schrittweise erläutert:

-   Schutz auf Verbindungsebene

    -   IP-Verbindungsfilterung

    -   Echtzeit-Sperrlisten

-   Schutz auf Protokollebene

    -   Empfänger- und Absenderblockierung

    -   Sender ID

-   Schutz auf Inhaltsebene

    -   Intelligenter Nachrichtenfilter für Exchange

    -   Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

##### Schutz auf Verbindungsebene

Exchange Server 2003 unterstützt die *Verbindungsfilterung* auf der Basis von Echtzeit-Sperrlisten. Diese Funktion vergleicht die eingehende Internet Protocol-Adresse (IP-Adresse) mit einer Echtzeit-Sperrliste eines Drittanbieters und überprüft dabei die Kategorien, die Sie filtern möchten. Wenn eine Übereinstimmung mit der Echtzeit-Sperrliste gefunden wird, antwortet SMTP mit einer Fehlermeldung des Typs *550 5.x.x* auf den Befehl *RCPT TO*, und eine benutzerdefinierte Fehlerantwort wird an den Absender geschickt. Sie können auch mehrere Verbindungsfilter verwenden und dabei festlegen, in welcher Reihenfolge diese Filter angewendet werden sollen.

Wenn Sie einen Verbindungsfilter erstellen, legen Sie eine Regel fest, nach der SMTP eine DNS-Suche in einer Sperrliste ausführt, die von einem RBL-Dienstanbieter bereitgestellt wird. Der Verbindungsfilter vergleicht jede eingehende IP-Adresse mit der Sperrliste des Drittanbieters. Der RBL-Anbieter sendet eine von zwei Antworten:

-   **Host nicht gefunden**. Diese Antwort bedeutet, dass die IP-Adresse nicht auf der Sperrliste steht.

-   **127.0.0.x**. Diese Antwort ist ein Antwortstatuscode, aus dem hervorgeht, dass die entsprechende IP-Adresse in der Sperrliste gefunden wurde. Das x kann je nach Anbieter verschiedene Werte annehmen.

Wenn die eingehende IP-Adresse auf der Liste gefunden wurde, antwortet SMTP mit einer Fehlermeldung des Typs *5.x.x* auf den Befehl *RCPT TO* (d. h. auf den SMTP-Befehl, den der verbindende Server erteilt, um den beabsichtigten Nachrichtenempfänger zu identifizieren).

###### Anbieter von Echtzeit-Sperrlisten

Da verschiedene Provider von Echtzeit-Sperrlisten verschiedene Arten von Listen und Diensten anbieten, sollten mittegroße Unternehmen zunächst mehrere Anbieter unter die Lupe nehmen, bevor sie sich für einen bestimmten Anbieter entscheiden. Zwei bekannte Anbieter sind [Spam Haus](http://www.spamhaus.org/) unter www.spamhaus.org und [Spam Cop](http://www.spamcop.net/) unter www.spamcop.net.

Die Antworten auf die folgenden Fragen können bei der Auswahl des richtigen RBL-Anbieters hilfreich sein:

-   **Qualität der Liste**. Überprüft jemand, ob es sich bei IP-Adressen, die der Liste hinzugefügt werden, tatsächlich um Spammer handelt? Kann jeder Ergänzungen an der Liste vornehmen?

-   **Sicherheit der Liste**. Durchläuft die Liste irgendwelche Sicherheitsprüfungen? Überprüft jemand, ob keine IP-Adressen versehentlich oder böswillig hinzugefügt wurden?

-   **Prozess zum Aktualisieren der Liste**. Wie werden die Listen aktualisiert? Wenn die Hinzufügung zur Liste automatisch erfolgt, sollte auch das Entfernen aus der Liste automatisch erfolgen, wenn kein Spamming mehr stattfindet. Wie schnell werden Listen aktualisiert?

-   **Listenübertragung**. Gestattet der Anbieter vollständige oder schrittweise BIND-Übertragungen (BIND = Berkeley Internet Name Domain), die mit Windows DNS direkt kompatibel sind?

-   **Support vom Sperrlistenanbieter**. Welches Maß an Support bietet der Anbieter?

###### IP-Verbindungsfilterung

**So konfigurieren Sie die IP-Verbindungsfilterung**

1.  Erweitern Sie innerhalb von Exchange-System-Manager den Container **Globale Einstellungen**.

2.  Klicken Sie mit der rechten Maustaste auf **Nachrichtenübermittlung**, und klicken Sie dann auf **Eigenschaften**.

3.  Klicken Sie auf die Registerkarte **Verbindungsfilterung**.

4.  Entscheiden Sie sich für eine der folgenden Optionen: **Annehmen**, **Verweigern** oder **Ausnahme**. Im nachstehenden Beispiel ist „Verweigern“ ausgewählt.

5.  Sie haben die Wahl zwischen **Einzelne IP-Adresse** und **Gruppe von IP-Adressen** (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE10(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese10_big(de-de,technet.10).gif)

###### Echtzeit-Sperrlisten (RBL)

**So konfigurieren Sie die Echtzeit-Sperrlistenfunktionalität auf der Ebene der globalen Einstellungen**

1.  Erweitern Sie innerhalb von Exchange-System-Manager den Container **Globale Einstellungen**.

2.  Klicken Sie mit der rechten Maustaste auf das Objekt **Nachrichtenübermittlung**, und wählen Sie **Eigenschaften**.

3.  Klicken Sie auf die Registerkarte **Verbindungsfilterung**.

4.  Zum Erstellen einer Verbindungsfilterregel klicken Sie auf **Hinzufügen** (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE11(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese11_big(de-de,technet.10).gif)

5.  Geben Sie in das Feld **Anzeigename** einen Namen für den Verbindungsfilter ein.

6.  Geben Sie unter **DNS-Suffix des Anbieters** das DNS-Suffix des Anbieters ein (Beispiel: contoso.com).

7.  Unter **Benutzerdefinierte Fehlermeldung für Rückgabe** können Sie auf Wunsch eine benutzerdefinierte Fehlermeldung eingeben, die an den Absender zurückgegeben werden soll. Lassen Sie dieses Feld leer, wenn die folgende Standardfehlermeldung verwendet werden soll:

    *&lt;IP-Adresse&gt;* wurde blockiert von *&lt;Name der Verbindungsfilterregel&gt;*

    Eine benutzerdefinierte Meldung kann mit folgenden Variablen generiert werden:

    -   **%0**. Verbindende IP-Adresse

    -   **%1**. Regelname des Verbindungsfilters

    -   **%2**. RBL-Anbieter

    Beispiel: Ihre benutzerdefinierte Meldung soll folgendermaßen lauten:

    Die IP-Adresse *&lt;IP-Adresse&gt;* wurde durch folgenden RBL-Anbieter blockiert: *&lt;Name des RBL-Anbieters&gt;*.

    In diesem Fall müssten Sie in das Feld **Benutzerdefinierte Fehlermeldung für Rückgabe** Folgendes eingeben:

    Die IP-Adresse %0 wurde durch folgenden RBL-Anbieter blockiert: %2.

    **Hinweis**   Exchange ersetzt „%0“ durch die verbindende IP-Adresse und „%2“ durch den RBL-Anbieter.

8.  Um festzulegen, welche vom RBL-Anbieter zurückgegebenen Rückgabestatuscodes in diesem Verbindungsfilter verglichen werden sollen, klicken Sie auf **Rückgabestatuscode**. Daraufhin wird das folgende Dialogfeld angezeigt:

    ![](images/Cc875815.AFSESE12(de-de,TechNet.10).gif)

9.  Wählen Sie im Dialogfeld **Rückgabestatuscode** eine der folgenden Optionen aus:

    -  **Filterregel auf beliebigen Rückgabecode anwenden**. Diese Verbindungsfilterregel wird mit jedem Rückgabestatuscode verglichen, der vom Providerdienst gesendet wird. Bei dieser Regel wird der Standardwert, der dem Verbindungsfilter entspricht, auf einen beliebigen Rückgabestatus gesetzt.

        Beispiele:

        **127.0.0.1**. Sperrliste

        **127.0.0.2**. Bekanntes offenes Relay

        **127.0.0.4**. DFÜ-IP-Adresse

    <!-- -->

    -  **Filterregel auf folgende Maske anwenden**. Diese Verbindungsfilterregel wird mit vom Anbieter zurückgegebenen Rückgabestatuscodes verglichen, wobei die Codes mithilfe einer Maske interpretiert werden. Geben Sie nach den vom Anbieter verwendeten Masken die Maske ein, nach der die Filterung erfolgen soll.

        Beispiele:

        **0000 | 0001**. Sperrliste

        **0000 | 0010**. Offenes Relay

        **0000 | 0011**. Offenes Relay oder Sperrliste

        **0000 | 0100**. DFÜ-Host

        **0000 | 0101**. DFÜ oder Sperrliste

        **0000 | 0110**. DFÜ oder offenes Relay

        **0000 | 0111**. DFÜ, offenes Relay oder Sperrliste

    <!-- -->

    -  **Filterregel auf eine der folgenden Antworten anwenden**. Diese Verbindungsfilterregel wird mit vom Anbieter gesendeten Rückgabestatuscodes verglichen, wobei die spezifischen Werte der Rückgabestatuscodes verwendet werden.

10. Klicken Sie auf **OK**.

Die Absender- und Empfängerfilterung, die intelligente Nachrichtenfilterung und die Verbindungsfilterung funktionieren ebenfalls nur dann korrekt, wenn sie auf SMTP-Ebene angewendet werden. Führen Sie hierzu die folgenden Schritte aus.

**So aktivieren Sie Filterfunktionen auf der SMTP-Ebene**

1.  Starten Sie den Exchange-System-Manager.

2.  Erweitern Sie **Server**.

3.  Erweitern Sie den ***&lt;Servernamen&gt;*** (des zu konfigurierenden E-Mail-Servers).

4.  Erweitern Sie **Protokolle**.

5.  Erweitern Sie **SMTP**.

6.  Klicken Sie mit der rechten Maustaste auf **Virtueller Standardserver für SMTP**, und wählen Sie **Eigenschaften** aus.

7.  Klicken Sie unter **Eigenschaften von Virtueller Standardserver für SMTP** auf **Erweitert**.

8.  Klicken Sie unter **Erweitert** auf **Bearbeiten**.

9.  Aktivieren Sie unter **Identifikation** das Kontrollkästchen **Verbindungsfilter anwenden**, um den Filter anzuwenden, den Sie zuvor festgelegt haben (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE13(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese13_big(de-de,technet.10).gif)

#### Schutz auf Protokollebene

Nachdem die SMTP-Nachricht den Schutz auf Verbindungsebene durchlaufen hat, trifft sie auf der SMTP-Protokollebene auf die nächste Schutzschicht. Hier wird der SMTP-Dialog zwischen dem sendenden SMTP-Host und dem empfangenden SMTP-Host analysiert, um festzustellen, ob Absender und Empfänger zugelassen sind, und um den SMTP-Domänennamen des Absenders zu ermitteln.

##### Empfängerfilterung

Mit der Empfängerfilterungsfunktion verhindern Sie, dass Nachrichten übermittelt werden, die an bestimmte Empfängeradressen gerichtet sind.

**So konfigurieren Sie die Empfängerfilterung**

1.  Starten Sie den Exchange-System-Manager.

2.  Erweitern Sie den Container **Globale Einstellungen**.

3.  Klicken Sie mit der rechten Maustaste auf **Nachrichtenübermittlung**, und wählen Sie **Eigenschaften** aus.

4.  Klicken Sie auf die Registerkarte **Empfängerfilterung**.

5.  Wählen Sie **Empfänger filtern, die nicht im Verzeichnis vorhanden sind** aus.

6.  Klicken Sie auf **Hinzufügen**, und fügen Sie dann die Empfängeradresse hinzu (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE14(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese14_big(de-de,technet.10).gif)

##### Sender ID-Filterung

Mit den Sender ID-Filterungsoptionen konfigurieren Sie verschiedene Sender ID-Aktionen. Über diese Optionen können Sie festlegen, wie der Server mit Nachrichten verfahren soll, die die Sender ID-Überprüfung nicht bestanden haben. Die Sender ID-Funktion ist ein Industriestandard, mit dem Sie besseren Schutz vor unerwünschten kommerziellen E-Mails (UCE) und Phishing-Angriffen erzielen können.

Standardmäßig ist die Sender ID-Filterung auf **Annehmen** eingestellt. Sie können jedoch den Sender ID-Filter hinter dem Umkreis Ihres Netzwerks aktivieren. Hierzu geben Sie die IP-Adressen der Server Ihres internen Netzwerks an, die von der Sender ID-Filterung ausgenommen sein sollen.

**So konfigurieren Sie die Sender ID-Filterung**

1.  Starten Sie den Exchange-System-Manager.

2.  Erweitern Sie den Container **Globale Einstellungen**.

3.  Klicken Sie mit der rechten Maustaste auf **Nachrichtenübermittlung**, und wählen Sie **Eigenschaften** aus.

4.  Klicken Sie auf die Registerkarte **Sender ID-Filterung**.

5.  Wählen Sie die gewünschten Sender ID-Filterungsoptionen aus (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE15(de-de,TechNet.10).gif)

#### Schutz auf Inhaltsebene

Die Inhaltsfilterung von Exchange Server 2003 SP2 basiert auf der Microsoft Research SmartScreen-Technologie für maschinelles Lernen. Diese Technologie ist in die intelligente Nachrichtenfilterung (IMF) integriert. Nachrichten aus dem Internet kommen am Exchange-SMTP-Gateway an und gelangen in das Antispam-Framework von Exchange Server. Die vorhergehenden Schichten der Exchange-Antispam-Lösung (Verbindungs-, Absender- und Empfängerfilterung) blockieren die Nachrichtenübermittlung, noch bevor die eigentlichen Daten der Nachrichten empfangen werden. Wenn eine Nachricht alle diese vorherigen Filter erfolgreich durchlaufen hat, wird der Nachrichtentext zugestellt.

IMF kann sehr genau die Wahrscheinlichkeit beurteilen, dass eine eingehende E-Mail eine legitime Nachricht oder aber Spam ist.

##### Intelligenter Nachrichtenfilter für Exchange

Der intelligente Nachrichtenfilter von Exchange ist eine äußerst wichtige Komponente zur Bekämpfung von Spam. Er ist ein SCL-kompatibler Filter, der eine fortschrittliche serverseitige Nachrichtenfilterung ermöglicht, die speziell zur Bekämpfung von Spam entwickelt wurde. Genauere Informationen finden Sie auf der Website zum [intelligenten Nachrichtenfilter von Exchange](http://go.microsoft.com/fwlink/?linkid=21607) unter http://go.microsoft.com/fwlink/?linkid=21607.

**So konfigurieren Sie den intelligenten Nachrichtenfilter von Exchange**

1.  Starten Sie den Exchange-System-Manager.

2.  Erweitern Sie den Container **Globale Einstellungen**.

3.  Klicken Sie mit der rechten Maustaste auf **Nachrichtenübermittlung**, und wählen Sie **Eigenschaften** aus.

4.  Klicken Sie auf die Registerkarte **Intelligente Nachrichtenfilterung**.

5.  Wählen Sie unter **Nachrichten blockieren, deren SCL-Bewertung größer oder gleich folgendem Wert ist** (siehe folgendes Bildschirmfoto) die gewünschte Bewertungsstufe.

    Die SCL-Bewertungsskala reicht von 0 bis 9. Je höher die Bewertung, desto größer die Wahrscheinlichkeit, dass es sich bei der Nachricht um Spam handelt.

    ![](images/Cc875815.AFSESE16(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese16_big(de-de,technet.10).gif)

##### Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access

Sowohl in Outlook 2003 als auch in Outlook Web Access 2003 sind Funktionen zum Schutz vor Spam vorhanden. Zu diesen Funktionen gehören folgende:

-   **Vom Benutzer zu verwaltende Sperr- und Sicherungslisten**. Die Sperr- und Sicherungslisten von Outlook 2003 und Outlook Web Access sind im Postfach des Benutzers gespeichert. Da beide Clientprogramme dieselbe Liste verwenden, brauchen die Benutzer nicht zwei verschiedene Versionen zu verwalten.

-   **Externe Inhaltsblockierung**. Mit Outlook 2003 und Outlook Web Access 2003 ist es für die Absender von Junk-E-Mails schwieriger, E-Mail-Adressen mithilfe von Beacons abzurufen. Wenn eingehende Nachrichten Inhalte aufweisen, die als Beacon verwendet werden könnten, wird in Outlook und Outlook Web Access automatisch eine entsprechende Warnmeldung angezeigt, unabhängig davon, ob sie tatsächlich einen Beacon enthalten. Wenn sich die Benutzer sicher sind, dass es sich um eine legitime Nachricht handelt, können sie auf die Warnmeldung klicken und den jeweiligen Inhalt herunterladen. Zweifeln die Benutzer an der Legitimität der Nachricht, können sie sie löschen, ohne über die Beacons eine Rückmeldung an den Absender der Junk-Mail auszulösen.

-   **Verbesserte Junk-E-Mail-Verwaltung**. Mit Outlook 2003 können Benutzer Regeln erstellen, mit denen E-Mail-Nachrichten, die bestimmte Wörter oder Zeichenfolgen enthalten, automatisch aus dem Posteingang in einen speziellen Ordner verschoben werden (z. B. in den Ordner Junk-E-Mail oder Gelöschte Objekte). Außerdem haben Benutzer die Möglichkeit, verdächtige Junk-E-Mails sofort zu löschen, anstatt sie in einen speziellen Ordner zu verschieben.

-   **Junk-E-Mail-Filter**. Outlook 2003 verfügt über einen Junk-E-Mail-Filter, der nach typischen Spam-Attributen sucht. (Diese Attribute werden jeweils in Verbindung mit Office-Updates aktualisiert.) Die Anzahl der verdächtigen Attribute wird in Outlook gezählt. Je höher die Zahl dieser Attribute bei einer bestimmten Mail ist, desto größer ist die Wahrscheinlichkeit, dass es sich um Spam handelt. Stellen Sie im Dialogfeld **Junk-E-Mail-Optionen** die gewünschte Junk-E-Mail-Schutzstufe ein.

**So konfigurieren Sie den Junk-E-Mail-Filter von Outlook 2003**

1.  Klicken Sie in Outlook 2003 in der Menüleiste auf **Aktion**.

2.  Wählen Sie **Junk-E-Mail** und anschließend **Junk-E-Mail-Optionen** aus (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE17(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese17_big(de-de,technet.10).gif)

3.  Das nachstehend abgebildete Dialogfeld wird angezeigt. Darin können Benutzer die gewünschte Junk-E-Mail-Schutzstufe wählen.

    ![](images/Cc875815.AFSESE18(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese18_big(de-de,technet.10).gif)

**So konfigurieren Sie den Junk-E-Mail-Filter in Outlook Web Access (OWA)**

1.  Melden Sie sich bei Ihrem Outlook Web Access-Konto an.

2.  Klicken Sie auf **Optionen**.

3.  Klicken Sie auf **Junk-E-Mail-Listen verwalten**.

4.  Wählen Sie die entsprechende Funktion unter **Liste anzeigen oder bearbeiten** aus (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE19(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese19_big(de-de,technet.10).gif)

5.  Nun können Sie Absender-E-Mail-Adressen **hinzufügen**, **bearbeiten** oder **entfernen**.

**Hinweis**   Wenn Benutzer zum ersten Mal diese Junk-E-Mail-Funktionen verwenden oder irgendwann die Optionen ändern, sollten sie sich regelmäßig vergewissern, dass keine berechtigten Nachrichten aus dem Posteingang in einen anderen Ordner verschoben wurden. Updates für die Junk-E-Mail-Funktionen in Outlook 2003 werden im Abschnitt **Office Update** der Website [Microsoft Office Online](http://go.microsoft.com/fwlink/?linkid=24393) unter http://go.microsoft.com/fwlink/?LinkId=24393 aufgeführt.

#### Überwachung und Problembehandlung beim intelligenten Nachrichtenfilter

Bei Problemen mit dem intelligenten Nachrichtenfilter von Microsoft Exchange können die Überwachungs- und Problembehandlungsfunktionen von Ereignisanzeige und Systemmonitor verwendet werden. In diesem Abschnitt finden Sie eine Schritt-für-Schritt-Anleitung zur Verwendung dieser Funktionen.

##### Ereignisanzeige

In der Ereignisanzeige werden sowohl im Anwendungsprotokoll als auch im Systemprotokoll Fehler, Warnungen und informative Ereignisse in Zusammenhang mit Vorgängen in Exchange, dem SMTP-Dienst und anderen Anwendungen angezeigt. Um die Ursache von Problemen mit dem intelligenten Nachrichtenfilter leichter ermitteln zu können, sollten Sie sich Daten im Anwendungs- und Systemprotokoll genau ansehen. Der intelligente Nachrichtenfilter schreibt Ereignisse mithilfe des Protokolls MSExchangeTransport (Quelle) und des SMTP-Protokolls (Kategorie) in die Ereignisanzeige.

**So finden Sie Ereignisse des intelligenten Nachrichtenfilters mithilfe der Ereignisanzeige**

1.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme** und auf **Verwaltung**, und klicken Sie dann auf **Ereignisanzeige**.

2.  Klicken Sie in der Konsolenstruktur auf **Anwendungsprotokoll**.

3.  Um das Protokoll alphabetisch zu sortieren und rasch einen Eintrag für einen Exchange-Dienst zu finden, klicken Sie im Detailbereich auf **Quelle** (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE20(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese20_big(de-de,technet.10).gif)

4.  Wenn Sie aus dem Protokoll diejenigen Ereignisse herausfiltern möchten, die für den intelligenten Nachrichtenfilter gelten, klicken Sie im Menü **Ansicht** auf **Filter**.

5.  Wählen Sie unter **Eigenschaften von Anwendungsprotokoll** in der Quellenliste **Ereignis** den Eintrag **MSExchangeTransport** aus.

6.  Wählen Sie in der Liste **Kategorie** den Eintrag **SMTP-Protokoll** aus.

##### Systemmonitor, Leistungsprotokolle und Leistungswarnungen

Der intelligente Nachrichtenfilter ist mit mehreren Leistungsindikatoren ausgestattet, mit denen Sie seine Leistung und seinen Betrieb überwachen können.

**So verwenden Sie Systemmonitor, Leistungsprotokolle und Leistungswarnungen**

1.  Klicken Sie auf **Start**, zeigen Sie auf **Alle Programme** und auf **Verwaltung**, und klicken Sie dann auf **Leistung**.

2.  Wählen Sie **Systemmonitor** aus, und klicken Sie auf die Schaltfläche **+**, um Leistungsindikatoren hinzuzufügen.

3.  Wählen Sie im Dialogfeld **Leistungsindikatoren hinzufügen** unter **Leistungsobjekt** den Eintrag **MSExchange Intelligenter Nachrichtenfilter** aus (siehe folgendes Bildschirmfoto).

    ![](images/Cc875815.AFSESE21(de-de,TechNet.10).gif)
    [Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875815.afsese21_big(de-de,technet.10).gif)

#### Bewusstsein der Benutzer

Wie bei jeder anderen Verteidigung gegen Bedrohungen und Angriffe, egal, ob Virenbekämpfung, Schutz von Arbeitsstationen vor unbefugten Benutzern oder Abwehr von Spam, sollte der Technologie nicht die alleinige Rolle zukommen. Auch die Benutzer können, wenn sie sich der Gefahren bewusst sind, einen wichtigen Beitrag zum richtigen Umgang mit Spam leisten. Die Benutzer sollten darüber informiert werden, wie sie unerwünschte E-Mails in ihrer Outlook-Umgebung vermeiden oder herausfiltern können.

Dazu sollten sie folgende Anweisungen erhalten:  

-   Antworten Sie niemals auf per E-Mail gesendete Aufforderungen zur Angabe von finanzbezogenen oder persönlichen Daten.

-   Verraten Sie niemals Ihre Kennwörter.

-   Öffnen Sie keine verdächtigen E-Mail-Dateianhänge.

-   Antworten Sie nicht auf verdächtige oder unerwünschte E-Mails.

-   Konfigurieren Sie Junk-E-Mail-Optionen in Outlook 2003 so, wie dies oben im Abschnitt „Junk-E-Mail-Filterung in Outlook 2003 und Outlook Web Access“ beschrieben wurde.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Zusammenfassung

In vielen mittelgroßen Unternehmen bauen zahlreiche entscheidende Prozesse auf der Funktionalität von Microsoft Exchange Server 2003 auf. Ein großer Teil der täglichen Aktivitäten ist abhängig von den Diensten, die Exchange Server bereitstellt.

Die steigende Zahl der Junk-E-Mails ist für mittelgroße Unternehmen eine ständige Herausforderung. Dies ist nicht nur lästig, sondern kann auch die Netzwerkleistung beeinträchtigen und eine Verschwendung von Zeit, Geld und anderen Ressourcen für Privatpersonen und Unternehmen auf der ganzen Welt bedeuten.

Das vorliegende Dokument hat gezeigt, dass es Möglichkeiten gibt, die Menge an Spam in Exchange Server 2003-Umgebungen einzudämmen. Das Antispam-Framework von Exchange Server 2003 vereinigt in sich verschiedene Spamschutzmethoden, die Administratoren und Endbenutzern genügend Flexibilität bieten, um die Zahl der unerwünschten E-Mails zu reduzieren und damit die Produktivität zu steigern.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Referenzen

Das Dokument [Übersicht über das Antispam-Framework von Microsoft Exchange Server 2003](http://download.microsoft.com/download/0/e/6/0e6a7113-dda4-4fd7-aaba-b9e264700225/anti-spam.doc) (möglicherweise in englischer Sprache) kann im Microsoft Download Center unter http://download.microsoft.com/download/0/E/6/0E6A7113-DDA4-4FD7-AABA-B9E264700225/Anti-Spam.doc heruntergeladen werden.

Das Thema [Besserer Schutz vor Spam](http://www.microsoft.com/exchange/evaluation/sp2/overview.mspx#antispam) (möglicherweise in englischer Sprache) in der Übersicht über Exchange Server 2003 SP2 ist unter www.microsoft.com/exchange/evaluation/sp2/overview.mspx\#antispam zu finden.

Informationen über den [intelligenten Nachrichtenfilter für Exchange (IMF)](http://www.microsoft.com/technet/prodtechnol/exchange/downloads/2003/imf/default.mspx) (möglicherweise in englischer Sprache) und Updates für den IMF finden Sie im Microsoft TechNet unter www.microsoft.com/technet/prodtechnol/exchange/downloads/2003/imf/default.mspx.

Das Whitepaper [Messaging-Hygiene bei Microsoft: Wie sich Microsoft IT gegen Spam, Viren und E-Mail-Angriffe verteidigt](http://www.microsoft.com/technet/itsolutions/msit/security/messaginghygienewp.mspx) ist im Microsoft TechNet unter www.microsoft.com/technet/itsolutions/msit/security/messaginghygienewp.mspx abrufbar.

Der Artikel [Echtzeit-Sperrlisten für Exchange Server 2003](http://www.microsoft.com/technet/prodtechnol/exchange/2003/insider/block_lists.mspx) (möglicherweise in englischer Sprache) ist im Microsoft TechNet unter www.microsoft.com/technet/prodtechnol/exchange/2003/insider/Block\_Lists.mspx abrufbar.

Den Microsoft Knowledge Base-Artikel [Konfigurieren der Verbindungsfilterung zur Verwendung von Echtzeit-Sperrlisten und Konfigurieren der Empfängerfilterung in Exchange 2003](http://support.microsoft.com/default.aspx?scid=823866) (möglicherweise in englischer Sprache) finden Sie unter http://support.microsoft.com/default.aspx?scid=823866.

**Download**

[Dokument „Ansätze zur Bekämpfung von Spam in einer Exchange Server-Umgebung“ herunterladen](http://go.microsoft.com/fwlink/?linkid=71052)

[](#mainsection)[Zum Seitenanfang](#mainsection)