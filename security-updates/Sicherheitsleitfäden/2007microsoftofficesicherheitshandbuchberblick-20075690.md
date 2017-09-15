---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Überblick'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Überblick'
ms:assetid: 'fe58931e-25fa-4a32-8497-416dbe4929c3'
ms:contentKeyID: 20075690
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443747(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch: Bedrohungen und Gegenmaßnahmen
=========================================================================

### Überblick

Veröffentlicht: 11. Nov 2007

Dieses Handbuch ist eine Komponente des [2007 Microsoft Office-Sicherheitshandbuchs](http://www.microsoft.com/germany/technet/security/guidance/clientsecurity/2007office/default.mspx). Er bietet detaillierte Informationen zu Sicherheitsrisiken, Gegenmaßnahmen und Auswirkungen im Bereich sicherheitsbezogener Gruppenrichtlinieneinstellungen für die 2007 Microsoft® Office-Version sowie Empfehlungen für Einstellungen in zwei verschiedenen Sicherheitsumgebungen: Enterprise Client (EC) und Specialized Security Limited Functionality (SSLF). Dieses Handbuch soll Ihnen durch Bereitstellung relevanter Informationen zu den einzelnen Einstellungen zu fundierteren Entscheidungen verhelfen.

Außerdem enthält das Handbuch die CCE-IDs (Common Configuration Enumeration) für alle Einstellungen. CCE stellt Bezeichner für Systemkonfigurationen bereit, die eine schnelle und präzise Korrelation von Konfigurationsdaten aus mehreren Informationsquellen und Tools ermöglichen. Im Zusammenhang mit dem Security Content Automation Protocol (SCAP) wird CCE hauptsächlich zum Erkennen sicherheitsbezogener Konfigurationsprobleme verwendet. CCE-IDs könnten beispielsweise dazu eingesetzt werden, Überprüfungsergebnisse von Konfigurationsbewertungstools mit Aussagen in Dokumenten zu bewährten Methoden im Bereich Konfiguration zu verknüpfen. Weitere Informationen zu CCE finden Sie auf der [CCE-Website](http://cce.mitre.org/).

Bei den meisten Einstellungen handelt es sich um Benutzerrichtlinieneinstellungen, die im ersten Abschnitt aufgeführt sind. Es folgt ein zweiter, kürzerer Abschnitt mit Informationen zu Computerrichtlinieneinstellungen.

Die Informationen unter **Betrifft:** für alle in diesem Handbuch erörterten Einstellungen geben den Speicherort bzw. die Speicherorte in der Gruppenrichtlinie an, in der die Einstellungen enthalten sind. Diese werden durch die administrativen Vorlagendateien bestimmt. Jede Einstellung betrifft eine oder mehrere 2007 Office-Anwendungen. Wenn angegeben ist, dass eine Einstellung das 2007 Microsoft Office System betrifft, heißt dies nicht unbedingt, dass die Einstellung für alle 2007 Office-Anwendungen gilt, auch wenn sie sich auf mehr als eine Anwendung beziehen kann.

#### Auf dieser Seite

[](#etd)[Danksagungen](#etd)
Danksagungen
------------

Das SA-SC-Team möchte dem für die Produktion des *2007 Microsoft Office-Sicherheitshandbuchs: Bedrohungen und Gegenmaßnahmen* verantwortlichen Team danken: Die folgenden Personen waren entweder unmittelbar beteiligt oder lieferten wichtige Beiträge zum Erstellen, Entwickeln und Testen dieses Handbuchs.

**Inhaltsentwicklung**

Bill Gruber – *Microsoft*

Paul Henry – *Wadeware LLC*

Paul Slater – *Wadeware LLC*

**Entwicklungsleitung**

Ross Carter – *Microsoft*

**Lektoren**

John Cobb – *Wadeware LLC*

Jennifer Kerns – *Wadeware LLC*

Steve Wacker – *Wadeware LLC*

**Produktmanager**

Alain Meeus – *Microsoft*

Jim Stuart – *Microsoft*

**Programm-Manager**

Flicka Enloe – *Microsoft*

**Release-Manager**

Karina Larson – *Microsoft*

**Lektoren**

Alan Myrvold – *Microsoft*

Alessio Roic – *Microsoft*

Alex Vandurme – *NCIRC/NATO*

Amanda Hartin – *Microsoft*

Amani Ahmed – *Microsoft*

Ambrose Treacy – *Microsoft*

Anurag Jain – *Microsoft*

Benjamin Gay – *Microsoft*

Brad Albrecht – *Microsoft*

Bryan Staats – *Microsoft*

Chase Carpenter – *Microsoft*

Dave Kesterson – *Microsoft*

David Vanophalvens – *NCIRC/NATO*

Dheeraj Sarpangal – *Microsoft*

Ed McGinn – *Microsoft*

Emily Kao Messmer – *Microsoft*

Eugene Siu – *Microsoft*

Harshal Doshi – *Microsoft*

Howie Dickerman – *Microsoft*

Jeremy Pankratz – *Microsoft*

Joshua Edwards – *Microsoft*

Koreanische Regierung

Kurt Dillard – *Microsoft*

Maithili Dandige – *Microsoft*

Mark Simos – *Microsoft*

Naresh Krishna Kumar Kulothungan – *Infosys Technologies Ltd*

Norman Vadnais – *Independent*

Padgett Peterson – *Lockheed Martin*

Patrick Smith – *Microsoft*

Patty Nicholson – *Microsoft*

Paul Prekeges – *Microsoft*

Raf Cox – *Microsoft*

Ryan Gregg – *Microsoft*

Stacia Snapp – *Microsoft*

Su-Piao Bill Wu – *Microsoft*

Tim Getsch – *Microsoft*

Tom Garity – *Independent*

Travis Ratnam – *Microsoft*

Travis Rhodes – *Microsoft*

Tristan Davis – *Microsoft*

Waqas Nazir – *V-Empower Inc.*

Yuriko Kobayashi – *Microsoft*

Zeyad Rajabi – *Microsoft*

Das United States Department of Commerce National Institute of Standards and Technology (NIST) beteiligte sich ebenfalls an der Prüfung dieses Microsoft-Sicherheitshandbuchs und stellte Anmerkungen zur Verfügung, die in die veröffentlichte Version aufgenommen wurden.

**Testmanager**

Gaurav Singh Bora – *Microsoft*

**Tester**

Harish Ananthapadmaanabhan – *Infosys Technologies Ltd.*

IndiraDevi Chandran – *Infosys Technologies Ltd.*

RaxitKumar Gajjar – *Infosys Technologies Ltd.*

Sumit Parikh – *Infosys Technologies Ltd.*

#### In diesem Beitrag

-   Überblick
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 1](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10))
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 2](https://technet.microsoft.com/de-de/library/b322971a-8efe-40a3-ba33-30a25cae5219(v=TechNet.10))
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 3](https://technet.microsoft.com/de-de/library/f3af8a5d-5067-4add-917b-f7ab8cdca16c(v=TechNet.10))
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 4](https://technet.microsoft.com/de-de/library/2324b4a2-1709-464a-ba66-7413a87d1188(v=TechNet.10))
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 5](https://technet.microsoft.com/de-de/library/30aec6b9-6584-4724-8f8e-46357eecddd6(v=TechNet.10))
-   [Auflistung der Sicherheitseinstellungen für Benutzerrichtlinien – Seite 6](https://technet.microsoft.com/de-de/library/ae3203f0-f0eb-426b-9deb-a1faea298982(v=TechNet.10))
-   [Sicherheitseinstellungen für Computerrichtlinien](https://technet.microsoft.com/de-de/library/e5d2501b-a96b-4c69-b912-59ad22c30503(v=TechNet.10))

**Download**

[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)

[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)

**Update-Benachrichtigungen**

[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)

**Feedback**

[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch,%20bedrohungen%20und%20gegenmaßnahmen:%20sicherheitseinstellungen%20in%202007%20office%20system)

|                                                  |                                                                                                                                                                                             |
|--------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [](#mainsection)[Zum Seitenanfang](#mainsection) | 1 von 8 [![](images/Dd443747.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/2e2c33dc-f4b7-41a4-a54b-1e08dcf57479(v=TechNet.10)) |
