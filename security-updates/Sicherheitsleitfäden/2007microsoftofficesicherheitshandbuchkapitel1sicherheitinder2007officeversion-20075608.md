---
TOCTitle: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 1: Sicherheit in der 2007 Office-Version'
Title: '2007 Microsoft Office-Sicherheitshandbuch: Kapitel 1: Sicherheit in der 2007 Office-Version'
ms:assetid: 'b9767904-ac34-4263-89e7-3c3e82eff607'
ms:contentKeyID: 20075608
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443664(v=TechNet.10)'
---

2007 Microsoft Office-Sicherheitshandbuch
=========================================

### Kapitel 1: Sicherheit in der 2007 Office-Version

Veröffentlicht: 11. Nov 2007

Eine sichere Desktopkonfiguration ist ein wichtiger Bestandteil der tief greifenden Schutzstrategie eines jeden Unternehmens. Doch bevor Sie eine sichere Bereitstellung für die 2007 Microsoft® Office-Version planen und bereitstellen können, müssen Sie sich über Folgendes im Klaren sein:

-   Die zugrunde liegenden Sicherheitsprinzipien, die die Grundlage des Sicherheitsmodells der 2007 Office-Version bilden.
-   Die Neuerungen und Änderungen in der 2007 Office-Version im Hinblick auf die Sicherheit.
-   Welche Sicherheits- und Datenschutzbedrohungen für die 2007 Office-Version relevant sind.
-   Die Merkmale einer sicheren 2007 Office-Umgebung

##### Auf dieser Seite

[Zugrunde liegende Sicherheitsprinzipien](#eyd)
[Neuerungen und Änderungen in der 2007 Office-Version](#eng)
[Risiken und Bedrohungen](#egac)
[Die Merkmale einer sicheren 2007 Office-Umgebung](#egbc)

Zugrunde liegende Sicherheitsprinzipien
---------------------------------------

Vor der 2007 Office-Version brachte eine sichere Office-Konfiguration, mit der sich Unternehmensrisiken einschränken ließen, oft eine erheblich reduzierte Funktionalität mit sich. Die Angriffsfläche für Desktopanwendungen konnte beispielsweise durch Deaktivieren potenziell risikobehafteter Funktionalität wie Microsoft ActiveX®-Steuerelemente, Add-Ins und Microsoft Visual Basic® for Applications (VBA)-Makros minimiert werden, doch hatte dieser Funktionalitätsverlust in der Regel eine verringerte Produktivität und negative Auswirkungen auf die Gesamtleistung des Unternehmens zur Folge.

In einer solchen Situation erlaubten die meisten Unternehmen informationsabhängigen Mitarbeitern, wichtige Sicherheitsentscheidungen selbst zu treffen. Wenn ein Dokument ActiveX-Steuerelemente oder Makros aus einer unbekannten Quelle enthielt, wurden die Benutzer aufgefordert zu entscheiden, ob die Steuerelemente oder Makros aktiviert werden sollten, und konnten erst nach einer Antwort auf das Dokument zugreifen. Dieser Ansatz war zwar nicht perfekt, stellte jedoch einen Mechanismus zum Mindern von Sicherheitsbedrohungen dar, ohne die Anwendungsfunktionalität zu stark einzuschränken. Da Benutzer jedoch Sicherheitswarnungen manchmal nicht ernst nehmen, weil sie zum Ausführen ihrer Arbeit auf Dokumente zugreifen müssen, könnten schädliche ActiveX-Steuerelemente und Makros aktiviert werden und dem Unternehmen möglicherweise Schaden zufügen.

Das allgemeine Sicherheitsmodell für die 2007 Office-Version wurde daher auf Grundlage der folgenden vier Hauptprinzipien konzipiert:

-   Bereitstellen einer sichereren Standardanwendungsfunktionalität.
-   Minimieren der Anzahl wichtiger Sicherheitsentscheidungen, wann immer möglich, und Bereitstellen leicht verständlicher Informationen zur Entscheidungsfindung für Benutzer.
-   Aufrechterhalten der Benutzerproduktivität durch Minderung von Bedrohungen ohne wesentliche Beeinträchtigung der Anwendungsfunktionalität.
-   Bereitstellen eines flexiblen Sicherheitsmodells, das an bestimmte Situationen angepasst und mithilfe gängiger Branchenpraktiken und -tools dynamisch gesteuert werden kann.

Diese Prinzipien bilden die Grundlage für die Sicherheitsziele der 2007 Office-Version – ein Maximieren von Schutz und Produktivität und ein Minimieren der Gesamtbetriebskosten.

### Funktionalität ist standardmäßig sicherer

Sicherheit hat in der 2007 Office-Version hohe Priorität. Es soll gewährleistet werden, dass die zugrunde liegenden Technologien des Produkts widerstandsfähig gegen Angriffe sind und die Standardkonfiguration der Anwendungen sicherer gestaltet ist als bei früheren Versionen von Microsoft Office.

Dieses Prinzip berücksichtigt die Tatsache, dass manche Funktionen zwar nützlich sind, aber potenziell von böswilligen Benutzern oder schädlichem Code ausgenutzt werden könnten. Auch können einige Funktionen unachtsame Benutzer möglicherweise dazu verleiten, unvorsichtig vorzugehen. Bei der Konfiguration vieler dieser Funktionen ist Schutz vor Angriffen ein wichtigerer Gesichtspunkt als Funktionalität.

Dokumente und E-Mail-Nachrichten enthalten beispielsweise oft verknüpfte Bilder, die auf Remotecomputern gespeichert sind. Diese Funktionalität ermöglicht ein einfaches Aktualisieren von Bildern und reduziert die Größe von Dokumenten und E-Mail-Nachrichten, sodass weniger Datenträgerspeicher und Netzwerkbandbreite erforderlich sind. Allerdings können Personen, die Spam-E-Mails senden, sowie andere Angreifer verknüpfte Bilder (so genannte Webbeacons) verwenden, um die Gültigkeit von E-Mail-Adressen zu bestätigen oder IP-Adressen von Computern zu erlangen. Daher sind verknüpfte Bilder in der 2007 Office-Version standardmäßig blockiert. Die Benutzer können trotzdem E-Mail-Nachrichten und Dokumente öffnen, die verknüpfte Bilder enthalten – der Zugriff auf den Text ist nicht eingeschränkt. Diese Funktionalität maximiert sowohl den Schutz vor Angriffen als auch die Produktivität.

### Minimieren der Behinderung von Benutzern

Vorherige Sicherheitsmodelle verließen sich zwar auf den Benutzer, um Risiken abzuschätzen und potenzielle Sicherheitsbedrohungen zu mindern, das Prinzip der 2007 Office-Version ist es jedoch, dass Benutzer so wenige Sicherheitsentscheidungen wie möglich treffen sollten. Dieses Prinzip wirkt sich in drei wichtigen Punkten darauf aus, wie Sicherheitsbedrohungen durch Benutzer und Anwendungen gehandhabt werden:

-   Die Anzahl sicherheitsbezogener Entscheidungen durch den Benutzer wird reduziert.
-   In Fällen, in denen aufgrund einer Sicherheitsbedrohung ein erhöhtes Risiko vorliegt und ein Benutzereingriff unbedingt erforderlich ist, enthält die Warnmeldung verständliche Informationen, die der Benutzer benötigt, um eine Entscheidung zu treffen.
-   In Fällen, in denen eine Benutzeraktion erforderlich ist, werden Eingabeaufforderungen und Informationen zu einem Zeitpunkt und in einem Kontext angezeigt, der für Benutzer am sinnvollsten ist. Beispielsweise müssen Benutzer nicht mehr jedes Mal auf Sicherheitseingabeaufforderungen reagieren, wenn sie ein Dokument öffnen, das Makros aus einer nicht vertrauenswürdigen oder unbekannten Quelle enthält. Obwohl Makros aus nicht vertrauenswürdigen oder unbekannten Quellen standardmäßig automatisch deaktiviert werden, erfordert der Benachrichtigungsprozess keine Sicherheitsentscheidung von Seiten des Benutzers, bevor dieser an dem Dokument arbeiten kann. Stattdessen werden Makrobenachrichtigungen in einem Infobereich (der so genannten „Statusleiste“) am oberen Rand des Dokuments angezeigt. Die Benutzer können auf die Statusleiste klicken, um die Benachrichtigungen zu lesen und Makros zu aktivieren. Außerdem enthält die Benachrichtigung Informationen und Gründe für das Sicherheitsrisiko und informiert den Benutzer, wie sich die Bedrohung mindern lässt.

### Aufrechterhalten der Benutzerproduktivität

Das Aufrechterhalten der Benutzerproduktivität ist ein weiteres wichtiges Prinzip des Sicherheitsmodells der 2007 Office-Version. Wenn Benutzer in der Vergangenheit ein Dokument öffnen wollten, das eine potenzielle Sicherheitsbedrohung enthielt (z. B. ein Makro oder ein ActiveX-Steuerelement), konnten sie erst mit der Datei arbeiten, nachdem sie auf eine Sicherheitswarnung reagiert hatten. In der 2007 Office-Version können Benutzer sofort auf Dokumente zugreifen und mit ihnen arbeiten. Die Benutzer werden nur dann zu einer Aktion aufgefordert, wenn zum Aufrechterhalten einer sicheren Arbeitsumgebung ein Benutzereingriff erforderlich ist.

Eine neue Sicherheitsfunktion namens „Vertrauenswürdige Speicherorte“ hilft dem Benutzer beispielsweise bei der Unterscheidung zwischen Dokumenten, die aus vertrauenswürdigen Quellen stammen (z. B. digital signierte Dokumente von Kollegen oder Geschäftspartnern), und Dokumenten, bei denen dies nicht der Fall ist.

An einem vertrauenswürdigen Speicherort abgelegte Dokumente werden als sicher eingestuft und können bedenkenlos geöffnet werden. Der gesamte Inhalt eines vertrauenswürdigen Dokuments wird ohne zusätzliche Sicherheitsüberprüfungen aktiviert. Benutzer müssen weder auf Sicherheitswarnungen reagieren noch in einem vertrauenswürdigen Dokument Inhalte aktivieren, um ihre Arbeit ausführen zu können – die Produktivität wird also nicht beeinträchtigt.

Der gesamte aktive Inhalt in Dokumenten, die nicht an einem vertrauenswürdigen Speicherort abgelegt sind, wird standardmäßig deaktiviert. Benutzer können solche Dokumente zwar öffnen und daran arbeiten, müssen aber auf die Benachrichtigung reagieren, um den risikobehafteten Inhalt dieser Dokumente zu aktivieren. Die Produktivität wird bei solchen Dokumenten also nur beeinträchtigt, wenn der Benutzer risikobehaftete Inhalte aktivieren möchte.

### Bereitstellen eines verwaltbaren und flexiblen Sicherheitsmodells

Bei diesem Prinzip wird berücksichtigt, dass das Standardsicherheitsmodell nicht für jede Computerumgebung oder für jeden Benutzer geeignet ist. Trotz der ersten drei Prinzipien gibt es Fälle, in denen Benutzer nicht auf Inhalte mit geringem Risiko zugreifen können, ohne zuerst auf eine Sicherheitsbenachrichtigung oder -warnung reagieren zu müssen. Um die Ziele der ersten drei Prinzipien besser umsetzen zu können, bietet die 2007 Office-Version eine Suite von Sicherheitseinstellungen, mit denen sich das Standardsicherheitsmodell ändern lässt. Diese Fähigkeit ist ebenfalls wichtig, um auf die ständigen Änderungen in der Bedrohungslandschaft reagieren zu können. Durch die Flexibilität zur schnellen Anpassung der Systemsicherheit Ihrer Umgebung können Sie neuen Bedrohungen effektiv begegnen. Mithilfe dieses verwaltbaren und flexiblen Sicherheitsmodells können Sie Sicherheitseinstellungen konfigurieren und die Umgebungen für Unternehmensclients (Enterprise Client, EC) und Hochsicherheit (Specialized Security - Limited Functionality, SSLF) einrichten, die in Kapitel 5 dieses Handbuchs beschrieben werden.

[](#mainsection)[Zum Seitenanfang](#mainsection)

Neuerungen und Änderungen in der 2007 Office-Version
----------------------------------------------------

Anhand der oben aufgeführten vier Hauptprinzipien wurde für die 2007 Office-Version ein neues Sicherheitsmodell entwickelt. Dieses Sicherheitsmodell enthält neue Funktionen, neue Einstellungen und neue Funktionalität. Außerdem kann das neue Sicherheitsmodell beeinflussen, wie Benutzer auf Risiken in ihren individuellen Arbeitsumgebungen reagieren und wie Administratoren Sicherheitsbedrohungen innerhalb des gesamten Unternehmens mindern und verwalten. Zu den Hauptänderungen im neuen Sicherheitsmodell gehören folgenden Elemente:

-   **Die Benutzeroberfläche**. Die aktualisierte Benutzeroberfläche hilft Benutzern, Sicherheitseinstellungen anzuzeigen und zu konfigurieren sowie auf Sicherheitswarnungen und -benachrichtigungen zu reagieren. Das Grundprinzip ist Transparenz und Einfachheit: Dem Benutzer sollen zeitgerechte, klare und kontextbezogene Informationen bereitgestellt werden, die Informationen zur Entscheidung und den möglichen Folgen enthalten, wobei die verschiedene Optionen deutlich und verständlich dargestellt sein sollten.
-   **Administrative Einstellungen und Funktionen**. Mithilfe dieser Einstellungen und Funktionen können IT-Experten sichere Desktopkonfigurationen entwerfen und implementieren, durch die Sicherheitsbedrohungen effektiver gemindert werden.
-   **Standardfunktionalität**. Die Standardeinstellungen tragen zur Benutzerproduktivität bei, helfen aber gleichzeitig, die Unternehmensressourcen zu schützen und Sicherheitsbedrohungen zu mindern.

### Änderungen an der Benutzeroberfläche

Die sicherheitsbezogenen Änderungen an der Benutzeroberfläche der 2007 Office-Version lassen sich in drei Kategorien einteilen:

-   Die meisten anwendungsspezifischen Sicherheitseinstellungen und Datenschutzoptionen werden jetzt an einem einzigen Speicherort angezeigt, dem so genannten Vertrauensstellungscenter.
-   Manche Einstellungen für den Dokumentschutz werden jetzt zusammen mit anderen Einstellungen zur Dokumentvorbereitung angezeigt, z. B. „Speichern“ und „Drucken“.
-   Die meisten Sicherheitswarnungen und -benachrichtigungen werden jetzt im neuen Infobereich namens „Statusleiste“ angezeigt.

Diese Änderungen an der Benutzeroberfläche sorgen für eine verbesserte Benutzerfreundlichkeit, da die Benutzer Sicherheitseinstellungen einfacher finden, anzeigen und konfigurieren sowie Sicherheitsbedrohungen ohne Auswirkungen auf die Produktivität handhaben können.

### Vertrauensstellungscenter

Das Vertrauensstellungscenter ist eine zentrale Konsole, über die Benutzer Sicherheitseinstellungen und Datenschutzoptionen anzeigen und konfigurieren können. Einige der Einstellungen in der Vertrauensstellungscenter-Konsole gelten für mehrere 2007 Office-Anwendungen, die meisten jedoch gelten lediglich für die Anwendung, von der aus das Vertrauensstellungscenter geöffnet wurde. Dadurch sind völlig neue Steuerungsmöglichkeiten verfügbar: Die Sicherheit kann auf Anwendungsbasis angepasst werden, sodass gewünschte Funktionen in bestimmten Anwendungen zugelassen, in anderen dagegen eingeschränkt werden. Das Vertrauensstellungscenter ist im folgenden Bildschirmfoto abgebildet.

![](images/Dd443664.929eeef6-ac42-4a3d-9f09-d1b9b4409c01(de-de,TechNet.10).gif)

**Abbildung 1.1. Vertrauensstellungscenter der 2007 Office-Version**

Die Benutzer können im Vertrauensstellungscenter die folgenden Einstellungen konfigurieren:

-   **Vertrauenswürdige Herausgeber und vertrauenswürdige Speicherorte**. Mit diesen Einstellungen lässt sich sicherer Inhalt festlegen, z. B. Dateien, die sichere ActiveX-Steuerelemente, Add-Ins und VBA-Makros enthalten.
-   **ActiveX-Steuerelemente, Add-Ins und VBA-Makros**. Mit diesen Einstellungen lässt sich die Funktionalität von ActiveX-Steuerelementen, Add-Ins und Makros aus unsicheren oder nicht überprüfbaren Quellen steuern.
-   **Statusleiste und Datenschutzoptionen**. Mit diesen Einstellungen können die Benachrichtigungsfunktionalität sowie die Behandlung persönlicher oder privater Informationen in den einzelnen Anwendungen gesteuert werden.
-   **Externer Inhalt**. Mithilfe dieser Einstellungen wird in Microsoft Office Excel® 2007 die Datenverbindungsfunktionalität gesteuert.

Zum Zugriff auf das Vertrauensstellungscenter in den 2007-Versionen von Microsoft Office Access™, Excel, PowerPoint® und Word klicken Benutzer auf die **Office-Schaltfläche** und anschließend auf *&lt;Programm&gt;***-Optionen**, wobei *&lt;Programm&gt;* das aktuell ausgeführte Programm darstellt. In den 2007-Versionen von Microsoft Office InfoPath® und Outlook® klicken Benutzer im Menü **Extras** auf **Vertrauensstellungscenter**.

#### Steuerelemente für den Dokumentschutz

Obwohl das Vertrauensstellungscenter die meisten anwendungsspezifischen Sicherheitseinstellungen und Datenschutzoptionen enthält, wurden bestimmte dokumentspezifische Sicherheitseinstellungen absichtlich nicht im Vertrauensstellungscenter aufgenommen, darunter Einstellungen zum Dokumentschutz, mit denen Benutzer Dokumente verschlüsseln können. Da Dokumentschutzeinstellungen beim Speichern oder Senden von Dokumenten zum Einsatz kommen, befinden sich diese Einstellungen am selben Ort wie andere Dokumentvorbereitungseinstellungen. Zum Zugriff auf Einstellungen für die Dokumentvorbereitung klicken Benutzer auf die **Office-Schaltfläche** und anschließend auf **Vorbereiten**.

#### Statusleiste

Die Statusleiste ist eine neue Funktion der Benutzeroberfläche, in der Benutzern beim Öffnen eines Dokuments mit möglicherweise schädlichem Inhalt Benachrichtigungen und Warnungen angezeigt werden. Die Statusleiste ist im folgenden Bildschirmfoto abgebildet.

![](images/Dd443664.296c6c90-9b11-4c52-acfb-43528024a764(de-de,TechNet.10).gif)

**Abbildung 1.2. Statusleiste der 2007 Office-Version**

![](images/Dd443664.note(de-de,TechNet.10).gif)**Hinweis:**
In Office Outlook 2007 und Office Publisher 2007 werden Sicherheitswarnungen in Dialogfeldern und nicht in der Statusleiste angezeigt.

Die Statusleiste informiert Benutzer darüber, dass bestimmte Funktionen in einem Dokument blockiert sind. In früheren Versionen von Microsoft Office wurde den Benutzern in der Regel ein Warnungsdialogfeld angezeigt, auf das sie vor dem Arbeiten in einem Dokument reagieren mussten. Wenn ein Benutzer beispielsweise ein Dokument öffnete, das Makros enthielt, konnte er erst auf das Dokument zugreifen, nachdem er auf ein Warnungsdialogfeld reagiert und die Makros entweder aktiviert oder deaktiviert hatte. Die Statusleiste ermöglicht Benutzern jetzt, ein Dokument zu öffnen und darin zu arbeiten, ohne auf die Statusleistenaufforderung zu reagieren. Nicht vertrauenswürdige ActiveX-Steuerelemente, Makros und andere potenziell schädliche Inhalte sind so lange deaktiviert, bis der Benutzer auf die Statusleiste klickt und auf eine Benachrichtigung oder Warnung reagiert. Das folgende Bildschirmfoto enthält ein Beispiel für eine Warnmeldung, die Benutzern beim Klicken auf die Statusleiste anzeigt wird.

![](images/Dd443664.46e5bd61-843a-4c4e-9738-ad66d407d1dc(de-de,TechNet.10).gif)

**Abbildung 1.3. Statusleisten-Warnmeldung in der 2007 Office-Version**

### Änderungen an administrativen Einstellungen und Funktionen

Die 2007 Office-Version enthält neue und verbesserte Einstellungen und Funktionen, zum Beispiel:

-   Eine neue Gruppe von Einstellungen namens „Vertrauenswürdige Speicherorte“
-   Änderungen an der Verwaltung von ActiveX-Steuerelementen, Add-Ins und Makros
-   Eine neue Gruppe von Einstellungen zum Blockieren von Dateiformateinstellungen
-   Ein neues Tool namens „Dokumentinspektor“

In den folgenden Abschnitten werden diese neuen und verbesserten Einstellungen und Funktionen näher beschrieben.

#### Einstellungen für vertrauenswürdige Speicherorte

Einstellungen für vertrauenswürdige Speicherorte ermöglichen ein Unterscheiden zwischen Dokumenten aus einer oder mehreren vertrauenswürdigen Quellen. Bei Angabe eines vertrauenswürdigen Speicherorts, z. B. ein Ordner auf der Festplatte des Benutzers oder eine gut verwaltete und sichere Dokumentfreigabe im Netzwerk, wird beim Öffnen eines Dokuments, das in diesem vertrauenswürdigen Speicherort abgelegt ist, der gesamte Dokumentinhalt aktiviert und initialisiert, einschließlich ActiveX-Steuerelemente, externe Verknüpfungen und Makros. Außerdem werden in der Statusleiste oder der Benutzeroberfläche keinerlei Eingabeaufforderungen oder Warnungen angezeigt, wenn Dokumente aus vertrauenswürdigen Speicherorten geöffnet werden.

![](images/Dd443664.caution(de-de,TechNet.10).gif)  **Vorsicht:**

Dokumente, die aus vertrauenswürdigen Speicherorten geöffnet werden, stellen für das Unternehmen ein größeres Risiko dar als Dokumente aus nicht vertrauenswürdigen Speicherorten. Die Benutzer sollten daher bei der Entscheidung, welche Dokumente in vertrauenswürdigen Speicherorten gespeichert werden, äußerst vorsichtig vorgehen.

Um zu verhindern, dass ein vertrauenswürdiger Speicherort für böswillige Zwecke und zum Ausführen von schädlichem Code erstellt wird, ermöglichen es die Standardeinstellungen in der 2007 Office-Version Benutzern nicht, Remoteordner als vertrauenswürdige Speicherorte festzulegen. Standardmäßig dürfen sich vertrauenswürdige Speicherorte nur lokal auf der Festplatte des Benutzers befinden. Außerdem können vertrauenswürdige Speicherorte im Fall eines Sicherheitsangriffs leicht gesperrt werden. Weiterhin wird in der 2007 Office-Version dauerhaft verhindert, dass Benutzer bestimmte risikobehaftete Ordner als vertrauenswürdige Speicherorte festlegen, darunter der Office Outlook 2007-Zwischenspeicher für Anlagen, temporäre Ordner sowie andere Ordner, in denen Dokumente temporär gespeichert werden.

Manche Unternehmen nutzen diese Fähigkeit, um Benutzern bestimmte Dokumente, die sicher sind und Makros bzw. ActiveX-Steuerelemente enthalten, zur Verfügung zu stellen und gleichzeitig Dokumente aus anderen Quellen, die diese Elemente enthalten, zu blockieren (z. B. Dokumentanlagen). Durch diese Fähigkeit lässt sich die Funktionalität bereitstellen, die für bestimmte Aktivitäten erforderlich ist, und die Umgebung trotzdem vor potenziellen Bedrohungen schützen. Wenn ein Remotespeicherort (beispielsweise eine Netzwerkfreigabe) in einem solchen Szenario verwendet wird, muss der Server unbedingt sicher und angemessen verwaltet werden, damit nur bekannte und vertrauenswürdige Dokumente dort abgelegt werden.

#### Einstellungen für ActiveX-Steuerelemente, Add-Ins und Makros

In der 2007 Office-Version können Sie die Funktionsweise von ActiveX-Steuerelementen, Add-Ins und Makros durch Konfigurieren globaler oder anwendungsspezifischer Einstellungen verwalten. In der Vergangenheit konnten Sicherheitsbedrohungen durch Makros mithilfe einer von nur vier globalen Einstellungen gemindert werden: „Niedrig“, „Mittel“, „Hoch“ und „Sehr Hoch“ Jede dieser Einstellungen entsprach einer jeweils immer eingeschränkteren Sicherheitssituation. Die Einstellung „Niedrig“ ermöglichte Benutzern ein Ausführen aller Makros, die Einstellung „Hoch“ lediglich das Ausführen von Makros, die von einem vertrauenswürdigen Hersteller signiert waren. Außerdem gab es keine globalen oder anwendungsspezifischen Einstellungen zum Verwalten von ActiveX-Steuerelementen (abgesehen von Änderungen an der Registrierung), und es standen keine anwendungsspezifischen Sicherheitseinstellungen zum Verwalten von Add-Ins zur Verfügung. Das neue Modell dagegen bietet Transparenz und Spezifizität: Sie verstehen genau, was für jeden Technologietyp aktiviert wird, und können die Funktionalität auswählen, die Ihrer Sicherheitsarchitektur und Ihren Nutzbarkeitszielen entsprechen.

##### Einstellungen für ActiveX-Steuerelemente

Zum Steuern der ActiveX-Steuerelementfunktion gibt es eine Reihe neuer Einstellungen. Die folgenden Optionen stehen zur Auswahl:

-   **Alle ActiveX-Steuerelemente deaktivieren**. Verhindert das Laden aller ActiveX-Steuerelemente und benachrichtigt die Benutzer nicht darüber, dass ActiveX-Steuerelemente deaktiviert sind. Die einzige Ausnahme bilden ActiveX-Steuerelemente, die in Dokumenten aus vertrauenswürdigen Speicherorten enthalten sind.
-   **ActiveX-Steuerelementinitialisierung konfigurieren**. Legt auf Grundlage der Parameter SFI (Safe for Initialization) und UFI (Unsafe for Initialization) fest, wie ActiveX-Steuerelemente geladen werden. Wie bereits oben erwähnt, wurde diese Einstellung in der Vergangenheit mithilfe von Änderungen an der Registrierung konfiguriert. In der 2007 Office-Version wird diese Einstellung mithilfe administrativer Vorlagen (ADM- oder ADMX-Dateien) konfiguriert.
-   **ActiveX-Eingabeaufforderungen konfigurieren**. Gibt an, welche Art von Aufforderungen der Benutzer erhält, wenn ActiveX-Steuerelemente geladen werden. Diese Einstellung kann so konfiguriert werden, dass der Benutzer beim Ladeversuch eines ActiveX-Steuerelements entweder eine Eingabeaufforderung erhält oder nicht.

##### Einstellungen für Add-Ins

Im Vergleich zu Microsoft Office 2003 verfügt die 2007 Office-Version nicht über eine Einstellung, mit der alle installierten Add-Ins und Vorlagen als vertrauenswürdig eingestuft werden können. Stattdessen gibt es eine Reihe neuer Einstellungen zum Steuern der Funktionalität von Add-Ins, zum Beispiel:

-   **Alle Anwendungs-Add-Ins deaktivieren (möglicherweise Funktionsbeeinträchtigung)**. Verhindert ein Ausführen aller Add-Ins. Der Benutzer wird nicht benachrichtigt, dass Add-Ins deaktiviert sind.
-   **Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein**. Prüft die Datei, die das Add-In enthält, auf eine digitale Signatur. Wenn es sich nicht um einen vertrauenswürdigen Herausgeber handelt, lädt das Programm das Add-In nicht, und in der Statusleiste wird eine Benachrichtigung angezeigt, dass das Add-In deaktiviert wurde.
-   **Benachrichtigung für Vertrauensstellungsleiste für nicht signierte Anwendungs-Add-Ins deaktivieren (Code bleibt deaktiviert)**. Diese Einstellung kann nur aktiviert sein, wenn Sie ebenfalls **Anwendungs-Add-Ins müssen von einem vertrauenswürdigen Herausgeber signiert sein** aktivieren. Manchmal sind Dateien, die ein Add-In enthalten, nicht signiert. Wenn diese Einstellung aktiviert ist, werden von vertrauenswürdigen Herausgebern signierte Add-Ins aktiviert, und unsignierte Add-Ins werden ohne Benachrichtigung des Benutzers deaktiviert.

##### Makros

Zum Steuern der Makrofunktionalität stehen mehrere neue Einstellungen zur Verfügung. Mithilfe dieser Einstellungen lassen sich Makros auf folgende Weise steuern:

-   **Visual Basic for Applications deaktivieren**. Deaktiviert Visual Basic for Applications für alle 2007 Office-Anwendungen
-   **Einstellungen für Makrowarnungen konfigurieren**. Legt die Bedingungen fest, unter denen Benutzer über Makros benachrichtigt werden. Die folgenden vier Optionen sind verfügbar:
    -   Benachrichtigungen über Makros immer anzeigen.
    -   Benachrichtigungen über digital signierte Makros immer anzeigen und nicht signierte Makros deaktivieren.
    -   Keine Benachrichtigung anzeigen und alle Makros deaktivieren.
    -   Keine Sicherheitsüberprüfungen durchführen und Ausführung aller Makros zulassen.
-   **Bestimmen, ob das Überprüfen verschlüsselter Makros in Microsoft Office Open XML-Dokumenten erzwungen wird**. Legt fest, dass für verschlüsselte Dateien im neuen Office Open XML-Format Makrosicherheitsüberprüfungen durchgeführt werden. Diese Einstellung kann nur über administrative Vorlagen konfiguriert werden (ADM- oder ADMX-Dateien). Ein Konfigurieren in der Benutzeroberfläche ist nicht möglich. Außerdem ist diese Einstellung standardmäßig aktiviert. Verschlüsselte Makros in Dokumenten im Office Open XML-Format werden also standardmäßig überprüft.

#### Einstellungen zum Blockieren von Dateiformaten

Eine Reihe neuer Einstellungen ermöglichen es, Benutzer am Öffnen oder Speichern bestimmter Dateitypen in den 2007-Versionen von Office Excel, PowerPoint und Word zu hindern. Diese Einstellungen sind nützlich, wenn Sie die Verwendung bestimmter Dateiformate im Unternehmen erzwingen oder Sicherheitsbedrohungen mindern möchten. Mit den Einstellungen zum Blockieren von Dateiformaten können Sie Folgendes erreichen:

-   Verringern von Zero-Day-Angriffen und Exploits, bis eine Lösung vorliegt
-   Benutzer am Öffnen oder Speichern bestimmter Dateiformate hindern
-   Benutzer am Öffnen von Dateien hindern, die mit früheren Versionen von Office Excel, PowerPoint und Word kompatibel sind
-   Benutzer am Öffnen von Dokumenten über externe Konverter hindern, z. B. den mit der 2007 Office-Version installierten WordPerfekt-Konverter
-   Benutzer am Öffnen von Dateiversionen hindern, die mit Vorabversionen (Betaversionen) von Anwendungsprogrammen erstellt wurden

#### Dokumentinspektor

Bei Dokumentinspektor handelt es sich um ein Tool, mit dem sich vertrauliche und ausgeblendete Informationen aus Dokumenten entfernen lassen, etwa persönliche Daten und Dokumenteigenschaften. Dokumentinspektor ist standardmäßig in den 2007-Versionen von Office Excel, PowerPoint und Word verfügbar, jedes Programm verwendet aber einen unterschiedlichen Satz an Inspektormodulen für das Entfernen unterschiedlicher Inhalte. Office Excel 2007 beispielsweise enthält ein Inspektormodul, mit dem ausgeblendete Arbeitsblätter entfernt werden können. Office Word 2007-Dokumente und Office PowerPoint  2007-Präsentationen unterstützen keine ausgeblendeten Arbeitsblätter, daher enthalten diese Anwendungen das entsprechende Modul nicht.

Benutzer können die Art von Inhalt angeben, die aus den Dateien entfernt werden soll, zum Beispiel:

-   Dokumenteigenschaften und persönliche Informationen (Metadaten)
-   Kommentare, Überarbeitungsmarkierungen, Versionsinformationen und Freihandanmerkungen
-   Kopfzeilen, Fußzeilen und Wasserzeichen
-   Ausgeblendeten Text
-   Ausgeblendete Zeilen, Spalten und Arbeitsblätter
-   Nicht sichtbarer Inhalt
-   Externer Folieninhalt
-   Präsentationsnotizen
-   Dokumentservereigenschaften
-   Benutzerdefinierte XML-Daten

Inspektormodule können aktiviert bzw. deaktiviert werden, es gibt allerdings keine administrativen Einstellungen, mit denen sich die Arbeitsweise einzelner Inspektormodule verwalten lässt. Sie können jedoch programmgesteuert benutzerdefinierte Inspektormodule erstellen.

### Änderungen an der Standardfunktionalität

In der 2007 Office-Version wurden eine Reihe von Standardsicherheitseinstellungen geändert. Diese Änderungen werden in den folgenden Abschnitten beschrieben.

#### Dokumente werden immer geöffnet

Wenn ein Benutzer versucht, ein Dokument mit potenziell schädlichem Inhalt wie nicht vertrauenswürdigen ActiveX-Steuerelementen und Makros oder Verknüpfungen zu nicht vertrauenswürdigen externen Quellen zu öffnen, wird das Dokument geöffnet, wobei der nicht vertrauenswürdige Inhalt deaktiviert ist. Es erfolgt eine Benachrichtigung an den Benutzer, dass Inhalte blockiert wurden. In früheren Versionen von Microsoft Office wurde das Öffnen solcher Dokumente in der Regel blockiert, bis der Benutzer eine Entscheidung traf, ob der nicht vertrauenswürdige Inhalt aktiviert werden sollte.

#### Externer Inhalt wird blockiert

2007 Office-Anwendungen blockieren den Zugriff auf potenziell gefährlichen externen Inhalt standardmäßig. Beispielsweise werden Office PowerPoint 2007-Dokumentverknüpfungen zu Bildern auf externen Netzwerken und Office Excel 2007-Daten blockiert. Wenn solche Verknüpfungen oder Verbindungen vorhanden sind, wird in der Statusleiste eine Benachrichtigung angezeigt. Wenn Benutzer auf die Statusleiste klicken, werden sie gefragt, ob sie den externen Inhalt aktivieren möchten.

Benutzer, die andere Office 2007-Dokumente öffnen, erhalten Sicherheitswarnungen, bevor sie auf möglicherweise gefährlichen externen Inhalt zugreifen. Wenn ein Benutzer zum Beispiel auf Links, die potenziell unsichere Protokolle verwenden, oder auf Verknüpfungen zu anderen Office-Dokumenten und ausführbaren Dateien klickt, wird ein Dialogfeld mit einer Sicherheitswarnung angezeigt.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Der externe Inhalt von Dokumenten in vertrauenswürdigen Speicherorten ist aktiviert.

#### ActiveX-Steuerelemente können unter bestimmten Umständen ausgeführt werden

Für die Funktionalität von ActiveX-Steuerelementen gibt es vier Standardoptionen. Diese Optionen hängen von den Merkmalen des jeweiligen ActiveX-Steuerelements und den Merkmalen des Dokuments ab, das das ActiveX-Steuerelement enthält.

-   Wenn in der Registrierung für ein ActiveX-Steuerelement ein Kill Bit eingerichtet ist, wird das Steuerelement nicht geladen und kann unter keinen Umständen geladen werden. Ein Kill Bit ist eine Funktion, mit der verhindert wird, dass Steuerelemente mit bekannten Exploits geladen werden. Weitere Informationen finden Sie im Knowledge Base-Artikel [So verhindern Sie die Ausführung von ActiveX-Steuerelementen in Internet Explorer.](http://support.microsoft.com/kb/240797)
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das kein VBA-Projekt enthält, und das ActiveX-Steuerelement als „Sicher für Initialisierung“ (Safe for Initialization, SFI) gekennzeichnet ist, wird das ActiveX-Steuerelement unter minimalen Einschränkungen geladen. Die Stausleiste wird nicht angezeigt, und der Benutzer wird nicht über das Vorhandensein von ActiveX-Steuerelementen in den Dokumenten informiert. Die ActiveX-Steuerelemente im Dokument müssen alle als SFI gekennzeichnet sein, damit keine Benachrichtigung ausgegeben wird.
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das kein VBA-Projekt enthält, und das ActiveX-Steuerelement als unsicher für die Initialisierung (Unsafe for Initialization, UFI) gekennzeichnet ist, wird der Benutzer in der Statusleiste darüber informiert, dass ein ActiveX-Steuerelement deaktiviert wurde. Wenn der Benutzer auf die Statusleiste klickt, wird ein Dialogfeld angezeigt, in dem der Benutzer das ActiveX-Steuerelement aktivieren kann. Wenn der Benutzer das ActiveX-Steuerelement aktiviert, werden alle ActiveX-Steuerelemente im Dokument (als SFI und UFI gekennzeichnete) unter minimalen Einschränkungen geladen.
-   Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das auch ein VBA-Projekt enthält, wird der Benutzer über die Statusleiste darüber informiert, dass ein ActiveX-Steuerelement deaktiviert wurde. Wenn der Benutzer auf die Statusleiste klickt, wird ein Dialogfeld angezeigt, in dem der Benutzer das ActiveX-Steuerelement aktivieren kann. Wenn der Benutzer das ActiveX-Steuerelement aktiviert, werden alle ActiveX-Steuerelemente im Dokument (als SFI und UFI gekennzeichnete) unter minimalen Einschränkungen geladen.

![](images/Dd443664.note(de-de,TechNet.10).gif) **Hinweis:**

Wenn ein ActiveX-Steuerelement in einem Dokument enthalten ist, das in einem vertrauenswürdigen Speicherort abgelegt ist, wird das ActiveX-Steuerelement standardmäßig aktiviert, und der Benutzer erhält keine Eingabeaufforderung zur Aktivierung.

#### Installierte und registrierte Add-Ins können ausgeführt werden

Standardmäßig kann jedes installierte und registrierte Add-In ohne Benutzereingriff oder Warnung ausgeführt werden. Zu installierten und registrierten Add-Ins zählen beispielsweise die folgenden:

-   COM-Add-Ins (Component Object Model)
-   Smarttags
-   Automatisierungs-Add-Ins
-   RTD-Server (RealTimeData)
-   Anwendungs-Add-Ins (zum Beispiel WLL, XLL- und XLAM-Dateien)
-   XML-Erweiterungspakete
-   XML-Stylesheets

Diese Standardkonfiguration entspricht der Einstellung „Allen installierten Add-Ins und Vorlagen vertrauen“, die standardmäßig in Microsoft Office 2003 aktiviert ist.

#### Nur vertrauenswürdige Makros können ausgeführt werden

Standardmäßig können vertrauenswürdige Makros ausgeführt werden, einschließlich von Makros in Dokumenten, die in vertrauenswürdigen Speicherorten abgelegt sind, und solchen, die die folgenden Kriterien erfüllen:

-   Das Makro wurde vom Entwickler mit einer digitalen Signatur versehen.
-   Die digitale Signatur ist gültig.
-   Die digitale Signatur ist aktuell (nicht abgelaufen).
-   Das mit der digitalen Signatur verbundene Zertifikat wurde von einer anerkannten Zertifizierungsstelle (Certification Authority, CA) ausgestellt.
-   Das mit der digitalen Signatur verbundene Zertifikat ist in der Liste vertrauenswürdiger Herausgeber auf dem Computer des Benutzers gespeichert.

Nicht vertrauenswürdige Makros können nicht ausgeführt werden, bis Benutzer auf die Statusleiste klicken und auswählen, das Makro zu aktivieren. In der Vergangenheit wurden unsignierte Makros deaktiviert, und die Benutzer hatten keine Möglichkeit, diese zu aktivieren. Diese Funktionalität hat sich in der 2007 Office-Version geändert, da der Benutzer benachrichtigt wird, wenn Dokumente unsignierte Makros enthalten, und diese dann aktivieren kann.

[](#mainsection)[Zum Seitenanfang](#mainsection)

Risiken und Bedrohungen
-----------------------

Mithilfe der neuen, verbesserten Sicherheitsfunktionen in der 2007 Office-Version können Sie vielfältige Sicherheitsstrategien entwickeln. Für eine gezielte und effektive Sicherheitsstrategie müssen jedoch die Risiken verstanden werden, denen ein Unternehmen möglicherweise ausgesetzt ist, sowie die Bedrohungen und Angriffsmethoden, die diese Risiken ausnutzen.

### Datensicherheitsrisiken

Aus der Perspektive eines IT-Experten stellen sich Risiken für die Datensicherheit normalerweise als Vertraulichkeitsrisiken, Integritätsrisiken und Verfügbarkeitsrisiken dar. (Diese Risiken werden in der Übersicht dieses Handbuchs beschrieben.)

Standardmäßig trägt das 2007 Office-Modell zur Risikominderung aller drei Risikoarten in Ihrem Unternehmen bei. Die Infrastruktur sowie die Anforderungen in den Bereichen Produktivität und Desktopsicherheit unterscheiden sich jedoch von Unternehmen zu Unternehmen. Um genau zu bestimmen, wie Ihr Unternehmen diese Unternehmensrisiken verringern kann, müssen Sie die Bedrohungen und Angriffsmethoden evaluieren, die diese Risiken ausnutzen.

### Bedrohungen für Desktopproduktivitätsanwendungen

Mithilfe des Sicherheitsmodells der 2007 Office-Version können Sie fünf Arten von Sicherheitsbedrohungen für Produktivitätssoftware mindern. Jeder dieser Bedrohungstypen umfasst verschiedene Angriffsmethoden und kann über eine Vielzahl von Sicherheitsangriffen ausgenutzt werden. Die folgende Abbildung zeigt Sicherheitsbedrohungen und Beispiele für die gängigsten Angriffsmethoden.

![](images/Dd443664.f7ecec0c-ddcb-44f3-864c-b2685bc74daa(de-de,TechNet.10).gif)

**Abbildung 1.4. Bedrohungen für**
**Desktopproduktivitätsanwendungen**

Die meisten Unternehmen sind mit einem gewissen potenziellen Risiko durch alle fünf Sicherheitsbedrohungen konfrontiert. Allerdings liegen in den meisten Unternehmen jeweils spezifische Kombinationen von Angriffsmethoden und potenziellen Sicherheitsangriffen oder Exploits vor.

#### Bedrohungen für aktive Inhalte

Bedrohungen für aktive Inhalte gehören zu den gängigen Desktopsicherheitsbedrohungen Typische Angriffsmethoden sind ActiveX-Steuerelemente, Add-Ins und Makros. Diese Angriffsmethoden können von Programmierern ausgenutzt werden, die schädlichen Code programmieren bzw. schädliche Programme erstellen, die auf dem Computer eines Benutzers ausgeführt werden. Bedrohungen für aktive Inhalte stellen ein potenzielles Risiko für Unternehmen jeder Größe dar, besonders aber für Unternehmen, die Benutzern Folgendes ermöglichen:

-   Ausführen von Makros, ActiveX-Steuerelementen oder Add-Ins
-   Öffnen von E-Mail-Anlagen
-   Gemeinsamer Zugriff auf Dokumente über ein öffentliches Netzwerk, z. B. das Internet
-   Öffnen von Dokumenten aus Quellen außerhalb des Unternehmens, beispielsweise von Kunden, Anbietern oder Partnern

#### Bedrohungen durch nicht autorisierten Zugriff

Bedrohungen durch nicht autorisierten Zugriff liegen vor, wenn sich nicht autorisierte Benutzer Zugriff auf Informationen verschaffen wollen. Zu den potenziellen Zielen nicht autorisierter Benutzer zählen:

-   **Dokumentdateien**. Wenn nicht autorisierte Benutzer Zugriff auf Dokumentdateien erlangen, können sie die Dateien löschen, ersetzen oder beschädigen.
-   **Informationen innerhalb von Dokumenten**. Zu diesen Informationen gehören Text, Grafiken, Kommentare, Revisionen, Anmerkungen, benutzerdefinierte XML-Daten, ausgeblendeter Text, Wasserzeichen sowie Kopf- und Fußzeileninformationen. Wenn nicht autorisierte Benutzer auf die Informationen innerhalb von Dokumenten zugreifen, erhalten sie damit unter Umständen Zugriff auf sensible Daten wie vertrauliche Unternehmensdaten und persönliche oder private Informationen über Benutzer. Darüber hinaus können sie Informationen ändern, beschädigen oder löschen bzw. Dokumenten in vertrauenswürdigen Speicherorten aktiven Inhalt hinzufügen.
-   **Metadaten**. Mit Dokumenten verbundene Informationen, einschließlich Dokumenteigenschaften wie Name des Autors, Name des Unternehmens, Bearbeitungszeit oder Versionsnummer des Dokuments. Wenn nicht autorisierte Benutzer Zugriff auf Metadaten erhalten, können sie möglicherweise auf vertrauliche persönliche oder Unternehmensdaten zugreifen. Darüber hinaus können sie Metadaten beschädigen oder entfernen.

Die Dokumente der meisten Unternehmen sind Bedrohungen ausgesetzt, viele Unternehmen ergreifen jedoch keine ausreichenden Maßnahmen, um diese Bedrohungen zu verringern, da die Bedrohung entweder als minimal angesehen wird oder die Verwaltungskosten zum Verringern von Bedrohungen als zu hoch erachtet werden. Diese Annahmen führen oft zu unsicheren Praktiken und Situationen wie den folgenden:

-   Die Netzwerksicherheitsarchitektur des Unternehmens kann Eindringlinge und Angreifer nicht vom Zugriff auf das interne Netzwerk abhalten. Dadurch erhöht sich das Risiko, dass Eindringlinge oder Angreifer Zugriff auf die Unternehmensdokumente erlangen.
-   Das Unternehmen lässt zu, dass Benutzer proprietäre Dokumente über das Internet senden, empfangen oder freigeben, beispielsweise Finanzdaten, Projektpläne, Präsentationen oder Zeichnungen.
-   Das Unternehmen hindert Benutzer nicht daran, Laptopcomputer mit öffentlichen Netzwerken zu verbinden. Dadurch erhöht sich das Risiko eines Zugriffs nicht identifizierbarer Angreifer auf die Dokumente, die auf diesen Laptops gespeichert sind.
-   Das Unternehmen hindert Benutzer nicht daran, Dokumente mit proprietären Informationen aus dem Büro zu entfernen.
-   Es besteht die Möglichkeit, dass nicht befugte Angreifer oder Eindringlinge Zugriff auf Dokumente mit proprietären Informationen erlangen.

#### Bedrohungen durch externe Inhalte

Zu Bedrohungen durch externe Inhalte zählen alle Angriffsmethoden, bei denen ein Dokument über ein Intranet oder ein öffentliches Netzwerk wie das Internet mit einem anderen Dokument, einer Datenbank oder einer Website verknüpft wird. Bedrohungen durch externe Inhalte werden über die folgenden Angriffsmethoden ausgenutzt:

-   **Hyperlinks**. Angreifer nutzen diese Angriffsmethode in der Regel aus, indem Hyperlinks zu nicht vertrauenswürdigen Dokumenten oder Websites erstellt werden, die schädlichen Code oder Inhalt enthalten.
-   **Datenverbindungen**. Angreifer nutzen diese Angriffsmethode in der Regel aus, indem Datenverbindungen zu Datenquellen oder Datenbanken erstellt und diese Verbindungen dann zum böswilligen Manipulieren oder Extrahieren von Daten verwenden werden.
-   **Webbeacons**. Ein typisches Szenario für die Ausnutzung dieser Angriffsmethode besteht darin, dass ein Angreifer einen unsichtbaren Link zu einem Remotebild in einer E-Mail-Nachricht einbettet. Wenn ein Benutzer die Nachricht öffnet, wird der Link aktiviert und das Remotebild heruntergeladen. Dabei können Benutzerinformationen wie E-Mail-Adresse und IP-Adresse des Benutzers an den Remotecomputer gesendet werden.
-   **Paketobjekte**. Angreifer können diese Angriffsmethode ausnutzen, indem sie ein eingebettetes Objekt böswilligen Code ausführen lassen.

Externe Inhalte stellen eine Bedrohung dar, wenn im Unternehmen folgende Praktiken gelten:

-   Benutzern wird uneingeschränkter Zugriff auf öffentliche Netzwerke, z. B. das Internet, bereitgestellt.
-   Benutzer werden nicht daran gehindert, E-Mail-Nachrichten mit eingebetteten Bildern und HTML zu empfangen.
-   Die Verwendung von Datenverbindungen in Tabellenkalkulationen und anderen Dokumenten durch Benutzer ist zugelassen.

#### Bedrohungen durch Browser

Diese Bedrohungen können auftreten, wenn eine Anwendung oder ein Dokument programmgesteuert die Funktionalität eines Webbrowsers wie Microsoft Internet Explorer® verwendet. Bedrohungen durch Browser stellen ein Risiko für Anwendungen und Dokumente dar, da Bedrohungen des Browsers gleichzeitig eine Bedrohung für die Anwendung bzw. das Dokument sind, die den Browser hosten. Bedrohungen durch Browser drücken sich in zahlreichen Angriffsmethoden aus und können über verschiedene Sicherheitsangriffe ausgenutzt werden. Beispiele für diese Angriffsmethoden sind die Installation von ActiveX-Steuerelementen, MIME-Ermittlung, Zonenanhebung und die Installation von Add-Ons.

Bedrohungen durch Browser stellen eine Bedrohung dar, wenn im Unternehmen folgende Praktiken gelten:

-   Die Ausführung von ActiveX-Steuerelementen, Add-Ins oder Makros, die Browserfunktionalität verwenden, durch Benutzer ist zugelassen.
-   Es werden Office-Lösungen entwickelt und verteilt, die Browserfunktionalität beinhalten.

Um das Risiko der Verwendung von Webbrowsern zu minimieren, wurde Internet Explorer 7 von Microsoft dahingehend entwickelt, dass standardmäßig deutlich mehr Sicherheit geboten wird. Microsoft hat zudem ein [Handbuch zur Desktopsicherheit mit Internet Explorer 7](http://go.microsoft.com/fwlink/?linkid=100953) (möglicherweise in englischer Sprache) veröffentlicht, in dem beschrieben wird, wie Internet Explorer auf Clientcomputern in Unternehmensumgebungen sicherer gestaltet werden kann.

#### Bedrohungen durch Zero-Day-Exploits

Zero-Day-Exploits können ausgeführt werden, wenn eine Sicherheitslücke gefunden wird, die noch nicht durch ein Softwareupdate (z. B. ein Microsoft-Sicherheitsbulletin oder ein Service Pack) behoben wurde. Zero-Day-Exploits können verschiedene Formen annehmen, beispielsweise:

-   Codeausführung von Remotestandorten aus
-   Erhöhung von Berechtigungen
-   Offenlegung von Informationen

Böswillige Programmierer und Benutzer können Sicherheitsrisiken über eine Reihe von Sicherheitsangriffen ausnutzen. Bis zur Veröffentlichung eines Sicherheitsbulletins oder eines Service Packs, durch das das Sicherheitsrisiko behandelt wird, stellt das Sicherheitsrisiko eine potenzielle Bedrohung für das Unternehmen dar.

[](#mainsection)[Zum Seitenanfang](#mainsection)

Die Merkmale einer sicheren 2007 Office-Umgebung
------------------------------------------------

Auch wenn die 2007 Office-Version als eigenständige Suite von Clientanwendungen bereitgestellt werden kann, ist diese Art von Bereitstellung ist kein gängiges Szenario für große Unternehmen. Die meisten großen Unternehmen stellen die 2007 Office-Version als Teil der Unternehmensinfrastruktur bereit. In einem solchen Szenario wird die 2007 Office-Version Bestandteil eines integrierten Systems, das Anwendungsserver wie Microsoft Office SharePoint® Server und Windows SharePoint Services, Kommunikationsserver wie Microsoft Exchange Server sowie Datenserver wie Microsoft SQL Server™ umfasst. Die folgende Abbildung zeigt eine typische integrierte 2007 Office-Umgebung.

![](images/Dd443664.7ecf7598-ac71-469a-bf42-b895d4c9eda2(de-de,TechNet.10).gif)

**Abbildung 1.5. Typische integrierte Microsoft**
**Office-Umgebung**

Diese Abbildung zeigt außerdem, wie die Sicherheitstechnologien und -einstellungen in der 2007 Office-Version zum Mindern von Bedrohungen durch Malware beitragen und inwiefern die Einstellungen eine entscheidende Rolle bei der tief greifenden Schutzstrategie spielen. Im Rahmen eines tief greifenden Schutzansatzes werden normalerweise die folgenden Sicherheitsmaßnahmen ergriffen:

-   Netzwerkfiltertechnologien wie Firewalls, Proxyserver und Angriffserkennungssysteme
-   Antimalwaretechnologien auf Messagingservern und auf Clientcomputern, z. B. Antiviren- oder Antispywareprogramme
-   Verschiedene mit der 2007 Office-Version bereitgestellte Sicherheitstechnologien und -einstellungen, z. B. Einstellungen für externe Datenverbindungen, VBA-Makros, Verschlüsselung, digitale Signaturen, Einstellungen für vertrauenswürdige Speicherorte und Einstellungen für vertrauenswürdige Herausgeber.

##### In diesem Beitrag

-   [Überblick](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))
-   Kapitel 1: Sicherheit in der 2007 Office-Version
-   [Kapitel 2: Vertraulichkeitseinstellungen](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10))
-   [Kapitel 3: Integrittseinstellungen](https://technet.microsoft.com/de-de/library/1e5968df-c831-421f-99f1-3799520a7132(v=TechNet.10))
-   [Kapitel 4: Verfgbarkeitseinstellungen](https://technet.microsoft.com/de-de/library/fe08a815-c260-4218-aea7-3f2f8447f81c(v=TechNet.10))
-   [Kapitel 5: Entwerfen und Implementieren von Sicherheitseinstellungen](https://technet.microsoft.com/de-de/library/6de5a362-72f8-4937-84ef-54ec91e040e6(v=TechNet.10))

**Download**

[2007 Microsoft Office-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=95736)

[GPOAccelerator herunterladen](http://go.microsoft.com/fwlink/?linkid=103576)

**Update-Benachrichtigungen**

[Melden Sie sich an, um ber Updates und neue Versionen informiert zu werden](http://go.microsoft.com/fwlink/?linkid=54982)

**Feedback**

[Senden Sie uns Ihre Kommentare und Anregungen](mailto:secwish@microsoft.com?subject=2007%20microsoft%20office-sicherheitshandbuch)

|                                                  |                                                                                                                                                                                                                                                                                                                                                                              |
|--------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [](#mainsection)[Zum Seitenanfang](#mainsection) | [![](images/Dd443664.pageLeft(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/ab515417-1c5b-44a1-b871-152c2a3b6d9b(v=TechNet.10))2 von 6[![](images/Dd443664.pageRight(de-de,TechNet.10).gif)](https://technet.microsoft.com/de-de/library/5204bf0f-65b9-403e-9d94-958dbd1553e1(v=TechNet.10)) |
