---
TOCTitle: 'Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients'
Title: 'Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients'
ms:assetid: 'bca34b8d-a1ca-42e4-b743-aa3ca12fd8f9'
ms:contentKeyID: 20072363
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc163074(v=TechNet.10)'
---

Windows XP-Sicherheitshandbuch
==============================

### Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients

Aktualisiert: 20.10.2005

##### Auf dieser Seite

[](#enaa)[Überblick](#enaa)
[](#emaa)[Einstellungen für Kontorichtlinien](#emaa)
[](#elaa)[Einstellungen für lokale Richtlinien](#elaa)
[](#ekaa)[Einstellungen für Überwachungsrichtlinien](#ekaa)
[](#ejaa)[Einstellungen zum Zuweisen von Benutzerrechten](#ejaa)
[](#eiaa)[Einstellungen der Sicherheitsoptionen](#eiaa)
[](#ehaa)[Sicherheitseinstellungen für das Ereignisprotokoll](#ehaa)
[](#egaa)[Eingeschränkte Gruppen](#egaa)
[](#efaa)[Systemdienste](#efaa)
[](#eeaa)[Zusätzliche Registrierungseinstellungen](#eeaa)
[](#edaa)[Ändern der Benutzeroberfläche des Sicherheitskonfigurations-Editors](#edaa)
[](#ecaa)[Zusätzliche Sicherheitseinstellungen](#ecaa)
[](#ebaa)[Sichern des Dateisystems](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

In diesem Kapitel werden ausführlich die primären Sicherheitseinstellungen beschrieben, die unter Microsoft® Windows® 2000 oder Windows Server™ 2003 in einer Active Directory®-Verzeichnisdienstdomäne durch Gruppenrichtlinien konfiguriert werden. Implementieren Sie die empfohlenen Richtlinieneinstellungen, um sicherzustellen, dass die Desktop- und Laptopcomputer in Ihrer Organisation, auf denen Microsoft Windows XP Professional mit Service Pack 2 (SP2) ausgeführt wird, sicher konfiguriert sind. Nicht für alle verfügbaren Richtlinieneinstellungen in Windows XP stehen Anleitungen zur Verfügung, sondern nur für jene, die direkt für die Sicherheit des Computers relevant sind.

Wie in Kapitel 1, „Einführung zum Sicherheitshandbuch für Windows XP“, beschrieben, gelten die in diesem Kapitel vorgestellten Anleitungen speziell für die in diesem Handbuch definierten Unternehmensclient- und Hochsicherheitsumgebungen. In einigen Fällen werden in diesem Kapitel Richtlinieneinstellungen für Laptops empfohlen, die sich von denen für Desktopcomputer unterscheiden. Tragbare Computer sind beweglich und nicht immer über das Netzwerk Ihrer Organisation mit Domänencontrollern in Ihrer Umgebung verbunden. Außerdem wird davon ausgegangen, dass Laptopbenutzer gelegentlich zu abweichenden Zeiten arbeiten, wenn vor Ort kein technischer Support zur Verfügung steht. Daher werden für Laptopclientcomputer andere Optionen verwendet, wenn Richtlinieneinstellungen beispielsweise eine Verbindung mit einem Domänencontroller erfordern oder Auswirkungen auf die zulässigen Anmeldezeiten haben.

Richtlinieneinstellungen, die nicht für bestimmte Umgebungen festgelegt sind, werden manchmal auf Domänenebene definiert. Dies wird in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, beschrieben. Andere Richtlinieneinstellungen, die in diesem Kapitel als **Nicht definiert** aufgeführt sind, werden auf diese Weise behandelt, da die Sicherheit der Standardeinstellung für diese spezielle Umgebung ausreicht. Außerdem erleichtern nicht definierte Richtlinieneinstellungen in diesen Gruppenrichtlinienobjekten (GPOs) die Bereitstellung von Anwendungen, die während der Installation Einstellungen ändern müssen. Tools für das Unternehmensmanagement müssen z. B. den lokalen Dienstkonten auf verwalteten Computern ggf. bestimmte Benutzerrechte zuweisen. Die Anleitung in diesem Kapitel besteht aus Empfehlungen. Sie sollten stets sorgfältig Ihre Geschäftsanforderungen ermitteln, bevor Sie Änderungen an Ihrer Umgebung vornehmen.

In der folgenden Tabelle werden die in dieser Anleitung verfügbaren Infrastrukturdateien (.inf-Dateien) definiert. In diesen Dateien sind alle empfohlenen Baseline-Sicherheitseinstellungen für die beiden in diesem Kapitel behandelten Umgebungen enthalten.

**Tabelle 3.1: Baseline-Sicherheitsvorlagen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Beschreibung</p></th>
<th><p>Unternehmensclient</p></th>
<th><p>Hochsicher</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Baseline-Sicherheitsvorlagen für Desktops</p></td>
<td style="border:1px solid black;"><p>Unternehmensclient - Desktop.inf</p></td>
<td style="border:1px solid black;"><p>Hochsicher - Desktop.inf</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Baseline-Sicherheitsvorlagen für Laptops</p></td>
<td style="border:1px solid black;"><p>Unternehmensclient - Laptop.inf</p></td>
<td style="border:1px solid black;"><p>Hochsicher - Laptop.inf</p></td>
</tr>  
</tbody>  
</table>
  
Ausführlichere Informationen zu den in diesem Kapitel behandelten Richtlinieneinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx heruntergeladen werden kann.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen für Kontorichtlinien
  
Informationen zur Einstellungen für Kontorichtlinien werden in diesem Kapitel nicht bereitgestellt. Diese Einstellungen werden in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, dieses Handbuchs behandelt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen für lokale Richtlinien
  
Einstellungen für lokale Richtlinien können über die Konsole „Lokale Sicherheitsrichtlinie“ oder mithilfe domänenbasierter Gruppenrichtlinienobjekten in Active Directory für alle Computer konfiguriert werden, auf denen Windows XP Professional ausgeführt wird. Zu den Einstellungen für lokale Richtlinien gehören Überwachungsrichtlinien, das Zuweisen von Benutzerrechten und Sicherheitsoptionen.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen für Überwachungsrichtlinien
  
Durch eine Überwachungsrichtlinie wird festgelegt, bei welchen Sicherheitsereignissen die Administratoren benachrichtigt werden, sodass Benutzer- und Systemaktivitäten in festgelegten Ereigniskategorien aufgezeichnet werden können. Der Administrator kann dann die sicherheitsrelevanten Aktivitäten überwachen. Dazu gehört z. B. die Überwachung der für Objektzugriffe verwendeten Konten, der An- und Abmeldezeiten der Benutzer oder der Änderungen, die an den Einstellungen der Überwachungsrichtlinien vorgenommen werden. Aus diesen Gründen wird das Erstellen einer Überwachungsrichtlinie empfohlen, die der Administrator in Ihrer Umgebung implementieren kann.
  
Bevor Sie jedoch eine Überwachungsrichtlinie implementieren, müssen Sie entscheiden, welche Ereigniskategorien in Ihrer Umgebung überwacht werden sollen. Die Überwachungsrichtlinie durch die Überwachungseinstellungen definiert, die in den Ereigniskategorien ausgewählt werden. Wenn Sie Überwachungseinstellungen für bestimmte Ereigniskategorien definieren, kann ein Administrator eine Überwachungsrichtlinie erstellen, die den Sicherheitsanforderungen Ihrer Organisation genügt.
  
Wenn keine Überwachungseinstellungen konfiguriert werden, ist es schwierig bzw. unmöglich, die genauen Umstände einer Sicherheitsverletzung zu bestimmen. Werden die Überwachungseinstellungen jedoch so konfiguriert, dass für zu viele autorisierte Aktivitäten Ereignisse produziert werden, sind die Sicherheitsereignisprotokolle schnell mit unnötigen Daten überfüllt. Anhand der Informationen in den folgenden Abschnitten können Sie entscheiden, was überwacht werden soll und wie relevante Überwachungsdaten für Ihre Organisation gesammelt werden.
  
Die Einstellungen für Überwachungsrichtlinien unter Windows XP können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Überwachungsrichtlinie**
  
In der folgenden Tabelle sind die Empfehlungen für Einstellungen für Überwachungsrichtlinien sowohl für Desktop- als auch Laptopclientcomputer in den beiden sicheren Umgebungen zusammengefasst, die in diesem Kapitel behandelt werden. Die Unternehmensclient-Umgebung wird zuweilen mit EC (Enterprise Client) und die Hochsicherheitsumgebung mit SSLF (Specialized Security – Limited Functionality) abgekürzt. Sie sollten diese Empfehlungen überprüfen und an die Gegebenheiten Ihrer Organisation anpassen. Seien Sie bei den Überwachungseinstellungen jedoch besonders vorsichtig, da sie einen erheblichen Datenverkehr erzeugen können. Wenn Sie z. B. für die Option **Rechteverwendung überwachen** Erfolgs- oder Fehlerüberwachung aktivieren, werden so viele Überwachungsereignisse erzeugt, dass es nicht mehr möglich ist, andere Arten von Einträgen im Sicherheitsereignisprotokoll zu finden. Eine solche Konfiguration könnte auch beträchtliche Auswirkungen auf die Leistung haben. Ausführlichere Informationen zu jeder Einstellung finden Sie in den folgenden Unterabschnitten.
  
**Tabelle 3.2: Empfohlene Einstellungen für Überwachungsrichtlinien**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Anmeldeversuche überwachen</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Kontenverwaltung überwachen</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Active Directory-Zugriff überwachen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Anmeldeereignisse überwachen</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
<td style="border:1px solid black;"><p>Erfolg, Fehler</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Objektzugriffsversuche überwachen</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Fehler</p></td>
<td style="border:1px solid black;"><p>Fehler</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Richtlinienänderungen überwachen</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Rechteverwendung überwachen</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Fehler</p></td>
<td style="border:1px solid black;"><p>Fehler</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Prozessverfolgung überwachen</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
<td style="border:1px solid black;"><p>Keine Überwachung</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Systemereignisse überwachen</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
<td style="border:1px solid black;"><p>Erfolg</p></td>
</tr>  
</tbody>  
</table>
  
#### Anmeldeversuche überwachen
  
Wenn diese Richtlinieneinstellung aktiviert ist, werden Ereignisse zur Prüfung von Anmeldeinformationen erzeugt. Diese Ereignisse finden auf dem Computer statt, der für die Anmeldeinformationen autorisierend ist. Für Domänenkonten ist der Domänencontroller autorisierend, und für lokale Konten der lokale Computer. In Domänenumgebungen finden die meisten Kontoanmeldeereignisse im Sicherheitsprotokoll der Domänencontroller statt, die für die Domänenkonten autorisierend sind. Diese Ereignisse können jedoch in Abhängigkeit von den zur Anmeldung verwendeten Konten auch auf anderen Computern in der Organisation stattfinden.
  
In dieser Anleitung ist die Einstellung **Anmeldeversuche überwachen** für die Unternehmensclient-Umgebung auf **Erfolg** und für die Hochsicherheitsumgebung auf **Erfolg** und **Fehler** gesetzt.
  
#### Kontenverwaltung überwachen
  
Mit dieser Richtlinieneinstellung kann jeder Versuch überwacht werden, neue Benutzer oder Gruppen zu erstellen, Benutzer oder Gruppen umzubenennen, Benutzerkonten zu aktivieren oder zu deaktivieren, Kontokennwörter zu ändern oder die Überwachung der Kontenverwaltung zu aktivieren. Wenn Sie diese Einstellung für Überwachungsrichtlinien aktivieren, können Administratoren Ereignisse überwachen, um die böswillige, zufällige und autorisierte Erstellung von Benutzer- und Gruppenkonten zu erkennen.
  
Die Einstellung **Kontoverwaltung überwachen** ist für die Unternehmensclient-Umgebung auf **Erfolg** und für die Hochsicherheitsumgebung auf **Erfolg** und **Fehler** gesetzt.
  
#### Active Directory-Zugriff überwachen
  
Diese Richtlinieneinstellung kann nur aktiviert werden, um Überwachungsaufgaben auf Domänencontrollern durchzuführen. Daher ist die Einstellung für Arbeitsstationen nicht definiert. Diese Richtlinieneinstellung gilt nicht für Computer mit Windows XP Professional. Stellen Sie deshalb sicher, dass die Einstellung **Active Directory-Zugriff überwachen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Nicht definiert** gesetzt ist.
  
#### Anmeldeereignisse überwachen
  
Diese Richtlinieneinstellung sorgt dafür, dass Ereignisse erzeugt werden, die die Erstellung und Zerstörung von Anmeldesitzungen aufzeichnen. Diese Ereignisse finden auf dem Computer statt, auf den zugegriffen wird. Bei interaktiven Anmeldungen würden diese Ereignisse auf dem Computer erzeugt, an dem die Anmeldung stattfand. Wenn eine Netzwerkanmeldung durchgeführt wird, um auf eine Freigabe zuzugreifen, werden diese Ereignisse auf dem Computer erzeugt, auf dem sich die Ressource befindet, auf die zugegriffen wurde.
  
Wenn Sie die Einstellung **Anmeldeereignisse überwachen** auf **Keine Überwachung** setzen, ist es schwierig bzw. unmöglich festzustellen, welcher Benutzer auf Computer in der Organisation zugegriffen oder zuzugreifen versucht hat.
  
In der Unternehmensclient-Umgebung ist die Einstellung **Anmeldeereignisse überwachen** so konfiguriert, dass Ereignisse des Typs **Erfolg** protokolliert werden. In der Hochsicherheitsumgebung ist diese Richtlinieneinstellung so konfiguriert, dass Ereignisse der Typen **Erfolg** und **Fehler** protokolliert werden.
  
#### Objektzugriffsversuche überwachen
  
Diese Richtlinieneinstellung allein führt nicht zur Überwachung von Ereignissen. Durch sie wird festgelegt, ob überwacht wird, ob ein Benutzer auf ein Objekt zugreift (z. B. eine Datei, einen Ordner, einen Registrierungsschlüssel oder einen Drucker), für das eine Systemzugriffssteuerungsliste (SACL) festgelegt wurde.
  
Eine SACL besteht aus Zugriffssteuerungseinträgen (ACEs). Jeder ACE enthält drei Informationen:
  
-   Den zu überwachenden Sicherheitsprinzipal (Benutzer, Computer oder Gruppe)
  
-   Den zu überwachenden Zugriffstyp (bezeichnet als Zugriffsmaske)
  
-   Ein Flag, das angibt, ob fehlgeschlagene Zugriffsereignisse, erfolgreiche Zugriffsereignisse oder beide Ereignistypen überwacht werden sollen
  
Wenn Sie die Einstellung **Objektzugriffsversuche überwachen** auf **Erfolg** setzen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn ein Benutzer erfolgreich auf ein Objekt mit definierter SACL zugreift. Wenn Sie diese Richtlinieneinstellung auf **Fehler** setzen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn ein Benutzer erfolglos versucht, auf ein Objekt mit definierter SACL zuzugreifen.
  
Organisationen sollten beim Konfigurieren von SACLs nur jene Aktionen definieren, die aktiviert sein sollen. Es kann z. B. sein, dass Sie die Überwachungseinstellung **Daten schreiben und Daten anhängen** für ausführbare Dateien aktivieren möchten, um Ersetzungen oder Änderungen dieser Dateien zu überwachen, weil Viren, Würmer und Trojaner meist ausführbare Dateien angreifen. Ebenso können Sie Änderungen an wichtigen Dokumenten oder den Zugriff auf solche Dokumente überwachen.
  
Die Einstellung **Objektzugriffsversuche überwachen** ist in der Unternehmensclient-Umgebung auf **Keine Überwachung** und in der Hochsicherheitsumgebung auf **Fehler** gesetzt. Sie müssen diese Einstellung aktivieren, damit die folgenden Verfahren wirksam werden.
  
Im Folgenden wird die manuelle Einrichtung von Überwachungsregeln für eine Datei oder einen Ordner beschrieben. Anschließend wird erklärt, wie die Überwachungsregeln für jedes Objekt in der angegebenen Datei oder dem Ordner getestet werden können. Das Testverfahren kann mithilfe einer Skriptdatei automatisiert werden.
  
**So definieren Sie eine Überwachungsregel für eine Datei oder einen Ordner**
  
1.  Suchen Sie die Datei in Windows Explorer, und wählen Sie sie aus.
  
2.  Klicken Sie im Menü **Datei** auf **Eigenschaften**.
  
3.  Wechseln Sie zur Registerkarte **Sicherheit**, und klicken Sie auf die Schaltfläche **Erweitert**.
  
4.  Klicken Sie auf die Registerkarte **Überwachung**.
  
5.  Klicken Sie auf die Schaltfläche **Hinzufügen**. Das Dialogfeld **Benutzer, Computer oder Gruppe wählen** wird angezeigt.
  
6.  Klicken Sie auf die Schaltfläche **Objekttypen**, und wählen Sie anschließend im Dialogfeld **Objekttypen** die zu suchenden Objekttypen aus.
  
    **Hinweis**: Die Objekttypen „Benutzer“, „Gruppe“ und „Integriertes Sicherheitsprinzipal“ sind in der Standardeinstellung bereits ausgewählt.
  
7.  Klicken Sie auf die Schaltfläche **Pfade...**, und wählen Sie im Dialogfeld **Pfad** entweder Ihre Domäne oder Ihren lokalen Computer aus.
  
8.  Geben Sie im Dialogfeld **Benutzer oder Gruppe wählen** den Namen der zu überwachenden Gruppe bzw. des Benutzers ein. Geben Sie anschließend im Feld **Geben Sie die zu verwendenden Objektnamen ein** den Text **Authentifizierte Benutzer** ein, um die Zugriffe aller authentifizierten Benutzer zu überwachen, und klicken Sie auf **OK**. Das Dialogfeld **Überwachungseintrag** wird angezeigt.
  
9.  Geben Sie im Dialogfeld **Überwachungseintrag** an, welche Zugriffe auf die Datei oder den Ordner überwacht werden sollen.
  
    **Hinweis**: Beachten Sie, dass durch jeden Zugriff mehrere Ereignisse im Ereignisprotokoll erzeugt werden können und dass das Protokoll entsprechend schnell anwächst.
  
10. Wählen Sie im Dialogfeld **Überwachungseintrag** neben **Ordner auflisten / Daten lesen** die Option **Erfolgreich und Fehlgeschlagen** aus, und klicken Sie auf **OK**.
  
11. Die aktivierten Überwachungseinträge werden im Dialogfeld **Erweiterte Sicherheitseinstellungen** auf der Registerkarte **Überwachung** angezeigt.
  
12. Klicken Sie zum Schließen des Dialogfelds **Eigenschaften** auf **OK**.
  
**So überprüfen Sie eine Überwachungsregel für eine Datei oder einen Ordner**
  
1.  Öffnen Sie die Datei oder den Ordner.
  
2.  Schließen Sie die Datei oder den Ordner.
  
3.  Starten Sie die Ereignisanzeige. Im Sicherheitsereignisprotokoll werden mehrere Objektzugriffsereignisse mit der **Ereignis-ID 560** angezeigt.
  
4.  Doppelklicken Sie auf ein Ereignis, um die zugehörigen Detailinformationen anzuzeigen.
  
#### Richtlinienänderungen überwachen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob sämtliche Änderungen in den Zuweisungsrichtlinien von Benutzerrechten, den Richtlinien der Windows-Firewall, den Vertrauensrichtlinien oder den Überwachungsrichtlinien selbst überwacht werden sollen. Die empfohlenen Einstellungen ermöglichen das Anzeigen aller Kontenberechtigungen, die ein Angreifer zu erhöhen versucht, indem er z. B. die Berechtigung **Debuggen von Programmen** oder **Sichern von Dateien und Verzeichnissen** hinzufügt.
  
Die Einstellung **Richtlinienänderungen überwachen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Erfolg** gesetzt. Der Einstellungswert für **Fehler** ist nicht enthalten, da dieser keine sinnvollen Zugriffsinformationen im Sicherheitsereignisprotokoll bereitstellt.
  
#### Rechteverwendung überwachen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob jede Ausübung eines Benutzerrechts durch Benutzer überwacht wird. Wenn Sie diesen Wert auf **Erfolg** einstellen, wird bei jeder erfolgreichen Ausübung eines Benutzerrechts ein Überwachungseintrag erzeugt. Wenn Sie diesen Wert auf **Fehler** einstellen, wird jedes Mal ein Überwachungseintrag erzeugt, wenn die Ausübung eines Benutzerrechts fehlschlägt. Diese Richtlinieneinstellung kann bewirken, dass eine sehr große Anzahl von Ereignisdatensätzen erzeugt wird.
  
Die Einstellung **Rechteverwendung überwachen** ist für Computer in der Unternehmensclient-Umgebung auf **Keine Überwachung** und für die Hochsicherheitsumgebung auf **Fehler** gesetzt, damit alle fehlgeschlagenen Versuche, zusätzliche Rechte zu verwenden, überwacht werden können.
  
#### Prozessverfolgung überwachen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob detaillierte Überwachungsinformationen für Ereignisse wie Programmaktivierung, Prozessbeendigung, Handleduplizierung und indirekter Objektzugriff erfasst werden. Da bei Aktivierung von **Prozessverfolgung überwachen** eine große Anzahl von Ereignissen erzeugt wird, wird normalerweise die Einstellung **Keine Überwachung** verwendet. Diese Einstellung kann jedoch aufgrund des detaillierten Protokolls zu gestarteten Prozessen und zugehörigen Startzeiten von großem Vorteil sein, wenn auf Zwischenfälle reagiert werden muss.
  
Die Einstellung **Prozessverfolgung überwachen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Keine Überwachung** gesetzt.
  
#### Systemereignisse überwachen
  
Diese Richtlinieneinstellung ist sehr wichtig, da auf diese Weise erfolgreiche und fehlgeschlagene Systemereignisse überwacht werden können. Anhand der Ereigniseinträge können daraufhin nicht autorisierte Systemzugriffe identifiziert werden. Zu Systemereignissen gehören das Starten und Herunterfahren von Computern in der Umgebung, zu große Ereignisprotokolldateien oder andere die Sicherheit betreffende Ereignisse mit Auswirkungen auf das gesamte System.
  
Die Einstellung **Systemereignisse überwachen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Erfolg** gesetzt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen zum Zuweisen von Benutzerrechten
  
In Verbindung mit vielen der privilegierten Gruppen von Windows XP Professional können bestimmten Benutzern oder Gruppen einige Benutzerrechte zugewiesen werden, über die die meisten Benutzer nicht verfügen.
  
Um den Wert eines Benutzerrechts auf **Niemand** zu setzen, aktivieren Sie die Einstellung, ohne ihr jedoch Benutzer oder Gruppen hinzuzufügen. Um den Wert eines Benutzerrechts auf **Nicht definiert** zu setzen, aktivieren Sie die Einstellung nicht.
  
Die Einstellungen zum Zuweisen von Benutzerrechten können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Zuweisen von Benutzerrechten**
  
In der folgenden Tabelle sind Empfehlungen für die Einstellungen zum Zuweisen von Benutzerrechten zusammengefasst, deren englische Bezeichnungen mit den Buchstaben A bis E beginnen. Empfehlungen werden sowohl für Desktop- als auch für Laptopclientcomputer in den beiden sicheren Umgebungen geboten, die in diesem Kapitel behandelt werden. Ausführlichere Informationen zu jeder Einstellung finden Sie in den folgenden Unterabschnitten.
  
Empfehlungen für Benutzerrechte, deren englisch Bezeichnungen mit den verbleibenden Buchstaben des Alphabets beginnen, sind in Tabelle 3.4 zusammengefasst. Weitere Informationen zu diesen Benutzerrechten finden Sie in den Unterabschnitten im Anschluss an die Tabelle.
  
**Hinweis**: Viele Funktionen in Internet Information Server (IIS) erfordern, dass bestimmte Konten wie zum Beispiel IIS\_WPG, IIS* *IUSR\_*&lt;Computername&gt;* und IWAM\_*&lt;Computername&gt;* über bestimmte Berechtigungen verfügen. Weitere Informationen dazu, welche Benutzerrechte für Konten erforderlich sind, die mit IIS in Zusammenhang stehen, finden Sie unter „[IIS und vordefinierte Konten (IIS 6.0)“](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/iis/3648346f-e4f5-474b-86c7-5a86e85fa1ff.mspx) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/WindowsServer2003/Library/  
IIS/3648346f-e4f5-474b-86c7-5a86e85fa1ff.mspx.
  
#### Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben A bis E beginnen
  
**Tabelle 3.3: Empfehlungen für Einstellungen zum Zuweisen von Benutzerrechten – Teil 1**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Auf diesen Computer vom Netzwerk aus zugreifen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Einsetzen als Teil des Betriebssystems</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Anpassen von Speicherkontingenten für einen Prozess</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren, Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Administratoren, Lokaler Dienst, Netzwerkdienst</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Lokal anmelden zulassen</p></td>
<td style="border:1px solid black;"><p>Benutzer, Administratoren</p></td>
<td style="border:1px solid black;"><p>Benutzer, Administratoren</p></td>
<td style="border:1px solid black;"><p>Benutzer, Administratoren</p></td>
<td style="border:1px solid black;"><p>Benutzer, Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Anmeldung über Terminaldienste zulassen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Sichern von Dateien und Verzeichnissen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Auslassen der durchsuchenden Prüfung</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Ändern der Systemzeit</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Auslagerungsdatei erstellen</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Permanente freigegebene Objekte erstellen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Erstellen eines Tokenobjekts</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Debuggen von Programmen</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Den Zugriff auf diesen Computer vom Netzwerk aus verweigern</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Anmeldung als Batchauftrag verweigern</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lokal anmelden verweigern</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0,<br />
Gast, beliebige Dienstkonten</p></td>
<td style="border:1px solid black;"><p>Support_<br />
388945a0, Gast, beliebige Dienstkonten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Anmeldung über Terminaldienste verweigern</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Jeder</p></td>
<td style="border:1px solid black;"><p>Jeder</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Computer und Benutzerkonten für Delegierungszwecke vertrauen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
</tbody>  
</table>
  
##### Auf diesen Computer vom Netzwerk aus zugreifen
  
Diese Richtlinieneinstellung ermöglicht es anderen Benutzern im Netzwerk, eine Verbindung zum Computer herzustellen. Sie ist für verschiedene Netzwerkprotokolle erforderlich, wie z. B. SMB-basierte Protokolle (Server Message Block), NetBIOS (Network Basic Input/Output System), CIFS (Common Internet File System) und COM+ (Component Object Model Plus).
  
Die Einstellung **Auf diesen Computer vom Netzwerk aus zugreifen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Administratoren** gesetzt.
  
##### Einsetzen als Teil des Betriebssystems
  
Diese Richtlinieneinstellung ermöglicht es einem Prozess, die Identität eines beliebigen Benutzers anzunehmen und dadurch Zugriff auf die dem Benutzer zugänglichen Ressourcen zu erlangen.
  
Aus diesem Grund ist die Einstellung **Einsetzen als Teil des Betriebssystems** für die beiden in diesem Kapitel behandelten Umgebungen auf den Wert **Niemand** beschränkt.
  
##### Anpassen von Speicherkontingenten für einen Prozess
  
Diese Richtlinieneinstellung ermöglicht es einem Benutzer, das maximale Arbeitsspeicherkontingent anzupassen, das einem Prozess zur Verfügung steht. Die Möglichkeit, Speicherkontingente festzulegen, ist für die Anpassung des Systems hilfreich, kann aber auch missbraucht werden. Dieses Recht könnte für einen DoS-Angriff verwendet werden.
  
Aus diesem Grund ist die Einstellung **Anpassen von Speicherkontingenten für einen Prozess** für beide Computertypen in der Hochsicherheitsumgebung auf **Administratoren**, **Lokaler Dienst** und **Netzwerkdienst** beschränkt und für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt.
  
##### Lokal anmelden zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer sich interaktiv bei Computern in Ihrer Umgebung anmelden können. Dieses Benutzerrecht ist für Anmeldungen erforderlich, die durch Drücken der Tastenkombination STRG+ALT+ENTF auf der am Clientcomputer angeschlossenen Tastatur eingeleitet werden. Auch Benutzer, die versuchen, sich über Terminaldienste oder Microsoft Internet Information Services (IIS) anzumelden, müssen über dieses Benutzerrecht verfügen.
  
Dieses Benutzerrecht wird dem Konto **Gast** standardmäßig zugewiesen. Obwohl dieses Konto standardmäßig deaktiviert ist, empfiehlt Microsoft, diese Einstellung durch Gruppenrichtlinien zu aktivieren. Dieses Benutzerrecht sollte jedoch generell auf die Gruppen **Administratoren** und **Benutzer** beschränkt werden. Weisen Sie dieses Benutzerrecht der Gruppe **Sicherungs-Operatoren** zu, wenn dies für Ihre Organisation erforderlich ist.
  
Die Einstellung **Lokal anmelden zulassen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf die Gruppen **Benutzer** und **Administratoren** beschränkt.
  
##### Anmeldung über Terminaldienste zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer oder Gruppen das Recht haben, sich als Terminaldiensteclient anzumelden. Dieses Benutzerrecht ist für Remotedesktopbenutzer erforderlich. Wenn Ihre Organisation als Teil der Helpdeskstrategie Remoteunterstützung anbietet, erstellen Sie eine Gruppe, und weisen Sie ihr dieses Recht über eine Gruppenrichtlinie zu. Wenn in Ihrer Organisation keine Remoteunterstützung verwendet wird, gewähren Sie dieses Recht nur der Gruppe **Administratoren**. Sie können auch die Funktion „Eingeschränkte Gruppen“ verwenden, um sicherzustellen, dass sich keine Benutzerkonten in der Gruppe **Remotedesktopbenutzer** befinden.
  
Beschränken Sie dieses Benutzerrecht auf die Gruppe **Administratoren** und möglicherweise auf die Gruppe **Remotedesktopbenutzer**. Dadurch wird sichergestellt, dass nur autorisierte Benutzer über die neue Remoteunterstützung in Windows XP Professional Zugriff auf Computer in Ihrem Netzwerk erhalten.
  
Die Einstellung **Anmeldung über Terminaldienste zulassen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung ist diese Richtlinieneinstellung zur Erhöhung der Sicherheit auf **Niemand** gesetzt.
  
##### Sichern von Dateien und Verzeichnissen
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, Datei- und Verzeichnisberechtigungen zum Sichern des Systems zu umgehen. Dieses Benutzerrecht wird nur dann aktiviert, wenn eine Anwendung wie z. B. NTBACKUP versucht, über die Dateisystemsicherungs-API (Application Programming Interface) für NTFS auf eine Datei oder ein Verzeichnis zuzugreifen. Andernfalls gelten die zugewiesenen Datei- und Verzeichnisberechtigungen.
  
Die Einstellung **Sichern von Dateien und Verzeichnissen** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung ist diese Richtlinieneinstellung für die Gruppe **Administratoren** konfiguriert.
  
##### Auslassen der durchsuchenden Prüfung
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die nicht über die besondere Zugriffsberechtigung „Ordner durchsehen“ verfügen, bei der Navigation entlang eines Objektpfades im NTFS-Dateisystem oder in der Registrierung Ordner zu passieren. Dieses Benutzerrecht ermöglicht es Benutzern nicht, den Inhalt eines Ordners anzuzeigen. Die Verzeichnisse können lediglich passiert werden.
  
Die Einstellung **Auslassen der durchsuchenden Überprüfung** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung ist die Einstellung für die Gruppen **Administratoren** und **Benutzer** konfiguriert.
  
##### Ändern der Systemzeit
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer und Gruppen die Uhrzeit und das Datum der internen Uhr der Computer in Ihrer Umgebung ändern können. Benutzer, denen dieses Benutzerrecht zugewiesen wird, können den Inhalt der Ereignisprotokolle beeinflussen. Wenn die Zeiteinstellung eines Computers geändert wird, wird bei den protokollierten Ereignissen die neue Uhrzeit wiedergegeben und nicht die tatsächliche Uhrzeit, zu der die Ereignisse stattgefunden haben.
  
Die Einstellung **Ändern der Systemzeit** ist für die beiden in diesem Kapitel behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
**Hinweis**: Abweichungen zwischen der Uhrzeit auf dem lokalen Computer und auf den Domänencontrollern Ihrer Umgebung führen beim Authentifizierungsprotokoll Kerberos u. U. zu Problemen. Dies kann dazu führen, dass Benutzer sich nicht mehr an der Domäne anmelden können oder nach der Anmeldung am Netzwerk nicht für den Zugriff auf Domänenressourcen autorisiert werden. Außerdem treten Probleme auf, wenn Gruppenrichtlinien auf Clientcomputer angewendet werden und die Systemzeit nicht mit den Domänencontrollern synchronisiert ist.
  
##### Auslagerungsdatei erstellen
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Größe der Auslagerungsdatei zu ändern. Wenn die Auslagerungsdatei extrem groß oder klein ist, kann ein Angreifer leicht die Leistung eines beeinträchtigten Computers beeinflussen.
  
Die Einstellung **Auslagerungsdatei erstellen** ist für alle Computer sowohl in der Unternehmensclient-Umgebung als auch in der Hochsicherheitsumgebung für **Administratoren** konfiguriert.
  
##### Permanente freigegebene Objekte erstellen
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, im Objektmanager Verzeichnisobjekte zu erstellen. Dieses Benutzerrecht ist für Kernelmoduskomponenten nützlich, die den Objekt-/Namespace erweitern. Komponenten, die im Kernelmodus ausgeführt werden, verfügen grundsätzlich über dieses Benutzerrecht. Deshalb ist es in der Regel nicht notwendig, diese Benutzerberechtigung explizit zuzuweisen.
  
Die Einstellung **Permanent freigegebene Objekte erstellen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
##### Erstellen eines Tokenobjekts
  
Diese Richtlinieneinstellung ermöglicht es einem Prozess, ein Zugriffstoken zu erstellen, das erhöhte Berechtigungen für den Zugriff auf vertrauliche Daten bereitstellen kann. In Umgebungen, in denen die Sicherheit Priorität hat, sollte dieses Benutzerrecht keinem Benutzer zugewiesen werden. Alle Prozesse, die diese Funktion erfordern, sollten das lokale Systemkonto verwenden, dem dieses Benutzerrecht standardmäßig zugewiesen ist.
  
Die Einstellung **Erstellen eines Tokenobjekts** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
##### Debuggen von Programmen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer einen beliebigen Prozess oder einen Kernel debuggen können, der vollständigen Zugriff auf vertrauliche und kritische Betriebssystemkomponenten bereitstellt. Dieses Benutzerrecht ist erforderlich, wenn Administratoren die Vorteile von Patches nutzen möchten, die „In-Memory-Patching“ unterstützen, auch „Hotpatching“ genannt. Weitere Informationen zu den neuesten Funktionen im Microsoft Package Installer finden Sie in „[Der Package Installer (früher Update.exe genannt) für Microsoft Windows-Betriebssysteme und Windows-Komponenten](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/deployment/winupdte.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/deployment/winupdte.mspx. Da ein Angreifer dieses Benutzerrecht ausnutzen könnte, wird es standardmäßig nur der Gruppe **Administratoren** zugewiesen.
  
**Hinweis**: Microsoft hat im Oktober 2003 mehrere Sicherheitspatches mit einer Version der Datei Update.exe veröffentlicht, die voraussetzte, dass der Administrator über das Benutzerrecht **Debuggen von Programmen** verfügt. Administratoren, die nicht über dieses Benutzerrecht verfügten, konnten diese Patches erst installieren, nachdem sie ihre Benutzerrechte neu konfiguriert hatten. Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Windows-Produktaktualisierungen reagieren nicht mehr oder beanspruchen die CPU-Ressourcen vollständig bzw. zum größten Teil](http://support.microsoft.com/default.aspx?kbid=830846)“ unter http://support.microsoft.com/default.aspx?kbid=830846.
  
Das Benutzerrecht **Debuggen von Programmen** ist sehr umfassend. Daher ist diese Richtlinieneinstellung in der Unternehmensclient-Umgebung auf **Administratoren** gesetzt, während in der Hochsicherheitsumgebung die Standardeinstellung **Niemand** beibehalten wird.
  
##### Den Zugriff auf diesen Computer vom Netzwerk aus verweigern
  
Durch diese Richtlinieneinstellung wird verhindert, dass Benutzer über das Netzwerk eine Verbindung zu einem Computer herstellen können, wodurch sie in die Lage versetzt würden, von Remotestandorten aus auf Daten zuzugreifen und diese möglicherweise zu verändern. In einer Hochsicherheitsumgebung sollte es für Remotebenutzer nicht erforderlich sein, auf Daten auf einem Computer zuzugreifen. Statt dessen sollte die Dateifreigabe durch Netzwerkserver erfolgen.
  
Die Einstellung **Den Zugriff auf diesen Computer vom Netzwerk aus verweigern** ist für Computer in den beiden in diesem Kapitel behandelten Umgebungen für die Konten **Support\_388945a0** und **Gast** konfiguriert.
  
##### Anmeldung als Batchauftrag verweigern
  
Diese Richtlinieneinstellung verhindert Benutzeranmeldungen über eine Batchwarteschlangeneinrichtung. Dies ist eine Funktion unter Windows Server 2003, mit der Aufträge für die künftige ein- oder mehrmalige automatische Ausführung geplant werden.
  
Die Einstellung **Anmeldung als Batchauftrag verweigern** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Support\_388945a0** und **Gast** gesetzt.
  
##### Lokal anmelden verweigern
  
Durch diese Richtlinieneinstellung wird verhindert, dass sich Benutzer lokal bei der Computerkonsole anmelden können. Wenn nicht autorisierte Benutzer sich lokal bei einem Computer anmelden können, könnten sie schädlichen Code herunterladen oder ihre Berechtigungen auf dem Computer erhöhen. (Wenn Angreifer physischen Zugriff auf die Konsole haben, müssen andere Risiken berücksichtigt werden). Dieses Benutzerrecht sollte nicht jenen Benutzern zugewiesen werden, die physischen Zugriff auf die Computerkonsole benötigen.
  
Die Einstellung **Lokal anmelden verweigern** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Support\_388945a0** und **Gast** gesetzt. Außerdem sollte dieses Benutzerrecht allen dem Computer hinzugefügten Dienstkonten zugewiesen werden, um deren Missbrauch zu verhindern.
  
##### Anmeldung über Terminaldienste verweigern
  
Durch diese Richtlinieneinstellung wird verhindert, dass sich Benutzer über Remotedesktopverbindungen bei Computern in Ihrer Umgebung anmelden können. Wenn Sie dieses Benutzerrecht der Gruppe **Jeder** zuweisen, halten Sie auch Mitglieder der Standardgruppe **Administratoren** davon ab, sich mithilfe von Terminaldiensten bei Computern in Ihrer Umgebung anzumelden.
  
Die Einstellung **Anmeldung über Terminaldienste verweigern** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Jeder** gesetzt.
  
##### Computer und Benutzerkonten für Delegierungszwecke vertrauen
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Einstellung **Für Delegierungszwecke vertrauenswürdig** in einem Computerobjekt in Active Directory zu ändern. Ein Missbrauch dieser Berechtigung könnte nicht autorisierten Benutzern ermöglichen, die Identität eines anderen Benutzers im Netzwerk anzunehmen.
  
Aus diesem Grund ist die Einstellung **Computer und Benutzerkonten für Delegierungszwecke vertrauen** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
#### Benutzerrechte, deren englische Bezeichnungen mit den Buchstaben F bis T beginnen
  
**Tabelle 3.4: Empfehlungen für Einstellungen zum Zuweisen von Benutzerrechten – Teil 2**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Erzwingen des Herunterfahrens von einem Remotesystem aus</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Generieren von Sicherheitsüberwachungen</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Anheben der Zeitplanungspriorität</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Laden und Entfernen von Gerätetreibern</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Seiten im Speicher sperren</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Anmelden als Stapelverarbeitungsauftrag</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
<td style="border:1px solid black;"><p>Niemand</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Als Dienst anmelden</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst, lokaler Dienst</p></td>
<td style="border:1px solid black;"><p>Netzwerkdienst, lokaler Dienst</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Verwalten von Überwachungs- und Sicherheitsprotokoll</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Firmware-Umgebungsvariablen ändern</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Wartungsaufgaben für Speichermedien ausführen</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Einzelprozessprofil erstellen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Erstellen eines Profils der Systemleistung</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Entfernen eines Computers aus der Dockingstation</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Ersetzen eines Prozessebenentokens</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
<td style="border:1px solid black;"><p>Lokaler Dienst, Netzwerkdienst</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Wiederherstellen von Dateien und Verzeichnissen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>System herunterfahren</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Benutzer</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Übernehmen des Besitzes an Dateien und Objekten</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
</tbody>  
</table>
  
In dieser Tabelle sind Empfehlungen für die Einstellungen zum Zuweisen von Benutzerrechten zusammengefasst, deren englische Bezeichnungen mit den Buchstaben F bis T beginnen. Ausführlichere Informationen zu jeder Einstellung finden Sie in den folgenden Unterabschnitten.
  
##### Erzwingen des Herunterfahrens von einem Remotesystem aus
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, Windows XP-basierte Computer von Remotestandorten im Netzwerk aus herunterzufahren. Jeder, dem dieses Benutzerrecht zugewiesen wurde, kann einen DoS-Situation (Denial of Service) herbeiführen und so verhindern, dass der Computer für Benutzeranfragen zur Verfügung steht. Daher empfiehlt Microsoft, dieses Benutzerrecht nur sehr vertrauenswürdigen Administratoren zuzuweisen.
  
Die Einstellung **Erzwingen des Herunterfahrens von einem Remotesystem aus** ist in den beiden in diesem Kapitel behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
##### Generieren von Sicherheitsüberwachungen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer oder Prozesse Überwachungseinträge im Sicherheitsprotokoll erzeugen können. Ein Angreifer könnte diese Funktion ausnutzen, um eine große Anzahl überwachter Ereignisse zu erzeugen, die es einem Systemadministrator erschweren würden, unberechtigte Aktivitäten aufzuspüren. Wenn außerdem das Ereignisprotokoll so konfiguriert ist, dass Ereignisse bei Bedarf überschrieben werden, könnte jeder Beweis über unberechtigte Aktivitäten von einer großen Anzahl nicht zugehöriger Ereignisse überschrieben werden.
  
Aus diesem Grund ist die Einstellung **Generieren von Sicherheitsüberwachungen** für die beiden in diesem Kapitel behandelten Umgebungen für die Gruppen **Lokaler Dienst** und **Netzwerkdienst** konfiguriert.
  
##### Anheben der Zeitplanungspriorität
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, die Zeitdauer zu verändern, für die ein Prozess den Prozessor beansprucht. Ein Angreifer könnte diese Möglichkeit ausnutzen, um die Priorität eines Prozesses auf Echtzeit zu erhöhen und eine DoS-Situation für einen Computer herbeizuführen.
  
Aus diesem Grund ist die Einstellung **Anheben der Zeitplanungspriorität** in den beiden in diesem Kapitel behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
##### Laden und Entfernen von Gerätetreibern
  
Diese Richtlinieneinstellung ermöglicht Benutzern das dynamische Laden eines neuen Gerätetreibers auf ein System. Ein Angreifer könnte diese Funktion möglicherweise dazu verwenden, schädlichen Code zu installieren, bei dem es sich um einen Gerätetreiber zu handeln scheint. Dieses Benutzerrecht und die Mitgliedschaft in entweder der Gruppe **Hauptbenutzer** oder der Gruppe **Administratoren** sind für Benutzer erforderlich, die unter Windows XP lokale Drucker oder Druckertreiber hinzufügen möchten.
  
Da diese Benutzerberechtigung von einem Angreifer ausgenutzt werden könnte, ist die Einstellung **Laden und Entfernen von Gerätetreibern** in den beiden in diesem Kapitel behandelten Umgebungen für die Gruppe **Administratoren** konfiguriert.
  
##### Seiten im Speicher sperren
  
Diese Richtlinieneinstellung ermöglicht einem Prozess das Speichern von Daten in einem physischen Speicher, wodurch das System daran gehindert wird, die Daten in einen virtuellen Speicher auf der Festplatte auszulagern. Durch das Zuweisen dieses Benutzerrechts kann die Systemleistung erheblich beeinträchtigt werden.
  
Aus diesem Grund ist die Einstellung **Seiten im Speicher sperren** in den beiden in diesem Kapitel behandelten Umgebungen auf **Niemand** gesetzt.
  
##### Anmelden als Stapelverarbeitungsauftrag
  
Diese Richtlinieneinstellung ermöglicht es Konten, sich mithilfe des Taskplanerdienstes anzumelden. Da der Taskplaner häufig zu Verwaltungszwecken verwendet wird, wird er möglicherweise in der Unternehmensclient-Umgebung benötigt. In der Hochsicherheitsumgebung sollte seine Verwendung jedoch eingeschränkt werden, um den Missbrauch von Systemressourcen zu verhindern. Außerdem wird dadurch verhindert, dass Angreifer mithilfe der Berechtigung schädlichen Code starten, nachdem sie auf Benutzerebene Zugriff auf einen Computer erlangt haben.
  
Daher ist das Benutzerrecht **Anmelden als Stapelverarbeitungsauftrag** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Niemand** gesetzt.
  
##### Als Dienst anmelden
  
Diese Richtlinieneinstellung ermöglicht es Konten, Netzwerkdienste zu starten oder einen Prozess als auf dem System ausgeführten Dienst zu registrieren. Dieses Benutzerrecht sollte auf jedem Computer in einer Hochsicherheitsumgebung eingeschränkt werden. Da diese Berechtigung jedoch möglicherweise für viele Anwendungen erforderlich ist, sollte sie sorgfältig bewertet und getestet werden, bevor sie in einer Unternehmensclient-Umgebung konfiguriert wird.
  
Die Einstellung **Als Dienst anmelden** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Netzwerkdienst** und **Lokaler Dienst** gesetzt.
  
##### Verwalten von Überwachungs- und Sicherheitsprotokoll
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Überwachungsoptionen für Dateien und Verzeichnisse ändern und das Sicherheitsprotokoll löschen können.
  
Da diese Möglichkeit eine relativ kleine Bedrohung darstellt, ist die Einstellung **Verwalten von Überwachungs- und Sicherheitsprotokoll** für die beiden in diesem Kapitel behandelten Umgebungen standardmäßig für die Gruppe **Administratoren** konfiguriert.
  
##### Firmware-Umgebungsvariablen ändern
  
Mit dieser Richtlinieneinstellung können Benutzer die systemweiten Umgebungsvariablen konfigurieren, die sich auf die Hardwarekonfiguration auswirken. Diese Informationen sind in der Regel in „Letzte als funktionierend bekannte Konfiguration“ gespeichert. Änderungen an diesen Werten könnten zu einem Hardwareversagen führen, was wiederum eine DoS-Situation verursacht.
  
Da diese Möglichkeit eine relativ kleine Bedrohung darstellt, ist die Einstellung **Firmware-Umgebungsvariablen ändern** für die beiden in diesem Kapitel behandelten Umgebungen standardmäßig für die Gruppe **Administratoren** konfiguriert.
  
##### Wartungsaufgaben für Speichermedien ausführen
  
Mit dieser Richtlinieneinstellung können Benutzer die Konfiguration von Datenträgern oder Laufwerken des Systems verwalten. Dadurch könnte ein Benutzer einen Datenträger löschen und Datenverluste sowie eine DoS-Situation verursachen.
  
Die Einstellung **Wartungsaufgaben für Speichermedien ausführen** ist für die beiden in diesem Kapitel behandelten Umgebungen standardmäßig für die Gruppe **Administratoren** konfiguriert.
  
##### Einzelprozessprofil erstellen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer mithilfe von Tools die Leistung von systemfremden Prozessen überwachen können. In der Regel müssen Sie dieses Benutzerrecht nicht konfigurieren, um das Snap-In „Leistung“ der Microsoft Management Console (MMC) zu verwenden. Sie benötigen dieses Benutzerrecht jedoch, wenn der Systemmonitor mit der Windows-Verwaltungsinstrumentation (WMI) zum Sammeln von Daten konfiguriert ist. Wenn Sie das Benutzerrecht **Einzelprozessprofil erstellen** beschränken, wird verhindert, dass Angreifer zusätzliche Informationen erhalten, mit deren Hilfe sie das System angreifen können.
  
Die Einstellung **Einzelprozessprofil erstellen** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt und in der Hochsicherheitsumgebung für die Gruppe **Administratoren** konfiguriert.
  
##### Erstellen eines Profils der Systemleistung
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, mithilfe von Tools die Leistung verschiedener Systemprozesse anzuzeigen, die von Angreifern missbraucht werden könnten, um die aktiven Prozesse eines Systems zu ermitteln und Einblick in die potenzielle Angriffsfläche des Computers zu erhalten.
  
Die Einstellung **Erstellen eines Profils der Systemleistung** ist für die beiden in diesem Kapitel behandelten Umgebungen standardmäßig für die Gruppe **Administratoren** konfiguriert.
  
##### Entfernen eines Computers aus der Dockingstation
  
Diese Richtlinieneinstellung ermöglicht es dem Benutzer eines tragbaren Computers, im Menü **Start** auf **PC trennen** zu klicken, um den Computer abzudocken.
  
Die Einstellung **Entfernen eines Computers aus der Dockingstation** ist für die beiden in diesem Kapitel behandelten Umgebungen für die Gruppen **Administratoren** und **Benutzer** konfiguriert.
  
##### Ersetzen eines Prozessebenentokens
  
Diese Richtlinieneinstellung ermöglicht es einem Prozess oder Dienst, einen weiteren Dienst oder Prozess mit einem anderen Sicherheitszugriffstoken zu starten, wodurch das Sicherheitszugriffstoken jenes Unterprozesses geändert und Berechtigungen erhöht werden können.
  
Die Einstellung **Ersetzen eines Prozessebenentokens** ist in den beiden in diesem Kapitel behandelten Umgebungen auf die Standardwerte **Lokaler Dienst** und **Netzwerkdienst** gesetzt.
  
##### Wiederherstellen von Dateien und Verzeichnissen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Benutzer die Berechtigungen für Dateien, Verzeichnisse, die Registrierung und andere ständige Objekte umgehen können, wenn sie gesicherte Dateien und Verzeichnisse auf Computern mit Windows XP in Ihrer Umgebung wiederherstellen. Durch dieses Benutzerrecht wird außerdem festgelegt, welche Benutzer gültige Sicherheitsprinzipale als Objektbesitzer festlegen dürfen. Dieses Benutzerrecht ähnelt dem Benutzerrecht **Sichern von Dateien und Verzeichnissen**.
  
Die Einstellung **Wiederherstellen von Dateien und Verzeichnissen** ist für Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt und in der Hochsicherheitsumgebung für die Gruppe **Administratoren** konfiguriert.
  
##### System herunterfahren
  
Durch diese Richtlinieneinstellung wird festgelegt, welche lokal bei den Computern in Ihrer Umgebung angemeldeten Benutzer das Betriebssystem mit dem Befehl „Herunterfahren“ herunterfahren können. Der Missbrauch dieses Benutzerrechts kann zu einer DoS-Situation führen. Microsoft empfiehlt, dieses Recht in Hochsicherheitsumgebungen nur den Gruppen **Administratoren** und **Benutzer** zuzuweisen.
  
Die Einstellung **System herunterfahren** ist für die beiden in diesem Kapitel behandelten Umgebungen für die Gruppen **Administratoren** und **Benutzer** konfiguriert.
  
##### Übernehmen des Besitzes an Dateien und Objekten
  
Diese Richtlinieneinstellung ermöglicht es Benutzern, den Besitz von Dateien, Ordnern, Registrierungsschlüsseln, Prozessen oder Threads zu übernehmen. Mit diesem Benutzerrecht werden alle Berechtigungen umgangen, die Objekte schützen und dem angegebenen Benutzer Besitzrechte zuweisen sollen.
  
Die Einstellung **Übernehmen des Besitzes an Dateien und Objekten** ist in den beiden in diesem Kapitel behandelten Umgebungen standardmäßig für die Gruppe **Administratoren** konfiguriert.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen der Sicherheitsoptionen
  
Die Einstellungen für Sicherheitsoptionen, die Ihrer Umgebung mithilfe von Gruppenrichtlinien auf Computer mit Windows XP in angewendet werden, können Sie für die Aktivierung und Deaktivierung von Berechtigungen und Funktionen (wie z. B. des Zugriffs auf Disketten- und CD-ROM-Laufwerke sowie der Anmeldeaufforderungen) verwenden. Diese Einstellungen werden auch zum Konfigurieren verschiedener anderer Einstellungen verwendet, wie z. B. jener für die digitale Datensignierung, für Administrator- und Gastkontennamen sowie für die Funktionsweise der Treiberinstallation.
  
Die Einstellungen der Sicherheitsoptionen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\Sicherheitsoptionen**
  
Nicht alle in diesem Abschnitt behandelten Einstellungen sind unter sämtlichen Systemtypen vorhanden. Deshalb müssen die in diesem Abschnitt definierten Einstellungen, die den Abschnitt der Sicherheitsoptionen der Gruppenrichtlinien bilden, auf Systemen, auf denen diese Einstellungen vorhanden sind, möglicherweise manuell geändert werden, damit sie vollständig funktionsfähig sind. Sie können die Gruppenrichtlinienvorlagen auch einzeln bearbeiten, um die entsprechenden Einstellungsoptionen einzuschließen, sodass die Einstellungsanordnungen sich vollständig auswirken.
  
In den folgenden Abschnitten werden Empfehlungen zu den Einstellungen der Sicherheitsoptionen bereitgestellt und nach Objekttyp gruppiert. Jeder Abschnitt enthält eine Tabelle, in der die Einstellungen zusammengefasst sind. In den Unterabschnitten im Anschluss an jede Tabelle werden ausführliche Informationen bereitgestellt. Empfehlungen werden sowohl für Desktop- als auch für Laptopclientcomputer in den beiden Sicherheitsumgebungen gegeben, die in diesem Kapitel behandelt werden (Unternehmensclient-Umgebung und Hochsicherheitsumgebung).
  
#### Konten
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für Konten zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.5: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Konten**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Konten: Administratorkontostatus</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Konten: Gastkontenstatus</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Konten: Administratorkonto umbenennen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Konten: Gastkonto umbenennen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
<td style="border:1px solid black;"><p>Empfohlen</p></td>
</tr>  
</tbody>  
</table>
  
##### Konten: Administratorkontostatus
  
Durch diese Richtlinieneinstellung wird das Administratorkonto während des normalen Betriebs aktiviert oder deaktiviert. Wenn ein Computer im sicheren Modus gestartet wird, ist das Administratorkonto unabhängig von der Konfiguration dieser Einstellung immer aktiviert.
  
Die Einstellung **Konten: Administratorkontostatus** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
##### Konten: Gastkontenstatus
  
Durch diese Richtlinieneinstellung wird festgelegt, ob das Gastkonto aktiviert oder deaktiviert ist. Das Gastkonto ermöglicht nicht authentifizierten Netzwerkbenutzern, auf das System zuzugreifen.
  
Die Sicherheitsoption **Konten: Gastkontostatus** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken
  
Durch diese Richtlinieneinstellung wird festgelegt, ob lokale Konten, die nicht durch ein Kennwort geschützt sind, sich von anderen Orten als der physischen Computerkonsole aus anmelden können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind lokale Konten mit leeren Kennwörtern nicht in der Lage, sich von Remoteclientcomputern aus beim Netzwerk anzumelden. Solche Konten können sich nur über die Tastatur des Computers anmelden.
  
Die Einstellung **Konten: Lokale Kontenverwendung von leeren Kennwörtern auf Konsolenanmeldung beschränken** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Konten: Administratorkonto umbenennen
  
Der vordefinierte Name des lokalen Administratorkontos ist ein bekannter Kontoname, auf den sich viele Angriffe richten. Microsoft empfiehlt, einen anderen Namen für dieses Konto zu wählen und Namen zu vermeiden, die auf administrative Konten oder erhöhte Zugriffsrechte hinweisen. Außerdem sollte die Standardbeschreibung für den lokalen Administrator über die Computerverwaltung geändert werden.
  
Die Empfehlung, die Einstellung **Konten: Administratorkonto umbenennen** zu verwenden, gilt für beide Umgebungen, die in diesem Kapitel erörtert werden.
  
**Hinweis**: Diese Richtlinieneinstellung ist in den Sicherheitsvorlagen nicht konfiguriert, und es wird in diesem Handbuch auch kein neuer Benutzername für das Konto vorgeschlagen. Vorgeschlagene Benutzernamen werden ausgelassen. Dadurch soll sichergestellt werden, dass Organisationen, die diese Anleitung implementieren, nicht den gleichen neuen Benutzernamen in ihren Umgebungen verwenden.
  
##### Konten: Gastkonto umbenennen
  
Der Name des vordefinierten lokalen Gastkontos ist Hackern ebenfalls wohlbekannt. Microsoft empfiehlt, diesem Konto ebenfalls einen Namen zu geben, aus dem sich der Zweck des Kontos nicht erkennen lässt. Selbst wenn Sie dieses Konto deaktivieren (was empfohlen wird), sollten Sie es zur Erhöhung der Sicherheit umbenennen.
  
Die Empfehlung, die Einstellung **Konten: Gastkonto umbenennen** zu verwenden, gilt für beide Umgebungen, die in diesem Kapitel erörtert werden.
  
**Hinweis**: Diese Richtlinieneinstellung ist in den Sicherheitsvorlagen nicht konfiguriert, und es wird hier auch kein neuer Benutzername für das Konto vorgeschlagen. Vorgeschlagene Benutzernamen werden ausgelassen. Dadurch soll sichergestellt werden, dass Organisationen, die diese Anleitung implementieren, nicht den gleichen neuen Benutzernamen in ihren Umgebungen verwenden.
  
#### Überwachung
  
In der folgenden Tabelle sind die empfohlenen Überwachungseinstellungen zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.6: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Überwachung**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Überwachung: Zugriff auf globale Systemobjekte prüfen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
</tr>  
</tbody>  
</table>
  
##### Überwachung: Zugriff auf globale Systemobjekte prüfen
  
Mit dieser Richtlinieneinstellung wird eine standardmäßige Systemzugriffssteuerungsliste (SACL) für Systemobjekte wie z. B. Mutexe, Ereignisse, Semaphore und MS-DOS®-Geräte erstellt. Der Zugriff auf diese Systemobjekte wird daraufhin überwacht.
  
Wenn die Einstellung **Überwachung: Zugriff auf globale Systemobjekte prüfen** aktiviert ist, könnte das Sicherheitsereignisprotokoll schnell mit einer sehr großen Anzahl von Sicherheitsereignissen gefüllt werden. Aus diesem Grund ist diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Verwendung aller Benutzerrechte (einschließlich Sicherung und Wiederherstellung) überwacht wird, wenn die Einstellung **Rechteverwendung überwachen** aktiviert ist. Wenn Sie beide Richtlinien aktivieren, wird für jede gesicherte oder wiederhergestellte Datei ein Überwachungsereignis erzeugt.
  
Wenn die Einstellung **Überwachung: Die Verwendung des Sicherungs- und Wiederherstellungsrechts überprüfen** aktiviert ist, könnte das Sicherheitsereignisprotokoll schnell mit einer sehr großen Anzahl von Sicherheitsereignissen gefüllt werden. Aus diesem Grund ist diese Richtlinieneinstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können
  
Durch diese Richtlinieneinstellung wird festgelegt, ob das System sofort heruntergefahren wird, wenn es Sicherheitsereignisse nicht protokollieren kann. Diese Einstellung ist für die TCSEC-C2-Zertifizierung (Trusted Computer System Evaluation Criteria) und die Common-Criteria-Zertifizierung erforderlich und verhindert, dass zu überwachende Ereignisse auftreten, wenn sie vom Überwachungssystem nicht protokolliert werden können. Microsoft erfüllt diese Anforderungen durch Anzeigen einer Abbruchmeldung und Herunterfahren des Systems, wenn das Überwachungssystem nicht ordnungsgemäß arbeitet. Wenn diese Richtlinieneinstellung aktiviert ist, wird das System heruntergefahren, wenn eine Sicherheitsüberwachung nicht protokolliert werden kann.
  
Wenn die Einstellung **Überwachung: System sofort herunterfahren, wenn Sicherheitsüberprüfungen nicht protokolliert werden können** aktiviert ist, können ungeplante Systemfehler auftreten. Diese Richtlinieneinstellung ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### Geräte
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für Geräte zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.7: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Geräte**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Geräte: Entfernen ohne vorherige Anmeldung erlauben</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Geräte: Formatieren und Auswerfen von Wechselmedien zulassen</p></td>
<td style="border:1px solid black;"><p>Administratoren, Interaktive Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren, Interaktive Benutzer</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Administratoren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Geräte: Verhalten bei der Installation von nicht signierten Treibern</p></td>
<td style="border:1px solid black;"><p>Warnen, aber Installation erlauben</p></td>
<td style="border:1px solid black;"><p>Warnen, aber Installation erlauben</p></td>
<td style="border:1px solid black;"><p>Warnen, aber Installation erlauben</p></td>
<td style="border:1px solid black;"><p>Warnen, aber Installation erlauben</p></td>
</tr>  
</tbody>  
</table>
  
##### Geräte: Entfernen ohne vorherige Anmeldung erlauben
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein tragbarer Computer durch einen nicht beim System angemeldeten Benutzer abgedockt werden kann. Wenn diese Einstellung aktiviert ist, entfällt die Anmeldeanforderung, und der Computer kann über eine Schaltfläche zum Trennen externer Hardware abgedockt werden. Wenn Sie diese Richtlinieneinstellung deaktivieren, muss ein nicht angemeldeter Benutzer über das Benutzerrecht **Entfernen eines Computers aus der Dockingstation** verfügen. Dieses ist im vorliegenden Handbuch nicht definiert.
  
Die Einstellung **Geräte:** **Entfernen ohne vorherige Anmeldung erlauben** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Geräte: Formatieren und Auswerfen von Wechselmedien zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, wer Wechselmedien formatieren und auswerfen darf. Mit dieser Richtlinieneinstellung können Sie nicht autorisierte Benutzer davon abhalten, Daten von einem Computer zu entfernen und auf diese auf einem anderen Computer zuzugreifen, auf dem die Benutzer lokale Administratorrechte besitzen.
  
Die Einstellung **Geräte:** **Formatieren und Auswerfen von Wechselmedien zulassen** ist zur Erhöhung der Sicherheit in der Unternehmensclient-Umgebung auf die Gruppen **Administratoren** und **Interaktive Benutzer** und in der Hochsicherheitsumgebung auf die Gruppe **Administratoren** beschränkt.
  
##### Geräte: Anwendern das Installieren von Druckertreibern nicht erlauben
  
Hacker verfügen über Möglichkeiten, einen Trojaner als Druckertreiber zu tarnen. Dadurch getäuschte Benutzer verwenden dieses Programm möglicherweise zum Drucken und führen damit schädlichen Code im Netzwerk aus. Zur Verringerung der Wahrscheinlichkeit eines solchen Ereignisses sollten nur Administratoren Druckertreiber installieren dürfen. Da Laptops mobile Geräte sind, kann es für Benutzer von Laptops jedoch notwendig sein, Druckertreiber von anderen Quellen zu installieren, um ihre Arbeit fortsetzen zu können. Diese Einstellung sollte für Laptopbenutzer deaktiviert und für Desktopbenutzer immer aktiviert werden.
  
Die Einstellung **Geräte:** **Anwendern das Installieren von Druckertreibern nicht erlauben** ist für die Desktops in den beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** und für Laptopbenutzer in beiden Umgebungen auf **Deaktiviert** gesetzt.
  
##### Geräte: Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken
  
Durch diese Richtlinieneinstellung wird festgelegt, ob sowohl lokale Benutzer als auch Remotebenutzer gleichzeitig auf das CD-ROM-Laufwerk zugreifen können. Wenn Sie diese Richtlinieneinstellung aktivieren, können nur interaktiv angemeldete Benutzer auf Medien im CD-ROM-Laufwerk zugreifen. Wenn diese Richtlinieneinstellung aktiviert und niemand angemeldet ist, kann über das Netzwerk auf das CD-ROM-Laufwerk zugegriffen werden. Wenn Sie diese Einstellung aktivieren, schlägt das Windows-Sicherungsprogramm fehl, wenn für den Sicherungsauftrag Volumenschattenkopien angegeben wurden. Sicherungssysteme von Drittanbietern, die Volumenschattenkopien verwenden, schlagen ebenfalls fehl.
  
Die Einstellung **Geräte:** **Zugriff auf CD-ROM-Laufwerke auf lokal angemeldete Benutzer beschränken** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Geräte: Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken
  
Durch diese Richtlinieneinstellung wird festgelegt, ob sowohl lokale Benutzer als auch Remotebenutzer gleichzeitig auf das Diskettenlaufwerk zugreifen können. Wenn Sie diese Richtlinieneinstellung aktivieren, können nur interaktiv angemeldete Benutzer auf Medien in Diskettenlaufwerken zugreifen. Wenn die Einstellung aktiviert und niemand angemeldet ist, kann über das Netzwerk auf Medien im Diskettenlaufwerk zugegriffen werden. Wenn Sie diese Einstellung aktivieren, schlägt das Windows-Sicherungsprogramm fehl, wenn für den Sicherungsauftrag Volumenschattenkopien angegeben wurden. Sicherungssysteme von Drittanbietern, die Volumenschattenkopien verwenden, schlagen ebenfalls fehl.
  
Die Einstellung **Geräte:** **Zugriff auf Diskettenlaufwerke auf lokal angemeldete Benutzer beschränken** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Geräte: Verhalten bei der Installation von nicht signierten Treibern
  
Durch diese Richtlinieneinstellung wird festgelegt, was passiert, wenn ein Benutzer versucht, einen nicht genehmigten und nicht vom Windows Hardware Quality Lab (WHQL) signierten Gerätetreiber zu installieren (mithilfe der Setup-API). Durch diese Option wird die Installation von nicht signierten Treibern verhindert, oder der Administrator wird gewarnt, wenn ein solcher Treiber installiert werden soll. Dadurch kann die Installation von Treibern verhindert werden, die nicht für Windows XP zertifiziert sind. Wenn Sie für diese Richtlinieneinstellung den Wert **Warnen, aber Installation erlauben** festlegen, besteht ein potenzielles Problem darin, dass unbeaufsichtigte Installationsskripts bei dem Versuch fehlschlagen, nicht signierte Treiber zu installieren.
  
Aus diesem Grund ist die Einstellung **Geräte:** **Verhalten bei der Installation von nichtsignierten Treibern** für die beiden in diesem Kapitel behandelten Umgebungen auf **Warnen, aber Installation erlauben** gesetzt.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung implementieren, sollten die Clients vollständig mit allen Standardanwendungen konfiguriert werden, bevor Sie die Gruppenrichtlinien anwenden. So verringern Sie das Risiko, dass durch diese Einstellung Installationsfehler verursacht werden.
  
#### Domänenmitglied
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für Domänenmitglieder zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.8: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Domänenmitglied**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Domänenmitglied: Maximalalter von Computerkennwörtern</p></td>
<td style="border:1px solid black;"><p>30 Tage</p></td>
<td style="border:1px solid black;"><p>30 Tage</p></td>
<td style="border:1px solid black;"><p>30 Tage</p></td>
<td style="border:1px solid black;"><p>30 Tage</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der gesamte Datenverkehr vom sicheren Kanal, der vom Domänenmitglied initiiert wird, signiert oder verschlüsselt werden muss. Wenn ein System so konfiguriert ist, dass Daten des sicheren Kanals immer verschlüsselt oder signiert werden, kann es keinen sicheren Kanal mit einem Domänencontroller herstellen, der nicht in der Lage ist, den gesamten Verkehr durch den sicheren Kanal zu signieren oder zu verschlüsseln.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln oder signieren (immer)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen kann, für den gesamten von ihm initiierten Verkehr über den sicheren Kanal die Verschlüsselung auszuhandeln. Wenn Sie diese Richtlinieneinstellung aktivieren, fordert das Domänenmitglied für den gesamten Verkehr über den sicheren Kanal eine Verschlüsselung an. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann das Domänenmitglied die Verschlüsselung für den sicheren Kanal nicht aushandeln.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital verschlüsseln (wenn möglich)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied versuchen kann, für den gesamten von ihm initiierten Verkehr über den sicheren Kanal die Signierung auszuhandeln. Durch die Signierung wird verhindert, dass der Verkehr geändert wird, wenn er bei der Übertragung über das Netzwerk abgefangen wird.
  
Die Einstellung **Domänenmitglied: Daten des sicheren Kanals digital signieren (wenn möglich)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Domänenmitglied sein Computerkontenkennwort regelmäßig ändern kann. Wenn Sie diese Richtlinieneinstellung aktivieren, kann das Domänenmitglied sein Computerkontenkennwort nicht ändern. Wenn Sie diese Richtlinieneinstellung deaktivieren, kann das Domänenmitglied sein Computerkontenkennwort entsprechend der Einstellung für **Domänenmitglied: Maximalalter von Computerkontenkennwörtern** ändern. Der Standardwert dieser Einstellung beträgt 30 Tage. Computer, die ihre Kontenkennwörter nicht automatisch ändern können, sind potenziell angreifbar, weil ein Angreifer das Kennwort für das Domänenkonto des Systems ermitteln kann.
  
Daher ist die Einstellung **Domänenmitglied: Änderungen von Computerkontenkennwörtern deaktivieren** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Domänenmitglied: Maximalalter von Computerkennwörtern
  
Durch diese Richtlinieneinstellung wird das maximal zulässige Alter für Computerkontenkennwörter festgelegt. Standardmäßig ändern Domänenmitglieder ihre Domänenkennwörter automatisch alle 30 Tage. Wenn Sie dieses Intervalls deutlich erhöhen oder auf 0 setzen, damit die Kennwörter von Computern nicht mehr geändert werden müssen, haben Angreifer mehr Zeit, um über Brute-Force-Angriffe das Kennwort von Computerkonten zu erraten.
  
Daher ist die Einstellung **Domänenmitglied: Maximalalter von Computerkontenkennwörtern** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows 2000 oder höher)
  
Wenn diese Richtlinieneinstellung aktiviert ist, kann ein sicherer Kanal nur mit Domänencontrollern eingerichtet werden, die Daten des sicheren Kanals mit einem starken Sitzungsschlüssel (128-Bit) verschlüsseln können.
  
Für diese Einstellung ist es erforderlich, dass alle Domänencontroller der Domäne fähig sind, Daten des sicheren Kanals mit einem starken Schlüssel zu verschlüsseln. Dies bedeutet, dass alle Domänencontrollern über Windows 2000 oder höher verfügen müssen. Wenn die Kommunikation mit Domänen erforderlich ist, die nicht auf Windows 2000 basieren, sollte diese Richtlinieneinstellung deaktiviert werden.
  
Die Einstellung **Domänenmitglied: Starker Sitzungsschlüssel erforderlich (Windows** **2000 oder höher)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### Interaktive Anmeldung
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für die interaktive Anmeldung zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.9: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Interaktive Anmeldung**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten</p></td>
<td style="border:1px solid black;"><p>Dieses System ist auf autorisierte Benutzer beschränkt. Der Versuch, nicht autorisierten Zugriff zu erlangen, wird strafrechtlich verfolgt.</p></td>
<td style="border:1px solid black;"><p>Dieses System ist auf autorisierte Benutzer beschränkt. Der Versuch, nicht autorisierten Zugriff zu erlangen, wird strafrechtlich verfolgt.</p></td>
<td style="border:1px solid black;"><p>Dieses System ist auf autorisierte Benutzer beschränkt. Der Versuch, nicht autorisierten Zugriff zu erlangen, wird strafrechtlich verfolgt.</p></td>
<td style="border:1px solid black;"><p>Dieses System ist auf autorisierte Benutzer beschränkt. Der Versuch, nicht autorisierten Zugriff zu erlangen, wird strafrechtlich verfolgt.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten</p></td>
<td style="border:1px solid black;"><p>SIE MACHEN SICH STRAFBAR, WENN SIE OHNE ERFORDERLICHE<br />
AUTORISIERUNG FORTFAHREN.</p></td>
<td style="border:1px solid black;"><p>SIE MACHEN SICH STRAFBAR, WENN SIE OHNE ERFORDERLICHE<br />
AUTORISIERUNG FORTFAHREN.</p></td>
<td style="border:1px solid black;"><p>SIE MACHEN SICH STRAFBAR, WENN SIE OHNE ERFORDERLICHE<br />
AUTORISIERUNG FORTFAHREN.</p></td>
<td style="border:1px solid black;"><p>SIE MACHEN SICH STRAFBAR, WENN SIE OHNE ERFORDERLICHE<br />
AUTORISIERUNG FORTFAHREN.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)</p></td>
<td style="border:1px solid black;"><p>2</p></td>
<td style="border:1px solid black;"><p>2</p></td>
<td style="border:1px solid black;"><p>0</p></td>
<td style="border:1px solid black;"><p>2</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern</p></td>
<td style="border:1px solid black;"><p>14 Tage</p></td>
<td style="border:1px solid black;"><p>14 Tage</p></td>
<td style="border:1px solid black;"><p>14 Tage</p></td>
<td style="border:1px solid black;"><p>14 Tage</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards</p></td>
<td style="border:1px solid black;"><p>Arbeitsstation sperren</p></td>
<td style="border:1px solid black;"><p>Arbeitsstation sperren</p></td>
<td style="border:1px solid black;"><p>Arbeitsstation sperren</p></td>
<td style="border:1px solid black;"><p>Arbeitsstation sperren</p></td>
</tr>  
</tbody>  
</table>
  
##### Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der Kontoname des zuletzt auf den Clientcomputern in Ihrer Organisation angemeldeten Benutzers auf dem Windows-Anmeldebildschirm jedes Computers angezeigt wird. Durch Aktivieren dieser Richtlinieneinstellung können Sie verhindern, dass Eindringlinge Kontonamen von den Bildschirmen der Desktop- oder Laptopcomputer in Ihrer Organisation ablesen können.
  
Die Einstellung **Interaktive Anmeldung: Letzten Benutzernamen nicht anzeigen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich
  
Mit der Tastenkombination STRG+ALT+ENTF wird ein vertrauenswürdiger Pfad zum Betriebssystem hergestellt, wenn der Benutzer Benutzernamen und Kennwort eingibt. Wenn diese Richtlinieneinstellung aktiviert ist, ist diese Tastenkombination nicht erforderlich, um sich im Netzwerk anzumelden. Diese Konfiguration stellt jedoch ein Sicherheitsrisiko dar, da sich Benutzer mit geringeren Anmeldeinformationen bei dem Client anmelden können.
  
Die Einstellung **Interaktive Anmeldung: Kein STRG+ALT+ENTF erforderlich** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten
  
Durch diese Richtlinieneinstellung wird eine Textmeldung festgelegt, die bei der Anmeldung eines Benutzers angezeigt wird. Dieser Text wird häufig aus rechtlichen Gründen verwendet, z. B. um Benutzer auf die Auswirkungen eines Missbrauchs von Firmeninformationen hinzuweisen, oder um sie davor zu warnen, dass ihre Aktionen überwacht werden. Der in der vorangegangenen Tabelle angegebene Nachrichtentext ist ein empfohlenes Beispiel sowohl für Unternehmensclient- als auch für Hochsicherheitsumgebungen.
  
Die Einstellung **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten** ist für die beiden in diesem Kapitel behandelten Umgebungen mit geeignetem Text aktiviert.
  
**Hinweis**: Jegliche angezeigte Warnung sollte zuerst von den juristischen Vertretern und der Personalabteilung der Organisation genehmigt werden. Außerdem müssen die Einstellungen **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten** und **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** beide aktiviert sein, damit jede für sich korrekt funktionieren kann.
  
##### Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten
  
Diese Richtlinieneinstellung ermöglicht das Festlegen von Text für die Titelleiste des Fensters, das Benutzer bei der Anmeldung beim System sehen. Der Grund für diese Richtlinieneinstellung ist derselbe wie für die vorangegangene Meldungstexteinstellung. Organisationen, die auf die Verwendung dieser Einstellung verzichten, sind rechtlich nicht gegen Unbefugte abgesichert, die das System angreifen.
  
Die Einstellung **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** ist für die beiden in diesem Kapitel behandelten Umgebungen mit geeignetem Text aktiviert.
  
**Hinweis**: Jegliche angezeigte Warnung sollte zuerst von den juristischen Vertretern und der Personalabteilung der Organisation genehmigt werden. Außerdem müssen die Einstellungen **Interaktive Anmeldung: Nachricht für Benutzer, die sich anmelden möchten** und **Interaktive Anmeldung: Nachrichtentitel für Benutzer, die sich anmelden möchten** beide aktiviert sein, damit jede für sich korrekt funktionieren kann.
  
##### Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Benutzer sich mit zwischengespeicherten Kontoinformationen bei einer Windows-Domäne anmelden kann. Anmeldeinformationen für Domänenkonten können lokal zwischengespeichert werden, um Benutzern selbst dann die Anmeldung zu ermöglichen, wenn kein Domänencontroller erreichbar ist. Durch diese Einstellung wird die Anzahl von eindeutigen Benutzern festgelegt, für die Anmeldeinformationen lokal zwischengespeichert werden. Der Standardwert für diese Richtlinieneinstellung lautet 10. Wenn dieser Wert auf 0 gesetzt wird, wird der Anmeldecache deaktiviert. Ein Angreifer mit Zugriff auf das Dateisystem des Servers kann die zwischengespeicherten Informationen suchen und mit Brute-Force-Methoden versuchen, die Benutzerkennwörter zu ermitteln.
  
Die Einstellung **Interaktive Anmeldung: Anzahl zwischenzuspeichernder vorheriger Anmeldungen (für den Fall, dass der Domänencontroller nicht verfügbar ist)** ist sowohl für Desktop- und Laptopcomputer in der Unternehmensclient-Umgebung und als auch für Laptopcomputer in der Hochsicherheitsumgebung auf **2** gesetzt. Für Desktops in der Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf **0** gesetzt, da diese Computer immer eine sichere Verbindung zum Netzwerk der Organisation haben sollten.
  
##### Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern
  
Durch diese Richtlinieneinstellung wird die Zeitspanne festgelegt, die Benutzer im Voraus auf den Ablauf ihrer Kennwörter hingewiesen werden. Microsoft empfiehlt, bei dieser Richtlinieneinstellung eine Frist von 14 Tagen einzugeben, damit Benutzer rechtzeitig über das Ablaufen des Kennworts informiert werden.
  
Die Einstellung **Interaktive Anmeldung: Anwender vor Ablauf des Kennworts zum Ändern des Kennworts auffordern** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **14 Tage** gesetzt.
  
##### Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich
  
Bei Aktivierung dieser Einstellung muss ein Domänencontroller das zum Entsperren des Computers verwendete Domänenkonto authentifizieren. Ist diese Richtlinieneinstellung deaktiviert, können zwischengespeicherte Anmeldeinformationen zum Aufheben der Sperrung des Computers verwendet werden. Microsoft empfiehlt, diese Richtlinieneinstellung für Laptopbenutzer in beiden Umgebungen zu deaktivieren, da mobile Benutzer keinen Netzwerkzugriff auf Domänencontrollern haben.
  
Die Einstellung **Interaktive Anmeldung: Domänencontrollerauthentifizierung zum Aufheben der Sperrung der Arbeitsstation erforderlich** ist sowohl in der Unternehmensclient-Umgebung als auch in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt. Diese Richtlinieneinstellung ist jedoch für Laptops in beiden Umgebungen auf **Deaktiviert** gesetzt, damit diese Benutzer auch außerhalb des Büros arbeiten können.
  
##### Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards
  
Durch diese Richtlinieneinstellung wird festgelegt, was passiert, wenn die Smartcard für einen angemeldeten Benutzer aus dem Smartcard-Leser entfernt wird. Wenn diese Richtlinieneinstellung auf **Arbeitsstation sperren** gesetzt ist, wird die Arbeitsstation beim Entfernen der Smartcard gesperrt. Auf diese Weise können Benutzer beim Verlassen des Arbeitsplatzes ihre Smartcards mitnehmen und ihre Arbeitsstationen automatisch sperren lassen. Wenn Sie diese Richtlinieneinstellung auf **Abmeldung erzwingen** einstellen, werden Benutzer bei der Entnahme der Smartcard automatisch abgemeldet.
  
Die Einstellung **Interaktive Anmeldung: Verhalten beim Entfernen von Smartcards** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Arbeitsstation sperren** gesetzt.
  
#### Microsoft-Netzwerk (Client)
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für Clientcomputer im Microsoft-Netzwerk zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.10: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Microsoft-Netzwerk (Client)**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Server zustimmt)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Microsoft-Netzwerk (Client): Kommunikation digital signieren (immer)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die SMB-Clientkomponente die Signierung von Paketen erfordert. Wenn Sie diese Richtlinieneinstellung aktivieren, kann der Microsoft-Netzwerkclient nur dann mit einem Microsoft-Netzwerkserver kommunizieren, wenn der Server der SMB-Paketsignierung zustimmt. In gemischten Umgebungen mit älteren Clients sollte diese Option auf **Deaktiviert** gesetzt werden, da diese Computer sich nicht authentifizieren und nicht auf Domänencontroller zugreifen können. In Umgebungen mit Windows 2000 oder höher kann diese Richtlinieneinstellung jedoch verwendet werden.
  
Die Einstellung **Microsoft Netzwerk (Client): Kommunikation digital signieren (immer)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis**: Wenn diese Richtlinieneinstellung auf Windows XP-Computern aktiviert ist und diese eine Verbindung zu Datei- oder Druckerfreigaben auf Remoteservern herstellen, muss die Einstellung unbedingt mit ihrer begleitenden Einstellung, **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)**, auf diesen Servern synchronisiert werden. Weitere Informationen zu diesen Einstellungen finden Sie im Abschnitt „Microsoft Netzwerk (Client und Server): Kommunikation digital signieren (vier zugehörige Einstellungen)“ in Kapitel 5 des Begleithandbuchs [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx heruntergeladen werden kann.
  
##### Microsoft-Netzwerk (Client): Kommunikation digital signieren (wenn Server zustimmt)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der SMB-Client versucht, die SMB-Paketsignierung auszuhandeln. Die Implementierung einer digitalen Signierung in Windows-Netzwerken trägt dazu bei, Sitzungsübernahmen zu verhindern. Wenn Sie diese Richtlinieneinstellung aktivieren, verwendet der Microsoft-Netzwerkclient die Signierung nur dann, wenn der Server, mit dem er kommuniziert, digital signierte Kommunikation akzeptiert.
  
Die Einstellung **Microsoft Netzwerk (Client): Kommunikationen digital signieren (wenn Server zustimmt)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis**: Aktivieren Sie diese Einstellung für SMB-Clients in Ihrem Netzwerk, damit Pakete bei der Kommunikation mit Clients und Servern in Ihrer Umgebung signiert werden.
  
##### Microsoft-Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden
  
Deaktivieren Sie diese Richtlinieneinstellung, um den SMB-Redirector davon abzuhalten, während der Authentifizierung Klartextkennwörter an Nicht-Microsoft-SMB-Server zu senden, die die Kennwortverschlüsselung nicht unterstützen. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, wenn keine wichtigen geschäftlichen Anforderungen dagegen sprechen. Wenn diese Richtlinieneinstellung aktiviert ist, sind im gesamten Netzwerk unverschlüsselte Kennwörter zugelassen.
  
Die Einstellung **Microsoft Netzwerk (Client): Unverschlüsseltes Kennwort an SMB-Server von Drittanbietern senden** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Microsoft-Netzwerk (Server)
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für Microsoft-Netzwerkserver zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.11: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Microsoft-Netzwerk (Server)**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung</p></td>
<td style="border:1px solid black;"><p>15 Minuten</p></td>
<td style="border:1px solid black;"><p>15 Minuten</p></td>
<td style="border:1px solid black;"><p>15 Minuten</p></td>
<td style="border:1px solid black;"><p>15 Minuten</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Client zustimmt)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung
  
Mit dieser Richtlinieneinstellung können Sie die Leerlaufzeitspanne in einer SMB-Sitzung festlegen, nach der die Sitzung aufgrund von Inaktivität angehalten wird. Administratoren können mit dieser Richtlinieneinstellung steuern, zu welchem Zeitpunkt eine nicht aktive Sitzung vom Computer angehalten wird. Wenn der Client seine Aktivität wieder aufnimmt, wird die Sitzung automatisch wiederhergestellt.
  
Die Einstellung **Microsoft-Netzwerk (Server): Leerlaufzeitspanne bis zum Anhalten der Sitzung** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** und auf eine Zeitspanne von **15 Minuten** gesetzt.
  
##### Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob SMB-Pakete vom SMB-Server signiert werden müssen. Aktivieren Sie diese Richtlinieneinstellung in einer gemischten Umgebung, damit Downstream-Clients Arbeitsstationen nicht als Netzwerkserver verwenden können.
  
Die Einstellung **Microsoft Netzwerk (Server): Kommunikation digital signieren (immer)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Microsoft-Netzwerk (Server): Kommunikation digital signieren (wenn Client zustimmt)
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der serverseitige SMB-Dienst SMB-Pakete signieren kann, wenn dies von einem Client angefordert wird, der eine Verbindung herzustellen versucht. Wenn vom Client keine Signaturanforderung kommt, wird eine Verbindung ohne Signatur zugelassen, wenn die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** nicht aktiviert ist.
  
Die Einstellung **Microsoft Netzwerk (Server): Kommunikation digital signieren (wenn Server zustimmt)** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
**Hinweis**: Aktivieren Sie diese Einstellung für SMB-Clients in Ihrem Netzwerk, damit Pakete bei der Kommunikation mit Clients und Servern in Ihrer Umgebung signiert werden.
  
#### Netzwerkzugriff
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für den Netzwerkzugriff zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.12: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Netzwerkzugriff**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>* In der folgenden Einstellungsbeschreibung finden Sie eine vollständige Liste von Named Pipes</p></td>
<td style="border:1px solid black;"><p>* In der folgenden Einstellungsbeschreibung finden Sie eine vollständige Liste von Named Pipes</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>* In der folgenden Einstellungsbeschreibung finden Sie eine vollständige Liste von Pfaden</p></td>
<td style="border:1px solid black;"><p>* In der folgenden Einstellungsbeschreibung finden Sie eine vollständige Liste von Pfaden</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>comcfg, dfs$</p></td>
<td style="border:1px solid black;"><p>comcfg, dfs$</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten</p></td>
<td style="border:1px solid black;"><p>Klassisch – lokale Benutzer authentifizieren sich als sie selbst</p></td>
<td style="border:1px solid black;"><p>Klassisch – lokale Benutzer authentifizieren sich als sie selbst</p></td>
<td style="border:1px solid black;"><p>Klassisch – lokale Benutzer authentifizieren sich als sie selbst</p></td>
<td style="border:1px solid black;"><p>Klassisch – lokale Benutzer authentifizieren sich als sie selbst</p></td>
</tr>  
</tbody>  
</table>
  
##### Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer Sicherheits-ID-Attribute anderer Benutzer anfordern können oder eine Sicherheits-ID (SID) verwenden können, um den zugehörigen Benutzernamen zu erhalten. Deaktivieren Sie diese Richtlinieneinstellung, um zu verhindern, dass nicht autorisierte Benutzer Benutzernamen über die zugehörigen Sicherheits-IDs in Erfahrung bringen.
  
Die Einstellung **Netzwerkzugriff: Anonyme SID-/Namensübersetzung zulassen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben
  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer die Konten in der Sicherheitskontenverwaltung (SAM, Security Accounts Manager) anzeigen lassen können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind Benutzer mit anonymen Verbindungen nicht in der Lage, Domänenkontonamen an einer Arbeitsstation in Ihrer Umgebung anzuzeigen. Durch diese Richtlinieneinstellung werden weitere Einschränkungen für anonyme Verbindungen ermöglicht.
  
Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben
  
Durch diese Richtlinieneinstellung wird festgelegt, ob anonyme Benutzer SAM-Konten und -Freigaben anzeigen lassen können. Wenn Sie diese Richtlinieneinstellung aktivieren, sind anonyme Benutzer nicht in der Lage, Domänenkontonamen und Namen für Netzwerkfreigaben an einer Arbeitsstation in Ihrer Umgebung anzuzeigen.
  
Die Einstellung **Netzwerkzugriff: Anonyme Aufzählung von SAM-Konten nicht erlauben** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben
  
Durch diese Richtlinieneinstellung wird die Speicherung der Anmeldeinformationen und Kennwörter auf dem lokalen System gesteuert.
  
Die Einstellung **Netzwerkzugriff: Speicherung von Anmeldeinformationen oder .NET-Passports für die Netzwerkauthentifikation nicht erlauben** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
##### Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen
  
Durch diese Richtlinieneinstellung wird festgelegt, welche zusätzlichen Berechtigungen anonymen Verbindungen mit dem Computer gewährt werden. Wenn Sie diese Richtlinieneinstellung aktivieren, können anonyme Windows-Benutzer bestimmte Aktivitäten ausführen, z. B. Auflisten der Namen von Domänenkonten und Netzwerkfreigaben. Ein nicht autorisierter Benutzer könnte Kontennamen und freigegebene Ressourcen anonym auflisten und anhand dieser Informationen Kennwörter erraten oder Social Engineering-Angriffe durchführen.
  
Deshalb ist die Einstellung **Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann
  
Durch diese Richtlinieneinstellung wird festgelegt, welche Kommunikationssitzungen oder Pipes über Attribute und Berechtigungen verfügen, die anonymen Zugriff zulassen.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Netzwerkzugriff: Named Pipes, auf die anonym zugegriffen werden kann** auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung werden jedoch folgende Standardwerte verwendet:
  
-   COMNAP
  
-   COMNODE
  
-   SQL\\QUERY
  
-   SPOOLSS
  
-   LLSRPC
  
-   Browser
  
##### Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann
  
Durch diese Richtlinieneinstellung wird festgelegt, auf welche Registrierungspfade zugegriffen werden kann, nachdem der Schlüssel WinReg zur Feststellung der Zugriffsberechtigungen für diese Pfade ausgewertet wurde.
  
Für die Unternehmensclient-Umgebung ist die Einstellung **Netzwerkzugriff: Registrierungspfade, auf die von anderen Computern aus zugegriffen werden kann** auf **Nicht definiert** gesetzt. Für die Hochsicherheitsumgebung werden jedoch folgende Standardwerte verwendet:
  
-   System\\CurrentControlSet\\Control\\ProductOptions
  
-   System\\CurrentControlSet\\Control\\Print\\Printers
  
-   System\\CurrentControlSet\\Control\\Server Applications
  
-   System\\CurrentControlSet\\Control\\ContentIndex
  
-   System\\CurrentControlSet\\Control\\Terminal Server
  
-   System\\CurrentControlSet\\Control\\Terminal Server\\UserConfig
  
-   System\\CurrentControlSet\\Control\\Terminal Server\\DefaultUserConfiguration
  
-   System\\CurrentControlSet\\Services\\Eventlog
  
-   Software\\Microsoft\\OLAP Server
  
-   Software\\Microsoft\\Windows NT\\CurrentVersion
  
##### Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann
  
Durch diese Richtlinieneinstellung werden die Netzwerkfreigaben festgelegt, auf die anonyme Benutzer zugreifen können. Die Standardeinstellung für diese Richtlinieneinstellung hat geringe Auswirkungen, da alle Benutzer authentifiziert werden müssen, bevor sie auf freigegebene Ressourcen auf dem Server zugreifen können.
  
Die Einstellung **Netzwerkzugriff: Freigaben, auf die anonym zugegriffen werden kann** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Sie sollten jedoch sicherstellen, dass diese Einstellung für die Hochsicherheitsumgebung auf **comcfg, dfs$** gesetzt ist.
  
**Hinweis**: Es kann sehr gefährlich sein, dieser Gruppenrichtlinieneinstellung weitere Freigaben hinzuzufügen. Jeder Benutzer im Netzwerk erhält Zugriff auf die aufgeführten Freigaben, was zur Offenlegung oder Beschädigung vertraulicher Daten führen kann.
  
##### Netzwerkzugriff: Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten
  
Durch diese Richtlinieneinstellung wird festgelegt, wie Netzwerkanmeldungen über lokale Konten authentifiziert werden. Die Option **Klassisch** ermöglicht eine präzise Steuerung des Zugriffs auf Ressourcen, einschließlich der Möglichkeit, verschiedenen Benutzern unterschiedliche Zugriffstypen für dieselbe Ressource zuzuweisen. Die Option **Nur Gast** ermöglicht Ihnen, alle Benutzer gleich zu behandeln. In diesem Fall werden alle Benutzer als **Nur Gast** authentifiziert und haben dieselben Zugriffsrechte auf die jeweilige Ressource.
  
Daher verwendet die Einstellung **Modell für gemeinsame Nutzung und Sicherheitsmodell für lokale Konten** für die beiden in diesem Kapitel behandelten Umgebungen die standardmäßige Option **Klassisch**.
  
#### Netzwerksicherheit
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für die Netzwerksicherheit zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.13: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Netzwerksicherheit**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerksicherheit: LAN Manager-Authentifizierungsebene</p></td>
<td style="border:1px solid black;"><p>Nur NTLMv2-Antworten senden\LM verweigern</p></td>
<td style="border:1px solid black;"><p>Nur NTLMv2-Antworten senden\LM verweigern</p></td>
<td style="border:1px solid black;"><p>Nur NTLMv2-Antworten senden\LM und NTLM verweigern</p></td>
<td style="border:1px solid black;"><p>Nur NTLMv2-Antworten senden\LM und NTLM verweigern</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerksicherheit: Signaturanforderungen für LDAP-Clients</p></td>
<td style="border:1px solid black;"><p>Signatur aushandeln</p></td>
<td style="border:1px solid black;"><p>Signatur aushandeln</p></td>
<td style="border:1px solid black;"><p>Signatur aushandeln</p></td>
<td style="border:1px solid black;"><p>Signatur aushandeln</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
<td style="border:1px solid black;"><p>Nachrichtvertraulichkeit erfordern, Nachrichtenintegrität erfordern, NTLMv2-Sitzungssicherheit erfordern,<br />
128-Bit-Verschlüsselung erfordern</p></td>
</tr>
</tbody>
</table>
<p> </p>

##### Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern

Durch diese Richtlinieneinstellung wird festgelegt, ob die bei der Änderung von Kennwörtern vom LAN Manager (LM) erzeugten Hashwerte für das neue Kennwort gespeichert werden. LM-Hashwerte sind anfälliger für Angriffe, weil für ihre Erzeugung im Vergleich zu Windows NT®-Hashwerten ein schwächerer kryptografischer Algorithmus verwendet wird.

Aus diesem Grund ist die Einstellung **Netzwerksicherheit: Keine LAN Manager-Hashwerte für nächste Kennwortänderung speichern** für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.

**Hinweis**: Sehr alte Betriebssysteme und einige Anwendungen von Drittanbietern fallen möglicherweise aus, wenn diese Einstellung aktiviert ist. Außerdem müssen Sie nach dem Aktivieren dieser Einstellung die Kennwörter sämtlicher Konten ändern.

##### Netzwerksicherheit: LAN Manager-Authentifizierungsebene

Durch diese Richtlinieneinstellung wird der Typ der Abfrage/Rückmeldung-Authentifizierung für Netzwerkanmeldungen von Clients festgelegt, die nicht Windows 2000 oder Windows XP Professional ausführen. Die Authentifizierung über LAN Manager (LM) ist die unsicherste Methode, da verschlüsselte Kennwörter leicht über das Netzwerk abgefangen und entschlüsselt werden können. NT LAN Manager (NTLM) ist etwas sicherer. NTLMv2 ist robuster als NTLM und kann unter Windows XP Professional, Windows 2000 und Windows NT 4.0 Service Pack 4 oder höher verwendet werden. NTLMv2 ist zusammen mit dem optionalen Client für Verzeichnisdienste auch unter Windows 95 und Windows 98 verfügbar.

Microsoft empfiehlt, für diese Richtlinieneinstellung in Ihrer Umgebung die höchste Authentifizierungsebene auszuwählen. Bei Verwendung von Windows 2000 Server oder Windows Server 2003 mit Windows XP Professional-Arbeitsstationen wird empfohlen, für diese Richtlinieneinstellung die Option **Nur NTLMv2-Antworten senden\\LM und NTLM verweigern** zu wählen, um maximale Sicherheit zu gewährleisten.

Die Einstellung **Netzwerksicherheit: LAN Manager-Authentifizierungsebene** ist für die Unternehmensclient-Umgebung auf **Nur NTLMv2-Antworten senden\\LM verweigern** gesetzt. Für die Hochsicherheitsumgebung ist diese Richtlinieneinstellung jedoch auf das stärker einschränkende **Nur NTLMv2-Antworten senden\\LM und NTLM verweigern** gesetzt.

##### Netzwerksicherheit: Signaturanforderungen für LDAP-Clients

Durch diese Richtlinieneinstellung wird die Datensignaturebene festgelegt, die im Auftrag von Clients angefordert wird, wenn diese LDAP-BIND-Anforderungen ausgeben. Nicht signierter Netzwerkverkehr ist für Man-in-the-Middle-Angriffe anfällig. Ein Angreifer könnte einen Server veranlassen, Entscheidungen zu treffen, die auf falschen Anfragen vom LDAP-Client basieren.

Daher wird der Wert für die Einstellung **Netzwerksicherheit: Signaturanforderungen für LDAP-Clients** für die beiden in diesem Kapitel behandelten Umgebungen auf **Signatur aushandeln** gesetzt.

##### Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)

Durch diese Richtlinieneinstellung werden die minimalen Sicherheitsstandards für die Kommunikation zwischen Anwendungen auf Clients festgelegt. Die Optionen für diese Richtlinieneinstellung lauten:

-   Nachrichtenintegrität erfordern

-   Nachrichtenvertraulichkeit erfordern

-   NTLMv2-Sitzungssicherheit erfordern

-   128-Bit-Verschlüsselung erfordern

Wenn alle Computer in Ihrem Netzwerk NTLMv2- und 128-Bit-Verschlüsselung unterstützen (z. B. Windows XP Professional SP2 und Windows Server 2003 SP1), können für maximale Sicherheit alle vier Einstellungsoptionen ausgewählt werden.

Für die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)** sind in den beiden in diesem Kapitel behandelten Umgebungen alle vier Optionen aktiviert.

##### Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Server (einschließlich sicherer RPC-Server)

Diese Richtlinieneinstellung ähnelt der vorherigen Einstellung, wirkt sich aber auf die serverseitige Kommunikation mit Anwendungen aus. Die Optionen für die Einstellung sind dieselben:

-   Nachrichtenintegrität erfordern

-   Nachrichtenvertraulichkeit erfordern

-   NTLMv2-Sitzungssicherheit erfordern

-   128-Bit-Verschlüsselung erfordern

Wenn alle Computer in Ihrem Netzwerk NTLMv2- und 128-Bit-Verschlüsselung unterstützen (z. B. Windows XP Professional SP2 und Windows Server 2003 SP1), können für maximale Sicherheit alle vier Optionen ausgewählt werden.

Für die Einstellung **Netzwerksicherheit: Minimale Sitzungssicherheit für NTLM-SSP-basierte Clients (einschließlich sicherer RPC-Clients)** sind in den beiden in diesem Kapitel behandelten Umgebungen alle vier Optionen aktiviert.

#### Wiederherstellungskonsole

In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für die Wiederherstellungskonsole zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.

**Tabelle 3.14: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Wiederherstellungskonsole**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Einstellung</p></th>
<th><p>Unternehmensclient-Desktop</p></th>
<th><p>Unternehmensclient-Laptop</p></th>
<th><p>Hochsicher-Desktop</p></th>
<th><p>Hochsicher-Laptop</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen
  
Die Wiederherstellungskonsole ist eine Befehlszeilenumgebung, mit der nach Systemproblemen eine Wiederherstellung vorgenommen werden kann. Wenn Sie diese Richtlinieneinstellung aktivieren, wird das Administratorkonto automatisch bei der Wiederherstellungskonsole angemeldet, wenn diese Einstellung beim Start aufgerufen wird. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, sodass Administratoren ein Kennwort eingeben müssen, um auf die Wiederherstellungskonsole zugreifen zu können.
  
Die Einstellung **Wiederherstellungskonsole: Automatische administrative Anmeldungen zulassen** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
##### Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen
  
Durch diese Richtlinieneinstellung wird in der Wiederherstellungskonsole der Befehl SET verfügbar, mit dem Sie die folgenden Umgebungsvariablen für die Wiederherstellungskonsole einstellen können:
  
-   **AllowWildCards**. Aktiviert die Platzhalterunterstützung für einige Befehle (z. B. für den Befehl DEL).
  
-   **AllowAllPaths**. Ermöglicht den Zugriff auf alle Dateien und Ordner auf dem Computer.
  
-   **AllowRemovableMedia**. Ermöglicht das Kopieren von Dateien auf Wechselmedien wie Disketten.
  
-   **NoCopyPrompt**. Unterdrückt die Anzeige einer Eingabeaufforderung beim Überschreiben einer vorhandenen Datei.
  
Die Einstellung **Wiederherstellungskonsole: Kopieren von Disketten und Zugriff auf alle Laufwerke und alle Ordner zulassen** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. Zum Gewährleisten maximaler Sicherheit wird diese Einstellung in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### Herunterfahren
  
In der folgenden Tabelle sind die Empfehlungen für die Einstellungen der Sicherheitsoptionen beim Herunterfahren zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.15: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Herunterfahren**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Herunterfahren: Auslagerungsdatei des virtuellen Arbeitspeichers löschen</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob ein Computer heruntergefahren werden kann, wenn ein Benutzer nicht angemeldet ist. Wenn diese Richtlinieneinstellung aktiviert ist, steht im Windows-Anmeldebildschirm der Befehl „Herunterfahren“ zur Verfügung. Microsoft empfiehlt, diese Richtlinieneinstellung zu deaktivieren, um nur jenen Benutzern das Herunterfahren von Computern zu ermöglichen, die über Anmeldeinformationen im System verfügen.
  
Die Einstellung **Herunterfahren: Herunterfahren des Systems ohne Anmeldung zulassen** ist in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
##### Herunterfahren: Auslagerungsdatei des virtuellen Arbeitspeichers löschen
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Auslagerungsdatei des virtuellen Arbeitsspeichers beim Herunterfahren des Systems gelöscht wird. Wenn diese Richtlinieneinstellung aktiviert ist, wird die Auslagerungsdatei des Systems bei jedem fehlerfreien Herunterfahren des Systems gelöscht. Bei Aktivierung dieser Sicherheitsoption wird die Ruhezustanddatei (hiberfil.sys) auch dann gelöscht, wenn die Ruhezustandfunktion auf einem tragbaren Computer deaktiviert ist. Das Herunterfahren und Neustarten des Servers dauert länger, insbesondere auf Servern mit großen Auslagerungsdateien.
  
Aus diesen Gründen ist die Einstellung **Herunterfahren: Auslagerungsdatei des virtuellen Arbeitspeichers löschen** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Systemkryptografie
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für die Systemkryptografie zusammengefasst. Im Anschluss an die Tabelle werden weitere Informationen bereitgestellt.
  
**Tabelle 3.16: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Systemkryptografie**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der TLS/SSL-Sicherheitsdienst nur die Verschlüsselungssammlung TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA unterstützt. Obwohl durch diese Richtlinieneinstellung die Sicherheit erhöht wird, werden diese Algorithmen von den meisten öffentlichen Websites, die mit TLS oder SSL gesichert sind, nicht unterstützt. Clientcomputer, für die diese Richtlinieneinstellung aktiviert ist, können auch keine Verbindung zu Terminaldiensten auf Servern herstellen, die nicht für die Verwendung der FIPS-konformen Algorithmen konfiguriert sind.
  
Die Einstellung **Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
**Hinweis**: Wenn Sie diese Richtlinieneinstellung aktivieren, verlangsamt sich die Systemleistung des Computers, da durch den Dreifach-DES-Prozess die Verschlüsselung für jeden einzelnen Datenblock in der betreffenden Datei dreimal ausgeführt wird. Diese Richtlinieneinstellung sollte nur aktiviert werden, wenn für Ihre Organisation FIPS-Konformität erforderlich ist.
  
#### Systemobjekte
  
In der folgenden Tabelle sind die empfohlenen Einstellungen der Sicherheitsoptionen für die Systemobjekte zusammengefasst. Weitere Informationen finden Sie in den Unterabschnitten, die der Tabelle folgen.
  
**Tabelle 3.16: Empfehlungen für die Einstellungen der Sicherheitsoptionen – Systemobjekte**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Systemobjekte: Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden</p></td>
<td style="border:1px solid black;"><p>Objektersteller</p></td>
<td style="border:1px solid black;"><p>Objektersteller</p></td>
<td style="border:1px solid black;"><p>Objektersteller</p></td>
<td style="border:1px solid black;"><p>Objektersteller</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
</tbody>  
</table>
  
##### Systemobjekte: Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden
  
Durch diese Richtlinieneinstellung wird festgelegt, ob die Gruppe **Administratoren** oder die Gruppe **Objektersteller** der Standardbesitzer neuer Systemobjekte ist.
  
Um Verantwortlichkeiten übersichtlicher zu gestalten, ist die Einstellung **Systemobjekte: Standardbesitzer für Objekte, die von Mitgliedern der Administratorengruppe erstellt werden** für die beiden in diesem Kapitel behandelten Umgebungen auf **Objektersteller** gesetzt.
  
##### Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren
  
Durch diese Richtlinieneinstellung wird festgelegt, ob für alle Subsysteme das Ignorieren der Groß-/Kleinschreibung erzwungen wird. Für das Microsoft Win32®-Subsystem wird die Groß-/Kleinschreibung ignoriert. Der Kernel unterstützt jedoch die Beachtung der Groß-/Kleinschreibung für andere Subsysteme, z. B. POIX (Portable Operating System Interface für UNIX). Da unter Windows die Groß-/Kleinschreibung ignoriert wird (das POSIX-Subsystem jedoch die Beachtung der Groß-/Kleinschreibung unterstützt), kann ein Benutzer dieses Subsystems durch Mischen von Groß- und Kleinbuchstaben eine Datei mit einem bereits vorhandenen Namen erstellen, wenn diese Richtlinieneinstellung deaktiviert ist. In so einer Situation kann der Zugriff auf diese Dateien durch einen anderen Benutzer blockiert werden, der typische Win32-Tools verwendet, weil nur eine der Dateien zur Verfügung steht.
  
Zum Gewährleisten der Konsistenz von Dateinamen ist die Einstellung **Systemobjekte: Groß-/Kleinschreibung für Nicht-Windows-Subsysteme ignorieren** in der Unternehmensclient-Umgebung auf **Nicht definiert** und in der Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
##### Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken
  
Durch diese Richtlinieneinstellung wird die Stärke der wahlfreien Zugriffssteuerungsliste (DACL) für Objekte festgelegt. Diese Einstellung trägt zur Sicherung von Objekten bei, die zwischen Projekten gesucht und freigegeben werden können. Die Standardkonfiguration der Einstellung verstärkt die DACL, wodurch Nicht-Administratoren das Lesen von freigegebenen Objekten ermöglicht wird. Sie können jedoch nur die von ihnen selbst erstellten Objekte ändern.
  
Daher ist die Einstellung **Systemobjekte: Standardberechtigungen interner Systemobjekte verstärken** (z. B. symbolische Verknüpfungen) für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Sicherheitseinstellungen für das Ereignisprotokoll
  
Im Ereignisprotokoll werden Ereignisse im System erfasst, während im Sicherheitsprotokoll Überwachungsereignisse aufgezeichnet werden. Der Ereignisprotokoll-Container der Gruppenrichtlinie dient zum Definieren von Attributen für die Anwendungs-, Sicherheits- und Systemereignisprotokolle, z. B. maximale Protokollgröße, Zugriffsrechte für jedes Protokoll sowie Einstellungen für die Dauer und Methode der Aufbewahrung. Die Einstellungen für die Anwendungs-, Sicherheits- und Systemereignisprotokolle werden in der Mitgliedsserver-Baseline-Richtlinie konfiguriert und auf alle Mitgliedsserver in der Domäne angewendet.
  
Die Ereignisprotokolleinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Ereignisprotokoll**
  
Dieser Abschnitt enthält Informationen zu den empfohlenen Einstellungen für die Umgebungen, die in diesem Kapitel erörtert werden. Eine Zusammenfassung der in diesem Abschnitt empfohlenen Einstellungen finden Sie in der Microsoft Excel®-Arbeitsmappe „Windows XP Security Guide Settings“. Informationen zu den Standardeinstellungen und ausführliche Erklärungen zu den in diesem Abschnitt beschriebenen Einstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx verfügbar ist. Das Begleithandbuch enthält auch ausführliche Informationen zur Gefahr des Verlustes von Ereignisprotokolldaten, wenn die Protokollgrößen auf sehr große Werte gesetzt sind.
  
In der folgenden Tabelle werden die empfohlenen Ereignisprotokolleinstellungen sowohl für Desktop- als auch für Laptopclients in den beiden Arten von Umgebungen zusammengefasst, die in diesem Kapitel erörtert werden: die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung. Ausführlichere Informationen zu jeder Einstellung finden Sie in den folgenden Unterabschnitten.
  
**Tabelle 3.18: Empfohlene Sicherheitseinstellungen für Ereignisprotokolle**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellung</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Maximale Größe des Anwendungsprotokolls</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Maximale Größe des Sicherheitsprotokolls</p></td>
<td style="border:1px solid black;"><p>81920 KB</p></td>
<td style="border:1px solid black;"><p>81920 KB</p></td>
<td style="border:1px solid black;"><p>81920 KB</p></td>
<td style="border:1px solid black;"><p>81920 KB</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Maximale Größe des Systemprotokolls</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
<td style="border:1px solid black;"><p>16384 KB</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Lokalen Gastkontozugriff auf Systemprotokoll verhindern</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Aufbewahrungsmethode des Anwendungsprotokolls</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Aufbewahrungsmethode des Sicherheitsprotokolls</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Aufbewahrungsmethode des Systemprotokolls</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
<td style="border:1px solid black;"><p>Bei Bedarf</p></td>
</tr>  
</tbody>  
</table>
  
#### Maximale Größe des Anwendungsprotokolls
  
Durch diese Richtlinieneinstellung wird die maximale Größe des Anwendungsereignisprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen an die Anwendungsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Anwendungsprotokolls** ist für alle Computer in den beiden in diesem Kapitel behandelten Umgebungen auf **16384 KB** gesetzt.
  
#### Maximale Größe des Sicherheitsprotokolls
  
Durch diese Richtlinieneinstellung wird die maximale Größe des Sicherheitsprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen an die Sicherheitsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Sicherheitsprotokolls** ist für alle Computer in den beiden in diesem Kapitel behandelten Umgebungen auf **81920 KB** gesetzt.
  
#### Maximale Größe des Systemprotokolls
  
Durch diese Richtlinieneinstellung wird die maximale Größe des Systemprotokolls festgelegt, dessen maximale Kapazität 4 GB beträgt. Diese Größe wird jedoch nicht empfohlen, da die Arbeitsspeicherfragmentierung zu einer verringerten Leistung und einer unzuverlässigen Ereignisprotokollierung führen kann. Die Anforderungen für die Anwendungsprotokollgröße richten sich nach der Funktion der Plattform und dem Bedarf an Verlaufsdatensätzen für anwendungsspezifische Ereignisse.
  
Die Einstellung **Maximale Größe des Systemprotokolls** ist für alle Computer in den beiden in diesem Kapitel behandelten Umgebungen auf **16384 KB** gesetzt.
  
#### Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Anwendungsereignisprotokoll zuzugreifen. Unter Windows Server 2003 ist der Gastzugriff standardmäßig auf allen Systemen nicht zulässig. Diese Einstellung hat daher keinen Einfluss auf standardmäßige Systemkonfigurationen. Diese Option gilt jedoch als Tiefenverteidigungseinstellung ohne unerwünschte Nebenwirkungen.
  
Die Einstellung **Lokalen Gastkontozugriff auf Anwendungsprotokoll verhindern** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Sicherheitsereignisprotokoll zuzugreifen. Für den Zugriff auf das Sicherheitsprotokoll muss ein Benutzer das Recht **Verwalten von Überwachungs- und Sicherheitsprotokoll** besitzen. (Dieses Recht wird in diesem Handbuch nicht beschrieben.) Diese Einstellung hat daher keinen Einfluss auf standardmäßige Systemkonfigurationen. Diese Option gilt jedoch als Tiefenverteidigungseinstellung ohne unerwünschte Nebenwirkungen.
  
Die Einstellung **Lokalen Gastkontozugriff auf Sicherheitsprotokoll verhindern** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### Lokalen Gastkontozugriff auf Systemprotokoll verhindern
  
Durch diese Richtlinieneinstellung wird festgelegt, ob Gäste daran gehindert werden, auf das Systemereignisprotokoll zuzugreifen. Unter Windows Server 2003 ist der Gastzugriff standardmäßig auf allen Systemen nicht zulässig. Diese Einstellung hat daher keinen Einfluss auf standardmäßige Systemkonfigurationen. Diese Option gilt jedoch als Tiefenverteidigungseinstellung ohne unerwünschte Nebenwirkungen.
  
Die Einstellung **Lokalen Gastkontozugriff auf Systemprotokoll verhindern** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### Aufbewahrungsmethode des Anwendungsprotokolls
  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Anwendungsprotokoll festgelegt. Das Anwendungsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen stellt sicher, dass im Protokoll immer die neuesten Ereignisse gespeichert werden. Dies kann jedoch auch zu einem Verlust von Verlaufsdaten führen.
  
Die **Aufbewahrungsmethode des Anwendungsprotokolls** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
#### Aufbewahrungsmethode des Sicherheitsprotokolls
  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Sicherheitsprotokoll festgelegt. Das Sicherheitsprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen stellt sicher, dass im Protokoll immer die neuesten Ereignisse gespeichert werden. Dies kann jedoch auch zu einem Verlust von Verlaufsdaten führen.
  
Die **Aufbewahrungsmethode des Sicherheitsprotokolls** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
#### Aufbewahrungsmethode des Systemprotokolls
  
Durch diese Richtlinieneinstellung wird die „Umbruchmethode“ für das Systemprotokoll festgelegt. Das Systemprotokoll muss regelmäßig archiviert werden, wenn Verlaufsdaten für forensische Zwecke oder zur Problembehandlung aufbewahrt werden sollen. Das bedarfsabhängige Überschreiben von Ereignissen stellt sicher, dass im Protokoll immer die neuesten Ereignisse gespeichert werden. Dies kann jedoch auch zu einem Verlust von Verlaufsdaten führen.
  
Die **Aufbewahrungsmethode des Systemprotokolls** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Bei Bedarf** gesetzt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Eingeschränkte Gruppen
  
Mit der Einstellung „Eingeschränkte Gruppen“ können Sie über die Gruppenrichtlinien von Active Directory die Gruppenzugehörigkeit unter Windows XP Professional verwalten. Prüfen Sie zunächst die Anforderungen Ihrer Organisation, bevor Sie die einzuschränkenden Gruppen festlegen. Für dieses Handbuch sind die Gruppen **Sicherungs-Operatoren** und **Hauptbenutzer** in beiden Umgebungen eingeschränkt, aber die Gruppe **Remotedesktopbenutzer** ist nur für die Hochsicherheitsumgebung eingeschränkt. Obwohl Mitglieder der Gruppen **Sicherungs-Operatoren** und **Hauptbenutzer** weniger Berechtigungen für den Systemzugriff haben als Mitglieder der Gruppe **Administratoren**, verfügen sie immer noch über einen weit reichenden Zugriff auf das System.
  
**Hinweis**: Wenn Ihre Organisation eine dieser Gruppen verwendet, sollten Sie deren Mitgliedschaft sorgfältig überprüfen und die Anleitung für die Einstellung „Eingeschränkte Gruppen“ nicht implementieren. Wenn Ihre Organisation der Gruppe „Hauptbenutzer“ Benutzer hinzufügt, sollten Sie u. U. die optionalen Dateisystemberechtigungen implementieren, die im Abschnitt „Sichern des Dateisystems“ weiter unten in diesem Kapitel beschrieben werden.
  
**Tabelle 3.19: Empfehlungen für eingeschränkte Gruppen**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Lokale Gruppe</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Sicherungs-Operatoren</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Hauptbenutzer</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Remotedesktopbenutzer</p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p> </p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
<td style="border:1px solid black;"><p>Keine Mitglieder</p></td>
</tr>  
</tbody>  
</table>
  
Die Einstellung „Eingeschränkte Gruppen“ kann im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Eingeschränkte Gruppen\\**
  
Administratoren können eingeschränkte Gruppen für ein Gruppenrichtlinienobjekt konfigurieren, indem sie die gewünschte Gruppe direkt dem Knoten **Eingeschränkte Gruppen** im Namespace des Gruppenrichtlinienobjekts hinzufügen.
  
Ist eine Gruppe eingeschränkt, können deren Mitglieder und andere Gruppen, denen sie angehört, festgelegt werden. Wenn Sie diese Gruppenmitglieder nicht angeben, bleibt die Gruppe vollkommen eingeschränkt. Gruppen können nur durch die Verwendung von Sicherheitsvorlagen eingeschränkt werden.
  
**So zeigen Sie die Einstellung „Eingeschränkte Gruppen“ an oder ändern diese**
  
1.  Öffnen Sie die Sicherheitsvorlagen-Verwaltungskonsole.
  
    **Hinweis**: Die Sicherheitsvorlagen-Verwaltungskonsole ist standardmäßig nicht im Menü **Verwaltung** nicht vorhanden. Um sie hinzuzufügen, starten Sie die Microsoft Management Console (mmc.exe), und fügen Sie das Add-In „Sicherheitsvorlagen“ hinzu.
  
2.  Doppelklicken Sie auf das Verzeichnis der Konfigurationsdatei und dann auf die Konfigurationsdatei.
  
3.  Doppelklicken Sie auf das Element **Eingeschränkte Gruppen**.
  
4.  Klicken Sie mit der rechten Maustaste auf **Eingeschränkte Gruppen** und dann auf **Gruppe hinzufügen**.
  
5.  Klicken Sie auf **Durchsuchen** und dann auf **Pfad**, wählen Sie den gewünschten Pfad aus, und klicken Sie auf **OK**.
  
    **Hinweis**: Normalerweise wird der lokale Computer oben in der Liste angezeigt.
  
6.  Geben Sie im Textfeld **Geben Sie die zu verwendenden Objektnamen ein** den Gruppennamen ein, und klicken Sie auf die Schaltfläche **Namen überprüfen**.
  
    – Oder –
  
    Klicken Sie auf **Erweitert** und anschließend auf **Suche starten**, um alle verfügbaren Gruppen aufzulisten.
  
7.  Wählen Sie die einzuschränkenden Gruppen aus, und klicken Sie auf **OK**.
  
8.  Klicken Sie im Dialogfeld **Gruppen hinzufügen** auf **OK**, um das Dialogfeld zu schließen.
  
In diesem Handbuch wurden die Einstellungen für alle Mitglieder – Benutzer und Gruppen – der Gruppen „Hauptbenutzer“ und „Sicherungs-Operatoren“ entfernt, um sie in beiden Umgebungen vollständig einzuschränken. In der Hochsicherheitsumgebung wurden ebenfalls alle Mitglieder der Gruppe „Remotedesktopbenutzer“ entfernt. Microsoft empfiehlt, alle vordefinierten Gruppen, die in Ihrer Organisation nicht verwendet werden, einschränken.
  
**Hinweis**: Die Konfiguration der in diesem Abschnitt beschriebenen Einstellung **Eingeschränkte Gruppen** ist sehr einfach. Versionen von Windows XP SP1 oder höher sowie Windows Server 2003 unterstützen komplexere Entwürfe. Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Updates to Restricted Groups ("Member of") Behavior of User-Defined Local Groups](http://support.microsoft.com/default.aspx?kbid=810076)“ (in englischer Sprache) unter http://support.microsoft.com/default.aspx?kbid=810076.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Systemdienste
  
Bei der Installation von Windows XP Professional werden Standardsystemdienste erstellt und für die Ausführung beim Systemstart konfiguriert. Viele dieser Systemdienste müssen in den diesem Kapitel beschriebenen Umgebungen nicht ausgeführt werden.
  
Unter Windows XP Professional sind zusätzliche optionale Dienste wie IIS verfügbar, die bei der Standardinstallation des Betriebssystems nicht installiert werden. Sie können diese optionalen Dienste einem installierten System hinzufügen, indem Sie in der Systemsteuerung den Eintrag „Software“ auswählen, oder indem Sie eine benutzerdefinierte automatisierte Installation von Windows XP Professional erstellen.
  
**Wichtig**: Beachten Sie, dass jeder Dienst und jede Anwendung einen potenziellen Angriffspunkt darstellt. Daher sollten nicht benötigte Dienste oder ausführbare Dateien in der Umgebung deaktiviert bzw. entfernt werden.
  
Die Einstellungen der Systemdienste können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellung\\Sicherheitseinstellungen\\Systemdienste**
  
Administratoren können den Startmodus der Systemdienste einstellen und die jeweiligen Sicherheitseinstellungen ändern.
  
**Wichtig**: Versionen der grafischen Tools zum Bearbeiten von Diensten, die in Prä-Windows 2003-Versionen des Windows-Betriebssystems enthalten sind, wenden automatisch Berechtigungen auf jeden Dienst an, wenn eine beliebige Eigenschaft eines Dienstes konfiguriert wird. Tools wie z. B. der Gruppenrichtlinienobjekt-Editor und das Snap-In „Sicherheitsvorlagen“ verwenden zum Anwenden dieser Berechtigungen die Sicherheitskonfigurations-Editor-DLL. Wenn die Standardberechtigungen verändert werden, treten bei vielen Diensten eine Reihe von Problemen auf. Microsoft empfiehlt, die Berechtigungen von Diensten, die in Windows XP oder Windows Server 2003 enthalten sind, nicht zu verändern, da die Standardberechtigungen bereits eine starke Einschränkung darstellen.  
Die Windows Server 2003-Version der Sicherheitskonfigurations-Editor-DLL zwingt Sie nicht zum Konfigurieren von Berechtigungen, wenn Sie die Eigenschaften eines Dienstes bearbeiten. Weitere Information finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx)*,* das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx verfügbar ist.
  
In der folgenden Tabelle sind die empfohlenen Systemdiensteinstellungen sowohl für Desktop- als auch für Laptopclients in den beiden Arten von Umgebungen zusammengefasst, die in diesem Kapitel behandelt werden: die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung. Ausführlichere Informationen zu jeder Einstellung finden Sie in den folgenden Unterabschnitten.
  
**Tabelle 3.20: Empfehlungen für die Sicherheitseinstellungen von Systemdiensten**
  
<table style="width:100%;">  
<colgroup>  
<col width="16%" />  
<col width="16%" />  
<col width="16%" />  
<col width="16%" />  
<col width="16%" />  
<col width="16%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Dienstname</p></th>  
<th><p>Anzeigename</p></th>  
<th><p>Unternehmensclient-Desktop</p></th>  
<th><p>Unternehmensclient-Laptop</p></th>  
<th><p>Hochsicher-Desktop</p></th>  
<th><p>Hochsicher-Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Warndienst</p></td>
<td style="border:1px solid black;"><p>Warndienst</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ClipSrv</p></td>
<td style="border:1px solid black;"><p>Ablagemappe</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Browser</p></td>
<td style="border:1px solid black;"><p>Computerbrowser</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Fax</p></td>
<td style="border:1px solid black;"><p>Fax</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSFtpsvr</p></td>
<td style="border:1px solid black;"><p>FTP-Publishing</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>IISADMIN</p></td>
<td style="border:1px solid black;"><p>IIS-Verwaltung</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>cisvc</p></td>
<td style="border:1px solid black;"><p>Indexdienst</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Messenger</p></td>
<td style="border:1px solid black;"><p>Messenger</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>mnmsrvc</p></td>
<td style="border:1px solid black;"><p>NetMeeting®-Remotedesktop-Freigabe</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RDSessMgr</p></td>
<td style="border:1px solid black;"><p>Sitzungs-Manager für Remotedesktophilfe</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RemoteAccess</p></td>
<td style="border:1px solid black;"><p>Routing und RAS</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>SNMP</p></td>
<td style="border:1px solid black;"><p>SNMP-Dienst</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SNMPTRAP</p></td>
<td style="border:1px solid black;"><p>SNMP-Trap-Dienst</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>SSDPSrv</p></td>
<td style="border:1px solid black;"><p>SSDP-Suchdienst</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Schedule</p></td>
<td style="border:1px solid black;"><p>Taskplaner</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>TlntSvr</p></td>
<td style="border:1px solid black;"><p>Telnet</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>TermService</p></td>
<td style="border:1px solid black;"><p>Terminaldienste</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Upnphost</p></td>
<td style="border:1px solid black;"><p>Host für universelle Plug &amp; Play-Geräte</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>W3SVC</p></td>
<td style="border:1px solid black;"><p>WWW-Publishing</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
</tbody>  
</table>
  
#### Warndienst
  
Durch diesen Dienst erhalten ausgewählte Benutzer und Computer administrative Warnmeldungen. Mit diesem Dienst können Sie Warnmeldungen an bestimmte Benutzer senden, die mit dem Netzwerk verbunden sind.
  
Der **Warndienst** ist auf **Deaktiviert** gesetzt, damit das Senden von Informationen über das Netzwerk vermieden wird. Diese Konfiguration gewährleistet größere Sicherheit für die beiden in diesem Kapitel behandelten Umgebungen.
  
**Hinweis**: Die Funktionsfähigkeit von Warnmeldesystemen für die unterbrechungsfreie Stromversorgung (USV) kann bei Deaktivierung dieses Dienstes beeinträchtigt werden.
  
#### Ablagemappe
  
Dieser Dienst ermöglicht es, mithilfe der Ablagemappe Datenseiten zu erstellen und freizugeben, die auf Remotecomputern angezeigt werden können. Dieser Dienst ist benötigt zur Erstellung der tatsächlichen Dateifreigaben, mit denen von anderen Computern eine Verbindung hergestellt werden kann, den NetDDE-Dienst (Network Dynamic Data Exchange). Mit der Anwendung **Ablagemappe** und dem gleichnamigen Dienst können Sie die freizugebenden Datenseiten erstellen. Alle Dienste, die explizit von diesem Dienst abhängig sind, können nicht ausgeführt werden. Sie können mit Clipbrd.exe aber die lokale Zwischenablage anzeigen. Dort werden Daten gespeichert, wenn ein Benutzer Text auswählt und anschließend im Menü **Bearbeiten** auf **Kopie** klickt oder STRG+C drückt.
  
Der Dienst **Ablagemappe** ist auf **Deaktiviert** gesetzt, um für die beiden in diesem Kapitel behandelten Umgebungen größere Sicherheit zu gewährleisten.
  
#### Computerbrowser
  
Dieser Dienst verwaltet eine aktuelle Liste der Computer im Netzwerk und stellt diese Liste Programmen zur Verfügung, die diese Liste anfordern. Auf Windows basierende Computer verwenden diesen Dienst, um Netzwerkdomänen und -ressourcen anzuzeigen.
  
Zur Erhöhung der Sicherheit ist der Dienst **Computerbrowser** für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### Fax
  
Bei diesem Dienst handelt es sich um einen mit der Telefonie-API (TAPI) kompatiblen Dienst, der den Clients in der Umgebung Faxfunktionen zur Verfügung stellt. Dieser Dienst ermöglicht es Benutzern, Faxnachrichten von einer Desktopanwendung aus zu senden und zu empfangen, entweder über einem lokales Faxgerät oder über ein gemeinsam genutztes Faxgerät im Netzwerk.
  
Der Dienst **Fax** ist für die Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung hingegen ist dieser Dienst zur Erhöhung der Sicherheit auf **Deaktiviert** gesetzt.
  
#### FTP-Publishing
  
Dieser Dienst ermöglicht die Verbindung und Verwaltung über das MMC-Snap-In „IIS“. Microsoft empfiehlt, diesen Dienst nicht auf Windows XP-Clients in Ihrer Umgebung zu installieren, sofern nicht entsprechende geschäftliche Anforderungen bestehen.
  
Der Dienst **FTP-Publishing** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### IIS-Verwaltung
  
Dieser Dienst ermöglicht die Verwaltung von IIS-Komponenten wie FTP, Anwendungspools, Websites und Webdiensterweiterungen. Deaktivieren Sie diesen Dienst, um zu verhindern, dass Benutzer auf ihren Computern Websites oder FTP-Sites ausführen, die auf den meisten Windows XP-Clientcomputern nicht erforderlich sind.
  
Der Dienst **IIS-Verwaltung** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Indexdienst
  
Dieser Dienst indiziert Inhalt und Eigenschaften von Dateien auf lokalen Computern und Remotecomputern und ermöglicht über eine flexible Abfragesprache den schnellen Zugriff auf die Dateien. Der Dienst ermöglicht auch die schnelle Suche nach Dokumenten auf lokalen Computern und Remotecomputern und bietet einen Suchindex für freigegebenen Inhalt im Internet.
  
Der **Indexdienst** ist für die Computer in der Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt. In der Hochsicherheitsumgebung hingegen ist dieser Dienst zur Erhöhung der Sicherheit auf **Deaktiviert** gesetzt.
  
#### Messenger
  
Mit diesem Dienst werden zwischen Clients und Servern Meldungen des **Warndienstes** übertragen und gesendet. Dieser Dienst steht in keiner Beziehung zu Windows Messenger oder MSN Messenger und ist auf Windows XP-Clientcomputern nicht erforderlich.
  
Aus diesem Grund ist der Dienst **Messenger** für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### NetMeeting-Remotedesktop-Freigabe
  
Mit diesem Dienst können autorisierte Benutzer auf einen Remoteclient zugreifen, indem Sie Microsoft NetMeeting im Intranet einer Organisation einsetzen. Dieser Dienst muss in NetMeeting ausdrücklich aktiviert werden. Sie können diesen Dienst auch in NetMeeting deaktivieren, mithilfe eines Symbols in der Windows-Taskleiste herunterfahren oder in der Gruppenrichtlinie deaktivieren, indem Sie die Einstellung **Remotedesktop-Freigabe deaktivieren** konfigurieren, die in Kapitel 4, „Administrative Vorlagen für Windows XP“, beschrieben wird. Microsoft empfiehlt, diesen Dienst zu deaktivieren, um zu verhindern, dass von Remotestandorten aus auf Ihre Clients zugegriffen wird.
  
Der Dienst **NetMeeting-Remotedesktop-Freigabe** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Sitzungs-Manager für Remotedesktophilfe
  
Dieser Dienst verwaltet und steuert die Remoteunterstützungsfunktion in der Hilfe- und Supportcenter-Anwendung (helpctr.exe).
  
Der Dienst **Sitzungs-Manager für Remotedesktophilfe** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### Routing und RAS
  
Dieser Dienst ermöglicht Multiprotokoll-LAN-zu-LAN, LAN-zu-WAN, VPN- und NAT-Routingdienste. Zusätzlich ermöglicht dieser Dienst DFÜ-Dienste und VPN-RAS-Dienste.
  
Der Dienst **Routing und RAS** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### SNMP-Dienst
  
Dieser Dienst ermöglicht die Bearbeitung von eingehenden SNMP-Anforderungen durch den lokalen Computer. Der **SNMP-Dienst** enthält Agenten, die die Aktivität im Netzwerk überwachen und Berichte an die Netzwerkkonsolen-Arbeitsstation senden.
  
Der **SNMP-Dienst** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### SNMP-Trap-Dienst
  
Dieser Dienst empfängt Trap-Nachrichten, die von lokalen oder Remote-SNMP-Agenten erzeugt wurden, und leitet die Nachrichten an SNMP-Verwaltungsprogramme auf Ihrem Computer weiter. Sofern der **SNMP-Dienst** für einen Agenten konfiguriert ist, werden Trap-Nachrichten erzeugt, wenn ein bestimmtes Ereignis eintritt. Diese Nachrichten werden an ein Trapziel gesendet.
  
Der **SNMP-Trap-Dienst** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### SSDP-Suchdienst
  
Dieser Dienst bietet dem UPnP-Host die Möglichkeit, UPnP-Netzwerkgeräte zu suchen und zu identifizieren. Wenn Sie den **SSDP-Suchdienst** deaktivieren, kann das System keine UPnP-Geräte im Netzwerk finden, und der UPnP-Host kann UPnP-Geräte nicht finden und nicht mit ihnen interagieren.
  
Der **SSDP-Suchdienst** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Taskplaner
  
Dieser Dienst ermöglicht Ihnen das Konfigurieren und Planen automatisierter Tasks auf Ihrem Computer. Der Dienst überwacht die von Ihnen ausgewählten Kriterien und führt die Tasks aus, wenn die Kriterien erfüllt werden.
  
Der Dienst **Taskplaner** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### Telnet
  
Dieser Dienst für Windows ermöglicht ASCII-Terminalsitzungen auf Telnet-Clients. Der Dienst unterstützt zwei Arten von Authentifizierung und die folgenden vier Terminaltypen: ANSI, VT-100, VT-52 und VTNT. Für die meisten Windows XP-Clients ist dieser Dienst jedoch nicht erforderlich.
  
Der Dienst **Telnet** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
#### Terminaldienste
  
Dieser Dienst bietet eine Multisessionumgebung, die Clientgeräten den Zugriff auf eine virtuelle Windows-Desktopsitzung und auf Windows-basierte Programme, die auf dem Server ausgeführt werden, ermöglichen. In Windows XP ermöglicht dieser Dienst Remotebenutzern, interaktiv mit einem Computer verbunden zu sein und Desktops und Anwendungen auf Remotecomputern anzuzeigen.
  
Der Dienst **Terminaldienste** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### Host für universelles Plug & Play
  
Dieser Dienst unterstützt Peer-to-Peer-Plug & Play für Netzwerkgeräte. Mit der UPnP-Spezifikation wird die Installation und Verwaltung von Geräten und Netzwerkdiensten vereinfacht. UPnP kann mithilfe treiberloser, standardgestützter Protokollierungsmechanismen Geräte und Dienste erkennen und steuern. Universelle Plug & Play-Geräte können die Netzwerkadressierung automatisch konfigurieren, ihre Anwesenheit in einem Subnetz ankündigen und den Austausch von Geräte- und Dienstbeschreibungen aktivieren. Ein Windows XP-Computer kann als UPnP-Steuerungspunkt dienen, um die Geräte durch eine Internet- oder Anwendungsschnittstelle zu steuern.
  
Der Dienst **Universelles Plug & Play** ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### WWW-Publishing
  
Dieser Dienst bietet Webverbindungs- und Verwaltungsfunktionen über das MMC-Snap-In „IIS“. Er ermöglicht HTTP-Dienste für Anwendungen auf der Windows-Plattform und beinhaltet einen Prozess- und einen Konfigurations-Manager. Für die meisten Windows XP-Clients ist dieser Dienst jedoch nicht erforderlich.
  
Der Dienst **WWW-Publishing** ist für die beiden in diesem Kapitel behandelten Umgebungen auf **Deaktiviert** gesetzt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusätzliche Registrierungseinstellungen
  
Für die Baseline-Sicherheitsvorlagendateien wurden zusätzliche Registrierungswerteinträge erstellt, die für die beiden in diesem Kapitel behandelten Umgebungen nicht in der Verwaltungsvorlagendatei (.adm) definiert sind.
  
Diese Einstellungen sind in die Sicherheitsvorlagen (im Abschnitt „Sicherheitsoptionen“) eingebettet, um ihre Implementierung zu automatisieren. Wenn die Richtlinie entfernt wird, werden die Einstellungen nicht automatisch entfernt. Sie müssen manuell mit einem Programm zum Bearbeiten der Registrierung (z. B. Regedt32.exe) geändert werden.
  
Dieses Handbuch enthält zusätzliche Einstellungen, die dem Sicherheitskonfigurations-Editor (SCE) durch Ändern der Datei sceregvl.inf im Ordner **%windir%\\inf** und erneutes Registrieren der Datei scecli.dll hinzugefügt werden. Die ursprünglichen und die zusätzlichen Sicherheitseinstellungen sind in den weiter oben in diesem Kapitel genannten Snap-Ins und Tools unter **Lokale Richtlinien\\Sicherheit** aufgeführt. Auf allen Computern, die eine Bearbeitung der in diesem Handbuch beschriebenen Sicherheitsvorlagen und Gruppenrichtlinien erfordern, sollte die Datei Sceregvl.inf aktualisiert und die Datei Scecli.dll erneut registriert werden, so wie im folgenden Unterabschnitt „Ändern der Benutzeroberfläche des Sicherheitskonfigurations-Editors“ beschrieben.
  
In der folgenden Tabelle sind die zusätzlichen empfohlenen Registrierungseinstellungen sowohl für Desktop- als auch für Laptopclients in den beiden Arten von Umgebungen zusammengefasst, die in diesem Kapitel behandelt werden: die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung.
  
Weitere Informationen zu jeder Einstellung finden Sie in den Unterabschnitten im Anschluss an die Tabelle. Weitere Informationen zu den Standardeinstellungen und eine ausführliche Erläuterung zu jeder Einstellung finden Sie im Begleithandbuch, [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx verfügbar ist.
  
**Tabelle 3.21: Zusätzliche Registrierungseinstellungen**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
<col width="20%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Einstellungsname</p></th>  
<th><p>Unternehmensclient-<br />  
Desktop</p></th>  
<th><p>Unternehmensclient-<br />  
Laptop</p></th>  
<th><p>Hochsicher-<br />  
Desktop</p></th>  
<th><p>Hochsicher-<br />  
Laptop</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (AutoAdminLogon) Automatische Anmeldung aktivieren (nicht empfohlen)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (DisableIPSourceRouting) Schutzebene für IP-Quellrouting (Schutz vor Paket-Spoofing)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Höchste Schutzebene, Quellrouting vollständig deaktiviert</p></td>
<td style="border:1px solid black;"><p>Höchste Schutzebene, Quellrouting vollständig deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (EnableDeadGWDetect) Automatische Erkennung von inaktiven Netzwerkgateways zulassen (DoS-Angriff möglich)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (EnableICMPRedirect) Überschreiben von OSPF-generierten Routen durch ICMP-Umleitungen zulassen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
<td style="border:1px solid black;"><p>Deaktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (Hidden) Computer aus der Suchliste ausblenden (nicht empfohlen mit Ausnahme von Hochsicherheitsumgebungen)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (KeepAliveTime) Sendehäufigkeit der Keep Alive-Pakete in Millisekunden</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>30.000 oder 5 Minuten (empfohlen)</p></td>
<td style="border:1px solid black;"><p>30.000 oder 5 Minuten (empfohlen)</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (NoDefaultExempt) NoDefaultExempt für IPSec-Filterung aktivieren (empfohlen)</p></td>
<td style="border:1px solid black;"><p>Multicast, Broadcast und ISAKMP sind ausgenommen (am besten für Windows XP)</p></td>
<td style="border:1px solid black;"><p>Multicast, Broadcast und ISAKMP sind ausgenommen (am besten für Windows XP)</p></td>
<td style="border:1px solid black;"><p>Multicast, Broadcast und ISAKMP sind ausgenommen (am besten für Windows XP)</p></td>
<td style="border:1px solid black;"><p>Multicast, Broadcast und ISAKMP sind ausgenommen (am besten für Windows XP)</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (NoDriveTypeAutoRun) Autorun für alle Laufwerke deaktivieren (empfohlen)</p></td>
<td style="border:1px solid black;"><p>255, Autorun für alle Laufwerke deaktivieren</p></td>
<td style="border:1px solid black;"><p>255, Autorun für alle Laufwerke deaktivieren</p></td>
<td style="border:1px solid black;"><p>255, Autorun für alle Laufwerke deaktivieren</p></td>
<td style="border:1px solid black;"><p>255, Autorun für alle Laufwerke deaktivieren</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (NoNameReleaseOnDemand) NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (NtfsDisable8dot3NameCreation) Erstellen der Dateinamen im 8.3-Format deaktivieren (empfohlen)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (PerformRouterDiscovery) Erkennung und Konfiguration von Standardgatewayadressen über IRDP zulassen (DoS-Angriff möglich)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (SafeDllSearchMode) Sicheren DLL-Suchmodus aktivieren (empfohlen)</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
<td style="border:1px solid black;"><p>Aktiviert</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (ScreenSaverGracePeriod) Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner (empfohlen: 0)</p></td>
<td style="border:1px solid black;"><p>0</p></td>
<td style="border:1px solid black;"><p>0</p></td>
<td style="border:1px solid black;"><p>0</p></td>
<td style="border:1px solid black;"><p>0</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (SynAttackProtect) Syn-Angriffschutzebene (Schutz vor DoS-Angriffen)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Bei Feststellen eines Angriffs Verbindung schneller trennen</p></td>
<td style="border:1px solid black;"><p>Bei Feststellen eines Angriffs Verbindung schneller trennen</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (TCPMaxConnectResponseRetransmissions) SYN-ACK-Neuübertragungen bei Nichtbestätigung einer Verbindungsanforderung</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>3 und 6 Sekunden, halb offene Verbindungen nach 21 Sekunden beendet</p></td>
<td style="border:1px solid black;"><p>3 und 6 Sekunden, halb offene Verbindungen nach 21 Sekunden beendet</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>MSS: (TCPMaxDataRetransmissions) Erneutes Senden von nicht bestätigten Daten (empfohlen: 3, Standardwert: 5)</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>3</p></td>
<td style="border:1px solid black;"><p>3</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>MSS: (WarningLevel) Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>Nicht definiert</p></td>
<td style="border:1px solid black;"><p>90</p></td>
<td style="border:1px solid black;"><p>90</p></td>
</tr>  
</tbody>  
</table>
  
#### (AutoAdminLogon) Automatische Anmeldung aktivieren
  
Der Registrierungswert **AutoAdminLogon** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\Windows NT\\CurrentVersion\\Winlogon\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (AutoAdminLogon) Automatische Anmeldung aktivieren (nicht empfohlen)** angezeigt.
  
Diese Einstellung ist vom **Begrüßungsbildschirm** in Windows XP getrennt. Wenn dieser deaktiviert ist, ist diese Einstellung nicht deaktiviert. Wenn Sie einen Computer für die automatische Anmeldung konfigurieren, kann jeder, der physischen Zugriff auf den Computer erlangen kann, außerdem Zugriff auf alle auf dem Computer befindlichen Daten erhalten. Dazu gehören auch alle Netzwerke, mit denen der Computer verbunden ist. Wenn Sie die automatische Anmeldung aktivieren, wird das Kennwort in Klartext in der Registrierung gespeichert. Der Registrierungsschlüssel, in dem dieser Wert gespeichert wird, kann von der Gruppe **Authentifizierte Benutzer** von einem Remotestandort aus gelesen werden. Aus diesen Gründen ist die Einstellung für die Unternehmensclient-Umgebung auf **Nicht definiert** gesetzt, und die standardmäßige Einstellung **Deaktiviert** wird in der Hochsicherheitsumgebung ausdrücklich erzwungen.
  
Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Aktivieren der automatischen Anmeldung in Windows XP](http://support.microsoft.com/default.aspx?scid=315231)“, der online unter http://support.microsoft.com/default.aspx?scid=315231 verfügbar ist.
  
#### (DisableIPSourceRouting) Schutzebene für IP-Quellrouting
  
Der Registrierungswert **DisableIPSourceRouting** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (DisableIPSourceRouting) Schutzebene für IP-Quellrouting (Schutz vor Paket-Spoofing)** angezeigt.
  
Über das IP-Quellrouting kann ein Sender die IP-Route eines Datagramms im Netzwerk festlegen. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Höchste Schutzebene, Quellrouting vollständig deaktiviert** gesetzt.
  
#### (EnableDeadGWDetect) Automatische Erkennung von inaktiven Netzwerkgateways zulassen
  
Der Registrierungswert **EnableDeadGWDetect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (EnableDeadGWDetect) Automatische Erkennung von inaktiven Netzwerkgateways zulassen (DoS-Angriff möglich)** angezeigt.
  
Wenn die Funktion „Dead Gateway Detection“ aktiviert ist, kann das IP-Protokoll zu einem Sicherungsgateway wechseln, wenn bei mehreren Verbindungen Fehler auftreten. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### (EnableICMPRedirect) Überschreiben von OSPF-generierten Routen durch ICMP-Umleitungen zulassen
  
Der Registrierungswert **EnableICMPRedirect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (EnableICMPRedirect) Überschreiben von OSPF-generierten Routen durch ICMP-Umleitungen zulassen** angezeigt.
  
ICMP-Umleitungen (Internet Control Message Protocol) führen dazu, dass Hostrouten über den Stapel verbunden werden. Diese Routen setzen die über OSPF (Open Shortest Path First) erstellten Routen außer Kraft. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### (Hidden) Computer aus der Netzwerkumgebungs-Suchliste ausblenden
  
Der Registrierungswert **Hidden** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Lanmanserver\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (Hidden) Computer aus der Suchliste ausblenden (nicht empfohlen mit Ausnahme von Hochsicherheitsumgebungen)** angezeigt.
  
Sie können einen Computer so konfigurieren, dass er den Browsern in der Domäne keine Ankündigungen sendet. Wenn Sie dies tun, blenden Sie den Computer aus der Suchliste aus. Das bedeutet, dass der Computer seine Anwesenheit vor anderen Computern im gleichen Netzwerk verbirgt. Ein Angreifer, der den Namen eines Computers kennt, kann viel leichter zusätzliche Informationen zum System sammeln. Sie können diese Einstellung aktivieren, um eine Methode zu entfernen, mit der ein Angreifer Informationen über Computer im Netzwerk sammeln könnte. Außerdem kann die Aktivierung dieser Einstellung zur Verringerung des Netzwerkverkehrs beitragen. Die Sicherheitsvorteile dieser Einstellung sind jedoch gering, da Angreifer alternative Methoden verwenden können, um potenzielle Ziele zu identifizieren und zu finden. Aus diesem Grund empfiehlt Microsoft, diese Einstellung nur in Hochsicherheitsumgebungen zu aktivieren.
  
Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Verbergen eines Windows 2000-basierten Computers in einer Browserliste (engl.)](http://support.microsoft.com/kb/321710/en-us)“, der online unter http://support.microsoft.com/kb/321710/en-us verfügbar ist.
  
#### (KeepAliveTime) Sendehäufigkeit der Keep Alive-Pakete in Millisekunden
  
Der Registrierungswert **KeepAliveTime** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (KeepAliveTime) Sendehäufigkeit der Keep Alive-Pakete in Millisekunden (empfohlen: 300.000)** angezeigt.
  
Mit diesem Wert wird die Anzahl der TCP-Versuche festgelegt, bei denen durch Senden von Keep Alive-Paketen überprüft wird, ob eine Leerlaufverbindung immer noch hergestellt ist. Wenn die Verbindung mit dem Remotecomputer noch besteht, bestätigt dieser die Keep Alive-Pakete. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **30.000 oder 5 Minuten** gesetzt.
  
#### (NoDefaultExempt) NoDefaultExempt für IPSec-Filterung aktivieren
  
Der Registrierungswert **NoDefaultExempt** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\IPSEC\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoDefaultExempt) NoDefaultExempt für IPSec-Filterung aktivieren (empfohlen)** angezeigt.
  
Die Standardausnahmen für die IPSec-Richtlinienfilter sind in der Onlinehilfe zu Microsoft Windows 2000 und Windows XP dokumentiert. Diese Filter ermöglichen die Funktion des gegenseitigen Schlüsselaustausches (Internet Key Exchange, IKE) und des Kerberos-Authentifizierungsprotokolls. Mit den Filtern kann das Netzwerk-QoS (Quality of Service) ausgegeben werden (RSVP), und zwar sowohl wenn der Datenverkehr durch IPSec gesichert wird als auch wenn dies nicht der Fall ist (z. B. bei Multicast- und Broadcastverkehr).
  
IPSec wird zunehmend für die grundlegende Hostfirewall-Paketfilterung verwendet, insbesondere in Szenarien mit einer Gefährdung durch Internetverbindungen. Die Auswirkungen dieser Standardausnahmen werden jedoch nicht immer richtig verstanden. Einige IPSec-Administratoren erstellen u. U. vermeintlich sichere IPSec-Richtlinien, die jedoch nicht vor eingehenden Angriffen schützen, bei denen die Standardausnahmen verwendet werden. Microsoft empfiehlt, für die beiden in diesem Kapitel behandelten Umgebungen die Standardeinstellung in Windows XP mit SP 2, **Multicast, Broadcast und ISAKMP sind ausgenommen**, zu verwenden.
  
Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[IPSec-Standardausnahmen können in einigen Szenarios zum Überwinden des IPSec-Schutzes verwendet werden](http://support.microsoft.com/default.aspx?scid=811832)“ (in englischer Sprache), der online unter http://support.microsoft.com/default.aspx?scid=811832 verfügbar ist.
  
#### (NoDriveTypeAutoRun) Autorun für alle Laufwerke deaktivieren
  
Der Registrierungswert **NoDriveTypeAutoRun** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\**  
**Policies\\Explorer\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoDriveTypeAutoRun) Autorun für alle Laufwerke deaktivieren (empfohlen)** angezeigt.
  
Bei Aktivierung von Autorun werden Daten unmittelbar nach dem Einlegen von Medien in ein Laufwerk gelesen. Daher werden die Setupdatei von Programmen und die Wiedergabe von Audiomedien sofort gestartet. Diese Einstellung ist für die beiden in diesem Kapitel behandelten Umgebungen auf **255, Autorun für alle Laufwerke deaktivieren** gesetzt.
  
#### (NoNameReleaseOnDemand) NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen
  
Der Registrierungswert **NoNameReleaseOnDemand** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Netbt\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NoNameReleaseOnDemand) NetBIOS-Namensfreigabeanforderungen nur von WINS-Servern zulassen** angezeigt.
  
„NetBIOS über TCP/IP“ ist ein Netzwerkprotokoll, das u. a. eine Möglichkeit zur einfachen Auflösung der in Windows-basierten Systemen registrierten NetBIOS-Namen in auf diesen Systemen konfigurierte IP-Adressen bereitstellt. Durch diese Einstellung wird festgelegt, ob der NetBIOS-Name des Computers beim Empfang einer Namensfreigabeanforderung freigegeben wird. Der Wert ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Aktiviert** gesetzt.
  
#### (NtfsDisable8dot3NameCreation) Erstellen der Dateinamen im 8.3-Format deaktivieren
  
Der Registrierungswert **NtfsDisable8dot3NameCreation** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Control\\FileSystem\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (NtfsDisable8dot3NameCreation) Erstellen der Dateinamen im 8.3-Format deaktivieren (empfohlen)** angezeigt.
  
Windows Server 2003 unterstützt 8.3-Dateinamensformate zur Gewährleistung der Abwärtskompatibilität mit 16-Bit-Anwendungen. Die 8.3-Dateinamenkonvention ist ein Namensformat, das Dateinamen von bis zu acht Zeichen zulässt. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### (PerformRouterDiscovery) Erkennung und Konfiguration von Standardgatewayadressen über IRDP zulassen
  
Der Registrierungswert **PerformRouterDiscovery** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (PerformRouterDiscovery) Erkennung und Konfiguration von Standardgatewayadressen über IRDP zulassen (DoS-Angriff möglich)** angezeigt.
  
Über diese Einstellung wird IRDP (Internet Router Discovery Protocol) aktiviert oder deaktiviert. Dies ermöglicht dem System, wie in RFC 1256 beschrieben Standardgatewayadressen automatisch pro Schnittstelle zu erkennen und zu konfigurieren. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Deaktiviert** gesetzt.
  
#### (SafeDllSearchMode) Sicheren DLL-Suchmodus aktivieren
  
Der Registrierungswert **SafeDllSearchMode** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\ SYSTEM\\CurrentControlSet\\Control\\Session Manager\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (SafeDllSearchMode) Sicheren DLL-Suchmodus aktivieren (empfohlen)** angezeigt.
  
Zum Konfigurieren der DLL-Suchreihenfolge für die Suche nach DLLs, die von laufenden Prozessen angefordert werden, stehen zwei Methoden zur Auswahl:
  
-   Zuerst die im Systempfad angegebenen Ordner durchsuchen und dann den aktuellen Arbeitsordner durchsuchen
  
-   Zuerst den aktuellen Arbeitsordner durchsuchen und dann die im Systempfad angegebenen Ordner durchsuchen
  
Bei Aktivierung wird der Registrierungswert auf **1** gesetzt. Bei einer Einstellung von **1** werden zuerst die im Systempfad angegebenen Ordner und anschließend der aktuelle Arbeitsordner durchsucht. Bei Deaktivierung wird der Registrierungswert auf **0** gesetzt. Bei dieser Einstellung werden zuerst der aktuelle Arbeitsordner und anschließend die im Systempfad angegebenen Ordner durchsucht. Diese Einstellung ist für beiden in diesem Kapitel behandelten Umgebungen auf **Aktiviert** gesetzt.
  
#### (ScreenSaverGracePeriod) Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner
  
Der Registrierungswert **ScreenSaverGracePeriod** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\SYSTEM\\Software\\Microsoft\\Windows NT\\CurrentVersion\\**  
**Winlogon\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (ScreenSaverGracePeriod) Zeitangabe in Sekunden vor Ablauf des Kulanzzeitraums für den Bildschirmschoner (empfohlen: 0)** angezeigt.
  
Windows enthält einen Kulanzzeitraum zwischen dem Start des Bildschirmschoners und der tatsächlichen automatischen Sperrung der Konsole, wenn die Bildschirmschonersperre aktiviert wird. Diese Einstellung ist für die beiden in diesem Kapitel behandelten Umgebungen auf **0 **Sekunden gesetzt.
  
#### (SynAttackProtect) Syn-Angriffschutzebene
  
Der Registrierungswert **SynAttackProtect** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (SynAttackProtect) Syn-Angriffschutzebene (Schutz vor DoS-Angriffen)** angezeigt.
  
Diese Einstellung zwingt das TCP-Protokoll zur Anpassung der Umleitung von SYN-ACKs. Wenn Sie diesen Wert konfigurieren, wird die Verbindungsantwort bei Feststellung eines Verbindungsanforderungsangriffs (SYN-Angriff) schneller beendet. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **Bei Feststellen eines Angriffs Verbindung schneller trennen** gesetzt.
  
#### (TCPMaxConnectResponseRetransmissions) SYN-ACK-Neuübertragungen bei Nichtbestätigung einer Verbindungsanforderung
  
Der Registrierungswert **TCPMaxConnectResponseRetransmissions** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (TCPMaxConnectResponseRetransmissions) SYN-ACK-Neuübertragungen bei Nichtbestätigung einer Verbindungsanforderung** angezeigt.
  
Durch diese Einstellung wird die Anzahl der erneuten Übertragungen von SYN-Paketen über TCP vor dem Abbruch der Verbindung festgelegt. Das Zeitlimit bis zur jeweils nächsten Neuübertragung wird mit jedem weiteren Verbindungsversuch verdoppelt. Der Standardwert beträgt 3 Sekunden. Diese Einstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **3 und 6 Sekunden, halb offene Verbindungen nach 21 Sekunden beendet** gesetzt.
  
#### (TCPMaxDataRetransmissions) Erneutes Senden von nicht bestätigten Daten
  
Der Registrierungswert **TCPMaxDataRetransmissions** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\System\\CurrentControlSet\\Services\\Tcpip\\Parameters\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (TCPMaxDataRetransmissions) Erneutes Senden von nicht bestätigten Daten (empfohlen: 3, Standardwert: 5)** angezeigt.
  
Mit diesem Eintrag wird die Anzahl der Versuche zur Übertragung einzelner Datensegmente vor einem Verbindungsabbruch festgelegt. Das Zeitlimit bis zur jeweils nächsten Neuübertragung wird mit jedem weiteren Verbindungsversuch verdoppelt. Der Wert für das Zeitlimit wird zurückgesetzt, nachdem die Verbindung hergestellt wurde. Der Standardwert für das Zeitlimit wird anhand der gemessenen RTT-Zeit der jeweiligen Verbindung ermittelt. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **3** gesetzt.
  
#### (WarningLevel) Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung
  
Der Registrierungswert **WarningLevel** wurde der Vorlagendatei im Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\ SYSTEM\\CurrentControlSet\\Services\\Eventlog\\Security\\** hinzugefügt. Der Eintrag wird im Sicherheitskonfigurations-Editor als **MSS: (WarningLevel) Schwellenwert in % für das Sicherheitsereignisprotokoll zur Erstellung einer Warnmeldung** angezeigt.
  
Diese Einstellung ist seit SP3 für Windows 2000 verfügbar. Durch diese neue Funktion wird im Sicherheitsereignisprotokoll ein Sicherheitsüberwachungseintrag erzeugt, wenn der vom Benutzer definierte Schwellwert des Sicherheitsprotokolls erreicht wird. Diese Richtlinieneinstellung ist für die Unternehmensclient-Umgebung auf **Nicht definiert** und für die Hochsicherheitsumgebung auf **90** gesetzt.
  
**Hinweis**: Wenn Protokolleinstellungen auf **Ereignisse bei Bedarf überschreiben** oder **Ereignisse überschreiben, die älter sind als x Tage** gesetzt sind, wird dieses Ereignis nicht erzeugt.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Ändern der Benutzeroberfläche des Sicherheitskonfigurations-Editors
  
Mit den SCE-Tools werden Sicherheitsvorlagen definiert, die auf einzelne Computer oder über eine Gruppenrichtlinie auf mehrere Computer angewendet werden können. Sicherheitsvorlagen können Kennwortrichtlinien, Sperrrichtlinien, Richtlinien für das Authentifizierungsprotokoll Kerberos, Überwachungsrichtlinien, Ereignisprotokolleinstellungen, Registrierungswerte, Startparameter für Dienste, Dienstberechtigungen, Benutzerrechte, Gruppenmitgliedschaftseinschränkungen, Registrierungsberechtigungen und Dateisystemberechtigungen enthalten. Der Sicherheitskonfigurations-Editor wird in zahlreichen MMC-Snap-Ins und Verwaltungstools angezeigt. Er wird im Snap-In „Sicherheitsvorlagen“ und im Snap-In „Sicherheitskonfiguration und -analyse“ verwendet. Im Snap-In „Gruppenrichtlinien-Editor“ wird der Sicherheitskonfigurations-Editor im Bereich Sicherheitseinstellungen der Struktur „Computerkonfiguration“ eingesetzt. Darüber hinaus wird er bei den lokalen Sicherheitseinstellungen, der Sicherheitsrichtlinie für Domänencontroller sowie der Sicherheitsrichtlinie für Domänen verwendet.
  
Dieses Handbuch enthält zusätzliche Einstellungen, die dem Sicherheitskonfigurations-Editor hinzugefügt wurden. Zum Hinzufügen dieser Einstellungen müssen Sie die Datei Sceregvl.inf verändern, die sich im Ordner **%systemroot%\\inf** Ordner befindet, und anschließend die Datei Scecli.dll neu registrieren.
  
**Wichtig**: Die benutzerdefinierte Version der Datei Sceregvl.inf, die mithilfe der folgenden Prozeduren erstellt wird, verwendet Funktionen, die nur unter Windows XP Professional mit SP 2 und Windows Server 2003 verfügbar sind. Versuchen Sie nicht, die benutzerdefinierte Datei unter älteren Windows-Versionen zu installieren.
  
Nachdem die Datei Sceregvl.inf geändert und registriert wurde, werden die geänderten Registrierungswerte in der Benutzeroberfläche des Sicherheitskonfigurations-Editors auf dem entsprechenden Computer angezeigt. Die neuen Einstellungen werden im Sicherheitskonfigurations-Editor am Ende der Liste mit den Einträgen angezeigt und beginnen alle mit „MSS:“. „MSS“ steht für „Microsoft Solutions for Security“ (Microsoft Sicherheitslösungen) und ist die Bezeichnung der Arbeitsgruppe, die dieses Handbuch herausgibt. Anschließend können Sie Sicherheitsvorlagen oder Richtlinien erstellen, die diese neuen Registrierungswerte definieren und die auf jeden Computer angewendet werden können, ungeachtet dessen, ob die Datei Sceregvl.inf auf dem Zielcomputer verändert wurde. Bei jedem weiteren Start des Sicherheitskonfigurations-Editors werden die folgenden benutzerdefinierten Registrierungswerte angezeigt.
  
Eine Reihe der neuen Einstellungen, die im Sicherheitskonfigurations-Editor angezeigt werden, sind nicht in diesem Handbuch dokumentiert, da sie für Endbenutzersysteme normalerweise nicht konfiguriert werden. Weitere Informationen zu diesen neuen Einstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx heruntergeladen werden kann.
  
Mithilfe der im Folgenden beschriebenen Verfahren kann die Benutzeroberfläche des Sicherheitskonfigurations-Editors angepasst werden. Befolgen Sie die Anweisungen für die manuelle Durchführung, wenn Sie bereits andere Anpassungen im Sicherheitskonfigurations-Editor vorgenommen haben. Die Einstellungen können mithilfe eines bereitgestellten Skripts mit geringem Benutzereingriff hinzugefügt werden. Obwohl das Skript über integrierte Funktionen zur Fehlerermittlung und Wiederherstellung verfügt, kann ein Fehlschlagen des Skripts nicht ausgeschlossen werden. Wenn das Skript nicht ausgeführt werden kann, sollten Sie die Fehlerursache ermitteln und entweder das Problem beheben oder die Anweisungen für die manuelle Durchführung befolgen. Mit einem anderen bereitgestellten Skript können Sie die Benutzeroberfläche des Sicherheitskonfigurations-Editors wieder auf die Standardwerte zurücksetzen. Durch dieses Skript werden alle benutzerdefinierten Einstellungen entfernt, und der Sicherheitskonfigurations-Editor wird wieder so wie bei einer Standardinstallation von Windows XP mit SP2 oder Windows Server 2003 mit SP1 konfiguriert.
  
**So aktualisieren Sie die Datei sceregvl.inf manuell**
  
1.  Verwenden Sie einen Texteditor (z. B. Notepad), um die Datei **Values-sceregvl.txt** im Downloadordner **SCE Update** dieses Handbuchs zu öffnen.
  
2.  Öffnen Sie ein weiteres Fenster im Texteditor, und öffnen Sie anschließend die Datei **%systemroot%\\inf\\sceregvl.inf**.
  
3.  Gehen Sie in der Datei **sceregvl.inf** zum Ende des Abschnitts „\[Register Registry Values\]“. Kopieren Sie den Text ohne Seitenumbrüche aus der Datei **Values-sceregvl.txt**, und fügen Sie ihn in diesen Abschnitt der Datei **sceregvl.inf** ein.
  
4.  Schließen Sie die Datei **Values-sceregvl.txt**, und öffnen Sie die Datei **Strings-sceregvl.txt** im Downloadordner **SCE Update**.
  
5.  Gehen Sie in der Datei **sceregvl.inf** zum Ende des Abschnitts „\[Strings\]“. Kopieren Sie den Text ohne Seitenumbrüche aus der Datei **Strings-sceregvl.txt**, und fügen Sie ihn in diesen Abschnitt der Datei **sceregvl.inf** ein.
  
6.  Speichern Sie die Datei **sceregvl.inf**, und schließen Sie den Texteditor.
  
7.  Öffnen Sie eine Eingabeaufforderung, und führen Sie zum erneuten Registrieren der DLL-Datei den Befehl **regsvr32 scecli.dll** aus.
  
Bei jedem weiteren Start des Sicherheitskonfigurations-Editors werden die folgenden benutzerdefinierten Registrierungswerte angezeigt.
  
**So aktualisieren Sie die Datei sceregvl.inf automatisch**
  
1.  Die im Downloadordner **SCE Update** dieses Handbuchs befindlichen Dateien **Values-sceregvl.txt**, **Strings-sceregvl.txt** und **Update\_SCE\_with\_MSS\_Regkeys.vbs** müssen alle im selben Verzeichnis gespeichert sein, damit das Skript ausgeführt werden kann.
  
2.  Führen Sie das Skript **Update\_SCE\_with\_MSS\_Regkeys.vbs** auf dem Computer aus, der aktualisiert werden soll.
  
3.  Befolgen Sie die Anweisungen auf dem Bildschirm.
  
Durch diese Vorgehensweise werden nur die benutzerdefinierten Einträge entfernt, die mit dem Skript **Update\_sce\_with\_mss\_regkeys.vbs** vorgenommen wurden, das im vorherigen Verfahren beschrieben wurde.
  
**So machen Sie die Änderungen des Skripts Update\_SCE\_with\_MSS\_Regkeys.vbs rückgängig**
  
1.  Führen Sie das Skript **Rollback\_SCE\_for\_MSS\_Regkeys.vbs** auf dem Computer aus, der aktualisiert werden soll.
  
2.  Befolgen Sie die Anweisungen auf dem Bildschirm.
  
Durch dieses Verfahren werden *alle* benutzerdefinierten Einträge entfernt, die der Benutzeroberfläche des Sicherheitskonfigurations-Editors hinzugefügt wurden. Dazu zählen auch die Einträge aus diesem Handbuch und andere Einträge, die u. U. in Vorgängerversionen dieses Handbuchs oder in anderen Sicherheitshandbüchern beschrieben wurden.
  
**So stellen Sie den Standardzustand des Sicherheitskonfigurations-Editors in Windows XP mit SP2 oder Windows Server 2003 mit SP1 wieder her**
  
1.  Die im Downloadordner **SCE Update** dieses Handbuchs befindlichen Dateien **sceregvl\_W2K3\_SP1.inf.txt**, **sceregvl\_XPSP2.inf.txt** und **Restore\_SCE\_to\_Default.vbs** müssen alle im selben Verzeichnis gespeichert sein, damit das Skript ausgeführt werden kann.
  
2.  Führen Sie das Skript **Restore\_SCE\_to\_Default.vbs** auf dem Computer aus, der aktualisiert werden soll.
  
3.  Befolgen Sie die Anweisungen auf dem Bildschirm.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusätzliche Sicherheitseinstellungen
  
Obwohl die meisten Gegenmaßnahmen zum Absichern der Clientsysteme in den beiden in diesem Kapitel behandelten Umgebungen mithilfe von Gruppenrichtlinien angewendet wurden, können einige Einstellungen nur schwer oder gar nicht mit Gruppenrichtlinien implementiert werden. Eine ausführliche Erläuterung der in diesem Abschnitt beschriebenen Gegenmaßnahmen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen unter Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx), das unter http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx verfügbar ist.
  
#### Manuelle Absicherungsverfahren
  
In diesem Abschnitt wird die manuelle Implementierung einiger zusätzlicher Gegenmaßnahmen zum Sichern der Windows XP Clients für jede der die in diesem Handbuch definierten Sicherheitsumgebungen beschrieben.
  
##### Dr. Watson deaktivieren: Automatische Ausführung des Dr. Watson-Systemdebuggers deaktivieren
  
Einige Organisationen sind möglicherweise der Meinung, dass Systemdebugger wie z. B. das in Windows enthaltene Tool „Dr. Watson“ von sachkundigen Angreifern ausgenutzt werden könnte. Anweisungen zum Deaktivieren des Systemdebuggers „Dr. Watson“ finden Sie im Microsoft Knowledge Base-Artikel „[Deaktivieren von Dr. Watson für Windows](http://support.microsoft.com/default.aspx?scid=188296)“, der online unter http://support.microsoft.com/default.aspx?scid=188296 verfügbar ist.
  
##### SSDP/UPnP deaktivieren: SSDP/UPnP deaktivieren
  
Einige Organisationen sind möglicherweise der Meinung, dass die universellen Plug & Play-Funktionen in den Unterkomponenten von Windows XP vollständig deaktiviert werden sollten. Obwohl der Dienst **Host für universelles Plug & Play** in diesem Handbuch deaktiviert ist, verwenden andere Anwendungen wie z. B. Windows Messenger den Prozess **SSDP-Suchdienst (Simple Service Discovery Protocol)**, um Netzwerkgateways oder andere Netzwerkgeräte zu identifizieren. Sie können sicherstellen, dass die in Windows XP enthaltenen SSDP- und UPnP-Funktionen nicht von Anwendungen verwendet werden. Fügen Sie dazu dem Registrierungsschlüssel **HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DirectPlayNATHelp\\DPNHUPnP\\** den REG\_DWORD-Registrierungswert **UPnPMode** hinzu, und setzen Sie seinen Wert auf **2**.
  
Weitere Informationen finden Sie im Microsoft Knowledge Base-Artikel „[Verkehr wird nach Abschalten des SSDP-Erkennungsdienstes und des Universal Plug & Play-Gerätehosts gesendet](http://support.microsoft.com/kb/317843/en-us)“ (in englischer Sprache), der online unter http://support.microsoft.com/kb/317843/en-us verfügbar ist.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Sichern des Dateisystems
  
Das NTFS-Dateisystem wurde mit jeder neuen Version von Microsoft Windows verbessert. Die Standardberechtigungen für NTFS sind für die meisten Organisationen geeignet. Die in diesem Abschnitt erörterten Einstellungen sind für Organisationen vorgesehen, die Laptops und Desktops in der in diesem Handbuch beschriebenen Hochsicherheitsumgebung verwenden.
  
Eine Änderung der Sicherheitseinstellungen für das Dateisystem ist mithilfe von Gruppenrichtlinien möglich. Die Dateisystemeinstellungen können im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Dateisystem**
  
**Hinweis**: Alle Änderungen an den vordefinierten Dateisystem-Sicherheitseinstellungen sollten in einer Testumgebung gründlich überprüft werden, bevor sie in einer großen Organisation implementiert werden. Es ist vorgekommen, dass Dateiberechtigungen derartig geändert wurden, dass die betroffenen Computer vollständig neu eingerichtet werden mussten.
  
Für die meisten Situationen sind die Standarddateiberechtigungen in Windows XP ausreichend. Wenn Sie die Mitgliedschaft der Gruppe **Hauptbenutzer** nicht durch die Funktion „Eingeschränkte Gruppen“ blockieren oder wenn Sie die Einstellung **Netzwerkzugriff: Die Verwendung von 'Jeder'-Berechtigungen für anonyme Benutzer ermöglichen** aktivieren, können Sie jedoch die im nächsten Absatz beschriebenen optionalen Berechtigungen verwenden. Diese optionalen Berechtigungen sind sehr spezifisch, und sie wenden zusätzliche Einschränkungen auf bestimmte ausführbare Tools an, mit denen ein unbefugter Benutzer mit erhöhten Berechtigungen das System oder das Netzwerk weiter gefährden kann.
  
Beachten Sie, dass diese Berechtigungsänderungen keine Auswirkungen auf mehrere Ordner oder das Stammverzeichnis des Systemlaufwerks haben. Berechtigungen auf diese Weise zu ändern, kann riskant sein und zu einer Instabilität des Systems führen. Alle Dateien befinden sich im Ordner **%SystemRoot%\\System32\\** und verfügen über die Berechtigungen **Administratoren: Vollzugriff**, und **System: Vollzugriff**.
  
-   regedit.exe
  
-   arp.exe
  
-   at.exe
  
-   attrib.exe
  
-   cacls.exe
  
-   debug.exe
  
-   edlin.exe
  
-   eventcreate.exe
  
-   eventtriggers.exe
  
-   ftp.exe
  
-   nbtstat.exe
  
-   net.exe
  
-   net1.exe
  
-   netsh.exe
  
-   netstat.exe
  
-   nslookup.exe
  
-   ntbackup.exe
  
-   rcp.exe
  
-   reg.exe
  
-   regedt32.exe
  
-   regini.exe
  
-   regsvr32.exe
  
-   rexec.exe
  
-   route.exe
  
-   rsh.exe
  
-   sc.exe
  
-   secedit.exe
  
-   subst.exe
  
-   systeminfo.exe
  
-   telnet.exe
  
-   tftp.exe
  
-   tlntsvr.exe
  
Diese optionalen Berechtigungen sind bereits in einer Sicherheitsvorlage mit dem Namen „Optional-File-Permissions.inf“ konfiguriert und können gemeinsam mit diesem Handbuch heruntergeladen werden.
  
#### Erweiterte Berechtigungen
  
Im Dialogfeld **Berechtigungen** können Sie Dateiberechtigungen mit mehr Steuerungsmöglichkeiten einrichten, als sie auf den ersten Blick zu bieten scheinen. Klicken Sie dazu auf die Schaltfläche **Erweitert**. In der folgenden Tabelle werden diese erweiterten Berechtigungen beschrieben.
  
**Tabelle 3.22: Erweiterte Dateiberechtigungen und Beschreibungen**

<p> </p>
<table style="border:1px solid black;">  
<colgroup>  
<col width="50%" />  
<col width="50%" />  
</colgroup>  
<thead>  
<tr class="header">  
<th><p>Name der erweiterter Berechtigung</p></th>  
<th><p>Beschreibung</p></th>  
</tr>  
</thead>  
<tbody>  
<tr class="odd">
<td style="border:1px solid black;"><p>Ordner durchsuchen / Datei ausführen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert, dass Benutzer Ordner passieren, um zu anderen Dateien oder Ordnern zu gelangen, selbst wenn der Benutzer keine Berechtigung für die passierten Ordner besitzt (gilt nur für Ordner).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Ordner auflisten / Daten lesen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Anzeigen der Namen von Dateien und Unterordnern im angegebenen Ordner. Dies betrifft nur die Inhalte des Ordners und hat keine Auswirkungen darauf, ob der Ordner, für den Sie die Berechtigung einstellen, aufgelistet wird (gilt nur für Ordner).</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Attribute lesen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Anzeigen der Attribute von Dateien und Ordnern.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Erweiterte Attribute lesen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Anzeigen der erweiterten Attribute von Dateien und Ordnern. Attribute werden durch NTFS definiert.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Dateien erstellen / Daten schreiben</p></td>
<td style="border:1px solid black;"><p>Die Berechtigung „Dateien erstellen“ ermöglicht oder verweigert das Erstellen von Dateien innerhalb des Ordners (gilt nur für Ordner). Die Berechtigung „Daten schreiben“ ermöglicht oder verweigert das Ändern von Dateien und das Überschreiben vorhandener Inhalte.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Ordner erstellen / Daten anhängen</p></td>
<td style="border:1px solid black;"><p>Die Berechtigung „Ordner erstellen“ ermöglicht oder verweigert das Erstellen von Ordnern innerhalb eines bestimmten Ordners (gilt nur für Ordner). Die Berechtigung „Daten anhängen“ ermöglicht oder verweigert das Vornehmen von Änderungen am Ende der Datei, aber nicht das Ändern, Löschen oder Überschreiben vorhandener Daten (gilt nur für Dateien).</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Attribute schreiben</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Ändern der Attribute von Dateien und Ordnern.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Erweiterte Attribute schreiben</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Ändern der erweiterten Attribute von Dateien und Ordnern. Attribute werden durch NTFS definiert.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Unterordner und Dateien löschen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Löschen untergeordneter Ordner und Dateien, selbst wenn die Berechtigung „Löschen“ nicht für den untergeordneten Ordner oder die Datei zugewiesen wurde (gilt für Ordner).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Löschen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Löschen von Ordnern und Dateien.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Berechtigungen lesen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Lesen der Berechtigungen für Dateien oder Ordner, wie z. B. „Vollzugriff“, „Lesen“ oder „Schreiben“.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Berechtigungen ändern</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert das Ändern der Berechtigungen für Dateien oder Ordnern, wie z. B. „Vollzugriff“, „Lesen“ oder „Schreiben“.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Besitz übernehmen</p></td>
<td style="border:1px solid black;"><p>Ermöglicht oder verweigert die Besitzübernahme in Bezug auf Dateien oder Ordner. Der Besitzer einer Datei oder eines Ordners kann die Berechtigungen für diese immer und unabhängig von vorhandenen Berechtigungen für die Datei oder den Ordner ändern.</p></td>
</tr>  
</tbody>  
</table>
  
Mit den folgenden drei zusätzlichen Begriffen wird die Vererbung der für Dateien und Ordner geltenden Berechtigungen beschrieben:
  
-   **Übertragen** bezeichnet das Übertragen vererbbarer Berechtigungen auf alle Unterordner und Dateien. Alle untergeordneten Objekte eines Objekts erhalten die Sicherheitseinstellungen des übergeordneten Objekts, vorausgesetzt, das untergeordnete Objekt ist nicht vor der Annahme vererbter Berechtigungen geschützt. Wenn ein Konflikt auftritt, gelten die expliziten Berechtigungen des untergeordneten Objekts vor den vom übergeordneten Objekt vererbten Berechtigungen.
  
-   **Ersetzen** bezeichnet das Ersetzen vorhandener Berechtigungen für alle Unterordner und Dateien durch vererbbare Berechtigungen. Die für das übergeordnete Objekt angegebenen Berechtigungen gelten vor allen Sicherheitseinstellungen des untergeordneten Objekts, unabhängig von dessen Einstellungen. Das untergeordnete Objekt verfügt über dieselben Zugriffsberechtigungen wie das übergeordnete Objekt.
  
-   **Ignorieren** bedeutet, dass Berechtigungen für eine Datei oder einen Ordner (oder Schlüssel) nicht ersetzt werden können. Verwenden Sie diese Konfigurationsoption, wenn Sie die Sicherheit für dieses oder eines der untergeordneten Objekte nicht konfigurieren oder analysieren möchten.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
Dieses Kapitel enthält eine detaillierte Beschreibung der primären Sicherheitseinstellungen und der empfohlenen Konfigurationen für jede Einstellung zum Schützen von Computern unter Windows XP Professional in den beiden in diesem Kapitel behandelten Umgebungen. Wenn Sie Überlegungen zu den Sicherheitsrichtlinien für Ihre Organisation anstellen, denken Sie auch an die Wechselwirkungen zwischen Sicherheit und Benutzerproduktivität. Obwohl Benutzer Schutz vor schädlichem Code und Angreifern benötigen, müssen sie ihre Aufgaben ohne Beschränkungen durch zu strenge Sicherheitsrichtlinien erledigen können.
  
#### Weitere Informationen
  
Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen hinsichtlich Windows XP Professional.
  
-   Weitere Informationen zur Gewährleistung der Sicherheit für Windows XP Professional finden Sie in dem in Windows XP enthaltenen Tool „Hilfe und Support“ und auf der Microsoft-Website [Sicherheit und Datenschutz unter Windows XP](http://www.microsoft.com/windowsxp/security/) (in englischer Sprache) unter www.microsoft.com/windowsxp/security/.
  
-   Weitere Informationen zu den Sicherheitsfunktionen in Windows XP SP2 finden Sie im Artikel „[Sicherheitsinformationen für Windows XP Service Pack 2](http://www.microsoft.com/technet/prodtechnol/winxppro/maintain/xpsp2sec.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/winxppro/maintain/xpsp2sec.mspx.
  
-   Weitere Informationen zu den unter Windows XP SP2 verfügbaren Sicherheitseinstellungen finden Sie im Microsoft TechNet-Artikel „[Beschreibungen von Sicherheitseinstellungen](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/dd980ca3-f686-4ffc-a617-50c6240f5582.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/dd980ca3-f686-4ffc-a617-50c6240f5582.mspx.
  
-   Weitere Informationen zu sicheren Kanälen finden Sie im Windows 2000 Magazine-Artikel „[Sichere Kanäle in NT 4.0](http://msdn.microsoft.com/archive/en-us/dnarntmag00/html/secure.asp)“ (in englischer Sprache) unter http://msdn.microsoft.com/archive/en-us/dnarntmag00/html/secure.asp.
  
-   Weitere Informationen zur Sicherheit für das Windows-Betriebssystem finden Sie im [Microsoft Windows Security Resource Kit](http://www.microsoft.com/mspress/books/6418.asp) (in englischer Sprache) unter www.microsoft.com/MSPress/books/6418.asp.
  
-   Weitere Informationen zum verschlüsselnden Dateisystem von Windows XP und Windows Server 2003 finden Sie im Artikel „[Verschlüsselndes Dateisystem in Windows XP und Windows Server 2003](http://www.microsoft.com/technet/prodtechnol/winxppro/deploy/cryptfs.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/winxppro/deploy/cryptfs.mspx.
  
##### In diesem Beitrag
  
-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/default.mspx)  
-   [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch01.mspx)  
-   [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch02.mspx)  
-   Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients  
-   [Kapitel 4: Administrative Vorlagen für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch04.mspx)  
-   [Kapitel 5: Schützen eigenständiger Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch05.mspx)  
-   [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch06.mspx)  
-   [Kapitel 7: Zusammenfassung](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgch07.mspx)  
-   [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)  
-   [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxa.mspx)  
-   [Anhang B: Testen des Sicherheitshandbuchs für Windows XP](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapxb.mspx)  
-   [Danksagungen](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgack.mspx)
  
##### Download
  
[![](images/Cc163074.icon_exe(de-de,TechNet.10).gif)Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
