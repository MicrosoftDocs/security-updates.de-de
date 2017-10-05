---
TOCTitle: 'Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline'
Title: 'Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline'
ms:assetid: 'f86f67bd-c150-4d0d-ad85-ff13a01afb01'
ms:contentKeyID: 20075669
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443726(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline

Aktualisiert: 27.12.2005

##### Auf dieser Seite

[](#eiaa)[Überblick](#eiaa)
[](#ehaa)[Einstellungen für Überwachungsrichtlinien](#ehaa)
[](#egaa)[Einstellungen zum Zuweisen von Benutzerrechten](#egaa)
[](#efaa)[Sicherheitsoptionen](#efaa)
[](#eeaa)[Ereignisprotokolleinstellungen](#eeaa)
[](#edaa)[Eingeschränkte Gruppen](#edaa)
[](#ecaa)[Zusätzliche Sicherheitseinstellungen](#ecaa)
[](#ebaa)[Erstellen der Richtlinie mithilfe des SCW](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Die Gewährleistung der Sicherheit mittels der Domänencontroller-Serverrolle ist einer der wichtigsten Aspekte aller Umgebungen mit Computern, auf denen Microsoft® Windows Server™ 2003 mit Service Pack 1 (SP1) und der Active Directory®-Dienst ausgeführt werden. Jeder Verlust oder jede Beeinträchtigung eines Domänencontrollers in einer solchen Umgebung kann ernsthafte Folgen für Clients, Server und Anwendungen haben, die für die Authentifizierung, für Gruppenrichtlinien und für ein zentralisiertes LDAP-Verzeichnis (Lightweight Directory Access Protocol) auf Domänencontroller angewiesen sind.

Aufgrund ihrer Wichtigkeit sollten sich Domänencontroller immer an physisch sicheren Orten befinden, zu denen nur qualifizierte, administrative Mitarbeiten Zugriff haben. Falls die Domänencontroller an ungesicherten Orten installiert werden müssen (z. B. Zweigstellen), können verschiedene Sicherheitseinstellungen angepasst werden, um potenziellen Schäden infolge physischer Risiken zu verringern.

#### Richtlinie für die Domänencontroller-Baseline

Im Unterschied zu den anderen Richtlinien für Serverrollen, die später in diesem Handbuch beschrieben werden, ist die Gruppenrichtlinie für die Domänencontroller-Serverrolle eine Baseline-Richtlinie, die in die gleiche Klasse wie die Richtlinie für die Mitgliedsserver-Baseline (Member Server Baseline Policy, MSBP) fällt, die in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“, definiert wurde. Die Richtlinie für die Domänencontroller-Baseline (Domain Controller Baseline Policy, DCBP) ist mit der Organisationseinheit (Organizational Unit, OU) des Domänencontrollers verbunden und hat Vorrang vor der standardmäßigen Domänencontrollerrichtlinie. Die in der DCBP enthaltenen Richtlinieneinstellungen erhöhen die Gesamtsicherheit aller Domänencontroller in jeder Umgebung.

Der Großteil der DCBP wurde aus der MSBP übernommen. Daher sollten Sie Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“, aufmerksam durchlesen, um die vielen Richtlinieneinstellungen, die auch in der DCBP enthalten sind, vollständig zu verstehen. In diesem Kapitel werden nur die Einstellungen der Domänencontroller-Baseline-Richtlinie beschrieben, die von den Einstellungen in der Mitgliedsserver-Baseline-Richtlinie abweichen.

Die Domänencontrollervorlagen wurden speziell für die Sicherheitsanforderungen der drei in diesem Handbuch definierten Umgebungen entwickelt. In der folgenden Tabelle werden die .inf-Dateien des Domänencontrollers aufgeführt, die in diesem Handbuch für Umgebungen mit älteren Clients sowie Unternehmensclient- und Hochsicherheitsumgebungen enthalten sind. Die Datei „Unternehmensclient - Domänencontroller.inf“ ist z. B. die Sicherheitsvorlage für die Unternehmensclient-Umgebung.

**Tabelle 5.1: Sicherheitsvorlagen für die Domänencontroller-Baseline**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Älterer Client - Domänencontroller.inf</td>
<td style="border:1px solid black;">Unternehmensclient - Domänencontroller.inf</td>
<td style="border:1px solid black;">Hochsicher - Domänencontroller.inf</td>
</tr>
</tbody>
</table>
  
**Hinweis**: Domänenvorgänge könnten ernsthaft beeinträchtigt werden, wenn ein falsch konfiguriertes Gruppenrichtlinienobjekt (GPO) mit der Domänencontroller-Organisationseinheit verknüpft wird. Seien Sie beim Importieren dieser Sicherheitsvorlagen äußerst vorsichtig, und stellen Sie sicher, dass alle importierten Richtlinieneinstellungen korrekt sind, bevor Sie ein Gruppenrichtlinienobjekt mit der Domänencontroller-Organisationseinheit verknüpfen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen für Überwachungsrichtlinien
  
Die Einstellungen für Überwachungsrichtlinien für die Domänencontroller entsprechen fast den in der Richtlinie für die Mitgliedsserver-Baseline festgelegten Einstellungen. Weitere Informationen finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Die Richtlinieneinstellungen der DCBP stellen sicher, dass alle relevanten Sicherheitsüberwachungsinformationen auf den Domänencontrollern protokolliert werden.
  
**Tabelle 5.2: Empfohlene Einstellungen für Überwachungsrichtlinien**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Active Directory-Zugriff überwachen</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Keine Überwachung</td>
<td style="border:1px solid black;">Fehler</td>
</tr>
</tbody>
</table>
  
#### Active Directory-Zugriff überwachen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Benutzerzugriff auf ein Active Directory-Objekt überwacht werden soll, das über eine eigene Systemzugriffssteuerungsliste (SACL) verfügt. Wenn Sie die Einstellung **Active Directory-Zugriff überwachen** definieren, können Sie festlegen, ob erfolgreiche Ereignisse oder Fehler überwacht werden oder ob keine Überwachung des Ereignistyps erfolgen soll. Bei der Erfolgsüberwachung wird ein Überwachungseintrag erzeugt, wenn ein Benutzer erfolgreich auf ein Active Directory-Objekt zugreift, für das eine SACL festgelegt wurde. Bei der Fehlerüberwachung wird ein Überwachungseintrag erzeugt, wenn der Zugriff eines Benutzers auf ein Active Directory-Objekt fehlschlägt, für das eine SACL festgelegt wurde.
  
Wenn Sie die Einstellung **Active Directory-Zugriff überwachen** in der DCBP aktivieren und für Verzeichnisobjekte SACLs konfigurieren, wird in den Sicherheitsprotokollen auf Domänencontrollern eine große Menge von Einträgen erzeugt. Diese Einstellung sollte nur aktiviert werden, wenn Sie tatsächlich beabsichtigen, die erstellten Informationen zu verwenden.
  
Die Einstellung **Active Directory-Zugriff überwachen** ist in den Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Keine Überwachung** gesetzt. Sie ist so konfiguriert, dass in der Hochsicherheitsumgebung **Fehler** protokolliert werden.
  
In der folgenden Tabelle sind wichtige Sicherheitsereignisse enthalten, die die Einstellung **Active Directory-Zugriff überwachen** im Sicherheitsprotokoll aufzeichnet.
  
**Tabelle 5.3: Active Directory-Zugriffsereignisse**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ereigniskennung</th>
<th style="border:1px solid black;" >Ereignisbeschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Beschreibung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">566</td>
<td style="border:1px solid black;">Es fand ein allgemeiner Objektvorgang statt.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen zum Zuweisen von Benutzerrechten
  
Die Richtlinie für die Domänencontroller-Baseline legt verschiedene Zuweisungen von Benutzerrechten für die Domänencontroller fest. Neben der Standardkonfiguration wurden mehrere Benutzerberechtigungseinstellungen modifiziert, um die Sicherheit für die Domänencontroller in den drei in diesem Handbuch definierten Umgebungen zu erhöhen.
  
Dieser Abschnitt enthält Informationen zu den empfohlenen Einstellungen für Benutzerrechte für die Richtlinie für die Domänencontroller-Baseline, die sich von denen in der Richtlinie für die Mitgliedsserver-Baseline unterscheiden. Eine Zusammenfassung der vorgeschriebenen Einstellungen in diesem Abschnitt finden Sie in der Microsoft Excel®-Arbeitsmappe „Sicherheitseinstellungen unter Windows Server 2003“, die in der herunterladbaren Version dieses Handbuchs enthalten ist.
  
In der folgenden Tabelle werden die empfohlenen Einstellungen zum Zuweisen von Benutzerrechten für die DCBP zusammengefasst. Weitere Informationen zu den einzelnen Einstellungen erhalten Sie in den nach der Tabelle angeführten Abschnitten.
  
**Tabelle 5.4: Empfohlene Einstellungen zum Zuweisen von Benutzerrechten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Auf diesen Computer vom Netzwerk aus zugreifen</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren, Authentifizierte Benutzer, Domänencontroller der Organisation</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Hinzufügen von Arbeitsstationen zur Domäne</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lokal anmelden zulassen</td>
<td style="border:1px solid black;">Administratoren, Server-Operatoren, Sicherungsoperatoren</td>
<td style="border:1px solid black;">Administratoren, Server-Operatoren, Sicherungsoperatoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anmeldung über Terminaldienste zulassen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ändern der Systemzeit</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Computer und Benutzerkonten für Delegierungszwecke vertrauen</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Laden und Entfernen von Gerätetreibern</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Wiederherstellen von Dateien und Verzeichnissen</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">System herunterfahren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Administratoren</td>
</tr>
</tbody>
</table>
  
#### Auf diesen Computer vom Netzwerk aus zugreifen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer und Gruppen über das Netzwerk eine Verbindung mit dem Domänencontroller herstellen können. Sie ist für eine Anzahl von Netzwerkvorgängen erforderlich, darunter die Active Directory-Replikation zwischen Domänencontrollern, Authentifizierungsanforderungen an Domänencontroller von Benutzern und Computern sowie der Zugriff auf freigegebene Ordner und Drucker.
  
Selbst wenn die der Sicherheitsgruppe **Jeder** zugewiesenen Berechtigungen keinen anonymen Benutzern in Windows Server 2003 mit SP1 mehr Zugriff gewähren, kann Gastgruppen und -konten weiterhin über die Sicherheitsgruppe **Jeder** Zugriff gewährt werden.
  
Deshalb wurde die Sicherheitsgruppe **Jeder** aus dem Benutzerrecht **Auf diesen Computer vom Netzwerk aus zugreifen** in der DCBP für die Hochsicherheitsumgebung entfernt. Dies stellt eine zusätzliche Sicherheitsmaßnahme gegen Angriffe auf den Gastzugriff zur Domäne dar. Diese Richtlinieneinstellung ist für die Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt.
  
#### Hinzufügen von Arbeitsstationen zur Domäne
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer Computerarbeitsstationen zu einer bestimmten Domäne hinzufügen können. Zur Aktivierung dieser Richtlinieneinstellung muss diese dem Benutzer als Teil der Standarddomänencontrollerrichtlinie der Domäne zugewiesen werden. Ein Benutzer mit dieser Berechtigung kann der Domäne bis zu zehn Arbeitsstationen hinzufügen. Benutzer mit der Berechtigung **Computerobjekte erstellen** für eine Organisationseinheit oder den Container „Computer“ in Active Directory können der Domäne eine unbegrenzte Anzahl von Computern hinzufügen, unabhängig davon, ob Ihnen die Benutzerberechtigung **Hinzufügen von Arbeitsstationen zur Domäne** zugewiesen wurde oder nicht.
  
Standardmäßig können alle Benutzer der Gruppe **Authentifizierte Benutzer** einer Active Directory-Domäne bis zu zehn Computer hinzufügen. Diese neuen Computerkonten werden im Container „Computer“ erstellt.
  
In windowsbasierten Netzwerken ist der Begriff *Sicherheitsprinzipal* als Benutzer, Gruppe oder Computer definiert, denen automatisch eine Sicherheits-ID zur Steuerung des Zugriffs auf Ressourcen zugewiesen wird. Innerhalb einer Active Directory-Domäne stellt jedes Computerkonto ein vollständiges Sicherheitsprinzipal dar, das Domänenressourcen authentifizieren und auf diese zugreifen kann. Manche Organisationen möchten möglicherweise die Anzahl der Computer in einer Active Directory-Umgebung begrenzen, um die Computer so einheitlich überwachen, einrichten und verwalten zu können. Wenn Benutzer der Domäne Computer hinzufügen können, werden Maßnahmen zur Überwachung und Verwaltung behindert. Außerdem könnten Benutzer aufgrund Ihrer Berechtigung zum Erstellen zusätzlicher, nicht genehmigter Domänencomputer Aktivitäten durchführen, die schwerer nachzuverfolgen sind.
  
Aus diesen Gründen wird das Benutzerrecht **Hinzufügen von Arbeitsstationen zur Domäne** nur **Administratoren** in der DCBP für die Hochsicherheitsumgebung zugewiesen. Diese Richtlinieneinstellung ist für die Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt.
  
#### Lokal anmelden zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer interaktive Sitzungen auf dem Domänencontroller starten können. Benutzer ohne dieses Recht können weiterhin eine interaktive Remotesitzung auf dem Domänencontroller starten, wenn sie über das Benutzerrecht **Anmeldung durch Terminaldienste zulassen** verfügen.
  
Die Anzahl der Konten, die sich bei Domänencontrollerkonsolen anmelden können, sollte eingeschränkt werden, um unerlaubten Zugriff auf Dateisysteme und Systemdienste des Domänencontrollers zu verhindern. Ein Benutzer, der sich bei der Konsole eines Domänencontrollers anmelden kann, könnte den Computer in böswilliger Absicht verwenden und die Sicherheit einer gesamten Domäne oder Gesamtstruktur beeinträchtigen.
  
Standardmäßig wird den Gruppen **Konten-Operatoren**, **Sicherungs-Operatoren**, **Druck-Operatoren** und **Server-Operatoren** auf Domänencontrollern die Benutzerberechtigung **Lokal anmelden zulassen** zugewiesen. Benutzer in diesen Gruppen sollten sich nicht bei einem Domänencontroller anmelden müssen, um ihre Verwaltungsaufgaben auszuführen, und sie sollten ihre Arbeit von anderen Arbeitsstationen aus durchführen können. Wartungsarbeiten an Domänencontrollern sollten nur von Benutzern in der Gruppe **Administratoren** ausgeführt werden.
  
Wenn das Benutzerrecht **Lokal anmelden zulassen** nur der Gruppe **Administratoren** zugewiesen wird, haben nur absolut vertrauenswürdige Benutzer physischen und interaktiven Zugriff auf Domänencontroller. Die Sicherheit wird dadurch erhöht. Aus diesem Grund wird das Benutzerrecht **Lokal anmelden zulassen** in der DCBP für die Hochsicherheitsumgebung nur der Gruppe **Administratoren** zugewiesen. Diese Richtlinieneinstellung ist für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen so konfiguriert, dass sie die Gruppen **Server-Operatoren** und **Sicherungs-Operatoren** enthält.
  
#### Anmeldung über Terminaldienste zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer sich beim Domänencontroller über eine Remotedesktopverbindung anmelden können.
  
Die Anzahl der Konten, die sich über Terminaldienste bei Domänencontrollerkonsolen anmelden können, sollte eingeschränkt werden, um unerlaubten Zugriff auf Dateisysteme und Systemdienste des Domänencontrollers zu verhindern. Ein Benutzer, der sich über Terminaldienste bei der Konsole eines Domänencontrollers anmelden kann, könnte den Computer ausnutzen und die Sicherheit einer gesamten Domäne oder Gesamtstruktur beeinträchtigen.
  
Wenn das Benutzerrecht **Anmeldung über Terminaldienste zulassen** nur der Gruppe **Administratoren** zugewiesen wird, haben nur absolut vertrauenswürdige Benutzer physischen und interaktiven Zugriff auf Domänencontroller. Die Sicherheit wird dadurch erhöht. Aus diesem Grund wird das Benutzerrecht **Anmeldung über Terminaldienste zulassen** der DCBP für alle drei in diesem Handbuch definierten Umgebungen nur der Gruppe **Administratoren** in zugewiesen. Obwohl das Anmelden bei einem Domänencontroller über Terminaldienste standardmäßig administrativen Zugriff erfordert, schützt das Konfigurieren dieser Richtlinieneinstellung vor unbeabsichtigten oder böswilligen Aktionen, die Ihr Netzwerk gefährden könnten.
  
Als zusätzliche Sicherheitsmaßnahme verweigert die DCBP dem standardmäßigen Administratorkonto das Benutzerrecht **Anmeldung über Terminaldienste zulassen**. Diese Konfiguration verhindert, dass Angreifer von einem Remotestandort aus unter Verwendung des standardmäßigen Administratorkontos auf einen Domänencontroller zugreifen können. Weitere Informationen zu dieser Richtlinieneinstellung finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“.
  
#### Ändern der Systemzeit
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Uhrzeit der internen Uhr des Computers einstellen können. Dieses Recht ist jedoch nicht zum Ändern der Zeitzone oder anderer Anzeigeeigenschaften der Systemzeit erforderlich.
  
Eine synchronisierte Systemzeit ist für das Funktionieren von Active Directory von entscheidender Bedeutung. Für eine ordnungsgemäße Durchführung der vom Kerberos-Authentifizierungsprotokoll verwendeten Prozesse zur Active Directory-Replikation und zur Authentifizierungsticketgenerierung ist eine Synchronisierung der Zeit in allen Umgebungen erforderlich.
  
Eine Domänencontrolleruhr, die nicht mit der Systemzeit auf anderen Domänencontrollern der Umgebung synchronisiert ist, könnte die Ausführung von Domänendiensten beeinträchtigen. Wenn nur Administratoren das Ändern der Systemzeit gestattet wird, kann das Risiko einer falschen Systemzeit auf einem Domänencontroller verringert werden.
  
Standardmäßig hat die Gruppe **Server-Operatoren** die Möglichkeit, die Systemzeit von Domänencontrollern zu ändern. Aufgrund der Probleme, die von Mitgliedern dieser Gruppe durch inkorrekte Änderung der Uhrzeit eines Domänencontrollers verursacht werden können, wird das Benutzerrecht **Ändern der Systemzeit** für alle drei in diesem Handbuch definierten Umgebungen in der DCBP nur der Gruppe **Administratoren** zugewiesen.
  
Weitere Informationen zum Microsoft Windows®-Zeitdienst finden Sie im Artikel [Technische Informationen zum Windows-Zeitdienst](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/techref/a0fcd250-e5f7-41b3-b0e8-240f8236e210.mspx) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/TechRef/a0fcd250-e5f7-41b3-b0e8-240f8236e210.mspx.
  
#### Computer und Benutzerkonten für Delegierungszwecke vertrauen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Einstellung **Für Delegierungszwecke vertrauen** auf einem Benutzer- oder Computerobjekt in Active Directory ändern können. Die Funktion zur Authentifizierungsdelegierung wird von mehrschichtigen Client-/Serveranwendungen verwendet. Sie ermöglicht es einem Front-End-Dienst, wie z. B. einer Anwendung, zur Authentifizierung bei einem Back-End-Dienst, wie einer Datenbank, die Anmeldeinformationen eines Clients zu verwenden. Damit eine solche Authentifizierung möglich ist, müssen sowohl der Client als auch der Server unter Konten ausgeführt werden, denen für Delegierungszwecke vertraut wird.
  
Der Missbrauch dieses Rechts kann es nicht autorisierten Benutzern ermöglichen, die Identität anderer Benutzer im Netzwerk anzunehmen. Ein Angreifer könnte dieses Recht ausnutzen, um mit der Identität eines anderen Benutzers Zugriff auf Netzwerkressourcen zu erlangen, was ein Bestimmen der Geschehnisse nach einer Sicherheitsverletzung erschweren könnte.
  
Das Benutzerrecht **Computer und Benutzerkonten für Delegierungszwecke vertrauen** wird auf Domänencontrollern für die Hochsicherheitsumgebung nur der Gruppe **Administratoren** zugewiesen. Diese Richtlinieneinstellung ist für die Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen auf **Nicht definiert** gesetzt.
  
**Hinweis**: Obwohl dieses Recht durch die Standarddomänencontrollerrichtlinie der Gruppe **Administratoren** zugewiesen wird, setzt die Richtlinie für die Domänencontroller-Baseline dieses Recht in der Hochsicherheitsumgebung nur durch, weil es ursprünglich auf der Richtlinie für die Mitgliedsserver-Baseline basierte. In der Richtlinie für die Mitgliedsserver-Baseline wird diesem Recht ein Nullwert zugewiesen.
  
#### Laden und Entfernen von Gerätetreibern
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer Gerätetreiber laden und entfernen können. Sie ist zudem für das Laden und Entfernen von Plug & Play-Geräten erforderlich.
  
Bei unsachgemäßer Verwaltung der Gerätetreiber auf Domänencontrollern kann der Betrieb der Domänencontroller durch Fehler und schädlichen Code beeinträchtigt werden. Wenn die Konten, unter denen Gerätetreiber geladen und entfernt werden können, in der DCBP auf die vertrauenswürdigsten Benutzer begrenzt werden, lässt sich die Gefahr, dass Gerätetreiber zur Beeinträchtigung von Domänencontrollern eingesetzt werden, verringern.
  
Standardmäßig ist das Benutzerrecht **Laden und Entfernen von Gerätetreibern** der Gruppe **Druck-Operatoren** zugewiesen. Wie bereits erwähnt, empfiehlt es sich nicht, Druckerfreigaben auf Domänencontrollern zu erstellen. Dadurch muss **Druck-Operatoren** nicht das Recht zugewiesen werden, Gerätetreiber zu laden und entfernen zu können. Das Benutzerrecht **Laden und Entfernen von Gerätetreibern** wird deshalb in der DCBP für alle drei in diesem Handbuch definierten Umgebungen nur der Gruppe **Administratoren** zugewiesen.
  
#### Wiederherstellen von Dateien und Verzeichnissen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer während des Wiederherstellungsprozesses Datei- und Verzeichnisberechtigungen umgehen können. Jeder gültige Sicherheitsprinzipal kann als Besitzer eines Objekts festgelegt werden.
  
Ein Konto, mit dem Dateien und Verzeichnisse auf dem Dateisystem eines Domänencontrollers wiederhergestellt werden können, kann ausführbare Dateien leicht modifizieren. Angreifer könnten diese Möglichkeit ausnutzen, um nicht nur einen Domänencontroller unbrauchbar zu machen, sondern auch die Sicherheit einer Domäne oder einer Gesamtstruktur zu gefährden.
  
Standardmäßig wird das Benutzerrecht **Wiederherstellen von Dateien und Verzeichnissen** den Gruppen **Server-Operatoren** und **Sicherungs-Operatoren** zugewiesen. Wenn Sie dieses Benutzerrecht diesen Gruppen entziehen und es nur der Gruppe **Administratoren** zuweisen, wird die Wahrscheinlichkeit einer Beeinträchtigung des Domänencontrollers durch fehlerhafte Änderungen am Dateisystem verringert. Das Benutzerrecht **Wiederherstellen von Dateien und Verzeichnissen** wird deshalb in der DCBP für alle drei in diesem Handbuch definierten Umgebungen nur der Gruppe **Administratoren** zugewiesen.
  
#### System herunterfahren
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer den lokalen Computer herunterfahren können.
  
Angreifer mit der Fähigkeit, Domänencontroller herunterzufahren, können auf einfache Weise eine DoS-Angriff (Denial of Service) starten, die schwerwiegende Auswirkungen auf eine gesamte Domäne oder Gesamtstruktur haben kann. Ein Angreifer könnte dieses Benutzerrecht ausnutzen, um das Konto eines Domänencontrollers mit dem Ziel der Erweiterung von Berechtigungen anzugreifen, wenn der Domänencontroller einen Neustart der Dienste durchführt. Ein erfolgreicher Angriff auf einen Domänencontroller zur Erweiterung von Berechtigungen beeinträchtigt die Sicherheit einer Domäne oder Gesamtstruktur.
  
Standardmäßig wird das Benutzerrecht **System herunterfahren** den Gruppen **Administratoren**, **Server-Operatoren**, **Druck-Operatoren** und **Sicherungs-Operatoren** zugewiesen. In sicheren Umgebungen benötigt keine dieser Gruppen mit Ausnahme der Gruppe **Administratoren** dieses Recht, um administrative Aufgaben ausführen zu können. Aus diesem Grund wird das Benutzerrecht **System herunterfahren** in der DCBP für alle drei in diesem Handbuch definierten Umgebungen nur der Gruppe **Administratoren** zugewiesen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Sicherheitsoptionen
  
Die meisten Einstellungen für Sicherheitsoptionen für Domänencontroller entsprechen den in der Richtlinie für die Mitgliedsserver-Baseline festgelegten Einstellungen. Weitere Informationen finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Unterschiede zwischen MSBP- und der DCBP-Richtlinieneinstellungen werden in den folgenden Abschnitten beschrieben.
  
#### Domänencontrollereinstellungen
  
**Tabelle 5.5: Sicherheitsoptionen: Empfehlungen zu Domänencontrollereinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serveroperatoren das Einrichten von geplanten Tasks erlauben</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Signaturanforderungen für LDAP-Server</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Nicht definiert</td>
<td style="border:1px solid black;">Signatur erforderlich</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Änderungen von Computerkontenkennwörtern verweigern</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
<td style="border:1px solid black;">Deaktiviert</td>
</tr>
</tbody>
</table>
  
##### Domänencontroller: Serveroperatoren das Einrichten von geplanten Tasks erlauben
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Mitglieder der Gruppe **Server-Operatoren** Aufträge mit der AT-Zeitplanfunktion senden können.
  
Die Einstellung **Domänencontroller: Serveroperatoren das Einrichten von geplanten Tasks erlauben** ist in der DCBP für alle drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt. In den meisten Organisationen hat diese Konfiguration der Richtlinieneinstellung nur geringfügige Auswirkungen. Benutzer, einschließlich Benutzern in der Gruppe **Server-Operatoren**, können weiterhin Aufträge über den Taskplaner-Assistenten erstellen. Diese Aufträge werden jedoch im Kontext des Kontos ausgeführt, mit dem sich der Benutzer beim Einrichten des Auftrags authentifiziert.
  
**Hinweis**: Ein AT-Dienstkonto kann geändert werden, um ein anderes Konto anstelle des lokalen Systemkontos auszuwählen. Zum Ändern des Kontos öffnen Sie **Systemprogramme**, klicken Sie auf **Geplante Tasks** und anschließend auf den Ordner **Zubehör**. Klicken Sie anschließend im Menü **Erweitert** auf **AT-Dienstkonto**.
  
##### Domänencontroller: Signaturanforderungen für LDAP-Server
  
Durch diese Richtlinieneinstellung wird festgelegt, ob für den LDAP-Server eine Signatur erforderlich ist, bevor dieser mit LDAP-Clients verhandeln kann. Nicht signierter bzw. unverschlüsselter Netzwerkverkehr ist anfällig für Man-in-the-Middle-Angriffe. Bei einem solchen Angriff fängt ein Eindringling Datenpakete zwischen dem Server und dem Client ab und ändert diese vor der Weiterleitung an den Client. Im Falle eines LDAP-Servers könnte ein Angreifer einen Client veranlassen, Entscheidungen zu treffen, die auf falschen Datensätzen aus dem LDAP-Verzeichnis basieren.
  
Wenn alle Domänencontroller unter Windows 2000 oder Windows Server 2003 ausgeführt werden, müssen Sie die Einstellung **Domänencontroller: Signaturanforderungen für LDAP-Server** auf **Signatur erforderlich** setzen. Andernfalls behalten Sie für diese Richtlinieneinstellung den Wert **Nicht definiert** bei. Dabei handelt es sich um die DCBP-Konfiguration für Umgebungen mit älteren Clients und Unternehmensclient-Umgebungen. Diese Richtlinieneinstellung ist in der DCBP für die Hochsicherheitsumgebung auf **Signatur erforderlich** gesetzt, da alle Computer in dieser Umgebung entweder unter Windows 2000 oder Windows Server 2003 ausgeführt werden.
  
##### Domänencontroller: Änderungen von Computerkontenkennwörtern verweigern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Domänencontroller Anforderungen von Mitgliedscomputern zum Ändern der Computerkontenkennwörter verweigern. Wenn Sie diese Richtlinieneinstellung auf allen Domänencontrollern in einer Domäne aktivieren, können Computerkontenkennwörter auf Domänenmitgliedern nicht geändert werden und sind anfälliger für Angriffe.
  
Die Einstellung **Domänencontroller: Änderungen von Computerkontenkennwörtern verweigern** ist deshalb in der DCBP für alle drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Netzwerksicherheitseinstellungen
  
**Tabelle 5.6: Sicherheitsoptionen: Empfehlungen für Netzwerksicherheitseinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
#### Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die bei der Änderung von Kennwörtern vom LAN Manager (LM) erzeugten Hashwerte für das neue Kennwort gespeichert werden. LM-Hashwerte sind anfälliger für Angriffe, weil für ihre Erzeugung im Vergleich zu Windows NT®-Hashwerten ein schwächerer kryptografischer Algorithmus verwendet wird.
  
Aus diesem Grund wird die Einstellung **Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern** durch die DCBP in allen drei in diesem Handbuch definierten Umgebungen aktiviert.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung aktivieren, kann es bei älteren Betriebssystemen und einige Anwendungen von Drittanbietern zu Fehlern kommen. So kommt es z. B. bei Windows 95 und Windows 98 zu Fehlern, wenn Active Directory Client Extension nicht installiert wurde. Darüber hinaus müssen, wenn Sie diese Richtlinieneinstellung aktivieren, die Kennwörter aller Konten geändert werden.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Ereignisprotokolleinstellungen
  
Die Ereignisprotokolleinstellungen für die Domänencontroller entsprechen den in der Richtlinie für die Mitgliedsserver-Baseline festgelegten Einstellungen. Weitere Informationen finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Die Richtlinieneinstellungen der DCBP stellen sicher, dass alle relevanten Sicherheitsüberwachungsinformationen, einschließlich des Verzeichnisdienstzugriffs, auf den Domänencontrollern protokolliert werden.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Eingeschränkte Gruppen
  
Wie im vorherigen Kapitel beschrieben, können Sie mit der Einstellung **Eingeschränkte Gruppen** die Mitgliedschaft von Gruppen in Windows Server 2003 mit SP1 über eine Active Directory-Gruppenrichtlinie verwalten. Prüfen Sie zunächst die Anforderungen Ihrer Organisation, bevor Sie die einzuschränkenden Gruppen festlegen. Für Domänencontroller sind die Gruppen **Server-Operatoren** und **Sicherungs-Operatoren** in allen drei in diesem Handbuch definierten Umgebungen eingeschränkt. Obwohl Mitglieder der Gruppen **Server-Operatoren** und **Sicherungs-Operatoren** weniger Zugriffsrechte als Mitglieder der Gruppe **Administratoren** haben, sind ihre Berechtigungen dennoch sehr umfassend.
  
**Hinweis**: Wenn Ihre Organisation eine dieser Gruppen verwendet, sollten Sie deren Mitgliedschaft sorgfältig überprüfen und die Anleitung für die Einstellung **Eingeschränkte Gruppen** nicht implementieren. Wenn Ihre Organisation Benutzer der Gruppe „Serverbenutzer“ hinzufügt, sollten Sie u. U. die optionalen Dateisystemberechtigungen implementieren, die im Abschnitt „Sichern des Dateisystems“ des vorigen Kapitels beschrieben werden.
  
**Tabelle 5.7: Empfehlungen für „Eingeschränkte Gruppen“**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Lokale Gruppe</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Sicherungs-Operatoren</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Server-Operatoren</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
<td style="border:1px solid black;">Keine Mitglieder</td>
</tr>
</tbody>
</table>
  
Die Einstellung **Eingeschränkte Gruppen** kann unter Windows Server 2003 mit SP1 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Eingeschränkte Gruppen\\**
  
Um eingeschränkte Gruppen für ein Gruppenrichtlinienobjekt zu konfigurieren, können Administratoren die gewünschte Gruppe direkt dem Knoten **Eingeschränkte Gruppen** im Namespace des Gruppenrichtlinienobjekts hinzufügen.
  
Ist eine Gruppe eingeschränkt, können deren Mitglieder und andere Gruppen, denen sie angehört, festgelegt werden. Wenn Sie diese Gruppenmitglieder nicht angeben, bleibt die Gruppe vollkommen eingeschränkt. Gruppen können nur mithilfe von Sicherheitsvorlagen eingeschränkt werden.
  
**So zeigen Sie die Einstellung „Eingeschränkte Gruppen“ an oder ändern diese**
  
1.  Öffnen Sie die Sicherheitsvorlagen-Verwaltungskonsole.
  
    **Hinweis**: Die Sicherheitsvorlagen-Verwaltungskonsole ist standardmäßig nicht im Menü **Verwaltung** nicht vorhanden. Um sie hinzuzufügen, starten Sie die Microsoft Management Console (mmc.exe), und fügen Sie das Add-In „Sicherheitsvorlagen“ hinzu.
  
2.  Doppelklicken Sie auf das Verzeichnis der Konfigurationsdatei und dann auf die Konfigurationsdatei.
  
3.  Doppelklicken Sie auf das Element **Eingeschränkte Gruppen**.
  
4.  Klicken Sie mit der rechten Maustaste auf **Eingeschränkte Gruppen**.
  
5.  Wählen Sie die Option **Gruppe hinzufügen** aus.
  
6.  Klicken Sie auf **Durchsuchen** und anschließend auf **Pfad**, wählen Sie den zu durchsuchenden Pfad aus, und klicken Sie auf **OK**.
  
    **Hinweis**: Einem lokaler Computer wird dadurch in der Regel oben in der Liste angezeigt.
  
7.  Geben Sie im Textfeld **Geben Sie die zu verwendenden Objektnamen ein** den Gruppennamen ein, und klicken Sie auf die Schaltfläche **Namen überprüfen**.
  
    – oder –
  
    Klicken Sie auf **Erweitert** und anschließend auf **Suche starten**, um alle verfügbaren Gruppen aufzulisten.
  
8.  Wählen Sie die einzuschränkenden Gruppen aus, und klicken Sie auf **OK**.
  
9.  Klicken Sie im Dialogfeld **Gruppen hinzufügen** auf **OK**, um das Dialogfeld zu schließen.
  
Alle Mitglieder (Benutzer und Gruppen) der Gruppen **Server-Operatoren** und **Sicherungs-Operatoren** wurden in dieser Anleitung entfernt, um sie in beiden Umgebungen vollkommen einzuschränken. Für die Hochsicherheitsumgebung wurden zudem alle Mitglieder der Gruppe **Remotedesktopbenutzer** entfernt. Microsoft empfiehlt, alle vordefinierten Gruppen, die in Ihrer Organisation nicht verwendet werden, einschränken.
  
**Hinweis**: Die Konfiguration der in diesem Abschnitt beschriebenen Einstellung **Eingeschränkte Gruppen** ist sehr einfach. Versionen von Windows XP mit SP1 und SP2 sowie Windows Server 2003 unterstützen komplexere Entwürfe. Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Updates to Restricted Groups ("Member of") Behavior of User-Defined Local Groups](http://support.microsoft.com/kb/810076/en-us)“ (in englischer Sprache) unter http://support.microsoft.com/kb/810076/en-us.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusätzliche Sicherheitseinstellungen
  
In diesem Abschnitt werden Änderungen beschrieben, die an der Richtlinie für die Domänencontroller-Baseline manuell vorgenommen werden müssen, sowie zusätzliche Einstellungen und Gegenmaßnahmen, die nicht durch Gruppenrichtlinien implementiert werden können.
  
#### Manuelles Hinzufügen von eindeutigen Sicherheitsgruppen zu den Zuweisungen von Benutzerrechten
  
Die meisten Zuweisungen von Benutzerrechten, die über die Richtlinie für die Domänencontroller-Baseline angewendet werden, sind in den zu diesem Handbuchs gehörenden Sicherheitsvorlagen genau definiert. Einige Konten und Sicherheitsgruppen konnten jedoch nicht in die Vorlagen aufgenommen werden, da ihre Sicherheits-IDs spezifisch für einzelne Windows Server 2003-Domänen sind. Zuweisungen von Benutzerrechten, die manuell konfiguriert werden müssen, sind in der folgenden Tabelle angegeben.
  
**Warnung**: Die folgende Tabelle enthält Werte für das vordefinierte Administratorkonto. Dieses Konto darf nicht mit der vordefinierten Sicherheitsgruppe **Administratoren** verwechselt werden. Wenn Sie die Sicherheitsgruppe **Administratoren** einem der nachfolgenden Benutzerrechte hinzufügen, die den Zugriff verweigern, müssen Sie sich lokal anmelden, um den Fehler zu beheben.
  
Wenn Sie das vordefinierte Administratorkonto gemäß den Empfehlungen in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“, umbenannt haben, müssen Sie sicherstellen, dass das neu benannte Administratorkonto ausgewählt ist, wenn Sie das Konto Benutzerrechten hinzufügen, die den Zugriff verweisen.
  
**Tabelle 5.8: Manuell hinzugefügte Zuweisungen von Benutzerrechten**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Den Zugriff auf diesen Computer vom Netzwerk aus verweigern</td>
<td style="border:1px solid black;">Vordefinierter Administrator; Support_388945a0;
Gast; alle betriebssystemfremden Dienstkonten</td>
<td style="border:1px solid black;">Vordefinierter Administrator; Support_388945a0;
Gast; alle betriebssystemfremden Dienstkonten</td>
<td style="border:1px solid black;">Vordefinierter Administrator; Support_388945a0;
Gast; alle betriebssystemfremden Dienstkonten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Anmeldung als Batchauftrag verweigern</td>
<td style="border:1px solid black;">Support_388945a0 und Gast</td>
<td style="border:1px solid black;">Support_388945a0 und Gast</td>
<td style="border:1px solid black;">Support_388945a0 und Gast</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Anmeldung über Terminaldienste verweigern</td>
<td style="border:1px solid black;">Vordefinierter Administrator; alle betriebssystemfremden Dienstkonten</td>
<td style="border:1px solid black;">Vordefinierter Administrator; alle betriebssystemfremden Dienstkonten</td>
<td style="border:1px solid black;">Vordefinierter Administrator; alle betriebssystemfremden Dienstkonten</td>
</tr>
</tbody>
</table>
  
**Wichtig**: „Alle betriebssystemfremden Dienstkonten“ schließt Dienstkonten mit ein, die unternehmensweit für bestimmte Anwendungen verwendet werden. Dazu gehören allerdings NICHT Konten des LOKALEN SYSTEMS, des LOKALEN DIENSTES oder des NETZWERKDIENSTES (die vom Betriebssystem verwendeten, vordefinierten Konten).
  
#### Verzeichnisdienste
  
Domänencontroller, auf denen Windows Server 2003 mit SP 1 ausgeführt wird, speichern Verzeichnisdaten und verwalten Benutzer- und Domäneninteraktionen, einschließlich Benutzeranmeldungen, Authentifizierungen und Verzeichnissuchen.
  
##### Verschieben von Daten – Active Directory-Datenbank und -Protokolldateien
  
Zur Aufrechterhaltung der Integrität und Zuverlässigkeit von Verzeichnissen ist es wesentlich, dass Sie die Aktive Directory-Datenbank und ihre Protokolldateien schützen.
  
Sie können die Dateien Ntds.dit, Edb.log und Temp.edb aus dem Standardspeicherort verschieben und damit vor einem Angreifer verbergen, der Zugriff auf einen Domänencontroller erlangt hat. Wenn Sie die Dateien vom Systemdatenträger entfernen und auf einem separaten physischen Datenträger speichern, erhalten Sie den zusätzlichen Vorteil einer verbesserten Leistung des Domänencontrollers.
  
Deshalb wird empfohlen, dass die Datenbank und die Protokolldateien von Active Directory für die Domänencontroller auf einem Stripeset-Datenträger bzw. gespiegelten Stripeset-Datenträger gespeichert werden, der kein Betriebssystem enthält. Diese Dateien sollten für alle drei in diesem Handbuch definierten Umgebungen verschoben werden.
  
##### Ändern der Größe von Active Directory-Protokolldateien
  
Um Integrität, Zuverlässigkeit und Verfügbarkeit von Active Directory effektiv zu überwachen und aufrechterhalten zu können, muss eine ausreichende Menge an Informationen protokolliert werden. Informationen von sämtlichen Domänencontrollern in der Umgebung sind erforderlich.
  
Sie können die maximale Größe der Protokolldateien erhöhen, um diese Bemühungen zu unterstützen. Mit mehr Protokollinformationen können Administratoren aussagekräftigere Analysen im Falle von Hacker-Angriffen durchführen.
  
In diesem Handbuch wird empfohlen, dass Sie die maximale Größe der Protokolldateien des Verzeichnisdienstes und des Dateireplikationsdienstes auf den Domänencontrollern in den drei in diesem Handbuch definierten Umgebungen von standardmäßig 512 KB auf 16 MB erhöhen.
  
##### Verwenden von Syskey
  
Auf Domänencontrollern werden Kennwortinformationen in Active Directory gespeichert. Software zum Entschlüsseln von Kennwörtern zielt häufig auf die Datenbank der Sicherheitskontenverwaltung (Security Accounts Manager, SAM) oder auf Verzeichnisdienste, um auf Kennwörter für Benutzerkonten zuzugreifen.
  
Das Systemschlüsseldienstprogramm (Syskey) bietet einen zusätzlichen Schutz vor offline-arbeitender Software zum Entschlüsseln von Kennwörtern. Syskey verwendet leistungsstarke Verschlüsselungsverfahren, um in der Sicherheitskontenverwaltung gespeicherte Kennwortinformationen zu schützen.
  
**Tabelle 5.9: Syskey-Modi**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Systemschlüsseloptionen</th>
<th style="border:1px solid black;" >Sicherheitsstufe</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Modus 1: Vom System generiertes Kennwort, Systemstartschlüssel lokal speichern</td>
<td style="border:1px solid black;">Sicher</td>
<td style="border:1px solid black;">Verwendet einen vom Computer generierten Zufallsschlüssel als Systemschlüssel und speichert eine verschlüsselte Version des Schlüssels auf dem lokalen Computer. Diese Option bietet eine leistungsstarke Verschlüsselung der Kennwortinformationen in der Registrierung und ermöglicht dem Benutzer das Neustarten des Computer, ohne das ein Administrator ein Kennwort eingeben oder eine Diskette einlegen muss.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Modus 2: Vom Administrator generiertes Kennwort, Kennwort für den Systemstart</td>
<td style="border:1px solid black;">Sicherer</td>
<td style="border:1px solid black;">Verwendet einen vom Computer generierten Zufallsschlüssel als Systemschlüssel und speichert eine verschlüsselte Version des Schlüssels auf dem lokalen Computer. Der Schlüssel wird zusätzlich durch einem Kennwort geschützt, das von einem Administrator gewählt wurde. Die Benutzer werden aufgefordert, das Systemschlüsselkennwort einzugeben, wenn sich der Computer in der ersten Startsequenz befindet. Das Systemschlüsselkennwort wird nicht auf dem Computer gespeichert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Modus 3: Vom System generiertes Kennwort, Systemstartschlüssel auf Diskette speichern</td>
<td style="border:1px solid black;">Am Sichersten</td>
<td style="border:1px solid black;">Verwendet einen vom Computer generierten Zufallsschlüssel und speichert den Schlüssel auf einer Diskette. Die Diskette mit dem Systemschlüssel ist für den Start des Computers erforderlich und muss während der Startsequenz bei Aufforderung eingegeben werden. Der Systemschlüssel wird nicht auf dem Computer gespeichert.</td>
</tr>
</tbody>
</table>
  
Syskey wird auf allen Windows Server 2003 SP1-Servern in Modus 1 aktiviert (verschleierter Schlüssel). Vom Sicherheitsstandpunkt aus erscheint diese Konfiguration zunächst vernünftig. Allerdings ermöglicht Syskey in Modus 1 einem Angreifer das Lesen und Verändern des Inhalts im Verzeichnis. Das macht den Domänencontroller anfällig für einen Angreifer mit physischem Zugriff.
  
Die Verwendung von Syskey in Modus 2 (Konsolenkennwort) oder Modus 3 (Diskettenspeicherung des Syskey-Kennworts) kann für jeden Domänencontroller empfohlen werden, der physischen Sicherheitsrisiken ausgesetzt ist. Der beim Betrieb u. U. erforderliche Neustart von Domänencontrollern erschwert jedoch die Unterstützung der Syskey-Modi 2 und 3. Um die Vorteile des zusätzlichen Schutzes nutzen zu können, der von diesen Syskey-Modi geboten wird, müssen die entsprechenden Betriebsprozesse in Ihre Umgebung implementiert werden, um bestimmte Verfügbarkeitsanforderungen für die Domänencontroller zu erfüllen.
  
Die Logistik der Syskey-Kennwortverwaltung oder -Diskettenverwaltung kann sehr komplex sein, vor allem in Zweigstellen. Es kann sich z. B. als ziemlich kostspielig erweisen, Zweigstellenleiter oder administrative Mitarbeiter um 3 Uhr morgens zu Zweigstelle zu beordern, um Kennwörter einzugeben oder um eine Diskette einzulegen, damit der Benutzerzugriff aktiviert wird. Solche kostspieligen Anforderungen können Service-Level-Vereinbarungen für hohe Verfügbarkeit zu einer großen Herausforderung werden lassen.
  
Die Möglichkeit, dass die IT-Mitarbeiter das Syskey-Kennwort von einem Remotestandort aus zur Verfügung stellen, macht dagegen zusätzliche Hardware erforderlich. Einige Hardwareanbieter bieten Zusatzlösungen an, die Remotezugriff auf Serverkonsolen ermöglichen.
  
Außerdem könnte der Domänencontroller bei Verlust des Syskey-Kennworts bzw. der Syskey–Diskette nicht mehr gestartet werden. Ein Domänencontroller kann nicht wiederhergestellt werden, wenn das Syskey-Kennwort oder die Syskey–Diskette verloren gegangen ist. In diesem Fall muss der Domänencontroller neu eingerichtet werden.
  
Syskey kann mit den entsprechenden Betriebsprozessen eine erhöhte Sicherheit bieten, um vertrauliche Verzeichnisinformationen auf Domänencontrollern zu schützen. Aus diesen Gründen werden Syskey-Modus 2 und 3 für Domänencontroller an Orten empfohlen, die physisch nicht gut gesichert sind. Diese Konfiguration gilt für Domänencontroller in allen drei in diesem Handbuch beschriebenen Umgebungen.
  
**So erstellen oder aktualisieren Sie einen Systemschlüssel**
  
1.  Klicken Sie auf **Start** und dann auf **Ausführen**, geben Sie **syskey** ein, und klicken Sie auf **OK**.
  
2.  Klicken Sie auf **Verschlüsselung aktiviert** und dann auf **Aktualisieren**.
  
3.  Klicken Sie auf die gewünschte Option und anschließend auf **OK**.
  
#### Active Directory-integriertes DNS
  
Microsoft empfiehlt in den drei in diesem Handbuch definierten Umgebungen den Einsatz von Active Directory-integriertem DNS. Einer der Gründe dafür liegt darin, dass die Integration der Active Directory-Zonen eine Sicherung der DNS-Infrastruktur in einer Umgebung mit Active Directory-integriertem DNS eher zulässt als in einer Umgebung, die kein Active Directory-integriertes DNS verwendet.
  
##### Schützen von DNS-Servern
  
Das Schützen der DNS-Server ist in jeder Active Directory-Umgebung von entscheidender Bedeutung. Die folgenden Abschnitten enthalten Empfehlungen und Erläuterungen zum Schützen von DNS-Servern.
  
Wenn ein DNS-Server angegriffen wird, ist ein mögliches Ziel des Angreifers die Kontrolle über die DNS-Informationen, die auf Abfragen von DNS-Clients zurückgegeben werden. Wenn ein Angreifer die Kontrolle über diese Informationen erlangt, können Clients unwissentlich an nicht autorisierte Computer weitergeleitet werden. Das IP-Spoofing und die Cache-Vergiftung sind Beispiele für diese Art von Angriff.
  
Beim IP-Spoofing wird einer Übertragung die IP-Adresse eines nicht autorisierten Benutzers gegeben, um Zugriff auf einen Computer oder ein Netzwerk zu erhalten. Bei der Cache-Vergiftung überträgt ein nicht autorisierter Host falsche Informationen bezüglich eines anderen Hosts in den Cache eines DNS-Servers. Der Angriff führt dazu, dass Clients an nicht autorisierte Computer weitergeleitet werden.
  
Wenn die Kommunikation von Clientcomputern mit nicht autorisierten Computern zugelassen wird, können nicht autorisierte Computer versuchen, auf Informationen auf den Clientcomputern zuzugreifen.
  
Nicht alle Angriffe verfolgen das Ziel des Spoofing von DNS-Servern. Einige DoS-Angriffe können die DNS-Einträge in zulässigen DNS-Servern verändern, um als Antwort auf Clientabfragen ungültige Adressen zu liefern. Wenn DNS-Server mit ungültigen Adressen antworten, können Clients und Server nicht die Ressourcen finden, die sie für den Betrieb benötigen, wie Domänencontroller, Webserver oder Dateifreigaben.
  
Deshalb sind die Router, die in den drei in diesem Handbuch definierten Umgebungen verwendet werden, so konfiguriert, dass sie durch Spoofing manipulierte IP-Pakete fallen lassen. Dadurch wird sichergestellt, dass die IP-Adressen von DNS-Servern nicht von anderen Computern durch Spoofing manipuliert werden.
  
##### Konfigurieren von sicheren dynamischen Updates
  
Der Dienst **DNS-Client** in Windows Server 2003 mit SP1 unterstützt dynamische DNS-Updates, wodurch Clientsysteme DNS-Einträge direkt in die Datenbank eingeben können. Wenn ein dynamischer DNS-Server so konfiguriert ist, dass er unsichere Updates akzeptiert, könnte ein Angreifer schädliche oder nicht autorisierte Updates von einem Clientcomputer senden, der das dynamische DNS-Updateprotokoll unterstützt.
  
Zumindest kann ein Angreifer der DNS-Datenbank falsche Einträge hinzufügen. Im schlimmsten Fall kann ein Angreifer zulässige Einträge in der DNS-Datenbank überschreiben oder löschen. Solch ein Angreifer könnte Folgendes bewirken:
  
-   **Clients werden an nicht autorisierte Domänencontroller weitergeleitet**. Wenn ein Client eine DNS-Abfrage sendet, in der er nach der Adresse eines Domänencontrollers sucht, kann ein beeinträchtigter DNS-Server angewiesen werden, die Adresse eines nicht autorisierten Servers zurückzugeben. Anschließend kann der Client mithilfe weiterer nicht DNS-bezogener Angriffe dazu verleitet werden, sichere Informationen an den falschen Server weiterzuleiten.
  
-   **DNS-Abfragen werden mit ungültigen Adressen beantwortet**. Clients und Server könnten einander dann nicht finden. Wenn Clients Server nicht finden können, können sie nicht auf das Verzeichnis zugreifen. Falls ein Domänencontroller andere Domänencontroller nicht finden kann, wird die Verzeichnisreplikation angehalten. Dies führt zu einem Denial-of-Service, der Auswirkungen auf Benutzer in einer Gesamtstruktur haben kann.
  
-   **Ein Denial-of-Service wird herbeigeführt**. Der Festplattenspeicher eines Servers kann durch eine große Zonendatei, die mit Dummy-Einträgen gefüllt ist, oder durch eine große Anzahl von Einträgen vollständig belegt sein, wodurch die Replikation verlangsamt wird.
  
Die Verwendung von sicheren dynamischen DNS-Aktualisierungen stellt sicher, dass Registrierungsabfragen nur verarbeitet werden, wenn sie von gültigen Clients in einer Active Directory-Gesamtstruktur gesendet werden. Durch diese Methode wird die Möglichkeit für einen Angreifer erheblich eingeschränkt, die Integrität eines DNS-Servers zu gefährden.
  
Aus diesen Gründen sind die Active Directory-DNS-Server in den drei in diesem Handbuch definierten Umgebungen so konfiguriert, dass sie nur sichere dynamische Updates akzeptieren.
  
##### Begrenzen von Zonenübertragungen zu autorisierten Systemen
  
Aufgrund der bedeutenden Rolle von Zonen in DNS sollten sie für mehr als einen DNS-Server im Netzwerk zur Verfügung stehen, um eine entsprechende Verfügbarkeit und Fehlertoleranz bei Anfragen zur Namensauflösung zu liefern. Beim Hosten einer Zone durch zusätzliche Server sind Zonenübertragungen erforderlich, um alle Kopien der Zone für jeden Server, der für das Hosten der Zone konfiguriert ist, zu replizieren und zu synchronisieren.
  
Ein DNS-Server, der nicht einschränkt, wer Zonenübertragungen anfordern kann, könnte die gesamte DNS-Zone an jeden übertragen, der dies anfordert. Diese Übertragung kann leicht mit Tools wie z. B. Nslookup.exe erreicht werden. Solche Tools können den gesamten DNS-Datensatz offen legen und damit z. B. verraten, welche Hosts als Domänencontroller, verzeichnisintegrierte Webserver oder Microsoft SQL Server™-Datenbanken dienen.
  
Aus diesen Gründen sind die Active Directory-integrierten DNS-Server in den drei in diesem Handbuch definierten Umgebungen so konfiguriert, dass Zonenübertragungen zugelassen werden, wobei jedoch eingeschränkt wird, welche Computer Übertragungsanforderungen stellen können.
  
##### Ändern der Größe des Ereignisprotokolls und des DNS-Dienstprotokolls
  
Es müssen genügend Informationen protokolliert werden, um die den DNS-Dienst effektiv überwachen und aufrechterhalten zu können. Informationen von sämtlichen Domänencontrollern in der Umgebung sind erforderlich.
  
Sie können die maximale Größe der Protokolldatei des DNS-Dienstes erhöhen, damit Administratoren im Falle eines Angriffs aussagekräftige Analysen durchführen können.
  
Es wird empfohlen, dass Sie die maximale Größe der Protokolldatei des DNS-Dienstes auf den Domänencontrollern in den drei in diesem Handbuch definierten Umgebungen auf mindestens 16 MB erhöhen. Stellen Sie auch sicher, dass die Option **Ereignisse bei Bedarf überschreiben** im DNS-Dienst ausgewählt ist, um die Anzahl der aufbewahrten Protokolleinträge zu maximieren.
  
#### Sichern von bekannten Konten
  
Windows Server 2003 mit SP1 verfügt über eine ganze Reihe von vordefinierten Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.
  
Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Daher sollten Sie das vordefinierte Administratorkonto umbenennen und seine Beschreibung ändern, damit sie Angriffen von Remoteservern vorbeugen und Angreifer dieses bekannte Konto nicht nutzen können.
  
Der Wert dieser Konfigurationsänderung hat sich in den letzten Jahren verringert, weil Angriffstools entwickelt wurden, mit denen über die SID (Sicherheits-ID) des vordefinierten Administratorkontos dessen wahrer Name ermittelt und somit Zugang zum Server erlangt werden kann. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf dieses Administratorkonto überwachen, wenn Sie es umbenennen und mit einem eindeutigen Namen versehen.
  
Führen Sie die folgenden Schritte aus, um bekannte Konten auf Domänen und Servern zu sichern:
  
-   Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie die zugehörigen Kennwörter zu langen und komplexen Werten.
  
-   Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server mit dem gleichen Kontonamen und -kennwort zugreifen.
  
-   Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.
  
-   Notieren Sie die vorgenommenen Änderungen, und bewahren Sie diese Informationen an einem sicheren Ort auf.
  
    **Hinweis**: Das vordefinierte Administratorkonto kann durch Gruppenrichtlinien umbenannt werden. Diese Richtlinieneinstellung wurde in den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen nicht implementiert, da jede Organisation Ihren eigenen eindeutigen Namen für dieses Konto auswählen sollte. Sie können jedoch die Einstellung **Konten: Administratorkonto umbenennen** so konfigurieren, dass Administratorkonten in den drei in diesem Handbuch definierten Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.
  
#### Sichern von Dienstkonten
  
Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx.
  
#### Einstellungen für Terminaldienste
  
**Tabelle 5.10: Empfohlene Einstellungen für Terminaldienste**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Standard</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Verschlüsselungsstufe der Clientverbindung festlegen</td>
<td style="border:1px solid black;">Hoch</td>
<td style="border:1px solid black;">Hoch</td>
<td style="border:1px solid black;">Hoch</td>
</tr>
</tbody>
</table>
  
Die Einstellung **Verschlüsselungsstufe der Clientverbindung festlegen** legt die Stufe der Verschlüsselung für Clientverbindungen von Terminaldiensten in der Umgebung fest. Die Option **Höchste Stufe** verwendet eine 128-Bit-Verschlüsselung und verhindert, dass ein Angreifer mithilfe von Paketanalysen Lauschangriffe auf Terminaldienstesitzungen durchführen kann. Einige ältere Versionen des Terminaldiensteclients unterstützen diese hohe Stufe der Verschlüsselung nicht. Wenn Ihr Netzwerk über solche Clients verfügt, setzen Sie die Verschlüsselungsstufe der Verbindung auf die höchste Stufe, die von diesen Clients beim Senden und Empfangen von Daten unterstützt wird.
  
Die Einstellung **Verschlüsselungsstufe der Clientverbindung festlegen** ist auf **Aktiviert** gesetzt, und in der DCBP für die drei in diesem Handbuch definierten Sicherheitsumgebungen ist die Verschlüsselungsoption **Höchste Stufe** ausgewählt.
  
Diese Richtlinieneinstellung kann unter Windows Server 2003 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\Windows-Komponenten\\**  
**Terminaldienste\\Verschlüsselung und Sicherheit**
  
Die drei verfügbaren Verschlüsselungsstufen werden in der folgenden Tabelle beschrieben:
  
**Tabelle 5.11: Verschlüsselungsstufen für Terminaldienste**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Verschlüsselungsstufe</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Höchste Stufe</td>
<td style="border:1px solid black;">Verschlüsselt die zwischen Client und Server übermittelten Daten mit einer leistungsfähigen 128-Bit-Verschlüsselung. Verwenden Sie diese Stufe, wenn der Terminalserver in einer Umgebung ausgeführt wird, die ausschließlich 128 Bit-Clients enthält (z. B. Clients mit Remotedesktopverbindung). Mit Clients, die diese Verschlüsselungsstufe nicht unterstützen, wird bei dieser Einstellung keine Verbindung hergestellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Clientkompatibel</td>
<td style="border:1px solid black;">Verschlüsselt die zwischen Client und Server übermittelten Daten mit der höchsten vom Client unterstützten Schlüsselstufe. Verwenden Sie diese Stufe, wenn der Terminalserver in einer Umgebung ausgeführt wird, die unterschiedliche bzw. ältere Clients enthält.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Niedrige Stufe</td>
<td style="border:1px solid black;">Verschlüsselt die vom Client zum Server gesendeten Daten mit einer 56-Bit-Verschlüsselung.
<strong>Wichtig</strong>: Vom Server an den Client gesendete Daten werden nicht verschlüsselt.</td>
</tr>
</tbody>
</table>
 

#### Fehlerberichterstattung

**Tabelle 5.12: Empfohlene Einstellungen für die Fehlerberichterstattung**

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Älterer Client</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
<th style="border:1px solid black;" >Hochsicher (SSLF)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Windows-Fehlerberichterstattung deaktivieren</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
Dieser Dienst hilft Microsoft bei der Erfassung und Behebung von Fehlern. Sie können diesen Dienst konfigurieren, um Berichte über Betriebssystemfehler, Windows-Komponentenfehler oder Programmfehler zu generieren. Er ist nur in Windows XP Professional und Windows Server 2003 verfügbar.
  
Mit dem Dienst **Fehlerberichterstattung** können solche Fehler über das Internet oder über eine interne Datenfreigabe Microsoft gemeldet werden. Obwohl Fehlerberichte sicherheitsrelevante oder sogar vertrauliche Daten enthalten können, wird durch die Microsoft-Datenschutzrichtlinie für die Fehlerberichterstattung sichergestellt, dass derartige Daten von Microsoft nicht zweckentfremdet werden. Die als Klartext-HTTP-Verkehr übertragenen Daten können jedoch im Internet abgefangen und von Dritten angezeigt werden.
  
Anhand der Einstellung zum **Deaktivieren der Windows**-**Fehlerberichterstattung** wird überwacht, ob der **Fehlerberichterstattungsdienst** Daten überträgt.
  
Diese Richtlinieneinstellung kann unter Windows Server 2003 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Administrative Vorlagen\\System\\Internetkommunikationsmanagement\\Internetkommunikationseinstellungen**
  
Setzen Sie die Einstellung zum Deaktivieren der **Windows**-**Fehlerberichterstattung** in der Domänencontroller-Baseline-Richtlinie für alle drei in diesem Handbuch definierten Umgebungen auf **Aktiviert**.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Erstellen der Richtlinie mithilfe des SCW
  
Zum Bereitstellen der notwendigen Sicherheitseinstellungen müssen Sie sowohl den Sicherheitskonfigurations-Assistenten (SCW) sowie die im Rahmen der herunterladbaren Version dieses Handbuchs verfügbaren Sicherheitsvorlagen verwenden, um eine Richtlinie für die Domänencontroller-Baseline zu erstellen.
  
Wenn Sie Ihre eigene Richtlinie erstellen, müssen Sie die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ überspringen. Diese Richtlinieneinstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den mit dem SCW konfigurierten Elementen haben.
  
Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie das Betriebssystem auf ähnlicher Hardware wie der bei der Bereitstellung verwendeten installieren, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.
  
**So erstellen Sie die Richtlinie für die Domänencontroller-Baseline (DCBP)**
  
Sie müssen zum Erstellen einer Richtlinie für die Domänencontroller-Baseline einen Computer verwenden, der als Domänencontroller konfiguriert ist. Sie können entweder einen vorhandenen Domänencontroller verwenden oder einen Referenzcomputer erstellen und diesen mit dem Dcpromo-Tool zum Domänencontroller machen. Die meisten Organisationen entscheiden sich jedoch dafür, keinen Domänencontroller zu ihrer Produktionsumgebung hinzuzufügen, weil sie dadurch u. U. gegen die vorhandene Sicherheitsrichtlinie verstoßen. Wenn Sie einen vorhandenen Domänencontroller verwenden, müssen Sie sicherstellen, dass Sie mit dem SCW keine Einstellungen auf ihn anwenden und dass Sie seine Konfiguration nicht ändern.
  
1.  Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.
  
2.  Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.
  
3.  Stellen Sie sicher, dass die ermittelten Serverrollen für Ihre Umgebung geeignet sind. Entfernen Sie nicht die Dateiserverrolle, da sie für den ordnungsgemäßen Betrieb der Domänencontroller erforderlich ist.
  
4.  Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.
  
5.  Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.
  
    **Hinweis**: Wenn Ihre Umgebung auf mehrere Standorte verteilte Domänencontroller enthält, stellen Sie sicher, dass die Option für die **Mail-basierte Active Directory-Replikation** ausgewählt ist.
  
6.  Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.
  
7.  Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.
  
8.  Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter**. Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.
  
    **Hinweis:** Stellen Sie sicher, dass die Option für die **Ports für RPC-Anwendungen des Systems** ausgewählt ist.
  
9.  Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
10. Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
11. Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. Unternehmensclient-Domänencontroller.inf).
  
12. Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Domänencontroller.xml**)**.
  
#### Testen der Richtlinie mithilfe des SCW
  
Nach dem Erstellen und Speichern der Richtlinie empfiehlt es sich unbedingt, sie in Ihrer Testumgebung bereitzustellen. Im Idealfall werden Ihre Testserver die gleiche Hardware- und Softwarekonfiguration wie Ihre Produktionsserver aufweisen. Mit diesem Ansatz können Sie mögliche Probleme, wie etwa das Vorhandensein unerwarteter Dienste, die von bestimmten Hardwaregeräten benötigt werden, ermitteln und beheben.
  
Zum Testen der Richtlinie gibt es zwei Möglichkeiten. Sie können die standardmäßigen SCW-Bereitstellungsgeräte verwenden oder mithilfe eines Gruppenrichtlinienobjekts Richtlinien anwenden.
  
Beim Verfassen der Richtlinien sollten Sie zunächst die Verwendung der standardmäßigen SCW-Bereitstellungsgeräte in Betracht ziehen. Sie können eine Richtlinie mit dem SCW jeweils auf einen einzelnen Server oder mithilfe von Scwcmd auf eine ganze Servergruppe anwenden. Die standardmäßige Bereitstellungsmethode bietet den Vorteil, dass bereitgestellte Richtlinien leicht vom SCW aus zurückgenommen werden können. Dies erweist sich als außerordentlich nützlich, wenn Sie im Testverfahren mehrere Änderungen an Ihren Richtlinien vornehmen.
  
Die Richtlinie wird getestet, um sicherzustellen, dass ihre Anwendung auf den Zielservern keine negativen Auswirkungen auf wichtige Funktionen hat. Nach Übernahme der Konfigurationsänderungen müssen Sie zunächst die Kernfunktionalität des Computers überprüfen. Ist der Server z. B. als Zertifizierungsstelle (CA) konfiguriert, müssen Sie sicherstellen, dass Clients Zertifikate anfordern und erhalten bzw. eine Zertifikatsperrliste herunterladen können usw.
  
Wenn Sie mit der Konfiguration von Richtlinien vertraut sind, können Sie Scwcmd verwenden, um wie im folgenden Verfahren veranschaulicht die Richtlinien in Gruppenrichtlinienobjekte umzuwandeln.
  
Weitere Informationen zum Testen von SCW-Richtlinien finden Sie im [Deployment Guide for the Security Configuration Wizard](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/scwdeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/SCWDeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx**sowie in der [Security Configuration Wizard Documentation](http://go.microsoft.com/fwlink/?linkid=43450) unter http://go.microsoft.com/fwlink/?linkid=43450 (jeweils in englischer Sprache).
  
#### Umwandeln und Bereitstellen der Richtlinie
  
Nachdem Sie die Richtlinie gründlich getestet haben, führen Sie folgende Schritte aus, um sie in ein Gruppenrichtlinienobjekt umzuwandeln und bereitzustellen:
  
1.  Geben Sie an der Eingabeaufforderung folgenden Befehl ein:
  
    ```  
 scwcmd transform /p:&lt;PathToPolicy.xml&gt; /g:&lt;GPODisplayName&gt;  
```
  
    und drücken Sie anschließend die Eingabetaste. Beispiel:
  
    ```  
 scwcmd transform /p:"C:\\Windows\\Security\\msscw\\Policies\\Domain Controller.xml" /g:"Domain Controller Policy"  
```
  
    **Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.
  
2.  Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der Domänencontroller-Organisationseinheit und stellen Sie sicher, dass es sich oberhalb der Standarddomänencontrollerrichtlinie befindet, damit es höchste Priorität erhält.
  
Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall**.
  
Bedenken Sie, dass es eine Weile dauern kann, bis das neu erstellte Gruppenrichtlinienobjekt auf allen Domänencontrollern repliziert ist, besonders in Umgebungen mit Domänencontrollern an mehreren Standorten. Nachdem Sie sich von der erfolgreichen Replikation des Gruppenrichtlinienobjekts überzeugt haben, sollten Sie einen abschließenden Test durchführen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Richtlinieneinstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Einstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurde erklärt, wie Domänencontrollerserver, auf denen Windows Server 2003 mit SP1 ausgeführt wird, in allen drei in diesem Handbuch definierten Umgebungen abgesichert werden. Die meisten erläuterten Richtlinieneinstellungen wurden durch Gruppenrichtlinien konfiguriert und angewendet. Die Richtlinie für die Domänencontroller-Baseline (DCBP), die die Standarddomänencontrollerrichtlinie ergänzt, wurde mit der Domänencontroller-Organisationseinheit verknüpft.
  
Die DCBP-Einstellungen verbessern die Gesamtsicherheit der Domänencontroller in beliebigen Umgebungen. Durch Verwenden von zwei Gruppenrichtlinienobjekten für das Sichern von Domänencontrollern kann die Standardumgebung erhalten bleiben, und die Problembehandlung wird vereinfacht.
  
Einige der hier erläuterten Einstellungen können nicht mithilfe von Gruppenrichtlinien angewendet werden. Für diese Einstellungen wurden Informationen für die manuelle Konfiguration bereitgestellt.
  
Nachdem die Domänencontroller für Sicherheit konfiguriert sind, können andere Serverrollen besser geschützt werden. In den folgenden Kapiteln dieses Handbuchs wird der Schwerpunkt auf den Schutz einiger anderer spezifischer Serverrollen gelegt.
  
#### Weitere Informationen
  
Die folgenden Links bieten zusätzliche Informationen zur Absicherung von Domänencontrollern, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
  
-   Informationen zu den MSA EDC-Vorschriftenhandbüchern zur Systemarchitektur (Microsoft Systems Architecture: Enterprise Data Center) finden Sie auf der Seite [MSA EDC-Vorschriftenhandbüchern zur Systemarchitektur](http://www.microsoft.com/resources/documentation/msa/edc/all/solution/en-us/pak/pag/default.mspx) (in englischer Sprache) unter www.microsoft.com/resources/documentation/msa/edc/all/solution/en-us/pak/pag/default.mspx.
  
-   Informationen zum Aktivieren des anonymen Zugriffs auf Active Directory finden Sie im Microsoft Knowledge Base-Artikel [Beschreibung der Dcpromo-Berechtigungsoptionen](http://support.microsoft.com/kb/257988/en-us) (in englischer Sprache) unter http://support.microsoft.com/kb/257988/en-us.
  
-   Informationen zum Windows 2000-DNS finden Sie im Whitepaper [Windows 2000-DNS](http://www.microsoft.com/windows2000/techinfo/howitworks/communications/nameadrmgmt/w2kdns.asp) (in englischer Sprache) unter www.microsoft.com/windows2000/techinfo/howitworks/communications/nameadrmgmt/w2kdns.asp.
  
-   Weitere Informationen zum Windows 2000-DNS finden Sie in Kapitel 6 der Online-Version des [Handbuch für TCP/IP-Netzwerke](http://www.microsoft.com/windows2000/techinfo/reskit/en-us/default.asp) (in englischer Sprache) im Windows 2000 Server Resource Kit unter www.microsoft.com/windows2000/techinfo/reskit/en-us/default.asp.
  
-   Informationen zum Windows 2003-DNS finden Sie auf der Seite [Änderungen im DNS in Windows Server 2003](http://www.microsoft.com/windows2000/technologies/communications/dns/dns2003.asp) (in englischer Sprache) unter www.microsoft.com/windows2000/technologies/communications/dns/dns2003.asp.
  
-   Informationen zum Einschränken von Active Directory finden Sie im Microsoft Knowledge Base-Artikel „[Einschränken von Active Directory-Replikationsverkehr an einem bestimmten Port](http://support.microsoft.com/kb/224196/en-us)“ unter http://support.microsoft.com/kb/224196/en-us.
  
-   Weitere Informationen zum Einschränken des FRS-Replikationsverkehrs finden Sie im Microsoft Knowledge Base-Artikel „[Einschränken des FRS-Replikationsverkehrs auf einen bestimmten statischen Port](http://support.microsoft.com/kb/319553/en-us)“ (in englischer Sprache) unter http://support.microsoft.com/kb/319553/en-us.
  
-   Weitere Informationen zum Windows-Zeitdienst finden Sie im Artikel [Technische Informationen zum Windows-Zeitdienst](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/techref/a0fcd250-e5f7-41b3-b0e8-240f8236e210.mspx) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/TechRef/a0fcd250-e5f7-41b3-b0e8-240f8236e210.mspx.
  
-   Weitere Informationen zum IP-Spoofing finden Sie im Artikel [Einführung in das IP-Spoofing](http://www.giac.org/practical/gsec/victor_velasco_gsec.pdf) (in englischer Sprache) unter www.giac.org/practical/gsec/Victor\_Velasco\_GSEC.pdf.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/sgch00.mspx)  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch01.mspx)  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch02.mspx)  
-   [Kapitel 3: Die Domänenrichtlinie](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch03.mspx)  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch04.mspx)  
-   Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline  
-   [Kapitel 6: Die Infrastrukturserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch06.mspx)  
-   [Kapitel 7: Die Dateiserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch07.mspx)  
-   [Kapitel 8: Die Druckserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch08.mspx)  
-   [Kapitel 9: Die Webserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch09.mspx)  
-   [Kapitel 10: Die IAS-Serverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch10.mspx)  
-   [Kapitel 11: Die Zertifikatdienstserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch11.mspx)  
-   [Kapitel 12: Die Bastion-Hostrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch12.mspx)  
-   [Kapitel 13: Zusammenfassung](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch13.mspx)  
-   [Anhang A: Sicherheitstools und Formate](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxa.mspx)  
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxb.mspx)  
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxc.mspx)  
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgapxd.mspx)  
-   [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgack.mspx)
  
**Download**
  
[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)
  
**Benachrichtigung über Neuerungen**
  
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
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch04.mspx"><img src="images/Dd443726.pageLeft(de-de,TechNet.10).gif" /></a> 6 von 19 <a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch06.mspx"><img src="images/Dd443726.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
