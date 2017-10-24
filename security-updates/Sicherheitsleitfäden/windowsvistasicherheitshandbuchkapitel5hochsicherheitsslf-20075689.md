---
Title: Windows Vista-Sicherheitshandbuch – Kapitel 5 (Hochsicherheit, SSLF)
TOCTitle: Windows Vista-Sicherheitshandbuch – Kapitel 5 (Hochsicherheit, SSLF)
ms:assetid: fc523caa-74da-4fd6-8a39-084c1217a4f0
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443746(v=TechNet.10)
ms:contentKeyID: 20075689
---


# Windows Vista-Sicherheitshandbuch



### Kapitel 5: Hochsicherheit (SSLF)
Veröffentlicht: 08. Nov 2006
 

Die SSLF-Sicherheitsbasis (Specialized Security – Limited Functionality) in diesem Handbuch erfüllt die Nachfrage nach Hochsicherheitsumgebungen für Computer, auf denen Windows Vista™ ausgeführt wird. Sicherheit spielt in diesen Umgebungen eine so wichtige Rolle, dass ein beträchtlicher Verlust an Funktionalität und Verwaltbarkeit akzeptabel ist. Die Unternehmensclient-Sicherheitsbasis (EC) trägt zur Bereitstellung einer größeren Sicherheit bei, die in den meisten Unternehmen für ausreichende Funktionalität des Betriebssystems und der Anwendungen sorgt.

**Achtung:**

Die SSLF-Sicherheitseinstellungen sind nicht für die Mehrzahl der Unternehmen vorgesehen. Die Konfiguration für diese Einstellungen wurde für Organisationen entwickelt, in denen Sicherheit wichtiger ist als Funktionalität.

Wenn Sie sich dafür entscheiden, die SSLF-Konfigurationseinstellungen auf den Clientcomputern in Ihrer Arbeitsumgebung zu testen und bereitzustellen, verzeichnen die IT-Mitarbeiter in Ihrem Unternehmen unter Umständen eine höhere Anzahl von Anrufen beim Helpdesk, die sich aus der eingeschränkten Funktionalität als Folge dieser Einstellungen ergeben. Die Konfiguration für diese Arbeitsumgebung bietet zwar eine höhere Sicherheit für Daten und Netzwerk, unterbindet andererseits jedoch die Ausführung einiger Dienste, auf die Ihre Organisation möglicherweise angewiesen ist. Als Beispiele seien hier Terminaldienste genannt, über die mehrere Benutzer eine interaktive Verbindung zu Desktops und Anwendungen auf Remotecomputern herstellen können, sowie der Faxdienst, der Benutzer in die Lage versetzt, Faxnachrichten vom Computer aus über das Netzwerk zu senden und zu empfangen. Eine vollständige Liste der Dienste, die in der SSLF-Arbeitsumgebung nicht mehr ausgeführt werden, finden Sie im Abschnitt „Eingeschränkte Dienste“ weiter unten in diesem Kapitel.

Es sollte unbedingt beachtet werden, dass die SSLF-Sicherheitsbasis keine Ergänzung zur EC-Sicherheitsbasis darstellt, sondern eine völlig andere Sicherheitsstufe bereitstellt. Versuchen Sie daher nicht, die SSLF-Sicherheitsbasis und die EC-Sicherheitsbasis auf demselben Computer mit Windows Vista anzuwenden. Für die Zwecke dieses Handbuchs ermitteln Sie in jedem Fall zunächst die notwendige Sicherheitsstufe für Ihre Arbeitsumgebung, und entscheiden Sie dann erst, ob die EC-Sicherheitsbasis oder die SSLF-Sicherheitsbasis implementiert werden soll. Einen Vergleich der Unterschiede bei den Einstellungen für die EC-Sicherheitsbasis und die SSLF-Sicherheitsbasis finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.

**Wichtig**: Falls Sie die Verwendung der SSLF-Sicherheitsbasis in Ihrer Umgebung in Betracht ziehen, stellen Sie sich darauf ein, die Computer in Ihrer Umgebung im Anschluss an die Zuweisung der SSLF-Sicherheitseinstellungen gründlichst zu testen. Damit stellen Sie sicher, dass die Sicherheitseinstellungen keine erforderliche Funktionalität für die Computer in der Umgebung abblocken.

Auf dieser Seite

[Besondere Sicherheitsumgebung](#edaa)  
[Arbeitsumgebung mit eingeschränkter Funktionalität](#ecaa)  
[Das GPOAccelerator-Tool](#ebaa)  
[Weitere Informationen](#eaaa)  



### Besondere Sicherheitsumgebung

Unternehmen, in denen Computer und Netzwerke zum Einsatz kommen, sollten Sicherheitsproblemen im System- und Netzwerkentwurf sowie der Konfiguration und Bereitstellung der Computer hohe Priorität zukommen lassen. Dies gilt insbesondere dann, wenn das Unternehmen auch auf externe Ressourcen wie das Internet zugreift. Fähigkeiten wie Prozessautomatisierung, Remoteverwaltung, Remotezugriff, Verfügbarkeit rund um die Uhr, weltweite Zugriffsmöglichkeiten und Geräteunabhängigkeit der Software versetzen ein Unternehmen in die Lage, am modernen Markt rationeller und produktiver vorzugehen. Jedoch werden die Computer dieser Unternehmen dadurch auch potenziellen Bedrohungen ausgesetzt.

Im Allgemeinen ergreifen Administratoren angemessene Vorsichtsmaßnahmen, mit denen der unbefugte Zugriff auf Daten, die Beeinträchtigung des laufenden Betriebs und der Missbrauch von Computern unterbunden werden soll. Bestimmte Organisationen (z. B. Stellen im Militär, Behörden in Staat und Gemeinden, Finanzunternehmen) müssen einige oder alle verwendeten Dienste, Systeme und Daten mit einer besonderen Sicherheitsstufe schützen. Die SSLF-Sicherheitsbasis bietet diesen Organisationen die gesuchte Sicherheitsstufe. Eine Übersicht der SSLF-Einstellungen finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.
[Zum Seitenanfanq](#mainsection)  



### Arbeitsumgebung mit eingeschränkter Funktionalität

Die besondere Sicherheit der SSLF-Sicherheitsbasis kann die Funktionalität in Ihrer Arbeitsumgebung einschränken. Die Benutzer können hier nur noch auf die Funktionen zugreifen, die sie für ihre jeweiligen Tätigkeiten unbedingt brauchen. Der Zugriff ist auf genehmigte Anwendungen, Dienste und Infrastrukturumgebungen beschränkt. Es steht weniger Konfigurationsfunktionalität zur Verfügung, da mit dieser Sicherheitsbasis zahlreiche Eigenschaftsseiten deaktiviert werden, die die Benutzer unter Umständen regelmäßig genutzt haben.

In den nachstehenden Abschnitten dieses Kapitels werden die Bereiche der höheren Sicherheit und der eingeschränkten Funktionalität erläutert, die die SSLF-Sicherheitsbasis mit sich bringt:
* Beschränkte Dienste und beschränkter Datenzugriff

* Eingeschränkter Netzwerkzugang

* Starker Netzwerkschutz

* Begrenzte Dienste



#### Beschränkte Dienste und beschränkter Datenzugriff

Bestimmte Einstellungen in der SSLF-Sicherheitsbasis sorgen dafür, dass auch befugte Benutzer nicht auf Dienste oder Daten zugreifen können, wenn sie ihr Kennwort vergessen oder falsch eingegeben haben. Diese Einstellungen können außerdem zu einem Anstieg der Anrufe beim Helpdesk führen. Die Sicherheitsvorteile dieser Einstellungen machen es jedoch für böswillige Benutzern wesentlich schwerer, Computer mit Windows Vista in dieser Arbeitsumgebung anzugreifen. Bestimmte Einstellungen in der SSLF-Sicherheitsbasis bewirken unter Umständen, dass die Benutzer keinen Zugriff mehr auf Dienste und Daten erhalten:
* Einstellungen zum Deaktivieren von Administratorkonten

* Einstellungen zum Durchsetzen strengerer Kennwortanforderungen

* Einstellungen zum Durchsetzen strengerer Kontensperrrichtlinien

* Einstellungen zum Durchsetzen einer strengeren Richtlinie für die folgenden Einstellungen unter **Zuweisen von Benutzerrechten**:  
**Als Dienst anmelden** und **Stapelverarbeitungsauftrag**

 

**Hinweis**:   Einzelheiten zu den Einstellungen der EC- und der SSLF-Sicherheitsbasis finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.


#### Eingeschränkter Netzwerkzugang

Die Zuverlässigkeit des Netzwerks und die Systemkonnektivität ist für den Erfolg eines Unternehmens von größter Bedeutung. Die Betriebssysteme von Microsoft bieten neue Netzwerkfunktionen, mit denen Sie eine Verbindung zu Systemen herstellen, die Konnektivität beibehalten und unterbrochene Verbindungen wiederherstellen können. Obwohl diese Funktionalität nützlich ist, um die Netzwerkkonnektivität aufrechtzuerhalten, kann sie jedoch von Angreifern ausgenutzt werden, um Störungen oder gar Sicherheitsverletzungen auf den Computern im Netzwerk zu verursachen.

In der Regel begrüßen Administratoren alle Funktionen, die die Netzwerkkommunikation unterstützen. In bestimmten Fällen sind jedoch Bedenken hinsichtlich der Sicherheit von Daten und Diensten vorrangig. In diesen besonderen Arbeitsumgebungen wird ein gewisser Verlust der Konnektivität in Kauf genommen, um so die Sicherheit der Daten sicherzustellen. Bestimmte Einstellungen in der SSLF-Sicherheitsbasis erhöhen die Netzwerksicherheit, bewirken jedoch unter Umständen, dass die Benutzer keinen Zugriff mehr auf das Netzwerk erhalten:
* Einstellungen zum Einschränken des Zugriffs auf Clientsysteme im gesamten Netzwerk

* Einstellungen zum Ausblenden von Systemen in durchsuchbaren Listen

* Einstellungen zum Steuern der Ausnahmen für die Windows-Firewall

* Einstellungen zum Umsetzen der Verbindungssicherheit (z. B. Paketsignierung)



#### Starker Netzwerkschutz

Angriffe auf Netzwerkdienste erfolgen oft in Form von DoS-Angriffen (Denial-of-Service). Bei einem solchen Angriff wird die Konnektivität zu Daten oder Diensten unterbunden, oder die Systemressourcen werden überfordert, und die Leistung sinkt. Die SSLF-Sicherheitsbasis schützt den Zugriff auf Systemobjekte und sorgt für die Zuweisung von Ressourcen, mit denen der Schutz vor diesem Angriffstyp verstärkt werden soll. Bestimmte Einstellungen in der SSLF-Sicherheitsbasis verstärken den Schutz vor DoS-Angriffen:
* Einstellungen zum Steuern der zugewiesenen Prozessspeicherkontingente

* Einstellungen zum Steuern der Objekterstellung

* Einstellungen zum Steuern der Möglichkeit, Programme zu debuggen

* Einstellungen zum Steuern der Prozessprofilerstellung

 

Alle diese Überlegungen zur Sicherheit erhöhen die Wahrscheinlichkeit, dass bestimmte Anwendungen in Ihrer Arbeitsumgebung aufgrund der Sicherheitseinstellungen in der SSLF-Sicherheitsbasis nicht ausgeführt werden oder dass die Benutzer nicht wie gewohnt auf Dienste und Daten zugreifen können. Aus diesem Grund ist es unbedingt erforderlich, die SSLF-Sicherheitsbasis nach der Implementierung und *vor* der Bereitstellung in einer Produktionsumgebung intensiv zu testen.


#### Begrenzte Dienste

Durch die SSLF-Sicherheitsbasis werden eine Reihe von Anwendungen und Dienstprogrammen nicht mehr automatisch ausgeführt. Außerdem werden die Bereiche „Run“ und „Run Once“ in der Registrierung nicht verarbeitet, und die automatische Wiedergabe von CDs wird deaktiviert.

Die SSLF-Sicherheitsbasis deaktiviert speziell die folgenden Dienste:
* **Computerbrowser** (**Browser**). Dieser Dienst führt eine aktuelle Liste der Computer im Netzwerk und übergibt diese Liste an Computer, die als Browser gekennzeichnet sind. Ist dieser Dienst deaktiviert, wird die Liste weder aktualisiert noch weiter gepflegt. Alle Dienste, die explizit von diesem Dienst abhängen, werden nicht gestartet.

* **Faxdienst** (**Fax**). Mit diesem Dienst können die Benutzer Faxnachrichten über die Faxressourcen auf dem Computer oder im Netzwerk senden und empfangen.

* **FTP-Publishingdienst** (**MSFtpsvc**). Dieser Dienst bietet FTP-Konnektivität und ermöglicht die Verwaltung über das IIS-Snap-In (Internetinformationsdienste).

* **Indexdienst** (**CiSvc**). Dieser Dienst erstellt einen Index für den Dateiinhalt und die Eigenschaften auf lokalen Computern und Remotecomputern. Über eine flexible Abfragesprache ermöglicht dieser Dienst außerdem den raschen Zugriff auf Dateien.

* **IIS-Verwaltungsdienst** (**IISADMIN**). Dieser Dienst ermöglicht die Administration von Web- und FTP-Diensten über das IIS-Snap-In.

* **Sitzungs-Managerdienst für Remotedesktophilfe** (**RDSessMgr**). Dieser Dienst verwaltet und steuert die Remoteunterstützung. Ist dieser Dienst deaktiviert, steht die Remoteunterstützung nicht zur Verfügung.

* **Routing- und RAS-Dienst** (**RemoteAccess**). Dieser Dienst bietet Routingdienste für Unternehmen in LAN- und WAN-Umgebungen (Local Area Network bzw. Wide Area Network).

* **SNMP-Trap-Dienst** (**SNMPTRAP**). Dieser Dienst empfängt Trap-Nachrichten, die von lokalen SNMP-Agenten oder Remote-SNMP-Agenten erstellt wurden, und leitet diese Nachrichten an SNMP-Verwaltungsprogramme auf Clientcomputern weiter.

* **SNMP-Dienst** (**SNMP**). Dieser Dienst enthält Agenten, die die Aktivität der Netzwerkgeräte überwachen und Berichte an die Netzwerkverwaltungskonsole senden.

* **SSDP-Suchdienst** (**SSDPSRV**). Dieser Dienst ermöglicht die Erkennung von UPnP-Geräten in Heimnetzwerken.

* **Taskplanerdienst** (**Schedule**). Mit diesem Dienst können die Benutzer automatisierte Tasks auf dem Computer konfigurieren und planen. Ist dieser Dienst deaktiviert, werden die geplanten Tasks nicht ausgeführt. Alle Dienste, die explizit von diesem Dienst abhängen, werden nicht gestartet.

* **Telnet-Dienst** (**TlntSvr**). Über diesen Dienst kann sich ein Remotebenutzer bei einem anderen Computer anmelden und dort Programme ausführen. Der Dienst unterstützt verschiedene TCP/IP-Telnet-Clients, unter anderem für UNIX- und Windows-basierte Computer. Ist dieser Dienst deaktiviert, ist unter Umständen kein Remotebenutzerzugriff auf Programme möglich. Alle Dienste, die explizit von diesem Dienst abhängen, werden nicht gestartet.

* **Terminaldienste** (**TermService**). Mit diesem Dienst können mehrere Benutzer eine interaktive Verbindung zu Desktops und Anwendungen auf Remotecomputern herstellen. Der Dienst liefert die Hintergrundsoftware für Remotedesktop (einschließlich Remotedesktop für Administratoren), schnelle Benutzerumschaltung, Remoteunterstützung und Terminalserver.

* **Universeller Plug &amp; Play-Gerätehostdienst** (**Upnphost**). Dieser Dienst liefert die nötige Unterstützung zum Hosten von universellen Plug &amp; Play-Geräten.

* **WWW-Publishingdienst** (**W3SVC**). Dieser Dienst bietet Webverbindungs- und Verwaltungsfunktionen über das IIS-Snap-In.

 

Die Funktionalität von Windows Vista auf Clientcomputern wird durch die SSLF-Sicherheitsbasis so weit kontrolliert, dass alle nicht explizit benötigten und angeforderten Funktionen deaktiviert werden. Im Vergleich zu früheren Sicherheitsrichtlinien bedeutet dies eine deutliche Änderung im Ansatz: Bislang wurden alle Elemente ermittelt, die speziell von Benutzern benötigt werden, und alle anderen Funktionen wurden deaktiviert. Bei dieser neuen Vorgehensweise werden von vornherein sämtliche Dienste und Dienstprogramme deaktiviert, die Schäden am Betriebssystem verursachen können.


#### Implementieren der Sicherheitsrichtlinien

Die in diesem Leitfaden beschriebene Hochsicherheitslösung beruht auf der Gruppenrichtlinien-Verwaltungskonsole (GPMC) und auf GPMC-basierten Skripts. GPMC ist in das Windows Vista-Betriebssystem integriert, Sie müssen die Konsole daher nicht jedes Mal herunterladen und installieren, wenn Sie Gruppenrichtlinienobjekte auf einem anderen Computer verwalten möchten.

**Wichtig**:   Sie müssen alle Anweisungen in diesem Handbuch auf einem Clientcomputer mit Windows Vista ausführen, der mit dem Active Directory®-Verzeichnisdienst einer Domäne hinzugefügt wurde. Der Benutzer, der die Schritte ausführt, muss außerdem über Domänenadministratorrechte verfügen. Wenn Sie das Betriebssystem Microsoft Windows® XP oder Windows Server® 2003 verwenden, werden die Windows Vista–spezifischen Sicherheitseinstellungen nicht in der GPMC angezeigt.

Zum Implementieren des Sicherheitsentwurfs müssen Sie drei Hauptaufgaben ausführen:
* Erstellen der Hochsicherheitsumgebung

* Verknüpfen der Domänenrichtlinie „VSG SSLF Domain Policy“ mit der Domäne mithilfe der GPMC

* Überprüfen der Ergebnisse mithilfe der Gruppenrichtlinien-Verwaltungskonsole


In diesem Abschnitt des Kapitels werden diese Aufgaben und Verfahren sowie die Funktionsweise des Skripts „GPOAccelerator.wsf“ beschrieben, das automatisch die vorgeschriebenen Gruppenrichtlinienobjekte erstellt.

Das Skript „GPOAccelerator.wsf“

Mit dem Skript **GPOAccelerator.wsf**, das diesem Handbuch beiliegt, werden alle erforderlichen Gruppenrichtlinienobjekte erstellt. Sie müssen nicht mit großem Zeitaufwand manuell Richtlinieneinstellungen bearbeiten oder Vorlagen anwenden. Zum Aufbau der Hochsicherheitsumgebung werden die folgenden vier Gruppenrichtlinienobjekte durch das Skript erstellt:
* **VSG SSLF Domain Policy** für die Domäne.

* **VSG SSLF Users Policy** für Benutzer.

* **VSG SSLF Desktop Policy** für Desktopcomputer.

* **VSG SSLF Laptop Policy** für Laptopcomputer.

 

**Wichtig**:   Um den Sicherheitsentwurf für die Hochsicherheitsumgebung erfolgreich implementieren zu können, müssen Sie den Entwurf unbedingt umfassend testen, bevor Sie ihn in der Produktionsumgebung bereitstellen.

Verwenden Sie das Skript „GPOAccelerator.wsf“ für die folgenden Aufgaben:
* **Testen des Entwurfs in einer Testumgebung** Erstellen Sie in der Testumgebung mit dem Skript „GPOAccelerator.wsf“ eine Organisationseinheitsstruktur, erstellen Sie die Gruppenrichtlinienobjekte, und erstellen Sie dann die automatische Verknüpfung zwischen den Gruppenrichtlinienobjekten und den Organisationseinheiten. Nach Abschluss der Testphase der Implementierung können Sie das Skript in der Produktionsumgebung verwenden.

* **Bereitstellen des Entwurfs in einer Produktionsumgebung.**   Wenn Sie anfangen, die Lösung in der Produktionsumgebung zu implementieren, müssen Sie zunächst eine geeignete Organisationseinheitsstruktur erstellen oder eine vorhandene Gruppe von Organisationseinheiten ändern. Sie können dann mit dem Skript „GPOAccelerator.wsf“ die Gruppenrichtlinienobjekte erstellen und die neuen Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten in der Umgebung verknüpfen.


**Testen des Entwurfs in einer Testumgebung**

Die mit diesem Handbuch bereitgestellten Gruppenrichtlinienobjekte wurden intensiv getestet. Sie müssen jedoch unbedingt eigene Tests in Ihrer Umgebung durchführen. Um Zeit zu sparen, können Sie mit dem Skript „GPOAccelerator.wsf“ die vorgeschriebenen Gruppenrichtlinienobjekte und die Beispiel-Organisationseinheitsstruktur erstellen und die Gruppenrichtlinienobjekte und die Organisationseinheiten dann automatisch verknüpfen.

Aufgabe 1: Erstellen der Hochsicherheitsumgebung

Das Skript „GPOAccelerator.wsf“ befindet sich in folgendem Ordner: Windows Vista Security Guide\GPOAccelerator Tool. Dieser wird von der Microsoft Windows Installer-Datei (MSI-Datei) erstellt.

**Hinweis:** Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

**So erstellen Sie die Gruppenrichtlinienobjekte und verknüpfen sie mit den entsprechenden Organisationseinheiten in der Testumgebung**
1. Melden Sie sich als Domänenadministrator an einem Computer mit Windows Vista an, der mit Active Directory der Domäne hinzugefügt wurde, in der Sie die Gruppenrichtlinienobjekte erstellen.

2. Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3. Öffnen Sie den Ordner **GPOAccelerator Tool\Security Group Policy Objects.**  

4. Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Domänenadministratorrechten zu öffnen.

    **Hinweis:**   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /SSLF /LAB** ein, und drücken Sie dann die EINGABETASTE.

6. Klicken Sie im Meldungsfeld **Click Yes to continue****,****or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

    **Hinweis:**   Dieser Schritt kann einige Minuten in Anspruch nehmen.

7. Klicken Sie im Meldungsfeld **The** **SSLF Lab Environment is created** (Die SSLF-Testumgebung wurde erstellt) auf **OK.**  

8. Klicken Sie im Meldungsfeld **Make sure to link the SSLF Domain GPO to your domain** (Gruppenrichtlinienobjekt für SSLF-Domäne mit der Domäne verknüpfen) auf **OK**, und führen Sie dann die Schritte in der nächsten Aufgabe aus, um die Domänenrichtlinie „VSG SSLF Domain Policy“ zu verknüpfen.

**Hinweis:**   Die Gruppenrichtlinie auf Domänenebene enthält Einstellungen, die auf alle Computer und Benutzer in der Domäne angewendet werden. Sie müssen entscheiden können, wann das Domänen-GPO verknüpft wird, da dieses Gruppenrichtlinienobjekt auf *alle* Benutzer und Computer angewendet wird. Aus diesem Grund wird das Domänen-GPO vom Skript „GPOAccelerator.wsf“ nicht automatisch mit der Domäne verknüpft.


Aufgabe 2: Verknüpfen der Domänenrichtlinie „VSG SSLF Domain Policy“ mit der Domäne mithilfe der GPMC

Sie können nun das Domänen-Gruppenrichtlinienobjekt mit der Domäne verknüpfen. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Domänenrichtlinie „VSG SSLF Domain Policy“ mit der Domäne verknüpfen.

**So verknüpfen Sie die Domänenrichtlinie „VSG SSLF Domain Policy“**
1. Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen.**   (Sie können auch die Windows-Logo-Taste + R drücken.)

2. Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK.**  

3. Klicken Sie in der Domänenstruktur mit der rechten Maustaste auf die Domäne, und klicken Sie dann auf **Vorhandenes Gruppenrichtlinienobjekt verknüpfen.**  

4. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG SSLF Domain Policy**, und klicken Sie dann auf **Ja.**  

5. Wählen Sie im Detailbereich **VSG SSLF Domain Policy** aus, und klicken Sie dann auf die Schaltfläche **Verknüpfung an den Anfang verschieben.**  


**Wichtig:**   Stellen Sie sicher, dass für **VSG SSLF Domain Policy** die Option **Verknüpfungsreihenfolge** auf **1** festgelegt ist. Wenn dies nicht der Fall ist, überschreiben andere mit der Domäne verknüpfte Gruppenrichtlinienobjekte, z. B. das Gruppenrichtlinienobjekt für die Standarddomänenrichtlinie, die Einstellungen des *Windows* *Vista-Sicherheitshandbuchs*.

Aufgabe 3: Überprüfen der Ergebnisse mithilfe der Gruppenrichtlinien-Verwaltungskonsole

Mit der GPMC können Sie die Ergebnisse des Skripts überprüfen. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Gruppenrichtlinienobjekte und die Organisationseinheitsstruktur überprüfen können, die vom Skript „GPOAccelerator.wsf“ erstellt wurden.

**So überprüfen Sie die Ergebnisse des Skripts „GPOAccelerator.wsf“**
1. Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen.**  

2. Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK.**  

3. Klicken Sie auf die entsprechende Struktur, klicken Sie auf **Domänen**, und klicken Sie dann auf die Domäne.

4. Klicken Sie auf **Vista Security Guide SSLF Client OU** (SSLF-Client-Organisationseinheit für Vista Security Guide), erweitern Sie diese Organisationseinheit, und klicken Sie dann auf die fünf Organisationseinheiten darunter, um sie zu öffnen.

5. Stellen Sie sicher, dass die Organisationseinheitsstruktur und die Verknüpfungen der Gruppenrichtlinienobjekte mit der folgenden Abbildung übereinstimmen.

![](images/dd443746.vsgf0501(de-de,technet.10).gif)

**Abbildung 5.1 GPMC-Ansicht der Organisationseinheitsstruktur und Verknüpfungen der Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt wurden**


Alle Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt werden, enthalten sämtliche in diesem Handbuch empfohlene Einstellungen. Sie können nun mit dem Tool „Active Directory-Benutzer und -Computer“ den Entwurf testen, indem Sie Benutzer und Computer in die entsprechenden Organisationseinheiten verschieben. Details zu den Einstellungen der einzelnen Gruppenrichtlinienobjekte finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

Bereitstellen des Entwurfs in einer Produktionsumgebung

Um Zeit zu sparen, können Sie mit dem Skript „GPOAccelerator.wsf“ die Gruppenrichtlinienobjekte für die Hochsicherheitsumgebung erstellen. Sie können dann die Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten in der vorhandenen Struktur verknüpfen. In größeren Domänen mit einer größeren Anzahl von Organisationseinheiten müssen Sie beachten, wie Sie die vorhandene Organisationseinheitsstruktur zum Bereitstellen der Gruppenrichtlinienobjekte verwenden.

In größeren Domänen mit einer größeren Anzahl von Organisationseinheiten müssen Sie beachten, wie Sie die vorhandene Organisationseinheitsstruktur zum Bereitstellen der Gruppenrichtlinienobjekte verwenden. Wenn möglich, sollten Sie Computer-Organisationseinheiten von Benutzer-Organisationseinheiten trennen. Laptop- und Desktopcomputer sollten ebenfalls jeweils in eigenen Organisationseinheiten organisiert werden. Wenn das Erstellen einer solchen Struktur in Ihrer Umgebung nicht möglich ist, müssen Sie möglicherweise die Gruppenrichtlinienobjekte ändern. In Anhang A finden Sie Informationen zu den Einstellungen, die Ihnen dabei helfen können, die erforderlichen Änderungen zu ermitteln.

**Hinweis:**   Wie im vorhergehenden Abschnitt beschrieben, können Sie das Skript „GPOAccelerator.wsf“  
mit der Option **/LAB** ausführen, um in einer Testumgebung die Beispiel-Organisationseinheitsstruktur zu erstellen. Bei Umgebungen mit einer flexiblen Organisationseinheitsstruktur kann diese Option jedoch auch in einer Produktionsumgebung zum Erstellen einer einfachen Organisationseinheitsstruktur und zum automatischen Verknüpfen der Gruppenrichtlinienobjekte verwendet werden. Sie können die Organisationseinheitsstruktur dann manuell an die Anforderungen in Ihrer Umgebung anpassen.

Aufgabe 1: Erstellen der Gruppenrichtlinienobjekte

Sie erstellen die in diesem Handbuch beschriebenen SSLF-Gruppenrichtlinienobjekte mit dem Skript „GPOAccelerator.wsf“. Das Skript „GPOAccelerator.wsf“ befindet sich in folgendem Ordner: Windows Vista Security Guide\GPOAccelerator Tool. Dieser wird von der Microsoft Windows Installer-Datei (MSI-Datei) erstellt.

**Hinweis:**   Sie können das Verzeichnis „GPOAccelerator Tool“ einfach von einem Computer, auf dem das Verzeichnis installiert ist, auf einen anderen Computer kopieren, auf dem Sie das Skript verwenden möchten. Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

**So erstellen Sie die Gruppenrichtlinienobjekte in einer Produktionsumgebung**
1. Melden Sie sich als Domänenadministrator an einem Computer mit Windows Vista an, der mit Active Directory der Domäne hinzugefügt wurde, in der Sie die Gruppenrichtlinienobjekte erstellen.

2. Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3. Öffnen Sie den Ordner **GPOAccelerator Tool\Security Group Policy Objects.**  

4. Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Domänenadministratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5. Öffnen Sie den Ordner **GPOAccelerator Tool\Security Group Policy Objects.**  

6. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /SSLF** ein, und drücken Sie dann die EINGABETASTE.

7. Klicken Sie im Meldungsfeld **Click Yes to continue****,****or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

    **Hinweis**   Dieser Schritt kann einige Minuten in Anspruch nehmen.

8. Klicken Sie im Meldungsfeld **The SSLF GPOs are created** (Die SSLF-Gruppenrichtlinienobjekte wurden erstellt) auf **OK.**  

9. Klicken Sie im Meldungsfeld **Make sure to link the SSLF GPOs to the appropriate OUs** (SSLF-Gruppenrichtlinienobjekte mit den richtigen Organisationseinheiten verknüpfen) auf **OK.**  


Aufgabe 2: Überprüfen der Ergebnisse mithilfe der Gruppenrichtlinien-Verwaltungskonsole

Mithilfe der GPMC können Sie sicherstellen, dass das Skript alle Gruppenrichtlinienobjekte erfolgreich erstellt hat. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Gruppenrichtlinienobjekte überprüfen können, die vom Skript „GPOAccelerator.wsf“ erstellt wurden.

**So überprüfen Sie die Ergebnisse des Skripts „GPOAccelerator.wsf“**
1. Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen.**  

2. Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK.**  

3. Klicken Sie auf die entsprechende Struktur, klicken Sie auf **Domänen**, und klicken Sie dann auf die Domäne.

4. Klicken Sie auf **Gruppenrichtlinienobjekte**, erweitern Sie den Eintrag, und stellen Sie sicher, dass alle vier VSG SSLF-Gruppenrichtlinienobjekte wie in der folgenden Abbildung dargestellt erstellt wurden.

![](images/dd443746.vsgf0502(de-de,technet.10).gif)

**Abbildung 5.2 GPMC-Ansicht der SSLF-Objekte für Unternehmensclients, die vom Skript „GPOAccelerator.wsf“ erstellt wurden**


Sie können nun mit der GPMC die einzelnen Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten verknüpfen. In der letzten Aufgabe dieses Verfahrens wird dies erläutert.

Aufgabe 3: Verknüpfen der Gruppenrichtlinienobjekte mit den Organisationseinheiten mithilfe der GPMC

Im Folgenden wird beschrieben, wie Sie diese Aufgabe mithilfe der GPMC auf einem Clientcomputer mit Windows Vista ausführen.

**So verknüpfen Sie die Gruppenrichtlinienobjekte in einer Produktionsumgebung**
1. Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen.**  

2. Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK.**  

3. Klicken Sie in der Domänenstruktur mit der rechten Maustaste auf die Domäne, und klicken Sie dann auf **Vorhandenes Gruppenrichtlinienobjekt verknüpfen.**  

4. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG SSLF Domain Policy**, und klicken Sie dann auf **OK.**  

5. Wählen Sie im Detailbereich **VSG SSLF Domain Policy** aus, und klicken Sie dann auf die Schaltfläche **Verknüpfung an den Anfang verschieben.**  

    **Wichtig:**   Stellen Sie sicher, dass für **VSG SSLF Domain Policy** die Option **Verknüpfungsreihenfolge** auf **1** festgelegt ist. Wenn dies nicht der Fall ist, überschreiben andere mit der Domäne verknüpfte Gruppenrichtlinienobjekte, z. B. das Gruppenrichtlinienobjekt für die Standarddomänenrichtlinie, die Einstellungen des *Windows* *Vista-Sicherheitshandbuchs*.

6. Klicken Sie mit der rechten Maustaste auf den Knoten **Windows Vista Users OU**, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen.**  

7. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG SSLF Users Policy**, und klicken Sie dann auf **OK.**  

8. Klicken Sie mit der rechten Maustaste auf den Knoten **Desktop OU**, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen.**  

9. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG SSLF Desktop Policy**, und klicken Sie dann auf **OK.**  

10. Klicken Sie mit der rechten Maustaste auf den Knoten **Laptop OU**, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen.**  

11. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG SSLF Laptop Policy**, und klicken Sie dann auf **OK.**  

12. Wiederholen Sie diese Schritte für alle weiteren erstellten Benutzer- oder Computer-Organisationseinheiten, um die weiteren Organisationseinheiten mit den entsprechenden Gruppenrichtlinienobjekten zu verknüpfen.


**Hinweis:**   Sie können ein Gruppenrichtlinienobjekt, das sich unter dem Knoten „Gruppenrichtlinienobjekte“ befindet, in eine Organisationseinheit ziehen. Drag &amp; Drop-Vorgänge sind jedoch nur innerhalb einer Domäne möglich.

**So bestätigen Sie die Gruppenrichtlinienobjekt-Verknüpfungen mithilfe der GPMC**
* Erweitern Sie den Knoten **Gruppenrichtlinienobjekte**, wählen Sie das Gruppenrichtlinienobjekt aus, klicken Sie im Detailbereich auf die Registerkarte **Bereich**, und notieren Sie dann die Informationen in den Spalten **Verknüpfung aktiviert** und **Pfad.**  


– Oder –
* Wählen Sie die Organisationseinheit aus, klicken Sie dann im Detailbereich auf die Registerkarte **Verknüpfte Gruppenrichtlinienobjekte**, und notieren Sie die Informationen in den Spalten **Verknüpfung aktiviert** und **Gruppenrichtlinienobjekt.**  

 

**Hinweis:**   Sie können mit der GPMC die Verknüpfungen der Gruppenrichtlinienobjekte auch aufheben oder ggf. löschen. Löschen Sie anschließend entweder mithilfe der GPMC oder dem MMC-Snap-In „Active Directory-Benutzer und -Computer“ alle nicht mehr benötigten Organisationseinheiten. Wenn Sie alle Active Directory-Änderungen rückgängig machen möchten, die vom Skript „GPOAccelerator.wsf“ vorgenommen wurden, müssen Sie manuell die Dateien „SSLF-VSGAuditPolicy.cmd“, „SSLF-ApplyAuditPolicy.cmd“ und „SSLF-AuditPolicy.txt“ aus der Freigabe NETLOGON auf einem der Domänencontroller löschen. Weitere Informationen zu diesen Dateien finden Sie im Abschnitt über die Überwachungsrichtlinien in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

Alle Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt werden, enthalten sämtliche in diesem Handbuch empfohlene Einstellungen. Sie können nun mit dem Tool „Active Directory-Benutzer und -Computer“ den Entwurf testen, indem Sie Benutzer und Computer in die entsprechenden Organisationseinheiten verschieben. Details zu den Einstellungen der einzelnen Gruppenrichtlinienobjekte finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

**Migrieren von Gruppenrichtlinienobjekten in eine andere Domäne (Optional)**

Wenn Sie in dieser Lösung die Gruppenrichtlinienobjekte geändert oder eigene Gruppenrichtlinienobjekte erstellt haben und diese in mehreren Domänen verwenden möchten, müssen Sie die Gruppenrichtlinienobjekte migrieren. Für das Migrieren eines in einer Domäne funktionierenden Gruppenrichtlinienobjekts in eine andere Domäne ist etwas Planung erforderlich, das grundlegende Verfahren ist jedoch relativ einfach. Bei der Planung sind im Hinblick auf Daten bei Gruppenrichtlinienobjekten zwei wichtige Aspekte zu beachten:
* **Komplexe Daten.**   Die Daten, aus denen ein Gruppenrichtlinienobjekt besteht, sind komplex und werden an mehreren Speicherorten gespeichert. Durch die Verwendung der GPMC zum Migrieren eines Gruppenrichtlinienobjekts wird sichergestellt, dass alle relevanten Daten richtig migriert werden.

* **Domänenspezifische Daten.**   Einige Daten in einem Gruppenrichtlinienobjekt können domänenspezifisch sein und sind daher möglicherweise ungültig, wenn Sie sie direkt in eine andere Domäne kopieren. Zum Beheben dieses Problems werden in der GPMC Migrationstabellen verwendet, mit denen Sie domänenspezifische Daten in einem Gruppenrichtlinienobjekt bei der Migration auf neue Werte aktualisieren können. Dies ist nur erforderlich, wenn das Gruppenrichtlinienobjekt Sicherheits-IDs (SIDs) oder UNC-Pfade (Universal Naming Convention) enthält, die für eine Domäne spezifisch sind.

 

Weitere Informationen zum Migrieren von Gruppenrichtlinienobjekten finden Sie in der Hilfe zur Gruppenrichtlinien-Verwaltungskonsole. Im Whitepaper [Migrating GPOs Across Domains with GPMC](http://www.microsoft.com/windowsserver2003/gpmc/migrgpo.mspx) finden Sie ebenfalls weitere Informationen zu diesem Thema (engl.).
[Zum Seitenanfanq](#mainsection)  



### Das GPOAccelerator-Tool

Die Tools und Vorlagen zu diesem Handbuch umfassen Skripts und Sicherheitsvorlagen. Dieser Abschnitt enthält Hintergrundinformationen zu diesen Ressourcen. Das wichtigste Tool, mit dem das Hauptskript für diesen Sicherheitsleitfaden ausgeführt wird, ist „GPOAccelerator.wsf“. Die Datei befindet sich im Ordner „Windows Vista Security Guide\GPOAccelerator Tool\Security Group Policy Objects“. Außerdem enthält dieser Abschnitt Informationen darüber, wie Sie die GPMC zur Anzeige der Einstellungen für Gruppenrichtlinienobjekte einrichten, sowie über die Unterverzeichnisstruktur und die Dateitypen, die zu diesem Handbuch gehören. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.


#### Erweiterungen für Gruppenrichtlinien-Verwaltungskonsole und Sicherheitskonfigurations-Editor

In der in diesem Handbuch vorgestellten Lösung werden Einstellungen für Gruppenrichtlinienobjekte verwendet, die nicht in der Standardbenutzeroberfläche für die Gruppenrichtlinien-Verwaltungskonsole in Windows Vista oder im Sicherheitskonfigurations-Editor (Security Configuration Editor, SCE) angezeigt werden. Diese Einstellungen, die alle das Präfix **MSS:** aufweisen, wurden von der „Microsoft Solutions for Security“-Gruppe für frühere Sicherheitsanleitungen entwickelt.

**Wichtig**:   Die SCE-Erweiterungen und das Skript GPOAccelerator.wsf sind für die Ausführung auf einem Windows Vista-basierten Computer konzipiert. Diese Tools funktionieren nicht ordnungsgemäß, wenn Sie versuchen, sie auf einem Computer mit Windows XP oder Windows Server 2003 auszuführen.

Daher müssen Sie diese Tools erweitern, so dass Sie die Sicherheitseinstellungen anzeigen und ggf. ändern können. Hierzu aktualisiert das Skript „GPOAccelerator.wsf“ beim Erstellen der Gruppenrichtlinienobjekte automatisch den Computer. Wenn Sie die Gruppenrichtlinienobjekte des *Windows* *Vista-Sicherheitshandbuchs* von einem anderen Computer mit Windows Vista aus verwalten möchten, aktualisieren Sie den Sicherheitskonfigurations-Editor auf diesem Computer wie folgt.

**So ändern Sie den Sicherheitskonfigurations-Editor zum Anzeigen von MSS-Einstellungen**
1. Stellen Sie sicher, dass die folgenden Voraussetzungen erfüllt sind:
    * Der von Ihnen verwendete Computer wurde mit Active Directory der Domäne hinzugefügt, in der die Gruppenrichtlinienobjekte erstellt wurden.

    * Das *Windows* *Vista-Sicherheitshandbuch*-Verzeichnis **GPOAccelerator** **Tool** wurde installiert.


    **Hinweis:**   Sie können das Verzeichnis „GPOAccelerator Tool“ einfach von einem Computer, auf dem das Verzeichnis installiert ist, auf einen anderen Computer kopieren, auf dem Sie das Skript verwenden möchten. Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

2. Melden Sie sich am Computer als Administrator an.

3. Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

4. Öffnen Sie den Ordner GPOAccelerator Tool\Security Group Policy Objects.

5. Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis:**   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

6. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /ConfigSCE** ein, und drücken Sie dann die EINGABETASTE.

7. Klicken Sie im Meldungsfeld **Click Yes to continue****,****or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

8. Klicken Sie im Meldungsfeld **The Security Configuration Editor is updated** (Der Sicherheitskonfigurations-Editor wurde aktualisiert) auf **OK.**  

 

**Wichtig**:   Dieses Skript ändert den Sicherheitskonfigurations-Editor nur insofern, dass MSS-Einstellungen angezeigt werden. Es werden keine Gruppenrichtlinienobjekte oder Organisationseinheiten erstellt.

Mit dem folgenden Verfahren werden die zusätzlichen MSS-Sicherheitseinstellungen entfernt, und das SCE-Tool wird auf die Standardeinstellungen in Windows Vista zurückgesetzt.

**So setzen Sie das SCE-Tool auf die Standardeinstellungen in Windows Vista zurück**
1. Melden Sie sich am Computer als Administrator an.

2. Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3. Öffnen Sie den Ordner GPOAccelerator Tool\Security Group Policy Objects.

4. Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /ResetSCE** ein, und drücken Sie dann die EINGABETASTE.

6. Klicken Sie im Meldungsfeld **Click Yes to continue****,****or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

**Hinweis:**   Bei Durchführen dieser Schritte wird der Sicherheitskonfigurations-Editor auf dem Computer auf die Standardeinstellungen in Windows Vista zurückgesetzt. Alle zum Sicherheitskonfigurations-Editor hinzugefügten Einstellungen werden entfernt. Dies hat nur Auswirkungen auf die Fähigkeit zur Anzeige der Einstellungen im Sicherheitskonfigurations-Editor. Konfigurierte Einstellungen für Gruppenrichtlinienobjekte bleiben unverändert.

7. Klicken Sie im Meldungsfeld **The Security Configuration Editor is updated** (Der Sicherheitskonfigurations-Editor wurde aktualisiert) auf **OK.**  



#### Vorherige Sicherheitseinstellungen

Es werden Sicherheitsvorlagen bereitgestellt, damit Sie, falls Sie eigene Richtlinien erstellen möchten, nicht die mit diesem Handbuch gelieferten Richtlinien verwenden oder ändern müssen, sondern die relevanten Sicherheitseinstellungen importieren können. Sicherheitsvorlagen sind Textdateien, die Werte für Sicherheitseinstellungen enthalten. Sie sind Unterkomponenten von Gruppenrichtlinienobjekten. Sie können die Richtlinieneinstellungen in den Sicherheitsvorlagen im MMC-Snap-In „Gruppenrichtlinienobjekt-Editor“ ändern. Im Gegensatz zu älteren Versionen des Windows-Betriebssystems umfasst Windows Vista keine vordefinierten Sicherheitsvorlagen. Sie können die vorhandenen Sicherheitsvorlagen bei Bedarf jedoch weiter verwenden.

Sicherheitsvorlagen sind in der Windows Installer-Datei (MSI-Datei) enthalten, die mit diesem Handbuch geliefert wird. Die folgenden Vorlagen für die Unternehmensclient-Umgebung befinden sich im Ordner „GPOAccelerator Tool\Security Templates“:
* VSG SSLF Desktop.inf

* VSG SSLF Domain.inf

* VSG SSLF Laptop.inf

 

**Wichtig:**   Sie benötigen die Sicherheitsvorlagen nicht zum Bereitstellen der in diesem Handbuch beschriebenen Lösung. Die Vorlagen stellen eine Alternative zur GPMC-basierten Lösung dar und betreffen lediglich Computersicherheitseinstellungen unter **Computerkonfiguration\Windows-Einstellungen\Sicherheitseinstellungen.**   Sie können beispielsweise keine Einstellungen für Internet Explorer oder Windows Firewall in den Gruppenrichtlinienobjekten mit einer Sicherheitsvorlage verwalten. Außerdem sind keine Benutzereinstellungen eingeschlossen.

**Verwenden von Sicherheitsvorlagen**

Wenn Sie die Sicherheitsvorlagen verwenden möchten, müssen Sie zunächst den Sicherheitskonfigurations-Editor erweitern, damit benutzerdefinierte MSS-Sicherheitseinstellungen in der Benutzeroberfläche angezeigt werden. Das Verfahren wird weiter oben in diesem Kapitel unter „Erweiterungen für Gruppenrichtlinien-Verwaltungskonsole und Sicherheitskonfigurations-Editor“ ausführlich beschrieben. Wenn Sie die Vorlagen anzeigen können, können Sie sie anhand des folgenden Verfahrens in die Gruppenrichtlinienobjekte importieren, die Sie für Ihren Bedarf erstellt haben.

**So importieren Sie eine Sicherheitsvorlage in ein Gruppenrichtlinienobjekt**
1. Öffnen Sie im Gruppenrichtlinienobjekt-Editor das zu ändernde Gruppenrichtlinienobjekt. In der GPMC klicken Sie hierzu mit der rechten Maustaste auf das Gruppenrichtlinienobjekt und anschließend auf **Bearbeiten.**  

2. Navigieren Sie im Gruppenrichtlinienobjekt-Editor zum Ordner **Windows-Einstellungen.**  

3. Erweitern Sie den Ordner **Windows-Einstellungen**, und wählen Sie dann **Sicherheitseinstellungen** aus.

4. Klicken Sie mit der rechten Maustaste auf den Ordner **Sicherheitseinstellungen**, und klicken Sie anschließend auf **Richtlinie importieren.**  

5. Navigieren Sie zum Ordner **Security Templates** im Ordner **Windows Vista Security Guide.**  

6. Wählen Sie die Sicherheitsvorlage aus, die Sie importieren möchten, und klicken Sie dann auf **Öffnen.**  

   Durch den letzten Schritt dieses Verfahrens werden die Einstellungen aus der Datei in das Gruppenrichtlinienobjekt importiert.


Mit den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen können Sie auch die lokale Sicherheitsrichtlinie auf eigenständigen Clientcomputern mit Windows Vista ändern. Das Skript „GPOAccelerator.wsf“ vereinfacht den Prozess zum Anwenden der Vorlagen.

**So wenden Sie die Sicherheitsvorlagen zum Erstellen einer lokalen Gruppenrichtlinie auf einem eigenständigen Clientcomputer mit Windows Vista an**
1. Melden Sie sich als Administrator auf einem Computer mit Windows Vista an.

2. Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3. Öffnen Sie den Ordner GPOAccelerator Tool\Security Group Policy Objects.

4. Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

**Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /SSLF /Desktop** oder **cscript GPOAccelerator.wsf /SSLF /Laptop** ein, und drücken Sie dann die EINGABETASTE.

Durch dieses Verfahren werden die lokalen Sicherheitsrichtlinieneinstellungen mit den Werten in den Sicherheitsvorlagen für die Unternehmensclient-Umgebung geändert.


**So setzen Sie die lokale Gruppenrichtlinie auf die Standardeinstellungen in Windows Vista zurück**
1. Melden Sie sich als Administrator auf einem Clientcomputer mit Windows Vista an.

2. Klicken Sie auf dem Desktop auf die Windows Vista Schaltfläche „Start“, klicken Sie auf **Alle Programme** und dann auf **Zubehör**, klicken Sie mit der rechten Maustaste auf **Eingabeaufforderung**, und klicken Sie auf **Als Administrator ausführen.**  

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

3. Öffnen Sie den Ordner **GPOAccelerator Tool\Security Group Policy Objects.**  

4. Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /Restore** ein, und drücken Sie dann die EINGABETASTE.

   Durch dieses Verfahren werden die lokalen Sicherheitsrichtlinieneinstellungen auf die Standardwerte in Windows Vista zurückgesetzt.

[Zum Seitenanfanq](#mainsection)  



### Weitere Informationen

Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen zu Windows Vista:
* [Administering Group Policy with Group Policy Management Console Abstract](http://go.microsoft.com/fwlink/?linkid=14320) (engl.)

* [Enterprise Management with the Group Policy Management Console](http://www.microsoft.com/windowsserver2003/gpmc/default.mspx) (engl.)

* [Migrating GPOs Across Domains with GPMC](http://www.microsoft.com/windowsserver2003/gpmc/migrgpo.mspx) (engl.)

* [*Verständnis der Gruppenrichtlinienfunktionen*](http://www.microsoft.com/germany/technet/datenbank/articles/600539.mspx)

* [*Verwendung des Assistenten zum Zuweisen der Objektverwaltung*](http://www.microsoft.com/germany/technet/datenbank/articles/600542.mspx)

* [Summary of New or Expanded Group Policy Settings](http://www.microsoft.com/technet/windowsvista/library/gpol/2b8dc2fd-eafe-4c74-914c-ec101133feb4.mspx?mfr=true) (engl.)

* [Windows-Hilfe und -Anweisungen](http://windowshelp.microsoft.com/windows/de-de/default.mspx)

* [Microsoft Windows Vista Security Advancements](http://www.microsoft.com/presspass/newsroom/security/vistasecurity.mspx) (engl.)

 
[Zum Seitenanfanq](#mainsection)

**In diesem Beitrag**
* [Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)
* [Kapitel 1: Implementieren der Sicherheitsbasis](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/implementing_security_baseline.mspx)
* [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)
* [Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)
* [Kapitel 4: Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)
* Kapitel 5: Hochsicherheit (SSLF)
* [Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/security_group_policy_settings.mspx)
 

**Download**  


[Windows Vista-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=74028) (engl.)

**Update Notifications**  


[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden.](http://go.microsoft.com/fwlink/?linkid=54982) (engl.)

**Feedback**  


[Senden Sie uns Ihre Kommentare und Anregungen.](mailto:secwish@microsoft.com?subject=windows vista security guide) (engl.)
 

<table style="border:1px solid black;">

<tr>

<td style="border:1px solid black;">

[Zum Seitenanfanq](#mainsection)

</td>

<td style="border:1px solid black;">

[![](https://technet.microsoft.com/de-de/Dd443746.pageLeft(de-de,TechNet.10).gif "Dd443746.pageLeft(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)
6 von 7[![](https://technet.microsoft.com/de-de/Dd443746.pageRight(de-de,TechNet.10).gif "Dd443746.pageRight(de-de,TechNet.10).gif")](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/security_group_policy_settings.mspx)

</td>

</tr>

</table>





