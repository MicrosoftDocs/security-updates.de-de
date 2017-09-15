---
TOCTitle: 'Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs'
Title: 'Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs'
ms:assetid: '2698b276-4c42-4a18-9930-3d69974746f8'
ms:contentKeyID: 20075664
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443721(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs

Aktualisiert: 27.12.2005

##### Auf dieser Seite

[](#edaa)[Überblick](#edaa)
[](#ecaa)[Testumgebung](#ecaa)
[](#ebaa)[Testmethoden](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Das *Windows Server 2003-Sicherheitshandbuch* ist eine bewährte und reproduzierbare Konfigurationsanleitung für die Absicherung von Microsoft® Windows* *Server™* *2003 mit Service Pack 1 (SP1) in verschiedenen Umgebungen.

Das *Windows Server 2003-Sicherheitshandbuch* wurde in einer Testumgebung getestet, um sicherzustellen, dass die Anleitungen wie erwartet funktionieren. Die Dokumentation wurde vom Testteam des *Windows Server 2003-Sicherheitshandbuch*s auf ihre Konsistenz hin überprüft, und die empfohlenen Schritte wurden getestet. Zudem wurden Funktionstests durchgeführt, um die benötigten Ressourcen der Leser dieser Anleitung beim Einrichten und Testen der eigenen Implementierungen zu minimieren.

#### Umfang

Das *Windows Server 2003-Sicherheitshandbuch* wurde in drei verschiedenen simulierten Sicherheitsumgebungen getestet: der Umgebung mit älteren Clients, der Unternehmensclient-Umgebung und der Hochsicherheitsumgebung. Diese Umgebungen werden in Kapitel 1 „Einführung in das Windows* *Server* *2003-Sicherheitshandbuch“ erläutert. Tests wurden auf Grundlage der im folgenden Abschnitt „Ziele“ beschriebenen Kriterien durchgeführt.

Eine Bewertung der Sicherheitsanfälligkeiten der Testumgebung, die zur Sicherung der Lösung des *Windows Server 2003-Sicherheitshandbuchs* verwendet wurde, konnte vom Testteam nicht vorgenommen werden.

#### Ziele

Das Testteam des *Windows Server 2003-Sicherheitshandbuchs* ließ sich von folgenden Testzielen leiten:

-   Überprüfen der empfohlenen Änderungen an den Sicherheitseinstellungen für die drei im Handbuch definierten Sicherheitsstufen. Gründe für diese Änderungen beinhalten:

    -   Durch die Veröffentlichung von SP1 für Windows* *Server* *2003 erforderliche Änderungen.

    -   Einsatz des neuen in SP1 erhältlichen Tools Sicherheitskonfigurations-Assistent (SCW) sowie neuer Funktionen wie Windows Firewall.

    -   Internes und externes Feedback zur Vorversion des Handbuchs.

-   Sicherstellen, dass die im Handbuch empfohlenen Sicherheitseinstellungen und Konfigurationsänderungen den Voraussetzungen der Umgebung mit älteren Clients sowie der Unternehmensclient- und der Hochsicherheitsumgebung entsprechen.

-   Sicherstellen, dass abgesicherte Domänenmitgliedsserver ihre Rollenaufgaben erfolgreich durchführen können.

-   Sicherstellen, dass die Kommunikation zwischen den Clientcomputern und den Domänencontrollern nicht beeinträchtigt wird.

-   Überprüfen, ob alle Anleitungen verständlich, vollständig und technisch richtig sind.

Außerdem soll die Anleitung wiederholbar sein und zuverlässig von einem Microsoft Certified Systems Engineer (MSCE) mit zwei Jahren Erfahrung verwendet werden können.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Testumgebung

Die Netzwerke der Testumgebung, die zum Testen des Handbuchs entwickelt wurden, sind mit den für die Vorversion des Handbuchs verwendeten Netzwerken vergleichbar. Drei separate, aber ähnliche Netzwerke wurden entwickelt, eines pro definierter Umgebung.

Jedes Testnetzwerk bestand aus einer Windows* *Server* *2003 mit SP1 und Active Directory®-Verzeichnisdienststruktur, Computern für Infrastrukturenserverrollen, die Domänencontroller-, DNS-, WINS- und DHCP-Dienste bereitstellten, sowie anderen Computern für Anwendungsserverrollen, die Datei-, Druck- und Webdienste bereitstellten. Das Unternehmensclient-Netzwerk beinhaltete zudem Computer für die Zertifikatdienste und IAS-Serverrollen, während die Bastion-Hostserverrolle (BH) Bestandteil des Hochsicherheitsnetzwerks war. Zu den Unternehmensclient- und Hochsicherheitsnetzwerken zählten zudem Microsoft Operations Manager (MOM) 2005 und Systems Management Server (SMS) 2003 zum Verwalten und Überwachen der Domänenmitgliedsserver und Clientcomputer. Diese Netzwerke beinhalteten auch Microsoft Exchange* *Server 2003 für den E-Mail-Dienst.

Die Clientcomputer in den verschiedenen Netzwerken verwendeten Windows XP Professional mit SP2 und Windows 2000 Professional mit SP4. Das Netzwerk für Umgebungen mit älteren Clients beinhaltete auch Clientcomputer, auf denen Windows 98 SR2 und Windows NT® 4.0-Arbeitsstationen mit Service Pack 6a ausgeführt wurden.

Im folgenden Diagramm wird das für die Unternehmensclient-Umgebung entwickelte Testumgebungsnetzwerk aufgezeigt.

![](images/Dd443721.apdxd_fg01(de-de,TechNet.10).gif)

**Abbildung D. 1 Logisches Diagramm des Testumgebungsnetzwerks für die Unternehmensclient-Umgebung**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443721.apdxd_fg01_big(de-de,technet.10).gif)
Zum Prüfen der Replikationsszenarien zwischen abgesicherten Domänencontrollern bestand die Active Directory-Gesamtstruktur aus zwei Sites. Eine davon war die Site der Zentrale mit einer leeren Stammdomäne und einer Unterdomäne mit den oben erwähnten Servern und Clientcomputern. Die zweite Site bestand lediglich aus einem zweiten Domänencontroller der Unterdomäne.

Im folgenden Diagramm wird das für die Hochsicherheitsumgebung entwickelte Testumgebungsnetzwerk aufgezeigt.

![](images/Dd443721.apdxd_fg02(de-de,TechNet.10).gif)

**Abbildung D. 2 Logisches Diagramm des Testumgebungsnetzwerks für die Hochsicherheitsumgebung**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443721.apdxd_fg02_big(de-de,technet.10).gif)
[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Testmethoden

In diesem Abschnitt werden die Verfahren beschrieben, nach denen beim Testen des *Windows Server 2003-Sicherheitshandbuchs* vorgegangen wurde.

Das Testteam richtete ein Labor ein, das die drei im vorigen Abschnitt beschriebenen Netzwerke beinhaltete. Nach einem bestandenen Test zur Prüfung des Konzepts (POC) wurden zwei weitere robuste Testzyklen durchgeführt. Bei jedem Durchlauf strebte das Team danach, die Lösung zu stabilisieren.

Bei einem Testzyklus wurden die folgenden Phasen durchlaufen:

1.  Phase der Sicherheitskonfigurationseinrichtung

    -   Manuelle Konfigurationsphase

    -   Phase der Gruppenrichtlinienkonfiguration

2.  Phase der Testausführung

Die Einzelheiten jeder Phase sind im Abschnitt „Phasen in einem Testdurchlauf“ dargelegt. Im Abschnitt „Testvorbereitungsphase“ werden jene Schritte beschrieben, mit deren Hilfe sichergestellt wurde, dass die Testumgebung frei von jeglichen Problemen war, die zu einer Missdeutung der eigentlichen Testergebnisse hätten führen könnten, nachdem die beiden Umgebungsszenarien durch die zwei inkrementellen Aufbauphasen abgesichert worden waren. Dieser Status wird auch als „Baseline“ bezeichnet.

#### Phasen in einem Testdurchlauf

Die Testphasen werden in den folgenden Abschnitten beschrieben. Kritische in dieser Aufbauphase gefundene Probleme wurden als Fehler identifiziert und in der Einrichtungsphase gelöst, bevor das Testteam zur Testausführungsphase überging. Dadurch wurde sichergestellt, dass die korrekte Sicherheitskonfiguration im Netzwerk implementiert und die Genauigkeit der erzielten Testergebnisse überprüft wurde.

##### Testvorbereitungsphase

In dieser Phase wird die Baselinekonfiguration eingerichtet, die im Rahmen der Sicherheitskonfigurationseinrichtung auf die Lösung angewendet wird. Die folgenden Schritte wurden für die jeweils drei verschiedenen Umgebungen – die Umgebung mit älteren Clients, die Unternehmensclient-Umgebung und die Hochsicherheitsumgebung – ausgeführt.

**So schließen Sie die Testvorbereitungsphase ab**

1.  Vernetzen Sie die Computer wie im Netzwerkdiagramm dargestellt. Installieren Sie die entsprechenden Versionen des Windows-Betriebssystems auf allen Server- und Clientcomputern.

2.  Erstellen und konfigurieren Sie die Domäne, die Domänencontroller und die zwei Sites.

3.  Schließen Sie die einzelnen Mitgliedsserver und Verwaltungsserver an, und konfigurieren Sie sie. Verbinden Sie außerdem die Clientcomputer mit der Domäne.

4.  Führen Sie grundlegenden Überprüfungen für die einzelnen Serverrollen durch, um die entsprechende Netzwerk- und Anwendungskonfiguration zu bestätigen.

5.  Prüfen Sie das Ereignisprotokoll der einzelnen Mitgliedsserver im Netzwerk, um sicherzustellen, dass keine Anwendungs- oder Systemfehler vorliegen.

6.  Stellen Sie sicher, dass die Clientcomputer auf die Dienste zugreifen können, die vom Domänencontroller und den Mitgliedsservern (DNS-, DHCP-, Zertifizierungsstellen-, Datei-, Druck-, Web- und E-Mail-Server) bereitgestellt werden. Prüfen Sie die Ereignisprotokolle auf den Clientcomputern, um sicherzustellen, dass keine Fehler vorliegen.

7.  Überprüfen Sie, ob alle erforderlichen Anwendungen, Dienste und Agents auf den einzelnen Domänenmitgliedern installiert sind. Sie sollten z. B. überprüfen, ob der MOM-Agent auf allen Servern installiert ist, die vom MOM-Server verwaltet werden.

8.  Sobald die vorangegangenen Schritte abgeschlossen sind, erstellen Sie von jedem Computer ein Sicherungsabbild. Diese zu Sicherungszwecken erstellten Abbilder werden verwendet, um das Netzwerk vor Beginn eines neuen Tests auf die Baselinekonfiguration zurückzusetzen.

##### Phase der Sicherheitskonfigurationseinrichtung

Bei dieser Phase sollten die im Handbuch angeführten Verfahren zur Konfiguration von Domäne, Domänencontroller und Mitgliedsserver befolgt werden, um eine sicherere Stufe als die Baselinekonfiguration zu erhalten.

###### Manuelle Konfigurationsphase

Diese Phase ist häufig die erste Aufbauphase für die Sicherheit. Die in den einzelnen Kapiteln bereitgestellten Empfehlungen zur manuellen Absicherung wurden in dieser Phase implementiert.

**Hinweis**: Möglicherweise treffen nicht alle Schritte auf Ihr Netzwerk zu. Überprüfen Sie die einzelnen Verfahren sorgfältig, um sich die Auswirkungen auf Ihr Netzwerk vor Augen zu führen.

**So führen Sie die manuelle Konfigurationsphase durch**

1.  Verwenden Sie das Computerverwaltungs-Snap-In der Microsoft Management Console (MMC) zum Vornehmen der empfohlenen Änderungen der Richtlinieneinstellungen (wie etwa das lokale Administratorkonto und -kennwort) auf den einzelnen Mitgliedscomputern. Führen Sie zum Schutz der Domänenkonten die folgenden Schritte durch:

    1.  Stellen Sie sicher, dass das vordefinierte lokale Administratorkonto mit einem komplexen Kennwort versehen, umbenannt und seine vorgegebene Kontenbeschreibung gelöscht wurde.

    2.  Nennen Sie die Gastkonten auf dem Host um, und deaktivieren Sie sie.

    3.  Berücksichtigen Sie die zusätzlichen Empfehlungen aus dem Handbuch zum Absichern der Domänenkonten.

2.  Fügen Sie den Einstellungen für Benutzerrechte eindeutige Sicherheitsgruppen oder -konten gemäß den Beschreibungen in den Kapiteln hinzu.

3.  Führen Sie alle anderen zutreffenden manuellen Absicherungsverfahren aus, die in den einzelnen Kapiteln vorgeschrieben wurden. Aktivieren Sie z. B. die Konfigurationen für manuelle Speicherauszüge und die Fehlerberichterstattung.

###### Phase der Gruppenrichtlinienkonfiguration

Diese Phase dient zur Erstellung und Anwendung der Gruppenrichtlinienobjekte (GPOs) auf Domänen- und Organisationseinheiten-Ebene. GPOs werden entsprechend den Empfehlungen in Kapitel 2, „Absicherungsmechanismen von Windows Server 2003* *Server* *2003“, auf die verschiedenen Organisationseinheiten angewendet.

Service Pack 1 für Windows Server 2003 hat neue Tools und Funktionen eingeführt, die dazu geführt haben, dass die Implementierung des Gruppenrichtliniendesigns im Vergleich zur Vorversion geändert wurde.

SCW ist ein Tool zur Reduktion der Angriffsfläche, das zum Erstellen des erforderlichen Sicherheitsrichtliniensatzes für die einzelnen Serverrollen, die in diesem Handbuch erläutert werden, dient. Die Verfügbarkeit von SCW hat zu den folgenden wichtigen Änderungen für die Phase der Gruppenrichtlinienkonfiguration geführt:

-   Mit der Vorversion dieses Handbuchs bereitgestellte IPSec-Filter wurden durch Portkonfigurationen der Windows Firewall ersetzt, die mit SCW erstellt wurden.

-   Im Handbuch enthaltene Sicherheitsvorlagen sind in Verbindung mit SCW zum Erstellen von XML-Sicherheitsvorlagendateien zu verwenden. Diese Vorlagen werden dann mit dem Befehlszeilenprogramm Scwcmd in entsprechende GPOs umgewandelt.

Für die drei Sicherheitsumgebungen wurden jeweils die folgenden Schritte wiederholt:

**So erstellen Sie Gruppenrichtlinienobjekte:**

1.  Stellen Sie sicher, dass alle erforderlichen Anwendungen, Dienste und Agents auf den einzelnen Domänenmitgliedern des Baseline-Netzwerks installiert wurden. Stellen Sie z. B. sicher, dass der MOM-Agent auf allen Domänenmitgliedsservern installiert wurde, die von MOM verwaltet werden.

2.  Verwenden Sie das MMC-Snap-In „Active* *Directory-Benutzer und -Computer“ zum Erstellen der beschriebenen Organisationseinheitstruktur.

3.  Erstellen Sie das Gruppenrichtlinienobjekt der Domänenrichtlinie mit der INF-Sicherheitsvorlage. Für diesen Schritt ist der SCW nicht erforderlich.

4.  Verwenden Sie das SCW-Tool zum Erstellen von XML-basierten Sicherheitsvorlagen für die einzelnen im Handbuch beschriebenen Serverrollen. Eine Anleitung ist in Kapitel 2, „Absicherungsmechanismen von Windows* *Server* *2003“, und den jeweiligen Kapiteln zu den einzelnen Serverrollen enthalten. Bei Durchführung dieses Schritts ist die entsprechende INF-Sicherheitsvorlage für die Serverrolle mit einzuschließen. Die Vorlagedateien sind in der Download-Version dieses Handbuchs enthalten.

5.  Verwenden Sie das Befehlszeilenprogramm Scwcmd zur Konvertierung der XML-Sicherheitsvorlagen, die im vorherigen Schritt zu GPOs erstellt wurden.

6.  Wiederholen Sie Schritt 4 auf dem Bastion-Hostserver, um die Bastion-Host-XML-Sicherheitsvorlage zu erstellen, und verwenden Sie danach den SCW erneut zur Konvertierung und Anwendung der Vorlage auf das lokale GPO.

Nach erfolgreicher Erstellung der GPOs vergleichen Sie die Einstellungen mit den Anweisungen in den Kapiteln, um fehlerhafte Konfigurationen zu identifizieren.

In dieser Phase befinden sich alle Domänenmitgliedsserver in der Organisationseinheit Computer. Diese Server werden dann zu ihren jeweiligen Organisationseinheiten unter der Mitgliedsserver-Organisationseinheit verschoben.

Die nächste im folgenden Verfahren genau geschilderte Aufgabe ist die Anwendung dieser GPOs auf die jeweiligen Organisationseinheiten. Mit dem Gruppenrichtlinien-Verwaltungskonsolen-Tool (Group Policy Management Console; GPMC) wurde das GPO mit der Organisationseinheit verknüpft. Das Gruppenrichtlinienobjekt der Domänencontrollerrichtlinie wurde zuletzt verknüpft.

Die folgenden Schritte wurden ausgeführt, um die Phase der Sicherheitskonfigurationsrichtung abzuschließen:

**So wenden Sie Gruppenrichtlinienobjekte an:**

1.  Verknüpfen Sie das Domänenrichtlinienobjekt mit dem Domänenobjekt.

    **Hinweis**: Wenn bereits standardmäßige GPO-Verknüpfungen vorhanden sind oder mehrere GPOs existieren, müssen Sie u. U. die GPO-Verknüpfungen in der Prioritätenliste erhöhen.

2.  Verwenden Sie die Gruppenrichtlinien-Verwaltungskonsole zum Verknüpfen des GPO für die Mitgliedsserver-Baseline-Richtlinie mit der Mitgliedsserver-Organisationseinheit. (Sie können diesen Schritt auch mit dem MMC-Snap-In „Active* *Directory-Benutzer und -Computer“ durchführen.)

3.  Verknüpfen Sie die einzelnen Serverrollen-GPOs mit der jeweiligen Serverrollen-Organisationseinheit.

4.  Verknüpfen Sie das GPO für die Domänencontrollerrichtlinie mit der Domänencontroller-Organisationseinheit.

5.  Um die Anwendung der aktuellsten Gruppenrichtlinieneinstellungen sicherzustellen, müssen Sie an einer Eingabeaufforderung **gpudpate /force** auf allen Domänencontrollern ausführen. Starten Sie dann alle Domänencontroller nacheinander neu, und beginnen Sie mit dem primären Domänencontroller. Räumen Sie genügend Zeit für Active* *Directory zum Replizieren der Änderungen zwischen den Sites ein.

    **Wichtig**: Nach Anwendung der GPO für die Domänencontrollerrichtlinie muss unbedingt ein Neustart der Domänencontroller durchgeführt werden. Unterlassen Sie diesen Schritt, werden möglicherweise Replikationsfehler im Verzeichnisdienstordner oder Userenv-Fehler im Anwendungsordner der Ereignisanzeige angezeigt.

6.  Wiederholen Sie Schritt 5 auf allen Mitgliedsservern der Domäne.

7.  Überprüfen Sie die Ereignisanzeige auf Fehler hin. Prüfen Sie die Fehlerprotokolle, um Fehler zu beheben und Missstände zu beseitigen.

8.  Verwenden Sie das SCW-Tool auf dem Bastion-Hostserver, um die Bastion-Host-XML-Sicherheitsvorlage auf das lokale GPO der Servers anzuwenden.

###### Überprüfen des Gruppenrichtliniendownloads auf die Mitgliedsservercomputer

Anhand der vorigen Verfahrens wurden GPOs erstellt und auf Organisationseinheiten angewendet, um die Computer in diesen Organisationseinheiten zu konfigurieren. Führen Sie die nachstehenden Schritte aus, um zu bestätigen, dass die Gruppenrichtlinie der Domänencontroller erfolgreich auf die Servercomputer heruntergeladen wurde. (Dabei wird vorausgesetzt, dass bei den Computern des Mitgliedsservers nach Verknüpfung des GPO mit der Organisationseinheit ein Neustart durchgeführt wurde.)

**So überprüfen Sie den Gruppenrichtliniendownload auf einen Mitgliedsservercomputer**

1.  Melden Sie sich beim Computer des Mitgliedsservers an.

2.  Klicken Sie auf **Start** und auf **Ausführen**, geben Sie **rsop.msc** ein, und drücken Sie die Eingabetaste.

3.  Erweitern Sie in der Konsole **Richtlinienergebnissatz** den **Konsolenstamm**, und wechseln Sie zu **Computerkonfiguration**.

4.  Klicken Sie mit der rechten Maustaste auf **Computerkonfiguration**, und klicken Sie auf **Eigenschaften**.

    Im Fenster **Eigenschaften von Computerkonfiguration** wird die Liste der Gruppenrichtlinienobjekte angezeigt. Das auf die Organisationseinheit angewendete Gruppenrichtlinienobjekt sollte in der Liste verfügbar sein, und es sollten keine Fehler damit verbunden sein.

##### Phase der Testausführung

In dieser Phase werden die Testfälle ausgeführt, die vom Testteam entwickelt wurden. Die Testausführungsphase soll Folgendes identifizieren:

-   Potenzielle Anwendungs-, Sicherheits- oder Systemfehlerereignisse, die von Prozessen zur Absicherung der Domänen, Domänencontroller, Mitgliederserver oder Bastion-Hostserver verursacht werden.

-   Ausfall von Diensten oder Funktionen, die durch die Änderungen der Sicherheitskonfiguration der Server im Netzwerk hervorgerufen wurde.

-   Technische Ungenauigkeiten zwischen dem Inhalt der Kapitel und der tatsächlichen Implementierung im Testlabor.

Das Testteam führte den Satz mit Testfällen aus, der im Ordner \\**Windows Server 2003-Sicherheitshandbuch Tools und Vorlagen\\Testtools** enthalten ist. (Die Tools und Vorlagen sind in der Online-Version dieses Handbuchs enthalten, die zum Download zur Verfügung steht.) Die Tests wurden auf jedem der drei separaten Netzwerken ausgeführt, außer bei Tests, die jeweils nur auf einem Netzwerk verfügbare Komponenten getestet haben, wie z. B. Zertifikatdienste, die nur in der Unternehmensclient-Umgebung verfügbar sind. Zusätzlich zu diesen Testfällen wurden manuelle Tests zu verschiedenen Zeitpunkten durchgeführt, etwa die regelmäßige Überprüfung der Ereignisanzeigeprotokolle oder die Überprüfung von speziellen, in der Vorversion des Handbuchs entdeckten Problemen. Alle identifizierten Probleme wurden in eine Datenbank aufgenommen und solange mit Mitgliedern des Entwicklungsteams besprochen, bis sie behoben wurden.

Ausführlichere Informationen zu den verschiedenen Arten der durchgeführten Tests werden im nächsten Abschnitt bereitgestellt.

#### Testtypen

Das Testteam führte im Rahmen der Testphase die folgenden Testtypen durch, um sicherzustellen, dass die gesicherten Domänen, Domänencontroller und Mitgliedsserver keinen beträchtlichen Funktionalitätsverlust erfahren würden. Informieren Sie sich nötigenfalls in der Excel-Arbeitsmappe im Ordner **Windows Server 2003-Sicherheitshandbuch Tools und Vorlagen\\Testtools**, die mit diesem Handbuch heruntergeladen werden kann und eine vollständige Liste der Testfälle enthält, die für domänenbasierte und eigenständige Server unter Windows Server 2003 mit SP1 ausgeführt wurden. Ausführliche Informationen wie z. B. Testszenarien, Ausführungsschritte und zu erwartende Ergebnisse werden ebenfalls bereitgestellt.

Diese Tests wurden mehrere Male durchgeführt. Noch wichtiger aber ist, dass sie vor und nach der Implementierung der in diesem Handbuch beschriebenen Sicherheitseinstellungen ausgeführt wurden Durch diesen Ansatz konnte das Testteam potenzielle Fehler und Funktionsvariationen für die angeführten Serverrollen identifizieren.

##### Clientseitige Tests

Diese Testfälle wurden auf den Clientcomputern im Netzwerk durchgeführt. Der Hauptzweck dieser Tests lag darin sicherzustellen, dass Domänendienste (wie zum Beispiel Authentifizierung, Zugriffsrechte, Namensauflösung usw.) und anwendungsbasierte Dienste (wie z. B. Datei-, Druck- und Webdienst) nach Absicherung der Netzwerkserver für Clientcomputer verfügbar sind. Für die Umgebung mit älteren Computern wurde durch diese Tests sichergestellt, dass alle Clientcomputer unter Windows* *NT* *4.0 Service Pack 6a und Windows* *98 die Authentifizierung mit der Active* *Directory-Domäne von Windows* *Server* *2003 durchführen konnten.

##### Dokumentationserstellungstests

Anhand dieser Tests wird bestätigt, dass die in der Implementierungsanleitung dokumentierten Aussagen, Verfahren und Funktionen korrekt, eindeutig und vollständig sind. Für diese Tests sind keine separaten Testfälle aufgeführt.

##### Skripttests

Einige der Client-Testszenarien wurden in VBScript erstellt. Diese Testfälle befassen sich hauptsächlich mit dem ordnungsgemäßen Funktionieren von Windows XP-Clientcomputern, die netzwerkbasierte Dienste wie z. B. Domänenanmeldung, Kennwortänderung und Druckserverzugriff verwenden. Die VBScript-Dateien für diese Testfälle stehen im Ordner **Windows Server 2003-Sicherheitshandbuch Tools und Vorlagen\\Testtools** zum Herunterladen in der Online-Version dieses Handbuchs zur Verfügung.

##### Serverseitige Tests

Diese Testfälle wurden zur Prüfung der Funktionalität und Auswirkungen auf die Einrichtungsverfahren unter Windows* *Server* *2003 mit SP1-Servern entwickelt, die anhand der Empfehlungen in diesem Handbuch geschützt wurden. Alle in diesem Handbuch beschriebenen Serverrollen wurden getestet. Die zusätzlichen Serverrollen, die im Testnetzwerk enthalten sind, wie z. B. Exchange, MOM und SMS, wurden ebenfalls getestet.

#### Erfolgs- und Misserfolgskriterien

Bevor Tests durchgeführt wurden, wurden die folgenden Kriterien festgelegt, um die Fehlervorbeugung und -behebung zu gewährleisten:

-   Alle Testfälle müssen mit den erwarteten Ergebnissen bestanden werden, die in den einzelnen Testfalltabellen beschrieben sind.

-   Ein Testfall wird als bestanden betrachtet, wenn das tatsächliche Ergebnis mit dem erwarteten Ergebnis übereinstimmt, das für den Fall dokumentiert ist. Ist dies nicht der Fall, wurde der Testfall negativ bewertet, ein Bug erstellt und ein Schweregrad zugewiesen.

-   Wenn ein Testfall nicht bestanden wird, wird nicht unbedingt davon ausgegangen, dass die Lösung mangelhaft ist. Fehler könnten z. B. durch eine Missdeutung der Produktdokumentation bzw. durch eine unvollständige oder unpräzise Dokumentation verursacht werden. Jeder Fehler wird analysiert, um seine Ursache zu ergründen. Dabei dienen die tatsächlichen Ergebnisse und die in der Projektdokumentation beschriebenen Ergebnisse als Grundlage. Fehlerinformationen werden auch an die entsprechenden Besitzer der jeweiligen Microsoft-Produkte weitergeleitet.

#### Veröffentlichungskriterien

Das wichtigste Kriterium für die Veröffentlichung des *Windows Server 2003-Sicherheitshandbuchs* stand in engem Zusammenhang mit dem Schweregrad der noch ungelösten Fehler. Es wurden jedoch auch andere Probleme erörtert, die nicht durch Bugs erfasst wurden. Die Veröffentlichungskriterien lauten wie folgt:

-   Keine offenen Bugs der Schweregrade 1 und 2.

-   Alle offenen Bugs werden vom Führungsteam behoben, und ihre Auswirkungen sind vollständig bekannt.

-   Lösungshandbücher enthalten keinerlei Kommentare und Korrekturzeichen.

-   Die Lösung besteht alle Testfälle in der Testumgebung.

-   Die Inhalte der Lösung enthalten keine Widersprüche.

#### Bug-Klassifizierung

Die Schweregradskala für Bugs wird in der nachstehenden Tabelle beschrieben. Die Skala reicht von 1 bis 4, wobei 1 der höchste und 4 der niedrigste Schweregrad ist.

**Tabelle D. 1 Klassifizierung des Fehlerschweregrads**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Schweregrad</p></th>
<th><p>Häufigste Typen</p></th>
<th><p>Erforderliche Bedingungen</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>– Bug blockierte Aufbau oder weitere Tests.<br />
– Bug hat unerwarteten Benutzerzugriff verursacht.<br />  
– Die in der Dokumentation definierten Schritte waren unklar.<br />  
– Ergebnisse oder Verhalten einer Funktion oder eines Prozesses widersprechen den erwarteten Ergebnissen (die in der funktionalen Spezifikation dokumentiert sind).<br />
– Grobe Ungleichheit zwischen den Sicherheitsvorlagendateien und der funktionalen Spezifikation.</p></td>
<td style="border:1px solid black;"><p>– Lösung hat nicht funktioniert.<br />
– Benutzer konnte wichtige Teile des Computers oder Netzwerks nicht verwenden.<br />  
– Benutzer hatte unerlaubte Zugriffsberechtigungen.<br />  
– Benutzerzugriff für bestimmte Server, die Zugriff erhalten sollten, wurde blockiert.<br />  
– Erwartete Ergebnisse wurden nicht erzielt.<br />
Testverfahren kann ohne Behebung nicht fortfahren.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>2</p></td>
<td style="border:1px solid black;"><p>– Im Handbuch definierte Schritte sind unklar.<br />
– Dokumentierte Funktionalität fehlt (Test wurde in diesem Fall blockiert).<br />  
– Dokumentation fehlt oder ist unzureichend.<br />
– Inkonsistenz zwischen Sicherheitsvorlagendateien und Inhalt des Handbuchs, doch die Sicherheitsvorlagendatei ist mit der funktionalen Spezifikation synchron.</p></td>
<td style="border:1px solid black;"><p>– Benutzer konnte auf keine Problemumgehung zur Linderung der Situation zurückgreifen.<br />
– Problemumgehung war für Benutzer nicht einfach.<br />
– Computer oder Netzwerk konnte primäre Geschäftsanforderungen nicht erfüllen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>3</p></td>
<td style="border:1px solid black;"><p>– Dokumentiertes Formatproblem.<br />
– Geringfügige Fehler und Ungenauigkeiten in der Dokumentation.<br />
– Rechtschreibfehler im Text.</p></td>
<td style="border:1px solid black;"><p>– Benutzer verfügt über eine einfache Problemumgehung.<br />
– Benutzer kann leicht eine Problemumgehung finden.<br />  
– Bug beeinträchtigt Benutzerfreundlichkeit nicht.<br />
– Wichtige Geschäftsanforderungen funktionieren noch.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>4</p></td>
<td style="border:1px solid black;"><p>– Vorschläge.<br />
– Zukünftige Verbesserungen.</p></td>
<td style="border:1px solid black;"><p>– Bezieht sich eindeutig nicht auf diese Version.</p></td>
</tr>  
</tbody>  
</table>
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusammenfassung
  
Durch diesen Anhang werden einem Unternehmen, das das *Windows Server 2003 Sicherheitshandbuch* verwendet, die Verfahren und Schritte verständlich dargelegt, die zum Testen der Implementierung der Lösung in einer Testlaborumgebung angewendet und durchgeführt wurden. Die Erfahrung des Testteams für das *Windows Server 2003-Sicherheitshandbuch* ist in diesem Anhang enthalten. Hier finden Sie Beschreibungen der Testumgebung, Testtypen, Veröffentlichungskriterien und Fehlerklassifizierungsdetails.
  
Alle vom Testteam durchgeführte Testfälle wurden mit den erwarteten Ergebnissen bestanden. Das Testteam bestätigte, dass die Empfehlungen aus dem *Windows Server 2003-Sicherheitshandbuch* zur erforderlichen Funktionalität für die definierten Umgebungen beigetragen haben.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))  
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))  
-   [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))  
-   [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))  
-   [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))  
-   [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))  
-   [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))  
-   [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))  
-   [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))  
-   [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))  
-   [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))  
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))  
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))  
-   Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs  
-   [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
  
**Download**
  
[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)
  
**Benachrichtigung über Neuerungen**
  
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10)"><img src="images/Dd443721.pageLeft(de-de,TechNet.10).gif" /></a> 18 von 19 <a href="https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10)"><img src="images/Dd443721.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>  
</tbody>  
</table>
