---
TOCTitle: 'Anhang B: Testen des Sicherheitshandbuchs für Windows XP'
Title: 'Anhang B: Testen des Sicherheitshandbuchs für Windows XP'
ms:assetid: '09c716f4-b167-49ec-8122-93e1b8c5f456'
ms:contentKeyID: 20072360
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc163067(v=TechNet.10)'
---

Windows XP-Sicherheitshandbuch
==============================

### Anhang B: Testen des Sicherheitshandbuchs für Windows XP

Aktualisiert: 20.10.2005

##### Auf dieser Seite

[](#edaa)[Einführung](#edaa)  
[](#ecaa)[Testumgebung](#ecaa)  
[](#ebaa)[Testmethoden](#ebaa)  
[](#eaaa)[Zusammenfassung](#eaaa)

### Einführung

Das *Windows* *XP-Sicherheitshandbuch* soll bewährte und wiederholbare Anleitungen für die Konfiguration bereitstellen, um Computer mit Microsoft® Windows® XP Professional mit Service Pack 2 (SP2) in verschiedenen Umgebungen abzusichern.

Das *Windows* *XP-Sicherheitshandbuch* wurde in einer Testumgebung geprüft, um sicherzustellen, dass die Anleitung wie erwartet funktioniert. Die Dokumentation und alle empfohlenen Verfahren wurden vom *Windows* *XP-Sicherheitshandbuch*-Testteam auf Konsistenz geprüft. Anhand von Tests wurde die Funktionalität überprüft. Außerdem sollte den Benutzern der Anleitung geholfen werden, die Anzahl der Ressourcen zu verringern, die zum Erstellen und Testen ihrer eigenen Implementierungen der Lösung erforderlich sind.

#### Umfang

Das *Windows* *XP-Sicherheitshandbuch* wurde in einer Testumgebung für zwei verschiedene Sicherheitsumgebungen geprüft, eine Unternehmensclient- und eine Hochsicherheitsumgebung. Diese Umgebungen sind in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, beschrieben. Die Tests wurden auf der Grundlage von Kriterien durchgeführt, die in dem folgenden Abschnitt, „Ziele“, beschrieben sind.

Eine Bewertung von Sicherheitsanfälligkeiten der Testumgebung, die zur Absicherung der *Windows* *XP-Sicherheitshandbuch*-Lösung verwendet wurde, konnte von den Testteams nicht vorgenommen werden. Die Simulation von Eindringversuchen wurde von Partnern durchgeführt.

#### Ziele

Das *Windows* *XP-Sicherheitshandbuch*-Testteam orientierte sich an den folgenden Testzielen:

-   Sicherstellen, dass die normative Konfiguration und die Richtlinieneinstellungen für Windows XP Professional mit SP2 korrekt und wie erwartet in einem Windows Server™ 2003-basierten Domänennetzwerk für die zwei verschiedenen Sicherheitsumgebungen zusammenarbeitet.

-   Sicherstellen, dass Windows XP Professional SP2-Clientcomputer die grundlegenden Aufgaben und Anwendungen durchführen können, die in den enthaltenen Testfällen aufgeführt sind.

-   Überprüfen, ob alle Anleitungen in Version 2.1 des *Windows* *XP-Sicherheitshandbuchs* klar, vollständig und inhaltlich korrekt sind.

-   Überprüfen, ob die Sicherheitsvorlagen wie erwartet auf dem Windows XP Professional SP2-Clientbetriebssystem funktionieren.

-   Überprüfen, ob die administrativen Vorlagen und die Empfehlungen für die Richtlinie für Softwareeinschränkungen wie erwartet auf dem Windows XP Professional SP2-Clientbetriebssystem funktionieren.

Außerdem soll die Anleitung wiederholbar sein und zuverlässig von einem Microsoft Certified Systems Engineer (MSCE) mit zwei Jahren Erfahrung verwendet werden können.

[](#mainsection)[Zum Seitenanfang](#mainsection)

### Testumgebung

Die Testumgebung setzte sich zusammen aus einem Windows Server 2003 SP1 Active Directory®-Verzeichnisdienst, aus Computern für Infrastrukturserverrollen, die Domänencontroller, DNS- und DHCP-Dienste bereitstellten sowie aus weiteren Computern für Anwendungsserverrollen, die Datei-, Druck-, Web-, CA- und Microsoft Exchange 2003 E-Mail-Dienste bereitstellten. Auf den Desktop- und Laptopclientcomputern in der Domäne wurde Windows XP Professional mit SP2 ausgeführt.

Das Netzwerk enthielt außerdem zwei Clientcomputer, auf denen Windows XP Professional mit SP2 im Arbeitsgruppenmodus ausgeführt wurde, um eigenständige Sicherheitsvorlagen zu prüfen. Laptopcomputer im Domänennetzwerk wurden wiederverwendet, um eigenständige Sicherheitsvorlagen für Laptops zu prüfen. In der folgenden Abbildung ist das Testnetzwerk dargestellt.

![](images/Cc163067.SGFG0B01(de-de,TechNet.10).jpg)

**Abbildung B.1: Das Netzwerk, mit dem das Windows XP-Sicherheitshandbuch im Domänen- sowie im eigenständigen Modus geprüft wurde**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163067.sgfg0b01_big(de-de,technet.10).jpg)  
Das Netzwerk in der folgenden Abbildung wurde entwickelt, um die abwärtskompatiblen Vorlagen zu prüfen, die in diesem Handbuch enthalten sind.

![](images/Cc163067.SGFG0B02(de-de,TechNet.10).jpg)

**Abbildung B.2: Das Netzwerk, mit dem die abwärtskompatiblen Sicherheitsvorlagen geprüft wurden, die in diesem Handbuch enthalten sind**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/cc163067.sgfg0b02_big(de-de,technet.10).jpg)  
[](#mainsection)[Zum Seitenanfang](#mainsection)

### Testmethoden

In diesem Abschnitt werden die Vorgehensweisen beschrieben, die beim Testen des *Windows* *XP-Sicherheitshandbuchs* befolgt wurden.

Das Testteam hat ein Labor mit den Netzwerken eingerichtet, die im vorherigen Abschnitt dargestellt sind. Das Testteam hat einen schnellen Testdurchlauf zur Prüfung des Konzepts und anschließend zwei umfassendere Textzyklen durchgeführt. Bei jedem Durchlauf strebte das Team danach, die Lösung zu stabilisieren.

Ein Testzyklus wurde als Sequenz der zwei folgenden inkrementellen Aufbauzyklen definiert:

1.  Manuelle Computerkonfigurationsphase

2.  Konfigurationshase der Gruppenrichtlinie/lokalen Richtlinie

Die Einzelheiten jeder Phase sind im Abschnitt „Phasen in einem Testdurchlauf“ dargelegt. Im Abschnitt „Testvorbereitungsphase“ werden jene Schritte beschrieben, mit deren Hilfe sichergestellt wurde, dass die Testumgebung frei von jeglichen Problemen war, die zu einer Missdeutung der eigentlichen Testergebnisse hätten führen könnten, nachdem die beiden Umgebungsszenarien durch die zwei inkrementellen Aufbauphasen abgesichert worden waren.

In jedem Testdurchlauf wurden verschiedene Sätze von Testfällen durchgeführt. Diese Tests sind im Abschnitt „Testarten“ im weiteren Verlauf dieses Anhangs erklärt.

#### Phasen in einem Testdurchlauf

Diese Lösung wurde in den Phasen getestet, die in den folgenden Unterabschnitten beschrieben sind. Alle kritischen Zustände, die in einer Phase festgestellt wurden, wurden als Bugs berichtet und korrigiert, bevor das Testteam mit der nächsten inkrementellen Phase fortfuhr. Durch diese Methode wurde die rasche Korrektur kritischer Zustände sichergestellt. Außerdem wurde der Bedarf an Ressourcen minimiert, die erforderlich wären, um Probleme in späteren Phasen zu debuggen.

##### Testvorbereitungsphase

In dieser Phase wurde das grundlegende Netzwerk eingerichtet, auf das die Lösung angewendet wurde. Die Phase bestand aus folgenden Schritten.

**So führen Sie die Testvorbereitungsphase durch**

1.  Vernetzen Sie die Computer wie im Netzwerkdiagramm dargestellt. Installieren Sie die entsprechenden Versionen des Windows-Betriebssystems auf allen Server- und Clientcomputern.

2.  Erstellen und konfigurieren Sie Domänencontroller, Domänen und jede Serverrolle. Fügen Sie die Windows XP Professional mit SP2-Clientcomputer der Domäne hinzu.

3.  Installieren Sie Benutzeranwendungen auf jedem Windows XP Professional mit SP2-Clientcomputer.

4.  Führen Sie grundlegende Überprüfungen durch, um die richtige Konfiguration des Netzwerks sicherzustellen. Stellen Sie sicher, dass die Clientcomputer auf die Dienste zugreifen können, die vom Domänencontroller und den Mitgliedsservern (DNS-, DHCP-, Zertifizierungsstellen-, Datei-, Druck-, Web- und E-Mail-Server) bereitgestellt werden.

5.  Führen Sie die installierten Anwendungen aus, um zu überprüfen, ob Installationsprobleme vorliegen und ob alle Anwendungen ordnungsgemäß ausgeführt werden.

6.  Prüfen Sie das Ereignisprotokoll, um sicherzustellen, dass keine Fehler vorliegen.

7.  Sobald die vorangegangenen Schritte abgeschlossen sind, erstellen Sie von jedem Computer ein Sicherungsabbild. Mit diesen Sicherungsabbildern wird das Netzwerk in den Standardzustand zurückversetzt, bevor ein neuer Testdurchlauf gestartet wird.

##### Manuelle Konfigurationsphase

Diese Phase ist häufig die erste Aufbauphase für die Sicherheit. Sie besteht aus dem folgenden Aufbauverfahren.

**So führen Sie die manuelle Konfigurationsphase durch**

1.  Mit dem Computerverwaltungs-Snap-In der Microsoft Management Console (MMC) werden die vorgeschriebenen Änderungen der Richtlinieneinstellungen durchgeführt, z. B. in Bezug auf das lokale Administratorkonto und das entsprechende Kennwort auf jedem Mitgliedscomputer. Führen Sie zum Absichern der Domänenkonten (Gast- und Administratorkonten) die folgenden Schritte aus:

    1.  Deaktivieren Sie das Gastkonto.

    2.  Stellen Sie sicher, dass das vordefinierte Administratorkonto über ein komplexes Kennwort verfügt und umbenannt wurde und dass seine Standardkontobeschreibung entfernt wurde.

    3.  Berücksichtigen Sie die zusätzlichen Empfehlungen aus dem Handbuch zum Absichern der Domänenkonten.

2.  Führen Sie alle weiteren anwendbaren manuellen Sicherungsverfahren durch, die in den einzelnen Kapiteln des Handbuchs beschrieben sind.

3.  Erstellen Sie manuell eine sichere Datenbank für eigenständige Windows XP-Clientcomputer.

##### Konfigurationshase der Gruppenrichtlinie/lokalen Richtlinie

In dieser Phase werden die Gruppenrichtlinienobjekte (GPOs) auf die Domänen- und Organisationsebenen angewendet. Gruppenrichtlinienobjekte werden anhand der Empfehlungen in Kapitel 2, „Konfigurieren der Domäneninfrastruktur von Active Directory“, auf die verschiedenen Organisationseinheiten angewendet. Bei eigenständigen Windows XP-Clientcomputern wird eine lokale Richtlinie konfiguriert. Diese Phase besteht aus folgenden Schritten.

**So führen Sie die Konfigurationsphase für die Gruppenrichtlinie/lokale Richtlinie durch**

1.  Erstellen Sie die beschriebene Organisationseinheitsstruktur, um die Empfehlungen für die Gruppenrichtlinien zu unterstützen, die in dem Handbuch dargelegt werden.

2.  Verschieben Sie die Windows XP-Desktop- und Laptopclientcomputer in die entsprechenden Organisationseinheiten.

3.  Identifizieren Sie die Domänenbenutzer, und verschieben Sie sie in die entsprechenden Organisationseinheiten, damit Sie die administrativen Vorlagen anwenden können.

4.  Fügen Sie für jede Organisationseinheit eine neue GPO-Verknüpfung hinzu.

    **Hinweis:** Gegebenenfalls müssen Sie die GPO-Verknüpfung in der Prioritätenliste erhöhen, in der bereits standardmäßige GPO-Verknüpfungen vorhanden sind.

5.  Importieren Sie die Sicherheitsvorlage, die mit dem Handbuch geliefert wurde, in das Gruppenrichtlinienobjekt.

6.  Wenden Sie für jedes Umgebungsszenario in den verschiedenen Kapiteln die entsprechende Gruppenrichtlinie auf jede Organisationseinheit an.

#### Details zur Testdurchführung

In den Kapiteln 2 bis 6 des *Windows* *XP-Sicherheitshandbuchs* werden Anweisungen zum Anwenden der Sicherheitsempfehlungen bereitgestellt, und zwar für die Domäne, Windows XP-Desktopcomputer, Windows XP-Laptopcomputer und eigenständige Windows XP-Clientcomputer für die Unternehmensclient- und Hochsicherheitsumgebungen, die im Handbuch definiert sind. Diese Empfehlungen werden von einer Microsoft Excel®-Arbeitsmappe, Sicherheitsvorlagen, administrativen Vorlagen und automatisierten Skripts begleitet. Mit den automatisierten Skripts werden auf den sicheren eigenständigen Clientcomputern Vorlagen in das lokale Gruppenrichtlinienobjekt importiert. In diesem Abschnitt wird erklärt, wie die Empfehlungen implementiert und getestet wurden.

##### Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory

Führen Sie zum Testen dieses Kapitels folgende Verfahren durch.

**So testen Sie das grundlegende Netzwerk**

-   Führen Sie die Testfälle zur grundlegenden Überprüfung durch, um das richtige Funktionieren der Sicherungsabbilderstellung zu gewährleisten. Ein erfolgreicher Abschluss dieser Testfälle bestätigt, dass die Einstiegskriterien erfüllt sind.

**So starten Sie die manuelle Konfigurationsphase**

1.  Synchronisieren Sie die Zeit aller Domänenmitgliedsserver und der Windows XP-Clientcomputer mit dem Domänencontroller.

2.  Deaktivieren Sie das Gastkonto.

3.  Benennen Sie die Administrator- und Gastkonten um.

4.  Ändern Sie das Administratorkennwort.

**So implementieren Sie die Konfiguration der Organisationseinheitsstruktur**

1.  Erstellen Sie in der Domäne corp.woodgrovebank.com eine Organisationseinheit mit dem Namen „Abteilungs-Organisationseinheit“.

2.  Erstellen Sie in der Abteilungs-Organisationseinheit zwei Suborganisationseinheiten. Nennen Sie sie „Organisationseinheit Windows XP“ und „Organisationseinheit Geschützte XP-Benutzer“.

3.  Erstellen Sie in der Organisationseinheit für Windows XP folgende vier Suborganisationseinheiten:

    -   Organisationseinheit EC-Desktop

    -   Organisationseinheit EC-Laptop

    -   Organisationseinheit SSLF-Desktop

    -   Organisationseinheit SSLF-Laptop

4.  Verschieben Sie die Windows XP-Computer, die jeder Sicherheitsumgebung zugewiesen sind, in die jeweiligen Organisationseinheiten.

5.  Verschieben Sie die Domänenbenutzer, die sich bei den Windows XP-Clientcomputern anmelden werden, in die Organisationseinheit für geschützte XP-Benutzer.

6.  Erstellen Sie in dem Objekt corp.woodgrovebank.com ein neues Gruppenrichtlinienobjekt mit dem Namen „Domänenrichtlinie“, und verknüpfen Sie es. Klicken Sie im MMC-Snap-In „Active Directory-Benutzer und -Computer“ auf der Registerkarte „Gruppenrichtlinie“ des Domänenobjekts auf **Nach oben**, um sicherzustellen, dass das neue Gruppenrichtlinienobjekt die höchste Priorität erhält. Importieren Sie anschließend die entsprechende Sicherheitsvorlage (Hochsicher-Domäne.inf oder Unternehmensclient-Domäne.inf) in das Gruppenrichtlinienobjekt.

7.  Führen Sie auf dem Domänencontroller den Befehl **gpupdate /force** aus, um die neuesten Gruppenrichtlinieneinstellungen herunterzuladen.

##### Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients

In diesem Kapitel werden die primären Einstellungen beschrieben, die in einer Windows Server 2003-Domäne durch Gruppenrichtlinien konfiguriert werden. Es werden Richtlinieneinstellungen für die beiden definierten Sicherheitsumgebungen empfohlen, mit denen die Sicherheit von Desktops und Laptops mit Windows XP mit SP2 gewährleistet werden kann.

**So konfigurieren Sie die Sicherheitsvorlageneinstellungen**

1.  Führen Sie die grundlegenden Bereitstellungsprüfungen durch, um zu überprüfen, ob sich alle Empfehlungen im Handbuch für Ihre Umgebung eignen. Überprüfen Sie die empfohlenen Richtlinieneinstellungen. Ändern Sie die Einstellungen in den Sicherheitsvorlagen nach Bedarf, bevor Sie mit der Bereitstellung fortfahren.

2.  Verknüpfen Sie neue Gruppenrichtlinienobjekte mit jeder der beiden Desktop-Organisationseinheiten. Importieren Sie für die Unternehmensclientumgebung die Sicherheitsvorlage „Unternehmensclient - Desktop.inf“ in das Gruppenrichtlinienobjekt. Importieren Sie für die Hochsicherheitsumgebung die Sicherheitsvorlage „Hochsicher - Desktop.inf“ in das Gruppenrichtlinienobjekt.

3.  Verknüpfen Sie neue Gruppenrichtlinienobjekte mit jeder der beiden Laptop-Organisationseinheiten. Importieren Sie für die Unternehmensclientumgebung die Sicherheitsvorlage „Unternehmensclient - Laptop.inf“ in das Gruppenrichtlinienobjekt. Importieren Sie für die Hochsicherheitsumgebung die Sicherheitsvorlage „Hochsicher - Laptop.inf“ in das Gruppenrichtlinienobjekt.

4.  Melden Sie sich bei einem Windows XP-Clientcomputer an und führen Sie den Befehl **gpupdate /force** aus. Starten Sie den Computer anschließend neu, um sicherzustellen, dass die neuesten Gruppenrichtlinieneinstellungen heruntergeladen werden.

5.  Führen Sie die Prüfungen durch, die im weiteren Verlauf dieses Dokuments aufgeführt sind.

##### Kapitel 4: Administrative Vorlagen für Windows XP

In diesem Kapitel wird beschrieben, wie unter Verwendung von administrativen Vorlagen zusätzliche Richtlinieneinstellungen auf Computern mit Microsoft Windows XP mit SP2 konfiguriert und angewendet werden.

**So konfigurieren Sie die Einstellungen der administrativen Vorlagen**

1.  Führen Sie die grundlegenden Bereitstellungsprüfungen durch, um zu überprüfen, ob sich alle Empfehlungen im Handbuch für Ihre Umgebung eignen. Überprüfen Sie die empfohlenen Richtlinieneinstellungen. Ändern Sie die Einstellungen in den administrativen Vorlagen nach Bedarf, bevor Sie mit der Bereitstellung fortfahren.

2.  Erstellen Sie vier neue Gruppenrichtlinienobjekte, eines für jeden der vier Typen von Windows XP-Clientcomputern. Da die Richtlinieneinstellungen für Desktops und Laptops voneinander abweichen, wird vorgeschlagen, separate Gruppenrichtlinienobjekte zu erstellen.

    -  Richtlinie administrativer Vorlagen für Unternehmensclient-Desktop

    -  Richtlinie administrativer Vorlagen für Unternehmensclient-Laptop

    -  Richtlinie administrativer Vorlagen für Hochsicherheits-Desktop

    -  Richtlinie administrativer Vorlagen für Hochsicherheits-Laptop

3.  Konfigurieren Sie in den administrativen Vorlagen die Computerkonfigurationseinstellungen und Benutzerkonfigurationseinstellungen für jedes der Gruppenrichtlinienobjekte gemäß der Anleitung in Kapitel 4, „Administrative Vorlagen für Windows XP“.

4.  Verknüpfen Sie die Gruppenrichtlinienobjekte mit ihren jeweiligen Organisationseinheiten.

5.  Melden Sie sich bei einem Windows XP-Clientcomputer an, und führen Sie den Befehl **gpupdate /force** aus. Starten Sie den Computer anschließend neu, um sicherzustellen, dass die neuesten Gruppenrichtlinieneinstellungen heruntergeladen werden.

6.  Führen Sie die Prüfungen durch, die im weiteren Verlauf dieses Anhangs aufgeführt sind.

##### Kapitel 5: Schützen eigenständiger Windows XP-Clients

In diesem Kapitel werden die primären Richtlinieneinstellungen beschrieben, die durch die Richtlinie für lokale Computer festgelegt werden. Durch die genannten Einstellungswerte wird in der Organisation die Sicherheit der eigenständigen Desktops und Laptops mit Windows XP mit SP2 gewährleistet.

**So konfigurieren Sie Sicherheitseinstellungen auf eigenständigen Windows XP-Clients**

1.  Führen Sie die grundlegenden Bereitstellungsprüfungen durch, um zu bestätigen, dass sich alle Empfehlungen im Handbuch für Ihre Umgebung eignen.

2.  Verwenden Sie zum Erstellen einer Sicherheitsdatenbank das MMC Snap-In für Sicherheitskonfiguration und -analyse. Mithilfe dieser Datenbank wird in die lokale Richtlinie geschrieben. In Kapitel 5, „Schützen eigenständiger Windows XP-Clients“, werden detaillierte Anweisungen zur Verfügung gestellt.

3.  Verwenden Sie das MMC Snap-In für Sicherheitskonfiguration und -analyse, um die Richtlinieneinstellungen anzuwenden, die in den eigenständigen Sicherheitsvorlagendateien enthalten sind. In Kapitel 5, „Schützen eigenständiger Windows XP-Clients“, werden detaillierte Anweisungen zur Verfügung gestellt. Das Snap-In für Sicherheitskonfiguration und -analyse muss verwendet werden, denn Richtlinieneinstellungen für Systemdienste können nicht mit dem Snap-In für die Richtlinie für lokale Computer angewendet werden.

4.  Führen Sie zum Importieren der Sicherheitsvorlagen das entsprechende automatisierte Skript aus (im Lieferumfang dieses Handbuchs enthalten).

5.  Führen Sie die Prüfungen durch, die im weiteren Verlauf dieses Anhangs aufgeführt sind.

##### Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients

Mithilfe dieses Kapitels können Administratoren die in ihrer Domäne ausgeführte Software identifizieren und kontrollieren. Bei dem Tool, mit dem diese Kontrolle erreicht wird, handelt es sich um einen auf Richtlinien beruhenden Mechanismus, der „Richtlinie für Softwareeinschränkungen“ genannt wird.

**So konfigurieren Sie die Richtlinie für Softwareeinschränkungen**

1.  Führen Sie die grundlegenden Bereitstellungsprüfungen durch, um zu bestätigen, dass sich alle Empfehlungen im Handbuch für Ihre Umgebung eignen.

2.  Suchen Sie nach der Organisationseinheit, die für die Windows XP-Desktops und -Laptops erstellt wurde. Bei eigenständigen Clientcomputern befinden sich die Richtlinieneinstellungen in der lokalen Sicherheitsrichtlinie. Erstellen Sie ein neues Gruppenrichtlinienobjekt für die Organisationseinheit für Windows XP. Dieses neue Gruppenrichtlinienobjekt wird nur für die Richtlinie für Softwareeinschränkungen verwendet.

3.  Konfigurieren Sie die Richtlinie für Softwareeinschränkungen wie folgt:

    a.  Erstellen Sie eine Standardrichtlinie für Softwareeinschränkungen.

    b.  Richten Sie die Pfadregeln ein.

    c.  Legen Sie die Richtlinienoptionen gemäß den bereitgestellten Verordnungen fest, z. B. Erzwingung, designierte Dateitypen und vertrauenswürdige Herausgeber.

4.  Überprüfen Sie die Richtlinieneinstellungen, und setzen Sie dann die Standardrichtlinieneinstellung auf **Nicht erlaubt** zurück.

5.  Melden Sie sich bei einem Windows XP-Clientcomputer an und führen Sie den Befehl **gpupdate /force** aus. Starten Sie den Computer anschließend neu, um sicherzustellen, dass die neuesten Gruppenrichtlinieneinstellungen heruntergeladen werden.

6.  Führen Sie die Prüfungen durch, die im weiteren Verlauf dieses Anhangs aufgeführt sind.

##### Überprüfen des Herunterladens von Gruppenrichtlinien auf dem XP-Client

In den vorangegangenen Abschnitten wurden Gruppenrichtlinienobjekte auf Organisationseinheiten angewendet, welche dann die Gruppenrichtlinienobjekte auf die Computer in den Organisationseinheiten angewendet haben. Führen Sie die folgenden Schritte durch, um das erfolgreiche Herunterladen von Gruppenrichtlinien vom Domänencontroller auf einen Windows XP-Clientcomputer zu bestätigen. Es wird davon ausgegangen, dass der Clientcomputer neu gestartet wurde, nachdem das Gruppenrichtlinienobjekt mit der Organisationseinheit verknüpft wurde.

**So überprüfen Sie das Herunterladen von Gruppenrichtlinien auf einen Windows XP-Clientcomputer**

1.  Melden Sie sich beim Windows XP-Clientcomputer an.

2.  Klicken Sie auf **Start** und auf **Ausführen**, geben Sie **rsop.msc** ein, und drücken Sie die Eingabetaste.

3.  Erweitern Sie in der Konsole **Richtlinienergebnissatz** den **Konsolenstamm**, und wechseln Sie zu **Computerkonfiguration**.

4.  Klicken Sie mit der rechten Maustaste auf **Computerkonfiguration**, und klicken Sie auf **Eigenschaften**.

    Im Fenster **Eigenschaften von Computerkonfiguration** wird die Liste der Gruppenrichtlinienobjekte angezeigt. Das auf die Organisationseinheit angewendete Gruppenrichtlinienobjekt sollte in der Liste verfügbar sein, und es sollten keine Fehler damit verbunden sein.

5.  Überprüfen Sie die Richtlinieneinstellungen für die administrativen Vorlagen.

    In dem entsprechenden Ordner **Administrative Vorlagen** unter **Computerkonfiguration** bzw. **Benutzerkonfiguration** sollten nur die Einstellungen zu sehen sein, die im Gruppenrichtlinienobjekt „Administrative Vorlage“ konfiguriert sind.

#### Testtypen

Das Testteam hat während der Testphasen die folgenden Arten von Tests durchgeführt, um sicherzustellen, dass die gesicherten Windows XP-Clientcomputer in der Lage sind, grundlegende Aufgaben ohne bedeutenden Verlust der Funktionalität durchführen zu können. Sie können die Excel-Arbeitsmappe „Windows XP Security Guide Test Cases.xls“ zu Rate ziehen. Diese befindet sich im Ordner **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\Testtools**, der im Download für dieses Handbuch enthalten sind. Diese Arbeitsmappendatei enthält die vollständige Liste der Testfälle, die für domänenbasierte XP-Clientcomputer und eigenständige XP-Clientcomputer durchgeführt wurden, sowie Details wie z. B. Testszenarien, Ausführungsschritte und erwartete Ergebnisse.

##### Anwendungstests

Bei diesen Tests wird geprüft, ob Benutzeranwendungen, die auf den Windows XP-Clientcomputern installiert sind (wie z. B. die Anwendungssuite Office 2003, Windows Media® Player und einige andere), ordnungsgemäß funktionieren. Ausführlichere Informationen zu den Testfällen finden Sie in der Excel-Arbeitsmappe „Windows XP Security Guide Test Cases.xls“, die in diesem Handbuch enthalten ist.

##### Tests mit automatisiertem Skript

Einige der Testfallszenarien wurden in VBScript erstellt. Diese Testfälle befassen sich hauptsächlich mit dem ordnungsgemäßen Funktionieren von Windows XP-Clientcomputern, die netzwerkbasierte Dienste wie z. B. Domänenanmeldung, Kennwortänderung und Druckserverzugriff verwenden. Die VBScript-Dateien für diese Testfälle befinden sich im Ordner **\\Tools und Vorlagen für das Windows XP Sicherheitshandbuch\\Testtools**, die im Download für dieses Handbuch enthalten sind.

##### Grundlegende Überprüfungen

Diese Testfälle sind ein Teil der Anwendungs- und Internettests sowie der Tests mit automatisiertem Skript. Es handelt sich dabei um grundlegende Tests, die eine Reihe verschiedener Szenarien abdecken, wie z. B. die Möglichkeit, auf dem Client installierte Anwendungen auszuführen, das Testen der Client-Server-Kommunikation, die Möglichkeit, auf das Internet zuzugreifen und Patches herunterzuladen sowie Tests, bei denen Fehler auf dem Host überwacht werden. Diese Testfälle werden auch ausgeführt, wenn Sie während der Testvorbereitungsphase eine Baseline für das Netzwerk einrichten.

##### Dokumentationserstellungstests

Anhand dieser Tests wird bestätigt, dass die in der Implementierungsanleitung dokumentierten Aussagen, Verfahren und Funktionen korrekt, eindeutig und vollständig sind. Für diese Tests sind keine separaten Testfälle aufgeführt.

##### Funktionstests

Anhand dieser Tests soll überprüft werden, ob das nach den Hinweisen zum Erstellen aufgebaute System richtig und wie erwartet funktioniert. Mit diesen Tests werden die Funktionalität und der Zustand der Erstellungsverfahren sowie ihre Auswirkungen auf die Desktop- und Laptopclientcomputer überprüft.

##### Internetbasierte Tests

Die Computerbenutzer von heute müssen in der Regel auf das Internet zugreifen. Mithilfe dieser Testfälle wird sichergestellt, dass einige der alltäglichen Funktionen (Besuchen von Websites, Verwenden von Windows Messenger, Herunterladen wichtiger Updates von der Microsoft Update-Website) nicht vom Sperrmodus des Windows XP-Clientcomputers betroffen sind.

#### Erfolgs- und Misserfolgskriterien

Bevor Tests durchgeführt wurden, wurden die folgenden Kriterien festgelegt, um die Fehlervorbeugung und -behebung zu gewährleisten:

-   Alle Testfälle müssen mit den erwarteten Ergebnissen bestanden werden, die in den einzelnen Testfalltabellen beschrieben sind.

-   Ein Testfall wird als bestanden betrachtet, wenn das tatsächliche Ergebnis mit dem erwarteten Ergebnis übereinstimmt, das für den Fall dokumentiert ist. Wenn das tatsächliche Ergebnis nicht mit dem erwarteten Ergebnis übereinstimmt, wird der Testfall als nicht bestanden betrachtet. Es wird ein Bug erstellt und ein Schweregrad zugewiesen.

-   Wenn ein Testfall nicht bestanden wird, wird nicht unbedingt davon ausgegangen, dass die Lösung mangelhaft ist. Fehler könnten z. B. durch eine Missdeutung der Produktdokumentation bzw. durch eine unvollständige oder unpräzise Dokumentation verursacht werden. Jeder Fehler wird analysiert, um seine Ursache zu ergründen. Dabei dienen die tatsächlichen Ergebnisse und die in der Projektdokumentation beschriebenen Ergebnisse als Grundlage. Fehlerinformationen werden auch an die entsprechenden Besitzer der jeweiligen Microsoft-Produkte weitergeleitet.

#### Veröffentlichungskriterien

Das primäre Veröffentlichungskriterium für das *Windows* *XP-Sicherheitshandbuch* stand in Zusammenhang mit dem Schweregrad der Bugs, die noch offen waren. Es wurden jedoch auch andere Probleme erörtert, die nicht durch Bugs erfasst wurden. Die Veröffentlichungskriterien lauten wie folgt:

-   Keine offenen Bugs der Schweregrade 1 und 2.

-   Alle offenen Bugs werden vom Führungsteam behoben, und ihre Auswirkungen sind vollständig bekannt.

-   Lösungshandbücher enthalten keinerlei Kommentare und Korrekturzeichen.

-   Die Lösung besteht alle Testfälle in der Testumgebung.

-   Die Inhalte der Lösung enthalten keine Widersprüche.

#### Bug-Klassifizierung

Die Schweregradskala für Bugs wird in der nachstehenden Tabelle beschrieben. Die Skala reicht von 1 bis 4, wobei 1 der höchste und 4 der niedrigste Schweregrad ist.

**Tabelle B.1: Schweregradklassifizierung für Bugs**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schweregrad</th>
<th style="border:1px solid black;" >Häufigste Typen</th>
<th style="border:1px solid black;" >Erforderliche Bedingungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">– Bug blockierte Aufbau oder weitere Tests.<br />
– Bug hat unerwarteten Benutzerzugriff verursacht.<br />
– Die in der Dokumentation definierten Schritte waren unklar.<br />
– Ergebnisse oder Verhalten einer Funktion oder eines Prozesses widersprechen den erwarteten Ergebnissen (die in der funktionalen Spezifikation dokumentiert sind).<br />
– Grobe Ungleichheit zwischen den Sicherheitsvorlagendateien und der funktionalen Spezifikation.</td>
<td style="border:1px solid black;">– Lösung hat nicht funktioniert.<br />
– Benutzer konnte bedeutende Teile des Systems nicht einmal ansatzweise verwenden.<br />
– Benutzer hatte Zugriffsberechtigungen, die nicht zulässig sein sollten.<br />
– Benutzerzugriff auf bestimmte Server war blockiert, hätte aber möglich sein müssen.<br />
– Erwartete Ergebnisse wurden nicht erreicht.<br />
– Die Tests können erst fortgesetzt werden, wenn die Bugs behoben sind.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">2</td>
<td style="border:1px solid black;">– Im Handbuch definierte Schritte sind unklar.<br />
– Dokumentierte Funktionalität fehlt (Test wurde in diesem Fall blockiert).<br />
– Dokumentation fehlt oder ist unzureichend.<br />
– Inkonsistenz zwischen Sicherheitsvorlagendateien und Inhalt des Handbuchs, doch die Sicherheitsvorlagendatei ist mit der funktionalen Spezifikation synchron.</td>
<td style="border:1px solid black;">– Benutzer hatte keine einfache Problemumgehung zur Verfügung, um die Situation zu verbessern.<br />
– Benutzer konnte keine einfache Problemumgehung finden.<br />
– Wichtige Geschäftsanforderungen konnten nicht vom System erfüllt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">3</td>
<td style="border:1px solid black;">– Dokumentiertes Formatproblem.<br />
– Geringfügige Fehler und Ungenauigkeiten in der Dokumentation.<br />
– Rechtschreibfehler im Text.</td>
<td style="border:1px solid black;">– Benutzer verfügt über eine einfache Problemumgehung.<br />
– Benutzer kann leicht eine Problemumgehung finden.<br />
– Bug beeinträchtigt Benutzerfreundlichkeit nicht.<br />
– Wichtige Geschäftsanforderungen funktionieren noch.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">4</td>
<td style="border:1px solid black;">– Vorschläge.<br />
– Zukünftige Verbesserungen.</td>
<td style="border:1px solid black;">– Bezieht sich eindeutig nicht auf diese Version.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
Mithilfe dieses Dokuments kann eine Organisation, die das *Windows* *XP-Sicherheitshandbuch* implementiert, die Verfahren und die Schritte verstehen, mit denen die Implementierung der Lösung in einer Testumgebung geprüft wurde. Die Erfahrungen des *Windows* *XP-Sicherheitshandbuch*-Testteams sind in diesem Dokument erfasst. Es beinhaltet Beschreibungen der Testumgebung, der Testtypen, der Veröffentlichungskriterien und der Klassifizierungsdetails für Bugs.
  
Alle vom Testteam durchgeführte Testfälle wurden mit den erwarteten Ergebnissen bestanden. Das Testteam hat bestätigt, dass die erforderliche Funktionalität zur Verfügung stand, nachdem die Empfehlungen des *Windows* *XP-Sicherheitshandbuchs* auf die definierten Umgebungen angewendet worden waren.
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))  
-   [Kapitel 1: Einführung zum Sicherheitshandbuch für Windows XP](https://technet.microsoft.com/de-de/library/4eddb4e4-fd7b-444c-8484-bb8ee220c0e1(v=TechNet.10))  
-   [Kapitel 2: Konfigurieren der Domäneninfrastruktur von Active Directory](https://technet.microsoft.com/de-de/library/620c0004-41a8-4d13-9a61-e6d879f9cc65(v=TechNet.10))  
-   [Kapitel 3: Sicherheitseinstellungen für Windows XP-Clients](https://technet.microsoft.com/de-de/library/bca34b8d-a1ca-42e4-b743-aa3ca12fd8f9(v=TechNet.10))  
-   [Kapitel 4: Administrative Vorlagen für Windows XP](https://technet.microsoft.com/de-de/library/adb79ec2-691f-4a9f-b940-36d2d9807fd7(v=TechNet.10))  
-   [Kapitel 5: Schützen eigenständiger Windows XP-Clients](https://technet.microsoft.com/de-de/library/a134d1cb-2ad1-4549-99c8-2a5e0128f2dc(v=TechNet.10))  
-   [Kapitel 6: Richtlinie für Softwareeinschränkungen auf Windows XP-Clients](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgap06.mspx)  
-   [Kapitel 7: Zusammenfassung](https://technet.microsoft.com/de-de/library/8001f9fb-f330-4ab4-a134-ff756091ea0d(v=TechNet.10))  
-   [Anhang A: Weitere Anleitungen für Windows XP Service Pack 2](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsxp/secwinxp/xpsgapa.mspx)  
-   [Anhang A: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/6b4fdfca-4c2c-47f6-8c92-de33a663ea03(v=TechNet.10))  
-   Anhang B: Testen des Sicherheitshandbuchs für Windows XP  
-   [Danksagungen](https://technet.microsoft.com/de-de/library/7e874ad0-7c5a-4f64-9349-760666ab3e61(v=TechNet.10))
  
##### Download
  
[![](images/Cc163067.icon_exe(de-de,TechNet.10).gif)Windows XP-Sicherheitshandbuch herunterladen (engl.)](http://go.microsoft.com/fwlink/?linkid=14840&clcid=0x409)
  
[](#mainsection)[Zum Seitenanfang](#mainsection)