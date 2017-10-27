---
TOCTitle: 'RMS – Häufig gestellte Fragen: Verwaltung'
Title: 'RMS – Häufig gestellte Fragen: Verwaltung'
ms:assetid: '43f77336-5e62-4405-9efb-55417a402d62'
ms:contentKeyID: 18118817
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747547(v=WS.10)'
---

RMS – Häufig gestellte Fragen: Verwaltung
=========================================

RMS-Verwaltung – Häufig gestellte Fragen
----------------------------------------

-   [Auf welche Art lassen sich die dokumentbezogenen Berechtigungen eines Benutzers, der die Organisation verlässt, am besten sperren?](#bkmk_1)
-   [Muss das XrML-Lizenzzertifikat, das beim Aufbau der Vertrauensstellungen zwischen zwei Organisationen zum Austausch von RMS-geschütztem Inhalt an das vertrauende Unternehmen übergeben wird, in besonderer Weise behandelt werden?](#bkmk_2)
-   [Wie arbeitet RMS mit servergespeicherten Benutzerprofilen?](#bkmk_3)
-   [Welche Gründe kann es dafür geben, dass eine Organisation RMS außer Betrieb setzen möchte?](#bkmk_4)
-   [Wie läuft der Außerbetriebsetzungsprozess im Allgemeinen ab?](#bkmk_5)
-   [Kann ein RMS-Server so außer Betrieb gesetzt werden, dass nur einige Benutzer Dokumente wiederherstellen können?](#bkmk_6)
-   [Was bedeutet die Meldung, dass der Server nicht auf das Anwendungsverzeichnis zugreifen kann?](#bkmk_7)
-   [Kann die Ablaufverfolgung für den RMS-Server verwendet werden?](#bkmk_8)
-   [Was versteht man unter einer Zeitabweichung, und was kann im Falle einer Zeitabweichung unternommen werden?](#bkmk_9)

<span id="BKMK_1"></span>
#### Auf welche Art lassen sich die dokumentbezogenen Berechtigungen eines Benutzers, der die Organisation verlässt, am besten sperren?

Im Allgemeinen ist es besser, Dokumente nicht für einzelne Benutzerkonten, sondern für Benutzergruppen zu lizenzieren, die in Active Directory definiert sind. Auf diese Weise kann ein Benutzer, der die Organisation verlässt, einfach aus der Active Directory-Gruppe gelöscht werden und anschließend keine an die Gruppe gesendeten Dokumente mehr lesen. Der Benutzer hat in diesem Fall jedoch weiterhin Zugriff auf Dokumente, für die eine Nutzungslizenz vorhanden ist, wenn in den Rechten des Dokuments nicht zuvor festgelegt wurde, dass der Benutzer bei jedem Öffnen des Dokuments eine Nutzungslizenz erwerben muss. Wenn dieses Recht nicht definiert ist, kann das Öffnen von Dokumenten mit vorhandener Nutzungslizenz durch den Benutzer nur dadurch verhindert werden, dass der Lizenzspeicher des Benutzers auf seinem Computer geleert wird.

<span id="BKMK_2"></span>
#### Muss das XrML-Lizenzzertifikat, das beim Aufbau der Vertrauensstellungen zwischen zwei Organisationen zum Austausch von RMS-geschütztem Inhalt an das vertrauende Unternehmen übergeben wird, in besonderer Weise behandelt werden?

Wenn eine vertrauenswürdige Benutzerdomäne oder Veröffentlichungsdomäne aufgebaut wird, entscheiden Sie sich dafür, der Partnerorganisation zu vertrauen und sie an Ihrem Rechteverwaltungssystem teilhaben zu lassen. Sie gehen damit automatisch das kalkulierte Risiko ein, dass die Sicherheit Ihrer Daten durch einen Vertrauensbruch seitens der anderen Organisation gefährdet wird. Es hat sich bewährt, die Partnerorganisation aufzufordern, ihr RMS-Server-Lizenzgeberzertifikat über einen authentifizierten Kanal, wie z. B. S/MIME-E-Mail, zu senden, um das Risiko einer Manipulation des Server-Lizenzgeberzertifikats vor dem Import auf Ihren RMS-Server zu minimieren.

<span id="BKMK_3"></span>
#### Wie arbeitet RMS mit servergespeicherten Benutzerprofilen?

Rechtekontozertifikate (Rights Account Certificates, RACs) zur Identifizierung von Benutzern sind computerspezifisch. Bei servergespeicherten Profilen wird bei der ersten Verwendung durch RMS auf einem bestimmten Computer ein neues Rechtekontozertifikat für den Benutzer auf diesem Computer erstellt.

<span id="BKMK_4"></span>
#### Welche Gründe kann es dafür geben, dass eine Organisation RMS außer Betrieb setzen möchte?

Beim Außerbetriebsetzen von RMS wird der RMS-Server aus der Infrastruktur entfernt, sodass Benutzer dann die Möglichkeit haben, durch Rechte geschützte Inhalte ohne Schutzfunktion zu speichern. Es gibt drei Hauptgründe, warum sich eine Organisation dafür entscheiden könnte:

-   Vereinfachung der Architektur, beispielsweise durch Anordnung der Server in Clustern
-   Umwandlung einer Proof-of-Concept-Pilotumgebung in eine Produktionsumgebung
-   Zusammenführen von RMS-Servern, z. B. nach einer Unternehmensfusion

<span id="BKMK_5"></span>
#### Wie läuft der Außerbetriebsetzungsprozess im Allgemeinen ab?

Der Außerbetriebsetzungsprozess beginnt damit, dass der Außerbetriebsetzungsdienst auf dem RMS-Stammcluster aktiviert wird. Sobald der Außerbetriebsetzungsdienst aktiviert wird, werden alle anderen Dienste (z. B. der Lizenzierungs- und Zertifizierungsdienst) deaktiviert. Danach muss die RMS-fähige Anwendung eines jeden Benutzers eine Verbindung zum Außerbetriebsetzungsdienst herstellen, wenn eine RMS-Funktion verwendet wird. Ein Beispiel für eine RMS-fähige Anwendung ist Microsoft Office 2003. In Office 2003 wird der RMS-Client mithilfe von Registrierungsschlüsseln an RMS-Dienste verwiesen. Der Außerbetriebsetzungsdienst wird durch einen bestimmten Registrierungsschlüssel identifiziert. Wenn dieser Schlüssel für den Verweis des Clients an den Außerbetriebsetzungsdienst konfiguriert wird, erteilt der RMS-Cluster dem Benutzer Nutzungslizenzen mit umfassenden Berechtigungen (Lesen, Schreiben, Kopieren, Drucken, Bearbeiten usw.) für den jeweiligen Inhalt, und dies unabhängig davon, ob der Benutzer ursprünglich diese Berechtigungen hatte. Anschließend werden die Benutzer angewiesen, sämtliche Rechteschutzfunktionen aus allen Dokumenten zu entfernen, die sie nach der vollständigen Außerbetriebnahme des RMS-Clusters behalten möchten. Wenn dies geschehen ist, kann der RMS-Cluster vollständig außer Dienst gestellt werden.

Es hat sich bewährt, die Konfigurationsdatenbank des RMS-Clusters für den Fall zu sichern, dass ein durch Rechte geschütztes Dokument nach der Außerbetriebsetzung des Clusters wiederhergestellt werden muss. Ohne den privaten Schlüssel des RMS-Stammclusters kann nur der Autor des jeweiligen Dokuments den durch Rechte geschützten Inhalt öffnen, nachdem der Server entfernt wurde.

<span id="BKMK_6"></span>
#### Kann ein RMS-Server so außer Betrieb gesetzt werden, dass nur einige Benutzer Dokumente wiederherstellen können?

Sie können eine Zugriffssteuerungsliste (Access Control List, ACL) für den Außerbetriebsetzungsdienst („decommission.asmx“) festlegen, damit nur bestimmte Benutzer den Schlüssel erwerben können, mit dem der durch Rechte geschützte Inhalt zu entschlüsseln ist.

<span id="BKMK_7"></span>
#### Was bedeutet die Meldung, dass der Server nicht auf das Anwendungsverzeichnis zugreifen kann?

Diese Fehlermeldung tritt manchmal auf, wenn Sie nach der Installation von RMS zum ersten Mal versuchen, die RMS-Verwaltungswebsite zu öffnen. Wenn diese Fehlermeldung angezeigt wird, kann RMS weder konfiguriert noch verwaltet werden.

Dieser Fehler tritt normalerweise auf, wenn die Internetinformationsdienste (Internet Information Services, IIS) im Isolationsmodus von IIS 5.0 ausgeführt werden. Mit den folgenden Schritten können Sie diese Einstellung auf dem Server deaktivieren und die Internetinformationsdienste erneut starten, um dieses Problem zu beheben.

**So deaktivieren Sie den Isolationsmodus von IIS 5.0**
1.  Melden Sie sich auf dem RMS-Server als Mitglied der Gruppe der lokalen Administratoren an.

2.  Klicken Sie auf **Start**, zeigen Sie auf **Verwaltung**, und klicken Sie anschließend auf **Internetinformationsdienste-Manager**.

3.  Erweitern Sie im **IIS-Manager** den lokalen Computer, klicken Sie mit der rechten Maustaste auf **Websites** und anschließend auf **Eigenschaften**.

4.  Klicken Sie auf die Registerkarte **Dienst**, deaktivieren Sie das Kontrollkästchen **WWW-Dienst im IIS 5.0-Isolationsmodus ausführen**, und klicken Sie anschließend auf **OK**.

5.  Damit diese Änderungen wirksam werden, müssen die Internetinformationsdienste erneut gestartet werden. Wenn Sie aufgefordert werden, die Internetinformationsdienste erneut zu starten, klicken Sie auf **Ja**.

<span id="BKMK_8"></span>
#### Kann die Ablaufverfolgung für den RMS-Server verwendet werden?

Da die Rechteverwaltungsdienste (Rights Management Services, RMS) mithilfe von Microsoft® .NET Framework erstellt wurden, können Sie zum Nachverfolgen von Systemereignissen und zum Beheben von Problemen die Ablaufverfolgung verwenden.

Sie können die Ablaufverfolgung implementieren, indem Sie die Datei „Web.config“ oder die Datei „Machine.config“ ändern. Wenn Sie diese Funktion in der Datei „Machine.config“ implementieren, wird die Ablaufverfolgung für jede Softwarekomponente auf dem Computer ausgeführt. Wenn Sie die Funktion jedoch in der Datei „Web.config“ implementieren, wird die Ablaufverfolgung nur für die in den Webdiensten auftretenden Ereignisse ausgeführt.

**So aktivieren Sie die Ablaufverfolgung**
1.  Öffnen Sie die Datei „Machine.config“ oder „Web.config“, und fügen Sie unter dem Abschnitt „&lt;system.diagnostics&gt;“ folgende Zeilen hinzu:
    ```
        <system.diagnostics>
        <switches>
        <add name="Microsoft Windows Rights Management Services-Global" value="4" />
        <add name="Microsoft Windows Rights Management Services-TimeStamps" value="1" /> 
        <add name="Microsoft Windows Rights Management Services-Indents" value="0" /> 
        </switches>
        <trace autoflush="false" indentsize="4"/>
        </system.diagnostics>
    ```
2.  Starten Sie IIS neu, indem Sie an einer Eingabeaufforderung IISRESET ausführen.

3.  Entfernen Sie die in Schritt 1 hinzugefügten Zeilen wieder aus der CONFIG-Datei, nachdem Sie die nötigen Daten gesammelt haben.

4.  Starten Sie IIS neu, indem Sie an einer Eingabeaufforderung IISRESET ausführen.

| ![](images/Cc747547.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                                                                                                               |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn die Ablaufverfolgung auf einem RMS-Server ausgeführt wird, kann sich dies negativ auf die Arbeitsgeschwindigkeit auswirken, d. h., es können Verzögerungen beim Erwerb von Nutzungslizenzen und bei der Ausstellung von Rechtekontozertifikaten auftreten. Verwenden Sie die Ablaufverfolgung deshalb nur dann, wenn Sie sie zur Diagnose und Behebung vorhandener Probleme benötigen. |

<span id="BKMK_9"></span>
#### Was versteht man unter einer Zeitabweichung, und was kann im Falle einer Zeitabweichung unternommen werden?

Eine Zeitabweichung liegt vor, wenn die Uhrzeit eines Computers von der eines anderen Computers abweicht. Diese Abweichung tritt ebenso häufig auf wie ein Unterschied bei der Uhrzeit auf den Armbanduhren von zwei verschiedenen Personen. Eine Zeitabweichung kann allerdings beim Angeben der Gültigkeitsdauer in einer Lizenz zu Problemen führen.

Die Gültigkeitsdauer wird immer gemäß der Uhrzeit auf dem Computer des Herausgebers festgelegt. Eine Zeitabweichung bei diesen Uhrzeiten kann im Zyklus aus Veröffentlichen und Abrufen an zwei Stellen zu Problemen führen:

-   Wenn eine Anwendung versucht, eine Nutzungslizenz zu erwerben und dabei eine Veröffentlichungslizenz verwendet, deren Gültigkeitsdauer gemäß der Uhrzeit auf dem RMS-Server in der Vergangenheit endet oder in der Zukunft beginnt. In diesem Fall schlägt die Anforderung fehl. Dies kann für einen Benutzer beim Anfordern einer Nutzungslizenz oder für eine Anwendung beim Versuch der Vorlizenzierung eines Dokuments (d. h. beim Erwerb einer Lizenz im Namen eines Benutzers) auftreten.
-   Wenn die Gültigkeitsdauer der Lizenz abgelaufen ist oder noch nicht begonnen hat, schlägt der Versuch, diese Lizenz zu verwenden, fehl. Andernfalls sind lediglich die bereits abgelaufenen oder noch nicht gültigen Rechte nicht verfügbar.

Wenn beispielsweise die Uhr eines Herausgebercomputers im Vergleich mit der Uhr eines abrufenden Computers um 15 Minuten nachgeht und der Herausgeber eine Veröffentlichungslizenz erstellt, in der angegeben ist, dass der Inhalt in 15 Minuten abläuft, erhält der Benutzer, der den Inhalt abrufen möchte, eine nicht verwendbare Nutzungslizenz, weil die von der Nutzungslizenz erteilten Rechte zum Anzeigen des Inhalts bereits abgelaufen sind.

Es gibt keine optimale Lösung zum Beheben von Problemen bei Zeitabweichungen. Eine gute Lösung ist es, bei abrufenden Benutzern, deren Uhr im Vergleich mit Ihrer Uhr nachgeht, die Anfangszeit der Gültigkeitsdauer auf eine Uhrzeit vor der aktuellen Uhrzeit festzulegen und, wenn möglich, bei Benutzern, deren Uhr im Vergleich zu Ihrer Uhr vorgeht, die Gültigkeitsdauer zu verlängern. Sie sollten die Problematik der Zeitabweichung stets berücksichtigen, insbesondere, wenn Sie Lizenzen mit kurzer Gültigkeitsdauer erstellen.