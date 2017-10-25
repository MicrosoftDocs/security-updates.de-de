---
Title: Unterstützung von Smartcard-Anmeldungen für VPN-Verbindungen für den Remotezugriff
TOCTitle: Unterstützung von Smartcard-Anmeldungen für VPN-Verbindungen für den Remotezugriff
ms:assetid: 8a7bcb4b-3c92-4c44-a9aa-be5bb20e7c62
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Cc875840(v=TechNet.10)
ms:contentKeyID: 20072351
---


# Unterstützung von Smartcard-Anmeldungen für VPN-Verbindungen für den Remotezugriff


Auf dieser Seite

[Einführung](#edaa)  
[Smartcard-Technologien](#ecaa)  
[Szenario für die Smartcard-Anmeldung für den VPN-Remotezugriff](#ebaa)  
[Zusammenfassung](#eaaa)  



### Einführung

Dank der Fortschritte in Kommunikationstechnologien, die durch die Notwendigkeit der Kostenminimierung und Wettbewerbsfähigkeit auf einem ständig wachsenden Markt angetrieben werden, sind Unternehmen nicht nur in der Lage, Kommunikationskanäle jeden Tag rund um die Uhr bereitzustellen, sondern auch Zugriff auf Geschäftsdaten und Dienste von entfernten Standorten aus zu bieten.

Das Internet befähigt Unternehmen wie Einzelpersonen, Computer für die Kommunikation und den Datenaustausch auf der ganzen Welt zu nutzen und Vorteile wie hohe Verfügbarkeit, Skalierbarkeit und Leistungsfähigkeit sowie sinkende geschäftsspezifische Kosten wahrzunehmen. Das Internet ist jedoch eine unsichere und potenziell sogar gefährliche Umgebung für Unternehmen, die sich der Herausforderung stellen müssen, die Vorteile des Internets zu nutzen, während gleichzeitig die Daten- und Kommunikationssicherheit im erforderlichen Maß gewahrt bleiben muss.

Virtuelle private Netzwerke (VPNs) ermöglichen Unternehmen die Internetnutzung auf eine Weise, durch die die Einsehbarkeit von Daten und Kommunikationskanälen reduziert wird. Dies erfolgt durch eine Reihe von Sicherheitsfunktionen wie beispielsweise zuverlässige Authentifizierungs- und Verschlüsselungsmechanismen.


#### Zielgruppe dieses Leitfadens

Zur Zielgruppe dieses Leitfadens gehören IT-Experten, die für die Bereitstellung eines VPN-Diensts in ihren Netzwerkumgebungen zuständig sind.

Die Angaben in diesem Leitfaden gelten für kleine bis mittelgroße Unternehmen mit einem Bedarf an zuverlässigem Remotezugriff auf ihre Netzwerke.


#### Übersicht

Für die Konfiguration des VPN-Remotezugriffs auf Netzwerkressourcen können die gleichen Anmeldedaten verwendet werden wie für den herkömmlichen Netzwerkzugriff, nämlich ein Benutzername für das Netzwerk sowie ein Kennwort. Dies ist jedoch nicht unbedingt auch die sicherste Lösung. Visitenkarten oder Dokumente enthalten zum Beispiel mitunter auch Benutzernamen. Außerdem besteht die Gefahr von Trial-and-Error-Angriffen. Falls Dritte Ihren Benutzernamen in Erfahrung bringen, stellt Ihr Kennwort den einzigen verbliebenen Sicherheitsmechanismus für den Schutz Ihres Unternehmensnetzwerks dar.

Ein einzelnes „Geheimnis“, etwa ein Kennwort, kann eine effektive Sicherheitseinrichtung darstellen. Ein langes Kennwort aus einer zufälligen Reihe von Buchstaben, Ziffern und Sonderzeichen lässt sich nur sehr schwer herausfinden. Passphrasen bieten darüber hinaus höhere Sicherheit als einzelne Kennwörter.

Leider lassen sich komplizierte Kombinationen leicht vergessen, weshalb manche Benutzer sie möglicherweise schriftlich notieren. Wenn keine Beschränkungen hinsichtlich der Komplexität von Kennwörtern bestehen, tendieren Benutzer dazu, einfach zu behaltende – und damit auch einfach zu erratende – Kennwörter zu wählen.

Lösungen aus Benutzername und Kennwort werden als Einfaktor-Lösungen bezeichnet, da ein Benutzer für den Netzwerkzugriff etwas verwendet, das ausschließlich ihm bekannt ist. Mehrfaktor-Authentifizierungssysteme umgehen die Problematik der Einfaktor-Authentifizierung durch Verwendung einer Kombination aus Anforderungen, wozu Folgendes gehört:
* Eine Angabe, die dem Benutzer bekannt ist, etwa ein Kennwort oder eine PIN-Nummer.

* Ein Gegenstand im Besitz des Benutzers, etwa ein Hardware-Token oder eine Smartcard.

* Ein Merkmal des Benutzers, etwa ein Fingerabdruck oder Charakteristika der Iris.


Smartcards und die zugehörigen PIN-Nummern finden zunehmend Verbreitung und zeichnen sich als zuverlässige und kostengünstige Zweifaktor-Authentifizierung aus. Benutzer benötigen ihre Smartcards und ihre PIN-Nummern, um Zugriff auf Netzwerkressourcen zu erhalten. Diese Erfordernis von zwei Faktoren reduziert die Wahrscheinlichkeit unberechtigter Zugriffe auf ein Unternehmensnetzwerk erheblich.


#### VPN-Vorteile

Wenn Ihr Unternehmen eine Verbindung für den Remotezugriff zwischen Netzwerken mit vertraulichen und proprietären Daten und dem Internet herstellen muss, stellt die erhöhte Konnektivität ein erhebliches Sicherheitsrisiko dar.

In der potenziell gefährlichen Umgebung des Internets kommt Ihrer VPN-Lösung tragende Bedeutung zu, da sie neben den möglichen Betriebskosteneinsparungen auch zur Wahrung der für eine private Netzwerkinfrastruktur typischen Sicherheit beiträgt. Die Sicherheit einer VPN-Lösung basiert auf der Verwendung einer getunnelten Verbindung, bei der Daten verschlüsselt werden und ausschließlich authentifizierte Benutzer auf das Unternehmensnetzwerk zugreifen können.

VPNs unterstützen eine breite Palette von Authentifizierungsmethoden, Tunneling-Protokollen und Verschlüsselungstechnologien zur Wahrung der Sicherheit von Geschäftsdaten.

Die VPN-Authentifizierungsmethoden umfassen Folgendes:
* Kennwortauthentifizierungsprotokoll (Password Authentication Protocol, PAP).

* Challenge Handshake Authentication-Protokoll (CHAP).

* Microsoft® Challenge-Handshake Authentication-Protokoll (MS-CHAP).

* MS-CHAP Version 2 (MS-CHAP v2).

* Extensible Authentication-Protokoll (EAP).


Zu den VPN-Tunneling-Protokollen gehören:
* Point-to-Point-Tunneling-Protokoll (PPTP).

* Layer Two Tunneling-Protokoll (L2TP).


VPN-Verschlüsselungsprotokolle umfassen:
* Microsoft Punkt-zu-Punkt-Verschlüsselung (Microsoft Point-to-Point Encryption, MPPE).

* IP-Sicherheit (IPsec).


Verwenden Sie zur Unterstützung einer möglichst breiten Palette von Microsoft-Clientbetriebssystemen eine Version von MS-CHAP, PPTP und MPPE.

Bei Verwendung von Microsoft Windows® 2000 oder höher lässt sich mit EAP, L2TP und IPsec eine höhere Sicherheitsstufe erreichen.

Weitere Informationen zu VPN-Authentifizierung, Tunneling und Verschlüsselung erhalten Sie im Whitepaper [Virtual Private-Netzwerkbetrieb: Ein Überblick](http://www.microsoft.com/technet/prodtechnol/windows2000serv/plan/vpnoverview.mspx) (möglicherweise in englischer Sprache) auf Microsoft TechNet unter www.microsoft.com/technet/prodtechnol/windows2000serv/plan/vpnoverview.mspx.
[Zum Seitenanfang](#mainsection)  



### Smartcard-Technologien

Smartcards bieten eine Zweifaktor-Authentifizierung. Die Zweifaktor-Authentifizierung geht über eine einfache Kombination aus Benutzernamen und Kennwort hinaus und macht die Verwendung eines eindeutigen Tokens und einer PIN-Nummer erforderlich.

Smartcards in Kreditkartengröße enthalten einen Mikrocomputer sowie eine kleine Speicherkapazität. Sie gewährleisten eine sichere und nicht manipulierbare Speicherung von privaten Schlüsseln und X.509-Sicherheitszertifikaten.

Um sich bei einem Computer oder über eine Remotezugriffsverbindung zu authentifizieren, führt ein Benutzer die Smartcard in ein geeignetes Lesegerät ein und gibt seine PIN-Nummer ein. Der Zugriff nur mit der PIN-Nummer oder nur mit der Smartcard ist nicht möglich. Umfangreichere Brute-Force-Angriffe auf Smartcard-PINs sind ausgeschlossen, da die Smartcard nach einigen erfolglosen PIN-Eingabeversuchen gesperrt wird.

Smartcards verfügen über eingebettete Betriebssysteme und eine Art Dateisystem zur Datenspeicherung. Das Betriebssystem einer Smartcard muss die folgenden Aufgaben durchführen können:
* Speichern der öffentlichen und privaten Schlüssel eines Benutzers

* Speichern des auf dem öffentlichen Schlüssel basierenden Zertifikats

* Abrufen dieses Zertifikats

* Durchführen von Aktionen mit dem privaten Schlüssel nach Benutzerbedarf


Weitere Informationen zu Smartcards sowie eine Liste der von Microsoft unterstützten Lesegeräte finden Sie im Artikel über [Smartcards](http://www.microsoft.com/technet/security/topics/identitymanagement/scard.mspx) im Microsoft TechNet unter www.microsoft.com/technet/security/topics/identitymanagement/scard.mspx.


#### Voraussetzungen für die Smartcard-Bereitstellung

Zur Unterstützung von Smartcard-Anmeldungen für Remotezugriff-VPNs benötigt Ihr Computersystem bestimmte Hardware- und Softwarekomponenten.

Weitere Informationen zu den Spezifikationen und Voraussetzungen für die Smartcard-Bereitstellung finden Sie im Artikel [*Planungshandbuch für sicheren Zugriff unter Verwendung von Smartcards*](http://www.microsoft.com/technet/security/topics/networksecurity/securesmartcards/default.mspx) im Microsoft TechNet unter www.microsoft.com/technet/security/topics/networksecurity/securesmartcards/  
default.mspx.

Voraussetzungen für die Smartcard-Clienthardware

Zur Unterstützung der Smartcard-VPN-Lösung müssen Benutzer über einen Clientcomputer verfügen, auf dem Windows XP ausgeführt werden kann.

Darüber hinaus benötigen Benutzer einen Smartcard-Leser, der an eine standardmäßige Peripherieschnittstelle, etwa die serielle Schnittstelle RS-232, PS/2, PC-Karte oder USB (Universal Serial Bus), angeschlossen ist.

Voraussetzungen für die Smartcard-Clientsoftware

Remotezugriffsclients benötigen zur Unterstützung der Smartcard-VPN-Lösung Windows XP. Darüber hinaus wird die Installation von Service Pack 2 (SP2) empfohlen.

Für jeden Clientcomputer ist die Installation eines Kryptografiedienstanbieters (CSP) erforderlich, der die jeweilige Smartcard unterstützt. Windows XP umfasst einen CSP, der mehrere Smartcard-Lösungen unterstützt. Alternativ kann der Anbieter der Smartcard-Lösung einen CSP besorgen. Der CSP führt die folgenden Funktionen aus:
* Verschlüsselungsfunktionen, z. B. digitales Signieren

* Verwaltung des privaten Schlüssels

* Sichere Kommunikation zwischen dem Smartcard-Leser des Clientcomputers und der Smartcard


Auf jedem Clientcomputer müssen Gerätetreiber für den jeweiligen Smartcard-Leser installiert werden. Die Gerätetreiber ordnen die Funktionalität des Lesers den nativen Diensten unter Windows XP und der Smartcard-Infrastruktur zu. Der Gerätetreiber des Smartcard-Lesers macht eine Mitteilung, wenn die Karte eingesetzt oder entnommen wird, und bietet Funktionen für die Datenkommunikation zu und von der Karte.

Der Verbindungs-Manager ist eine Standardfunktion unter Windows XP, mit der Netzwerk-, Einwahl- und VPN-Verbindungen erleichtert und verwaltet werden. Mit dem Verbindungs-Manager-Verwaltungskit können außerdem Verbindungs-Manager-Profile angepasst und eine Installationsdatei erstellt werden, die die VPN-Verbindung automatisch konfiguriert, so dass sie an die Clients verteilt werden kann.

Die Smartcard-Bereitstellung kann Kartenverwaltungssoftware auf dem Client einschließen. Diese Software umfasst Tools zur Verwaltung, Konnektivität und Sicherheit von Smartcards, mit denen der Inhalt von Smartcards eingesehen, PINs zurückgesetzt und zusätzliche Zertifikate hinzugefügt werden können.

Voraussetzungen für die VPN-Serverhardware

VPN-Verbindungen bedeuten zusätzliche Prozessorauslastungen auf dem Remotezugriffsserver. Sichere Smartcard-Anmeldungen tragen nur geringfügig dazu bei. VPN-Remotezugriffsserver mit einem hohen Aufkommen an eingehenden Verbindungen benötigen neben der Tauglichkeit für starken Netzwerkverkehr schnelle Prozessoren, möglichst in einer Mehrprozessorkonfiguration. Unternehmen, die durch IPsec gesicherte VPNs verwenden, können Netzwerkkarten einsetzen, die den IPsec-Verschlüsselungsvorgang auf einen separaten Prozessor auf der Netzwerkkarte umlagern.

Voraussetzungen für die VPN-Serversoftware

Die Voraussetzungen für die VPN-Serversoftware für den Smartcard-Zugriff sind relativ einfach. Auf den Remotezugriffsservern muss Windows 2000 Server oder höher ausgeführt werden, und Routing und RAS muss aktiviert sein. Außerdem ist Unterstützung von EAP-TLS (Extensible Authentication Protocol-Transport Layer Security) erforderlich.

Bei EAP-TLS handelt es sich um einen Mechanismus zur gegenseitigen Authentifizierung, der für die Verwendung in Verbindung mit Sicherheitsgeräten wie Smartcards und Hardware-Tokens konzipiert wurde. EAP-TLS unterstützt das Point-to-Point-Protokoll (PPP) und VPN-Verbindungen und ermöglicht den Austausch von gemeinsamen geheimen Schlüsseln für MPPE zusätzlich zu IPsec.

Die Hauptvorteile von EAP-TLS bestehen in der Widerstandskraft gegenüber Brute-Force-Angriffen und der Unterstützung gegenseitiger Authentifizierungen. Bei der gegenseitigen Authentifizierung müssen sich Client und Server untereinander identifizieren. Falls der Client oder der Server kein Zertifikat zur Identitätsüberprüfung überträgt, wird die Verbindung abgebrochen.

Microsoft Windows Server™ 2003 unterstützt EAP-TLS für Einwähl- und VPN-Verbindungen, wodurch Remotebenutzer Smartcards verwenden können. Weitere Informationen zu EAP-TLS finden Sie im Artikel zum [Extensible Authentication-Protokoll (EAP)](http://www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/auth_eap.mspx) (möglicherweise in englischer Sprache) unter www.microsoft.com/resources/documentation/windows/xp/all/proddocs/en-us/auth_eap.mspx.

Weitere Informationen zu EAP-Zertifikatsvoraussetzungen finden Sie im Microsoft Knowledge Base-Artikel [Anforderungen Zertifikat, verwenden Sie EAP-TLS oder PEAP mit EAP-TLS](http://support.microsoft.com/default.aspx?scid=814394) unter http://support.microsoft.com/default.aspx?scid=814394.


#### Netzwerkinfrastrukturvoraussetzungen für Smartcard-Bereitstellungen

Für Smartcards ist eine geeignete Infrastruktur erforderlich, die vom Betriebssystem und den Netzwerkelementen unterstützt wird. Vor Beginn des Smartcard-Bereitstellungsvorgangs ist die Notwendigkeit der folgenden Komponenten zu berücksichtigen:
* Benutzeranforderungen

* Public Key-Infrastruktur (PKI)

* Zertifikatvorlagen

* Der Active Directory®-Verzeichnisdienst

* Sicherheitsgruppen

* Registrierungsstellen und -Agenten


Benutzeranforderungen

Die Identifizierung von Benutzern und Gruppen, die VPN-Zugriff benötigen, ist ein wichtiger Bestandteil der Smartcard-Bereitstellung. Ermitteln Sie diese Konten zu einem frühen Zeitpunkt des Vorgangs, um den Projektumfang festlegen und die Kosten kontrollieren zu können.

Public Key-Infrastruktur (PKI)

Für Smartcard-Lösungen ist eine PKI erforderlich, um Zertifikate mit Paaren aus öffentlichen und privaten Schlüsseln bereitzustellen, mit denen Konten in Active Directory zugeordnet werden können. Solch eine PKI lässt sich auf zwei Arten implementieren: Überlassen Sie die interne Zertifikatsstruktur einer externen Organisation, oder nutzen Sie die Zertifikatsdienste unter Windows Server 2003. Zur Nutzung der Zertifikatsdienste unter Windows Server 2003 für Ihre Smartcard-Lösung muss die Zertifizierungsstelle eine Unternehmensstelle sein, für die Active Directory erforderlich ist.

Weitere Informationen zu den Zertifikatsdiensten in Windows Server 2003 finden Sie auf der Website [Public Key-Infrastruktur für Windows Server 2003](http://www.microsoft.com/windowsserver2003/technologies/pki/default.mspx) (möglicherweise in englischer Sprache) unter www.microsoft.com/windowsserver2003/technologies/pki/default.mspx.

Die PKI muss über einen Mechanismus zur Zertifikatssperrung verfügen. Die Zertifikatssperrung ist erforderlich, wenn ein Zertifikat abläuft oder möglicherweise von einem Angreifer manipuliert wurde. Durch das Sperren eines Zertifikats kann ein Administrator jedem, der dieses Zertifikat verwendet, den Zugriff verweigern. Jedes Zertifikat enthält den Speicherort seiner Zertifikatssperrliste (CRL, Certificate Revocation List).

Weitere Informationen zur Handhabung der Zertifikatssperrung finden Sie im Artikel [Zertifikatssperrung verwalten](http://technet2.microsoft.com/windowsserver/en/library/92a5e655-3eb2-4843-b9cb-58c84c0a91d61033.mspx?mfr=true) (möglicherweise in englischer Sprache) im Microsoft TechNet unter http://technet2.microsoft.com/WindowsServer/en/library/92a5e655-3eb2-4843-b9cb-58c84c0a91d61033.mspx?mfr=true.

Verwenden Sie die PKI zur Zuordnung eines Zertifikats zu jeder Smartcard in Ihrer VPN-Lösung. Das Zertifikat muss von einer Zertifizierungsstelle ausgestellt werden, die vom VPN-Server als vertrauenswürdig eingestuft wird. Achten Sie bei der Nutzung der Zertifikatsdienste unter Windows Server 2003 darauf, das PKI-Stammzertifikat auf dem VPN-Server zu installieren.

Für die gegenseitige Authentifizierung müssen Sie dem VPN-Server ein Zertifikat von einer Zertifizierungsstelle zuordnen, die vom Client als vertrauenswürdig eingestuft wird. Achten Sie bei der Nutzung der Zertifikatsdienste unter Windows Server 2003 darauf, das PKI-Stammzertifikat auf dem VPN-Client zu installieren.

Zertifikatvorlagen

Windows Server 2003 umfasst spezielle Zertifikatvorlagen für die Ausstellung digitaler Zertifikate zur Verwendung mit Smartcard-Lösungen. Die folgenden drei Zertifikatvorlagen stehen für die Smartcard-Verwendung zur Verfügung:
* Der Registrierungs-Agent, mit dem ein autorisierter Benutzer Zertifikate für andere Personen anfordern kann.

* Smartcard-Benutzer, mit dem ein Benutzer sich mit einer Smartcard anmelden und E-Mails signieren kann. Darüber hinaus bietet dieses Zertifikat Clientauthentifizierung.

* Smartcard-Anmeldung, die die Benutzeranmeldung mit einer Smartcard und Clientauthentifizierung, jedoch keine signierten E-Mails ermöglicht.


**Hinweis**   Zur Nutzung verbesserter Sicherheitsfunktionen empfiehlt Microsoft ausdrücklich die Aktualisierung einer vorhandenen Windows Server 2003-PKI auf eine Windows Server 2003-PKI mit Service Pack 1 (SP1).

Für Ihre VPN-Lösung ist mindestens ein Administrator mit einem Registrierungs-Agent-Zertifikat erforderlich, der den Smartcards Zertifikate zuordnet. Darüber hinaus werden für Ihre Clients Smartcard-Anmeldezertifikate auf deren Smartcards benötigt.

Weitere Informationen zu Zertifikatvorlagen finden Sie im Artikel über [Zertifikatvorlagen](http://technet2.microsoft.com/windowsserver/en/library/7d82b420-10ef-4f20-a56f-17ee7ee352d21033.mspx?mfr=true) (möglicherweise in englischer Sprache) im TechNet unter http://technet2.microsoft.com/WindowsServer/en/Library/7d82b420-10ef-4f20-a56f-17ee7ee352d21033.mspx?mfr=true.

Active Directory

Active Directory stellt die Mittel zur Verwaltung der Identitäten und Beziehungen zur Verfügung, aus denen Netzwerkumgebungen bestehen, und ist eine Schlüsselkomponente für die Implementierung von Smartcard-Lösungen. Unter Windows Server 2003 bietet Active Directory Unterstützung für die Erzwingung von Smartcard-Anmeldungen sowie die Möglichkeit, Konten Zertifikaten zuzuordnen. Durch diese Möglichkeit wird der private Schlüssel auf der Smartcard mit dem Zertifikat in Active Directory verknüpft.

Wenn der Registrierungs-Agent der Smartcard eines Benutzers ein Zertifikat zuordnet, wird das Zertifikat dabei dem Benutzerkonto in Active Directory zugeordnet. Bei der Angabe der Smartcard-Anmeldeinformationen muss Active Directory die jeweilige Karte mit dem Benutzerkonto abgleichen, wonach der Benutzer die erforderlichen Berechtigungen und Funktionen für das Netzwerk erhält.

Weitere Informationen zur Zertifikatszuordnung finden Sie im Artikel [Zuordnen von Zertifikaten zu Benutzerkonten](http://www.microsoft.com/resources/documentation/windowsserv/2003/all/deployguide/en-us/dssch_pki_cyek.asp) (möglicherweise in englischer Sprache) im Microsoft TechNet unter www.microsoft.com/resources/documentation/WindowsServ/2003/all/deployguide/en-us/dssch_pki_cyek.asp.

Weitere Informationen zu Active Directory finden Sie auf der Seite über [Windows Server 2003 Active Directory](http://www.microsoft.com/windowsserver2003/technologies/directory/activedirectory/default.mspx) unter www.microsoft.com/windowsserver2003/technologies/directory/activedirectory/  
default.mspx.

Sicherheitsgruppen

Der Smartcard-Bereitstellungs- und -Verwaltungsprozess ist bedeutend einfacher, wenn innerhalb von Active Directory Sicherheitsgruppen zum Organisieren von Benutzern verwendet werden. Für eine typische Smartcard-Bereitstellung kann z. B. die Einrichtung der folgenden Sicherheitsgruppen erforderlich sein:
* **Smartcard-Registrierungs-Agenten.**   Smartcard-Registrierungs-Agenten sind für die Verteilung von Smartcards an Benutzer zuständig.

* **Smartcard-Staging.**   Die Smartcard-Staging-Gruppe umfasst alle Benutzer, die Smartcards erhalten, deren Karten jedoch noch von keinem Registrierungs-Agenten registriert und aktiviert wurden.

* **Smartcard-Benutzer.**   Die Gruppe der Smartcard-Benutzer umfasst alle Benutzer, für die der Registrierungsvorgang abgeschlossen ist und deren Karten aktiviert wurden. Der Registrierungs-Agent verschiebt entsprechende Benutzer aus der Smartcard-Staging-Gruppe in die Gruppe der Smartcard-Benutzer.

* **Smartcard – temporäre Ausnahmen.**   Die Gruppe der temporären Ausnahmen für Smartcards ist für Benutzer gedacht, die vorübergehende Ausnahmen von den Smartcard-Erfordernissen benötigen, etwa weil Smartcards verloren gegangen sind oder vergessen wurden.

* **Smartcard – permanente Ausnahmen.**   Die Gruppe der permanenten Ausnahmen für Smartcards umfasst Konten, für die permanente Ausnahmen von der Erfordernis von Smartcard-Anmeldungen notwendig sind.


Für Ihre VPN-Lösung sind zumindest Gruppen für Registrierungs-Agenten und Smartcard-Benutzer erforderlich. Die Einrichtung dieser Gruppen ermöglicht Ihnen eine vereinfachte Verwaltung und Konfiguration mehrerer Benutzer.

Registrierungsstellen und -Agenten

Um Smartcards für Benutzer auszustellen bzw. Benutzer für Smartcards zu registrieren, kann zwar eine webbasierte Oberfläche verwendet werden, doch wird diese Vorgehensweise nicht empfohlen. Da Benutzer zum Erhalt von Smartcards ihre Benutzernamen und Kennwörter angeben müssen, wird hierbei die Sicherheit der Smartcard im Endeffekt auf die Stufe herabgesetzt, die für die Eingabe von Anmeldeinformationen im Web gilt. Die empfohlene Vorgehensweise besteht darin, Registrierungsstellen einzurichten und mindestens einen Administrator als Registrierungs-Agenten einzusetzen.

Eine typische Registrierungsstelle besteht aus einem Computer mit einem Lese- und Schreibgerät für Smartcards. Über das Lesegerät kann sich der Registrierungs-Agent anmelden, und über das Schreibgerät können neue Smartcards ausgegeben werden. Die Registrierungsstelle enthält eine Gruppenrichtlinieneinstellung, infolge derer nach Entnahme der Smartcard des Registrierungs-Agenten automatisch eine sofortige Abmeldung erfolgt.

Ein Administrator übernimmt die Rolle des Registrierungs-Agenten und verwendet seine Smartcard für die Anmeldung bei der Registrierungsstelle. Er öffnet danach die Webseite für die Zertifikatsdienste, überprüft die Identität des Benutzers, registriert ihn und stellt die registrierte Smartcard aus. Registrierungs-Agenten benötigen ein Registrierungs-Agent-Zertifikat und die Berechtigung zum Zugriff auf die Zertifikatvorlagen.


#### Erwägungen zum Einsatz

Ihre Smartcard-VPN-Lösung muss in der Lage sein, den einwandfreien Einsatz der Lösung zu überwachen. Die Überwachungstools müssen die für die fortwährende Einsetzbarkeit notwendigen Informationen anzeigen. Sollte dies nicht gegeben sein, kann das Sicherheitspersonal nicht feststellen, ob die Lösung auf effektive Weise für sichere Remotezugriffsverbindungen sorgt.

Folgende Punkte sind in die Erwägungen einzubeziehen:
* **Testen der Authentifizierung bei internen Anwendungen.**   Die Verwendung einer Smartcard sollte nur die anfängliche Anmeldung betreffen. Mit dem Pilotprogramm sollte der Erfolg der Authentifizierung bei internen Anwendungen getestet und überprüft werden.

* **Beheben von Problemen auf dem Remoteclient.**   Zur erfolgreichen Behebung von Clientproblemen kann eine enge Zusammenarbeit von mehreren Teams in verschiedenen Zeitzonen erforderlich sein. Strenge Tests und eine geeignete Pilot-Bereitstellung tragen zur Reduzierung von Supportanrufen bei.

* **Verständnis der Remotezugriffsszenarien und Bedrohungen für das Unternehmen.**   Das Verständnis der Remotezugriffsszenarien und Sicherheitsbedrohungen in Ihrem Unternehmen sowie des Verhältnisses zwischen ihnen ist unabdingbar. Sie müssen den Anlagen mit dem größten Schutzbedarf Priorität einräumen und ein geeignetes Kosten-Risiko-Verhältnis ermitteln.

* **Einplanen technischer Herausforderungen.**   Planen Sie technische Herausforderungen ein, etwa Installationsroutinen und die Verteilung von Smartcard-Verwaltungstools. Möglicherweise muss die Smartcard-Lösung in Ihre vorhandenen Unternehmensverwaltungstools integriert werden.

* **Überwachen und Verwalten von Leistungsaspekten.**   Sie müssen Leistungsaspekte überwachen und verwalten und vor der Bereitstellung klären, was Benutzer erwarten können.

* **Berücksichtigung privater Anlagen.**   Vergessen Sie nicht, dass die Heimcomputer von Mitarbeitern deren Besitz sind und nicht von der IT-Abteilung eines Unternehmens verwaltet werden. Für den Fall, dass ein Mitarbeiter nicht in der Lage ist, die für den sicheren Smartcard-Remotezugriff erforderliche Hardware und Software zu installieren, gibt es andere Optionen. So bietet z. B. Microsoft Outlook® Web Access (OWA) Mitarbeitern Zugriff auf ihre Microsoft Exchange Server-Postfächer über verschlüsselte SSL- (Secure Sockets Layer-)Verbindungen.

Weitere Informationen zur E-Mail-Sicherheit finden Sie im Dokument [Schutz der Vertraulichkeit von E-Mails in regulierten Branchen](http://go.microsoft.com/fwlink/?linkid=71176) dieser Serie unter http://go.microsoft.com/fwlink/?LinkId=71176.

* **Verwalten von Änderungen an der Lösung.**   Jegliche Änderungen und Verbesserungen, die an der Lösung vorgenommen werden, müssen anhand ähnlicher Prozesse wie die für die anfängliche Bereitstellung verwaltet werden.

* **Optimierung der Lösung.**   Sämtliche Aspekte der Smartcard-Lösung bedürfen einer regelmäßigen Überprüfung und ggf. Optimierung. Überprüfen Sie in regelmäßigen Abständen die Registrierungsprozesse und die Notwendigkeit von Kontoausnahmen zum Zweck der Verbesserung der Sicherheit und Integrität.

 
[Zum Seitenanfang](#mainsection)  



### Szenario für die Smartcard-Anmeldung für den VPN-Remotezugriff

Der in diesem Abschnitt beschriebene Prozess zur Konfiguration der Smartcard-Anmeldung für Remotezugriff-VPNs ist für kleine und mittelgroße Unternehmen gedacht. Die folgende Abbildung stellt das Netzwerk eines mittelgroßen Unternehmens dar. In Ihrer eigenen Umgebung können einige oder alle der angegebenen Dienste vorhanden sein.


**Abbildung 1. Remotezugriff in mittelgroßen IT-Umgebungen**
 

Dieser Prozess ist speziell für Szenarien geeignet, in denen Remotebenutzer von externen Standorten aus Zugriff auf Unternehmensdaten und -dienste benötigen. Um Zugriff zu erhalten, stellen die Remotebenutzer eine VPN-Verbindung zu einem VPN-Server her, auf dem Windows Server 2003 ausgeführt wird, und verwenden Smartcards zur Authentifizierung.

Die folgenden Verfahren helfen Ihnen bei der Vorbereitung, Bereitstellung und Konfiguration der Smartcard-Unterstützung für Remotezugriff-VPNs.


#### Vorbereitung einer Zertifizierungsstelle für die Ausstellung von Smartcard-Zertifikaten

Zuerst ist die Zertifizierungsstelle für die Zuordnung der erforderlichen Zertifikate, des Registrierungs-Agenten und der Smartcard-Anmeldung vorzubereiten.

**So bereiten Sie eine Zertifizierungsstelle für die Ausstellung von Smartcard-Zertifikaten vor**
* Melden Sie sich mit Administratorrechten an.

* Öffnen Sie **Active Directory-Standorte und -Dienste.**  

* Klicken Sie im Menü **Ansicht** auf **Dienstknoten anzeigen.**  

* Erweitern Sie **Dienste**, klicken Sie auf **Public Key Services** und danach auf **Zertifikatvorlagen** (siehe Abbildung).

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn02_big(de-de,technet.10).gif)

* Klicken Sie mit der rechten Maustaste auf die Zertifikatvorlage **EnrollmentAgent**, und wählen Sie **Eigenschaften** aus.

* Fügen Sie die Sicherheitsgruppe für die Registrierungs-Agenten hinzu, die Sie im Rahmen der Bereitstellungsvoraussetzungen eingerichtet haben, und weisen Sie **Lese**- und **Registrierungsberechtigungen** zu (siehe Abbildung). Klicken Sie danach auf **OK.**  

&gt;  
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn03_big(de-de,technet.10).gif)

* Schließen Sie **Active Directory-Standorte und -Dienste.**  

* Öffnen Sie **Zertifizierungsstelle.**  

* Erweitern Sie den Servernamen, und wählen Sie **Zertifikatvorlagen** aus. Im rechten Fensterbereich sehen Sie die Liste der Zertifikate, die von der Zertifizierungsstelle zugeordnet werden können (siehe Abbildung).

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn04_big(de-de,technet.10).gif)

* Klicken Sie mit der rechten Maustaste auf **Zertifikatvorlagen**, zeigen Sie auf **Neu**, und klicken Sie danach auf **Auszustellende Zertifikatvorlage.**  

* Halten Sie die STRG-Taste gedrückt, während Sie in der Liste **Zertifikatvorlagen aktivieren** die Einträge **Registrierungs-Agent** und **Smartcard-Anmeldung** markieren (siehe Abbildung). Klicken Sie danach auf **OK.**  

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn05_big(de-de,technet.10).gif)

* Schließen Sie **Zertifizierungsstelle.**  



#### Bereitstellung von Zertifikaten für Smartcards

Nun können Sie Zertifikate Smartcards und Remotebenutzern zuordnen. Melden Sie sich als Registrierungs-Agent für die Domäne an, in der sich das betreffende Benutzerkonto befindet.

**So stellen Sie Zertifikate für Smartcards bereit**
* Öffnen Sie Microsoft Internet Explorer®.

* Geben Sie in der Adressleiste die Adresse der Zertifizierungsstelle ein, die Smartcard-Anmeldezertifikate ausstellt, und drücken Sie die Eingabetaste.

* Klicken Sie auf **Ein Zertifikat anfordern** und danach auf **Erweiterte Zertifikatanforderung.**   Ein Bildschirm ähnlich dem folgenden wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn06_big(de-de,technet.10).gif)

* Klicken Sie auf **Ein Smartcardzertifikat für einen anderen Benutzer mit Hilfe der Smartcard-Zertifikatregistrierungsstelle anfordern.**   Klicken Sie bei der Aufforderung, ein Microsoft ActiveX®-Steuerelement anzunehmen, auf **Ja.**   Sie müssen die Verwendung von ActiveX-Steuerelementen in Internet Explorer aktivieren.

* Wählen Sie auf dem Bildschirm **Smartcard-Zertifikatregistrierungsstelle** (siehe Abbildung) **Smartcard-Anmeldung** aus. Es sollten die Namen der **Zertifizierungsstelle**, des **Kryptografiedienstanbieters** und des **Administratorsignaturzertifikats** angezeigt werden. Falls kein Administratorsignaturzertifikat ausgewählt werden kann, wurde dem angemeldeten Benutzer kein Registrierungs-Agent-Zertifikat zugeordnet.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn07_big(de-de,technet.10).gif)

* Wählen Sie in der Dropdownliste **Zertifizierungsstelle** den Namen der Zertifizierungsstelle aus, die das Smartcard-Zertifikat ausstellen soll.

* Wählen Sie in der Dropdownliste **Kryptografiedienstanbieter** den Hersteller der Smartcard aus.

* Geben Sie unter **Administratorsignaturzertifikat** den Namen des Registrierungs-Agent-Zertifikats ein, das die Registrierungsanforderung signieren wird, oder klicken Sie auf **Zertifikat auswählen**, um einen Namen auszuwählen.

* Klicken Sie auf **Benutzer wählen**, und wählen Sie danach das gewünschte Benutzerkonto aus. Klicken Sie auf **Registrieren.**  

* Schieben Sie bei Aufforderung die Smartcard in den Smartcard-Leser an Ihrem Computer ein, und klicken Sie auf **OK.**   Geben Sie bei Aufforderung die PIN-Nummer für die Smartcard ein.



#### Konfiguration von VPN-Servern für die Smartcard-Authentifizierung

Nun können Sie den VPN-Server konfigurieren.

**So konfigurieren Sie den Routing- und RAS-Dienst zur Annahme der EAP-Authentifizierung**
* Starten Sie das Routing- und RAS-Snap-In.

* Klicken Sie mit der rechten Maustaste auf ***&lt;servername&gt;***, und klicken Sie auf **Eigenschaften** und danach auf die Registerkarte **Sicherheit.**  

* Klicken Sie auf **Authentifizierungsmethoden.**  

* Aktivieren Sie das Kontrollkästchen **Extensible Authentication-Protokoll (EAP)** (siehe Abbildung), und klicken Sie auf **OK.**  

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn08_big(de-de,technet.10).gif)

* Klicken Sie auf **OK.**  



#### Konfiguration von RAS-Richtlinien für die Smartcard-Authentifizierung

Nun können Sie EAP in RAS-Richtlinien aktivieren. Die RAS-Richtlinienkomponente ist standardmäßig im Routing- und RAS-Snap-In enthalten. Sofern der Internetauthentifizierungsdienst (IAS; auch als RADIUS-Protokoll für Remoteauthentifizierung bezeichnet) installiert ist, ist die RAS-Richtlinienkomponente stattdessen im IAS-Snap-In enthalten.

**So aktivieren Sie EAP mit RAS-Richtlinien**
* Klicken Sie im linken Bereich von „Routing und RAS“ auf **RAS-Richtlinien.**  

* Doppelklicken Sie im rechten Bereich auf **Verbindungen mit dem Microsoft Routing- und RAS-Server.**   Ein Bildschirm ähnlich dem folgenden wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn09_big(de-de,technet.10).gif)

* Klicken Sie auf **Profil bearbeiten**, auf die Registerkarte **Authentifizierung** und danach auf **EAP-Methoden** (siehe Abbildung).

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn10_big(de-de,technet.10).gif)

* Falls **Smartcard oder anderes Zertifikat** in der Liste **EAP-Typen** nicht wie in der folgenden Abbildung dargestellt angezeigt wird, klicken Sie auf **Hinzufügen**, markieren Sie **Smartcard oder anderes Zertifikat**, und klicken Sie auf **OK.**  

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn11_big(de-de,technet.10).gif)

* Markieren Sie **Smartcard oder anderes Zertifikat**, und klicken Sie auf **Bearbeiten.**   Ein Bildschirm ähnlich dem folgenden wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn12_big(de-de,technet.10).gif)

* Markieren Sie in der Dropdownliste das Zertifikat, das für die EAP-Authentifizierung verwendet werden soll, und klicken Sie danach dreimal auf **OK.**  

* Vergewissern Sie sich, dass **RAS-Berechtigung erteilen** ausgewählt ist, klicken Sie auf **OK**, und schließen Sie dann „Routing und RAS“.



#### Konfiguration von VPN-Clients für die Smartcard-Authentifizierung

Als nächstes konfigurieren Sie den Client für die Verwendung der EAP-Authentifizierung zur Unterstützung von Smartcards.

**So erstellen Sie einen Telefonbucheintrag**
* Klicken Sie auf **Start**, zeigen Sie auf **Verbinden mit** und danach auf **Alle Verbindungen anzeigen**, und klicken Sie in der Liste **Netzwerkaufgaben** auf **Neue Verbindung erstellen.**   Klicken Sie danach auf der Willkommensseite des **Assistenten für neue Verbindungen** auf **Weiter.**   Der folgende Bildschirm wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn13_big(de-de,technet.10).gif)

* Wählen Sie **Verbindung mit dem Netzwerk am Arbeitsplatz herstellen** aus, und klicken Sie auf **Weiter.**  

* Wählen Sie **VPN-Verbindung** aus, und klicken Sie auf **Weiter.**  

* Geben Sie einen Namen für die Verbindung im Feld **Firmenname** ein, und klicken Sie auf **Weiter.**   Der folgende Bildschirm wird angezeigt.


 

* Sofern Sie permanent mit dem Internet verbunden sind, wählen Sie **Keine Anfangsverbindung automatisch wählen** aus, und klicken Sie danach auf **Weiter.**   Falls Sie vor der Einrichtung eines VPN eine Verbindung per Einwahl herstellen müssen, können Sie alternativ **Automatisch diese Anfangsverbindung wählen** und danach die Einwählverbindung in der Dropdownliste auswählen und auf **Weiter** klicken.

* Geben Sie den VPN-Servernamen oder die IP-Adresse im Feld **Hostname oder IP-Adresse** ein, und klicken Sie auf **Weiter.**  

* Wählen Sie **Eigene Smartcard verwenden** aus, klicken Sie auf **Weiter** und danach auf **Fertig stellen.**  


Konfigurieren Sie den Telefonbucheintrag nach dessen Erstellung für die Verwendung von EAP.

**So konfigurieren Sie eine vorhandene Verbindung für die Verwendung der Smartcard-Authentifizierung**
* Klicken Sie mit der rechten Maustaste auf die Verbindung, wählen Sie **Eigenschaften** aus, und klicken Sie danach auf die Registerkarte **Sicherheit.**   Der folgende Bildschirm wird angezeigt.


 

* Vergewissern Sie sich, dass **Typisch (empfohlene Einstellungen)** ausgewählt ist, und klicken Sie danach in der Dropdownliste **Identität folgendermaßen bestätigen** auf die Option **Smartcard verwenden.**  

* Wählen Sie **Erweitert (benutzerdefinierte Einstellungen)** aus, und klicken Sie auf **Einstellungen.**  

* Klicken Sie auf **Smartcard oder anderes Zertifikat (Verschlüsselung aktiviert).**  

* Klicken Sie auf **Eigenschaften** und danach auf **Eigene Smartcard verwenden.**  

* Vergewissern Sie sich, dass die Option **Serverzertifikat überprüfen** aktiviert ist.

* Aktivieren Sie bei Bedarf das Kontrollkästchen **Verbindung herstellen, wenn Servername folgendermaßen endet.**  

* Klicken Sie im Feld **Vertrauenswürdige Stammzertifizierungsstellen** auf den Namen der Zertifizierungsstelle, die das Zertifikat zur Verwendung mit einer Smartcard ausgestellt hat, oder auf das installierte Benutzerzertifikat.

* Aktivieren Sie bei Bedarf das Kontrollkästchen **Anderen Benutzernamen für die Verbindung verwenden.**  

* Der Benutzer muss beim Computer angemeldet sein, um EAP mit einem Benutzerzertifikat zu nutzen.



#### Konfiguration von VPN-Clients für die Smartcard-Authentifizierung mit dem Verbindungs-Manager

Falls VPN-Verbindungen für mehrere Clients zu konfigurieren sind, können Sie den Verbindungs-Manager verwenden.

**So installieren Sie das Verbindungs-Manager-Verwaltungskit auf einem Windows Server 2003-Computer**
* Klicken Sie auf **Start**, **Systemsteuerung** und anschließend auf **Software.**  

* Klicken Sie im Dialogfeld **Software** auf **Windows-Komponenten hinzufügen/entfernen.**  

* Markieren Sie auf dem Bildschirm **Assistent für Windows-Komponenten** die Option **Verwaltungs- und Überwachungsprogramme**, und klicken Sie auf **Details.**   Ein Bildschirm ähnlich dem folgenden wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn16_big(de-de,technet.10).gif)

* Markieren Sie im Dialogfeld **Verwaltungs- und Überwachungsprogramme** die Option **Verbindungs-Manager-Verwaltungskit**, und klicken Sie auf **OK**, auf **Weiter** und schließlich auf **Fertig stellen.**  


**So verwenden Sie das Verbindungs-Manager-Verwaltungskit zur Einrichtung eines VPN-Verbindungsprofils zur Verteilung an Benutzer**
* Klicken Sie auf **Start**, **Verwaltung** und danach auf **Verbindungs-Manager-Verwaltungskit.**  

* Klicken Sie auf dem Bildschirm **Willkommen** auf **Weiter.**  

* Vergewissern Sie sich, dass **Neues Profil** ausgewählt ist, und klicken Sie auf **Weiter.**  

* Geben Sie im Feld **Dienstname** einen Profilnamen und im Feld **Dateiname** einen Namen für die ausführbare Datei ein, die Sie an die Clients verteilen.

* Auf dem Bildschirm **Bereichsname** (siehe Abbildung) können Sie einen Bereichsnamen zum Benutzernamen hinzufügen. Sie müssen u. U. einen Bereichsnamen zur Identifizierung der Benutzer hinzufügen, falls diese die Verbindung zu Ihrem VPN über den Netzwerkzugriffsserver eines Dritten herstellen, der RADIUS zur Übertragung von Netzwerkauthentifizierungsinformationen auf Ihre Internetauthentifizierungsdienst- (IAS-)Server verwendet.

Wählen Sie **Keinen Bereichsnamen zum Benutzernamen hinzufügen** aus (es sei denn, dies ist erforderlich), und klicken Sie auf **Weiter.**  


 

* Auf dem Bildschirm **Profilinformation zusammenführen** können Sie zuvor konfigurierte Verbindungs-Manager-Profile zusammenführen. Dies dient dazu, in anderen Profilen vorhandene Informationen (etwa Netzwerkzugriffsnummern) in das aktuelle Profil zu übernehmen. Fügen Sie jegliche erforderlichen Profile hinzu, und klicken Sie auf **Weiter.**  

* Auf dem Bildschirm **VPN-Unterstützung** (siehe Abbildung) können Sie ein Telefonbuch aus dem Profil erstellen und den bzw. die VPN-Server für Ihre VPN-Clients konfigurieren.


 

Ein Telefonbuch enthält Informationen wie z. B. Vorwahl, Anschlussnummer und Benutzerauthentifizierungsmethoden. Das Telefonbuch des Verbindungs-Managers umfasst außerdem verschiedene Netzwerkeinstellungen, die Sie bei der Ausführung des Assistenten für das Microsoft Verbindungs-Manager-Verwaltungskit konfigurieren.

Soll Ihr Client die Option erhalten, Verbindungen mit mehreren VPN-Servern herzustellen, können Sie eine VPN-Serverliste in einer Textdatei erstellen (siehe Abbildung). Soll für die Verbindung eine VPN-Serverliste verwendet werden, wählen Sie **Benutzer kann VPN-Server selbst wählen** aus, navigieren Sie zur Textdatei, und klicken Sie danach auf **Weiter.**  


 

* Wählen Sie auf dem Bildschirm **VPN-Einträge** das Profil aus, das Sie erstellen, und klicken Sie auf **Bearbeiten** und danach auf die Registerkarte **Sicherheit.**   Das folgende Dialogfeld wird angezeigt.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn20_big(de-de,technet.10).gif)

* Wählen Sie in der Dropdownliste **Sicherheitseinstellungen** die Option **Erweiterte Sicherheitseinstellungen verwenden** aus, und klicken Sie auf **Konfigurieren.**   Das folgende Dialogfeld wird angezeigt.


 

* Stellen Sie sicher, dass in der Dropdownliste **Datenverschlüsselung** der Eintrag **Verschlüsselung ist erforderlich** aktiviert ist, und dass Sie das korrekte Tunneling-Protokoll in der Dropdownliste „VPN-Strategie“ auswählen.

Wählen Sie **Extensible-Authentication-Protokoll (EAP) verwenden** und „Smartcard oder anderes Zertifikat (Verschlüsselung aktiviert)“ in der entsprechenden Dropdownliste aus, und klicken Sie danach auf **Eigenschaften.**   Ein Bildschirm ähnlich dem folgenden wird angezeigt.


 

* Vergewissern Sie sich, dass **Eigene Smartcard verwenden** ausgewählt ist. Wählen Sie außerdem **Serverzertifikat überprüfen** aus, sofern der Client die Gültigkeit des Servers bestätigen soll. Sie können darüber hinaus den Namen von einem oder mehreren Servern, zu denen die Verbindung hergestellt werden soll, sowie die Stammzertifizierungsstelle für die Serverüberprüfung eingeben. Falls Ihr Client sich anhand eines anderen Benutzernamens als dem im Zertifikat authentifizieren muss, wählen Sie **Anderen Benutzernamen für die Verbindung verwenden** aus. Klicken Sie dreimal auf **OK** und danach auf **Weiter.**  

* Auf dem Bildschirm **Telefonbuch** können Sie eine zusätzliche Telefonbuchdatei in das Profil einschließen und Updates für das Telefonbuch automatisch herunterladen. Das Telefonbuch enthält Informationen wie z. B. Vorwahl, Anschlussnummer und unterstützte Benutzerauthentifizierungsmethoden. Das Telefonbuch des Verbindungs-Managers umfasst außerdem verschiedene Netzwerkeinstellungen, die Sie bei der Ausführung des Assistenten für das Microsoft Verbindungs-Manager-Verwaltungskit konfigurieren. Bei Auswahl von **Automatischer Download von Telefonbuchupdates** müssen Sie den Speicherort angeben, von dem die Updates heruntergeladen werden. Sind keine Telefonbuchupdates erforderlich, wählen Sie diese Option nicht aus. Klicken Sie auf **Weiter.**  

* Markieren Sie bei Verwendung des DFÜ-Netzwerkbetriebs für die Verbindung den Eintrag, und klicken Sie auf dem Bildschirm „DFÜ-Netzwerkeinträge“ auf **Bearbeiten.**   (Verwenden Sie den DFÜ-Netzwerkbetrieb nicht für die Verbindung, erfahren Sie später mehr über die Deaktivierung.) Sobald die erforderliche Konfiguration vorgenommen wurde oder falls der DFÜ-Netzwerkbetrieb nicht gebraucht wird, klicken Sie auf **Weiter.**   Die in den Aufgaben 14 bis 25 erläuterten Bildschirme des Assistenten dienen zur Konfiguration optionaler Komponenten, die hauptsächlich das Erscheinungsbild der Verbindung ändern.

* Sie können die Einstellungen auf dem Bildschirm **Routingtabellenaktualisierung** zur Konfiguration der Routinginformationen für die Verbindung verwenden. Bei Verwendung der Standardeinstellung stellt der VPN-Client die Verbindung zu allen nicht direkt verbundenen Netzwerken über die VPN-Schnittstelle her. Wird der VPN-Client jedoch nicht zur Verwendung der VPN-Verbindung als Standardgateway konfiguriert, können Sie angepasste Routingtabelleneinträge erstellen, mit denen der VPN-Client auf ausgewählte Subnetze im internen Netzwerk zugreifen kann. Klicken Sie zum Abschluss auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Automatische Proxykonfiguration** die Verwendung des VPN-Servers als Webproxyserver durch die VPN-Clients erzwingen. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Benutzerdefinierte Aktionen** Programme angeben, die automatisch vor, nach oder während der VPN-Verbindung gestartet werden. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Anmeldungsbitmap** eine Grafik erstellen, die dem Benutzer beim Öffnen der VPN-Verbindung angezeigt wird. Eine benutzerdefinierte Grafik muss 330 x 140 Pixel groß sein. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Telefonbuchbitmap** eine Grafik erstellen, die dem Benutzer beim Öffnen des Telefonbuchs angezeigt wird. Eine benutzerdefinierte Grafik muss 114 x 309 Pixel groß sein. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Symbole** Symbole festlegen, die in der Benutzeroberfläche des Verbindungs-Managers angezeigt werden sollen. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Infobereichkontextmenü** Elemente in die Kontextmenüs des Verbindungs-Managers aufnehmen. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Hilfedatei** eine benutzerdefinierte Hilfedatei für Ihre Benutzer verwenden. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Supportinformationen** Ihren Benutzern Supportinformationen zur Verfügung stellen. Klicken Sie auf **Weiter.**  

* Sie können nun die Einstellungen auf dem Bildschirm **Verbindungs-Manager-Software** erneut überprüfen. Sie haben die Möglichkeit, Version 1.3 des Verbindungs-Managers auf Clients zu installieren, auf deren Computern das Programm noch nicht installiert wurde. Klicken Sie auf **Weiter.**  

* Sie können anhand der Einstellungen auf dem Bildschirm **Lizenzvertrag** einen benutzerdefinierten Lizenzvertrag für die Verbindung einschließen. Klicken Sie auf **Weiter.**  

* Sie können auf dem Bildschirm **Weitere Dateien** zusätzliche Dateien in das Verbindungs-Manager-Profil aufnehmen. Klicken Sie auf **Weiter.**  

* Wählen Sie auf dem Bildschirm **Dienstprofil erstellen** die Option **Erweiterte Anpassung** aus, und klicken Sie auf **Weiter.**  

* auf dem Bildschirm **Erweiterte Anpassung** (siehe Abbildung) können Sie die Werte der Einstellungen in Ihren Profilkonfigurationsdateien konfigurieren. Sie sollten für Smartcard-fähige VPN-Verbindungen die Einwahl durch Festlegen des Werts 0 deaktivieren. Die Einstellungen HideDomain, HideUserName und HidePassword wurden ebenfalls aktiviert.


 

* Die Profilkonfigurationsdateien sind textbasiert und weisen die Erweiterungen.inf,.cms und.cmp auf. Der Assistent liest die Standarddateien template.inf, template.cms und template.cmp ein, die mit dem Verbindungs-Manager-Verwaltungskit installiert wurden.

Nach Abschluss des Assistenten werden neue Konfigurationsdateien für das Profil mit den Namen profilename.inf, profilename.cms und profilename.cmp erstellt. Sie können in die standardmäßigen Vorlagedateien zusätzliche Einstellungen einfügen, die von jedem Benutzer des Assistenten konfiguriert werden können.

Weitere Informationen zu erweiterten Anpassungsoptionen für den Verbindungs-Manager finden Sie auf der Seite [Erweiterte Anpassungsoptionen für den Verbindungs-Manager](http://www.microsoft.com/resources/documentation/windows/2000/server/reskit/en-us/ierk/ch14_d.asp) (möglicherweise in englischer Sprache) unter www.microsoft.com/resources/documentation/Windows/2000/server/reskit/en-us/ierk/Ch14_d.asp.

Die Datei **template.cms** (siehe Abbildung) wurde dahingehend bearbeitet, dass die Felder für die Domäne, den Benutzernamen und das Kennwort ausgeblendet werden können, sodass die Funktionalität bei Bedarf eingeschlossen werden kann. MPPE zieht beim Verschlüsselungsprozess das Benutzerkennwort heran, sodass für die Lösung in einigen Fällen die Felder für Benutzername und Kennwort erforderlich sind.

 
[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc875840.sclvpn24_big(de-de,technet.10).gif)

* Wenn Sie alle Einstellungsänderungen vorgenommen haben, klicken Sie auf **Weiter**, um die ausführbaren und die Konfigurationsdateien zu erstellen. Merken Sie sich den Speicherort der Dateien, und klicken Sie auf **Fertig stellen.**   Die ausführbare Datei wird über Ihre standardmäßigen Softwareverteilungsmechanismen an die Clients verteilt. Auf einem Client kann die Datei manuell ausgeführt werden, Sie können den Vorgang zur Installation der VPN-Verbindung jedoch auch automatisieren.



#### Überprüfung der Smartcard-VPN-Lösung

Ziel des Überprüfungsprozesses ist die Problemerkennung hinsichtlich des Entwurfs und der Konfiguration der Lösung, bevor sie bereitgestellt wird. Sie müssen zur Überprüfung der Smartcard-VPN-Lösung die Hauptverfahren der Lösung durchführen. Überprüfen Sie die folgenden Hauptverfahren:
* Zuordnen eines Zertifikats zu einer Smartcard

* Verteilen des Verbindungs-Manager-Profils

* Installieren des Verbindungs-Manager-Profils

* Herstellen der Verbindung zum VPN-Server anhand der Smartcard-Authentifizierung

* Zugreifen auf interne Netzwerkressourcen über die VPN-Verbindung



#### Fehlerbehebung bei der Smartcard-VPN-Lösung

Ziel des Überprüfungsprozesses ist es, Fehler in der Lösung zu beheben, Verfahrensschwachstellen zu erkennen und besonderes Augenmerk auf betroffene Bereiche zu richten.

Die folgende Tabelle enthält einige Fehlerbehebungsrichtlinien für die Smartcard-VPN-Lösung.

**Tabelle 1. Fehlerbehebungsrichtlinien für Smartcard-VPN**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Problem

</th>

<th style="border:1px solid black;">

Lösung

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Erforderliche Zertifikate sind in der Zertifizierungsstelle nicht verfügbar.

</td>

<td style="border:1px solid black;">


Aktivieren Sie Zertifikatvorlagen unter „Active Directory-Standorte und -Dienste“.

Weisen Sie Registrierungsberechtigungen zu.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Zertifikate können der Smartcard nicht zugeordnet werden.

</td>

<td style="border:1px solid black;">


Installieren Sie ein Smartcard-Schreibgerät.

Weisen Sie ein Registrierungs-Agent-Zertifikat zu.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


VPN-Server kann Remoteclients nicht authentifizieren.

</td>

<td style="border:1px solid black;">


Konfigurieren Sie den Server für die Unterstützung der EAP-TLS-Authentifizierung.

Stellen Sie sicher, dass das auf dem Server verwendete Zertifikat vom Client als vertrauenswürdig eingestuft wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Der Client versucht, vor der Herstellung der VPN-Verbindung eine Verbindung per Einwahl herzustellen.

</td>

<td style="border:1px solid black;">


Konfigurieren Sie den Client so, dass keine Anfangsverbindung automatisch gewählt wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Der Client versucht nicht, vor der Herstellung der VPN-Verbindung eine Verbindung per Einwahl herzustellen.

</td>

<td style="border:1px solid black;">


Konfigurieren Sie den Client so, dass automatisch eine Anfangsverbindung gewählt wird.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Beim Versuch des Clients, die VPN-Verbindung herzustellen, wird die Angabe des Benutzernamens, des Domänennamens und des Kennworts angefordert.

</td>

<td style="border:1px solid black;">


Vergewissern Sie sich, dass die VPN-Verbindung für die Verwendung einer Smartcard konfiguriert ist.

Stellen Sie sicher, dass die Einstellungen HideUserName, HideDomain und HidePassword aktiviert sind.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Der Client hat kein Verbindungsobjekt in Netzwerkverbindungen.

</td>

<td style="border:1px solid black;">


Stellen Sie sicher, dass der Client das Verbindungs-Manager-Profil erhalten hat.

Stellen Sie sicher, dass die ausführbare Datei des Verbindungs-Manager-Profils ausgeführt wurde.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Der Client stellt keine Verbindung zum VPN-Server her.

</td>

<td style="border:1px solid black;">


Stellen Sie sicher, dass die Clientverbindung mit dem korrekten VPN-Servernamen konfiguriert wurde.

Stellen Sie sicher, dass der Client den korrekten Server aus der VPN-Serverliste auswählt.

</td>

</tr>

<tr>

<td style="border:1px solid black;">


Die Authentifizierung des Clients mit dem VPN-Server schlägt fehl.

</td>

<td style="border:1px solid black;">


Stellen Sie sicher, dass der Client die Verbindung mit dem korrekten VPN-Server herstellt.

Vergewissern Sie sich, dass die Smartcard ein Zertifikat aufweist, das vom VPN-Server als vertrauenswürdig eingestuft wird.

</td>

</tr>

</table>


Weitere Informationen zur allgemeinen Fehlerbehebung bei VPN-Verbindungen finden Sie im Artikel [VPN-Fehlerbehebung](http://technet2.microsoft.com/windowsserver/en/library/4543aff5-e10f-487c-92ad-bb5518a736201033.mspx) (möglicherweise in englischer Sprache) im Microsoft TechNet unter http://technet2.microsoft.com/WindowsServer/en/Library/4543aff5-e10f-487c-92ad-bb5518a736201033.mspx.
[Zum Seitenanfang](#mainsection)  



### Zusammenfassung

Die Implementierung von Smartcards zur Authentifizierung von Remotezugriffsverbindungen bietet eine größere Sicherheit als einfache Kombinationen aus Benutzername und Kennwort. Mit Smartcards liegt durch Kombination aus Smartcard und PIN-Nummer eine Zweifaktor-Authentifizierung vor. Eine solche Zweifaktor-Authentifizierung lässt sich erheblich schwieriger manipulieren, und eine PIN-Nummer lässt sich einfacher merken als ein sicheres Kennwort.

Durch die Smartcard-Authentifizierung für Benutzer mit Remotezugriff lässt sich eine zuverlässige und kostengünstige Methode zur Erhöhung der Netzwerksicherheit umsetzen.
 

**Download**  


[Dokument „Unterstützung von Smartcard-Anmeldungen für VPN-Verbindungen für den Remotezugriff“ herunterladen](http://go.microsoft.com/fwlink/?linkid=71173)
 
[Zum Seitenanfang](#mainsection)




