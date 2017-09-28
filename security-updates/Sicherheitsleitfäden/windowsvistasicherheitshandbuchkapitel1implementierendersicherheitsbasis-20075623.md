---
TOCTitle: 'Windows Vista-Sicherheitshandbuch – Kapitel 1 (Implementieren der Sicherheitsbasis)'
Title: 'Windows Vista-Sicherheitshandbuch – Kapitel 1 (Implementieren der Sicherheitsbasis)'
ms:assetid: '83b1e449-f399-4511-b3c5-9d868a321ad7'
ms:contentKeyID: 20075623
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443680(v=TechNet.10)'
---

Windows Vista-Sicherheitshandbuch
=================================

### Kapitel 1: Implementieren der Sicherheitsbasis

Veröffentlicht: 08. Nov 2006

Windows Vista™ ist das sicherste Betriebssystem, das Microsoft bisher entwickelt hat. Möglicherweise müssen Sie jedoch bestimmte Änderungen an der Konfiguration vornehmen, um den Netzwerkanforderungen Ihrer Umgebung gerecht zu werden. In diesem Kapitel soll gezeigt werden, dass Sie auf relativ einfache Weise Sicherheitseinstellungen konfigurieren können, um so Clientcomputer abzusichern, die mit dem Standardbetriebssystem ausgeführt werden und über den Active Directory®-Verzeichnisdienst einer Domäne hinzugefügt wurden.

Dieses Kapitel enthält eine Reihe einfacher Verfahren zum Implementieren empfohlener Sicherheitseinstellungen, mit denen die Sicherheit des Betriebssystems in seiner Standardeinstellung noch weiter verbessert wird. Die optimierten Verfahren in diesem Kapitel bieten eine schnelle und effiziente Möglichkeit zum Absichern von Windows Vista–basierten Clientcomputern in Ihrer Umgebung.

Sie können nun das Standardbetriebssystem unter der ausschließlichen Verwendung von Gruppenrichtlinienobjekten absichern. Ältere Vorgehensweisen von Microsoft sahen vor, INF-Dateien mit Sicherheitsvorlagen zu importieren und dann manuell umfassende Änderungen im Abschnitt „Administrative Vorlagen“ verschiedener Gruppenrichtlinienobjekten vorzunehmen. Das Arbeiten mit diesem Dateien und Vorlagen ist nicht länger erforderlich. Die INF-Dateien für Sicherheitsvorlagen werden in diesem Handbuch jedoch weiter aufgeführt, damit Sie sie zum Absichern eigenständiger Clientcomputer verwenden können. Alle empfohlenen Gruppenrichtlinieneinstellungen werden in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“ beschrieben.

Zum Bereitstellen dieser Richtlinien müssen Sie folgende Aktionen ausführen:

-   Erstellen einer Organisationseinheitsstruktur (Organisational Unit, OU) für Ihre Umgebung

-   Ausführen des mit diesem Handbuch gelieferten Skripts „GPOAccelerator.wsf“

-   Verknüpfen und Verwalten der Gruppenrichtlinienobjekte mithilfe der Gruppenrichtlinien-Verwaltungskonsole (Group Policy Management Console, GPMC)

![](images/Dd443680.warning(de-de,TechNet.10).gif)**Achtung:**

Sie müssen die Organisations- und Gruppenrichtlinienentwürfe unbedingt gründlich testen, bevor Sie sie in einer Produktionsumgebung bereitstellen. Im Abschnitt „Implementieren der Sicherheitsrichtlinien“ in diesem Kapitel finden Sie Anweisungen zum Erstellen und Bereitstellen der Organisationseinheitsstruktur und Sicherheitsgruppenrichtlinienobjekte während der Test- und Produktionsphase der Implementierung.

Die mit diesem Handbuch bereitgestellten Baseline-Gruppenrichtlinienobjekte bieten eine Kombination aus getesteten Einstellungen, die die Sicherheit für Clientcomputer unter Windows Vista in den beiden folgenden Umgebungen erhöhen:

-   **Unternehmensclient (EC)**

-   **Hochsicherheit (SSLF)**

In diesem Kapitel wird die Unternehmensclient-Umgebung behandelt. Eine Erläuterung der SSLF-Umgebung und des Verfahrens zum Anwenden der entsprechenden Sicherheitseinstellungen finden Sie in Kapitel 5, „Hochsicherheit (SSLF)“.

##### Auf dieser Seite

[](#edaa)[Unternehmensclient-Umgebung](#edaa)
[](#ecaa)[Sicherheitsentwurf und Implementierung](#ecaa)
[](#ebaa)[Das GPOAccelerator-Tool](#ebaa)
[](#eaaa)[Weitere Informationen](#eaaa)

### Unternehmensclient-Umgebung

Die in diesem Kapitel behandelte Unternehmensclient-Umgebung (Enterprise Client, EC) besteht aus einer Domäne, die den Active Directory®-Verzeichnisdienst verwendet und in der Computer unter Microsoft® Windows Server® 2003 R2 oder Windows Server 2003 mit Service Pack 1 (SP1) und Active Directory Clientcomputer verwalten, die unter Windows Vista oder Windows XP® ausgeführt werden. Die Clientcomputer werden in dieser Umgebung mithilfe von Gruppenrichtlinien verwaltet, die auf Standorte, Domänen und Organisationseinheiten angewendet werden. Gruppenrichtlinien stellen eine zentralisierte Infrastruktur in Active Directory bereit, durch die eine verzeichnisbasierte Änderungs- und Konfigurationsverwaltung von Benutzer- und Computereinstellungen ermöglicht wird, einschließlich von Sicherheits- und Benutzerdaten.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Sicherheitsentwurf und Implementierung

Der in diesem Kapitel empfohlene Sicherheitsentwurf ist der Ausgangspunkt für die Szenarios in diesem Handbuch sowie für die Lösungsvorschläge zu den Szenarios. In den folgenden Abschnitten in diesem Kapitel wird der grundlegende Sicherheitsentwurf dieses Handbuchs erläutert, und es werden Verfahren zum Testen und Implementieren des Entwurfs für Computer unter Windows Vista vorgestellt:

-   **Entwurf der Organisationseinheiten für Sicherheitsrichtlinien**

-   **Entwurf der Gruppenrichtlinienobjekte für Sicherheitsrichtlinien**

-   **Implementieren der Sicherheitsrichtlinien**

#### Entwurf der Organisationseinheiten für Sicherheitsrichtlinien

Bei einer Organisationseinheit handelt es sich um einen Container innerhalb einer Domäne, in der Active Directory verwendet wird. Eine Organisationseinheit kann Benutzer, Gruppen, Computer und andere Organisationseinheiten enthalten. Wenn eine Organisationseinheit andere Organisationseinheiten beinhaltet, handelt es sich um eine übergeordnete Organisationseinheit. Eine Organisationseinheit innerhalb einer übergeordneten Organisationseinheit wird als untergeordnete Organisationseinheit bezeichnet.

Sie können ein Gruppenrichtlinienobjekt mit einer Organisationseinheit verknüpfen. Hierdurch werden die Einstellungen des Gruppenrichtlinienobjekts auf die Benutzer und Gruppen in dieser Organisationseinheit sowie in ihren untergeordneten Organisationseinheiten angewendet. Für Verwaltungszwecke können Sie Administratorrechte an die einzelnen Organisationseinheiten delegieren.

Organisationseinheiten erleichtern das Gruppieren von Benutzern und Computern und können zur effektiven Segmentierung administrativer Bereiche verwendet werden. Microsoft empfiehlt Unternehmen, Benutzer und Computer getrennten Organisationseinheiten zuzuordnen, da einige Einstellungen nur für Benutzer gelten und andere nur für Computer.

Mithilfe des Assistenten zum Erstellen neuer Delegierungen, der Bestandteil des Snap-Ins „Active Directory-Benutzer und -Computer“ der Microsoft Management Console (MMC) ist, kann die Steuerung einer Gruppe oder einzelner Organisationseinheiten delegiert werden. Verweise auf Dokumentation zum Thema Delegieren von Autorität finden Sie im Abschnitt „Weitere Informationen“ am Ende dieses Kapitels.

Eine der Hauptaufgaben eines Organisationseinheitsentwurfs für eine Umgebung ist das Bereitstellen einer Grundlage für eine nahtlose Implementierung von Gruppenrichtlinien, die auf alle Clientcomputer in Active Directory angewendet wird. So wird sichergestellt, dass die Clientcomputer die Sicherheitsstandards Ihres Unternehmens erfüllen. Der Organisationseinheitsentwurf muss außerdem eine geeignete Struktur für die verschiedenen Sicherheitseinstellungen für bestimmte Typen von Benutzern in einem Unternehmen bereitstellen. Entwickler müssen beispielsweise in einer Weise auf ihre Computer zugreifen können, die für normale Benutzer nicht erforderlich ist. Auch können für Laptopbenutzer andere Sicherheitsstandards gelten als für Desktopbenutzer. Die folgende Abbildung enthält ein Beispiel einer einfachen Organisationseinheitsstruktur, das für die Erläuterung von Gruppenrichtlinien in diesem Kapitel ausreichend ist. Diese Organisationseinheitsstruktur unterscheidet sich möglicherweise von den Anforderungen in der Umgebung Ihres Unternehmens.

![](images/Dd443680.VSGF0101(de-de,TechNet.10).gif)

**Abbildung 1.1 Beispielstruktur für Organisationseinheiten für Computer unter Windows Vista**

##### Organisationseinheit „Abteilung“

Da es innerhalb einer Organisation oft unterschiedliche Sicherheitsanforderungen gibt, ist es sinnvoll, in Ihrer Umgebung Organisationseinheiten für Abteilungen zu erstellen. Mithilfe dieser Organisationseinheiten können Sie Sicherheitseinstellungen über ein Gruppenrichtlinienobjekt auf Computer und Benutzer in den jeweiligen Abteilungsorganisationseinheiten anwenden.

##### Organisationseinheit „Windows Vista-Benutzer“

Diese Organisationseinheit enthält die Benutzerkonten für die EC-Umgebung. Die auf diese Organisationseinheit angewendeten Einstellungen werden detailliert in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“, beschrieben.

##### Organisationseinheit „Windows Vista-Computer“

Diese Organisationseinheit enthält untergeordnete Organisationseinheiten für alle Typen von Clientcomputern mit Windows Vista in der EC-Umgebung. Dieses Handbuch beschäftigt sich schwerpunktmäßig mit Anleitungen zur Sicherheit für Desktop- und Laptop-Computer. Für dieses Handbuch wurden daher die folgenden Computer-Organisationseinheiten erstellt:

-   **Organisationseinheit „Desktop“**. In dieser Organisationseinheit sind Desktopcomputer enthalten, die permanent mit dem Netzwerk verbunden sind. Die auf diese Organisationseinheit angewendeten Einstellungen werden detailliert in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“, beschrieben.

-   **Organisationseinheit „Laptop“**. In dieser Organisationseinheit sind Laptopcomputer mobiler Benutzer enthalten, die nicht permanent mit dem Netzwerk verbunden sind. In Anhang A finden Sie außerdem Einzelheiten zu den Einstellungen für diese Organisationseinheit.

#### Gruppenrichtlinienobjekt-Entwurf für Sicherheitsrichtlinien

Ein Gruppenrichtlinienobjekt ist eine Sammlung von Gruppenrichtlinieneinstellungen, bei denen es sich im Wesentlichen um die vom Snap-In für Gruppenrichtlinien erstellten Dateien handelt. Diese Einstellungen werden auf Domänenebene gespeichert und betreffen Benutzer und Computer in Standorten, Domänen und Organisationseinheiten.

Mithilfe von Gruppenrichtlinienobjekten können Sie sicherstellen, dass bestimmte Richtlinieneinstellungen, Benutzereinstellungen, Benutzerberechtigungen und Computerverhalten für alle Clientcomputer oder Benutzer in einer Organisationseinheit gelten. Das Verwenden von Gruppenrichtlinien anstelle einer manuellen Konfiguration vereinfacht das Verwalten und Aktualisieren von Änderungen für eine große Anzahl von Computern und Benutzern. Die manuelle Konfiguration ist nicht nur ineffizient, da ein Techniker jeden einzelnen Computer vor Ort konfigurieren muss, sondern potenziell auch nicht wirkungsvoll. Der Hauptgrund hierfür liegt darin, dass bei einer Abweichung der Richtlinieneinstellungen in domänenbasierten Gruppenrichtlinienobjekten von den lokalen Einstellungen die domänenbasierten Einstellungen für Gruppenrichtlinienobjekte die lokal angewendeten Richtlinieneinstellungen überschreiben.

![](images/Dd443680.VSGF0102(de-de,TechNet.10).gif)

**Abbildung 1.2 Rangfolge der Gruppenrichtlinienobjekte**

Die Abbildung oben zeigt die Rangfolge, mit der Gruppenrichtlinienobjekte auf einen Computer angewendet werden, der Mitglied der untergeordneten Organisationseinheit ist. Die Darstellung erfolgt von der niedrigsten Priorität (1) zur höchsten (5). Gruppenrichtlinien werden zuerst aus der lokalen Sicherheitsrichtlinie der jeweiligen Clientcomputer unter Windows Vista angewendet. Nach dem Anwenden der lokalen Sicherheitsrichtlinie werden Gruppenrichtlinienobjekte auf Standortebene und dann auf Domänenebene angewendet.

Auf Windows Vista-Clients, die auf mehreren Schichten von Organisationseinheiten verschachtelt sind, werden Gruppenrichtlinienobjekte in absteigender Reihenfolge von der übergeordneten zur niedrigsten untergeordneten Ebene der Organisationseinheiten in der Hierarchie angewendet. Das letzte Gruppenrichtlinienobjekt wird aus der Organisationseinheit angewendet, die den Clientcomputer enthält. Diese Reihenfolge der Verarbeitung von Gruppenrichtlinienobjekten – lokale Sicherheitsrichtlinie, Standort, Domäne, übergeordnete Organisationseinheit und untergeordnete Organisationseinheit – ist bedeutsam, weil Gruppenrichtlinienobjekte, die später im Prozess angewendet werden, zu einem früheren Zeitpunkt angewendete überschreiben. Gruppenrichtlinienobjekte für Benutzer werden in gleicher Weise angewendet.

Beim Entwerfen von Gruppenrichtlinien sollten Sie die folgenden Punkte berücksichtigen:

-   Der Administrator muss die Reihenfolge festlegen, in der mehrere Gruppenrichtlinienobjekte mit einer Organisationseinheit verknüpft werden. Andernfalls werden die Gruppenrichtlinien standardmäßig in der Reihenfolge angewendet, in der sie mit der Organisationseinheit verknüpft wurden. Wenn in mehreren Richtlinien die gleiche Einstellung festgelegt wird, hat die Richtlinie Vorrang, die sich in der Richtlinienliste für den Container am weitesten oben befindet.

-   Ein Gruppenrichtlinienobjekt kann mithilfe der Option **Erzwungen** konfiguriert werden. Wenn Sie diese Option auswählen, können die in diesem Gruppenrichtlinienobjekt festgelegten Einstellungen nicht von anderen Gruppenrichtlinienobjekten außer Kraft gesetzt werden.

    **Hinweis**:   In Windows 2000 trägt die Option **Erzwungen** die Bezeichnung **Kein Vorrang**.

-   Die Option **Richtlinienvererbung deaktivieren** kann für Active Directory, einen Standort, eine Domäne oder eine Organisationseinheit festgelegt werden. Durch diese Option werden die Einstellungen der Gruppenrichtlinienobjekte für in der Active Directory-Hierarchie höher stehende Gruppenrichtlinienobjekte gesperrt, sofern für diese nicht die Option **Erzwungen** ausgewählt wurde. Das bedeutet, dass die Option **Erzwungen** Vorrang vor der Option **Richtlinienvererbung deaktivieren** hat.

-   Gruppenrichtlinieneinstellungen werden auf Benutzer und Computer entsprechend ihrem Speicherort in Active Directory angewendet. In einigen Fällen kann es notwendig sein, Richtlinien auf ein Benutzerobjekt auf Grundlage des Speicherortes des Computerobjekts anstelle des Speicherortes des Benutzerobjekts anzuwenden. Mithilfe der Loopback-Funktion für Gruppenrichtlinien kann der Administrator Gruppenrichtlinieneinstellungen für Benutzer auf Grundlage des Computers anwenden, an dem der Benutzer angemeldet ist. Im Artikel [Loopbackverarbeitung von Gruppenrichtlinien](http://support.microsoft.com/default.aspx?id=231287) finden Sie weitere Informationen zu dieser Option.

##### Empfohlene Gruppenrichtlinienobjekte

Zum Implementieren des oben beschriebenen Entwurfs für Organisationseinheiten werden mindestens vier Gruppenrichtlinienobjekte benötigt:

-   Eine Richtlinie für die Domäne

-   Eine Richtlinie für die Organisationseinheit „Windows Vista-Benutzer“

-   Eine Richtlinie für die Organisationseinheit „Desktop“

-   Eine Richtlinie für die Organisationseinheit „Laptop“

In der folgenden Abbildung wird die vorläufige Organisationseinheitsstruktur erweitert, um die Verknüpfung zwischen diesen Gruppenrichtlinienobjekten und dem Organisationseinheitsentwurf darzustellen.

![](images/Dd443680.VSGF0103(de-de,TechNet.10).gif)

**Abbildung 1.3 Beispiel-Organisationeneinheitsstruktur und Verknüpfungen von Gruppenrichtlinienobjekten für Computer unter Windows Vista**

[Bild in voller Größe anzeigen](https://technet.microsoft.com/de-de/dd443680.vsgf0103_big(de-de,technet.10).gif)
Im Beispiel in Abbildung 1.3 sind Laptopcomputer Mitglied der Organisationseinheit „Laptop“. Zuerst wird die lokale Sicherheitsrichtlinie auf die Laptopcomputer angewendet. Da es in diesem Beispiel nur einen Standort gibt, wird auf Standortebene kein Gruppenrichtlinienobjekt angewendet. Folglich wird als nächstes das Gruppenrichtlinienobjekt der Domäne angewendet. Zum Schluss wird das Gruppenrichtlinienobjekt für Laptops angewendet.

**Hinweis**:   Die Richtlinie **Desktoprichtlinie** wird nicht auf Laptops angewendet, da sie mit keiner Organisationseinheit in der Hierarchie verknüpft ist, die die Organisationseinheit „Laptop“ enthält.

Betrachten Sie als Beispiel für die Vorrangigkeit ein Szenario, in dem die Richtlinieneinstellung **Anmelden über Terminaldienste zulassen** für die folgenden Organisationseinheiten und Benutzergruppen gesetzt wird:

-   Organisationseinheit „Windows Vista-Computer“ – Gruppe **Administratoren**

-   Organisationseinheit „Laptop“ – Gruppen **Remotedesktopbenutzer** und **Administratoren**

In diesem Beispiel kann ein Benutzer, dessen Konto sich in der Gruppe **Remotedesktopbenutzer** befindet, sich bei einem Laptop über Terminaldienste anmelden, da die Organisationseinheit „Laptop“ ein untergeordnetes Element der Organisationseinheit „Windows Vista-Computer“ ist und die untergeordnete Richtlinie Vorrang hat.

Wenn Sie die Richtlinienoption **Kein Vorrang** im Gruppenrichtlinienobjekt für die Organisationseinheit „Windows Vista-Computer“ aktivieren, können sich nur Benutzer mit Konten in der Gruppe **Administratoren** über Terminaldienste beim Laptopcomputer anmelden. Dies liegt daran, dass durch die Option **Kein Vorrang** verhindert wird, dass die Richtlinie der untergeordneten Organisationseinheit die zuvor angewendete Richtlinie überschreibt.

#### Implementieren der Sicherheitsrichtlinien

Zum Implementieren des Sicherheitsentwurfs für die beiden in diesem Handbuch beschriebenen Umgebungen müssen Sie die Gruppenrichtlinien-Verwaltungskonsole (GPMC) und GPMC-basierte Skripts verwenden. GPMC ist in das Windows Vista-Betriebssystem integriert, Sie müssen die Konsole daher nicht jedes Mal herunterladen und installieren, wenn Sie Gruppenrichtlinienobjekte auf einem anderen Computer verwalten möchten. Im Gegensatz zu den Sicherheitsanweisungen für vorherige Windows-Betriebssysteme wird in den Anleitungen in diesem Handbuch für Windows Vista das Verfahren zum Testen und Implementieren des Sicherheitsentwurfs für die Unternehmensclient-Umgebung weitgehend automatisiert. Diese Anleitungen wurden im Hinblick darauf entwickelt und getestet, Ihnen einen so effizienten Prozess wie möglich bereitzustellen und so den Mehraufwand bei der Implementierung zu reduzieren.

**Wichtig:**   Sie müssen alle Anweisungen in diesem Handbuch auf einem Clientcomputer mit Windows Vista ausführen, der mit Active Directory einer Domäne hinzugefügt wurde. Darüber hinaus muss der Benutzer, der die Schritte ausführt, über Domänenadministratorrechte verfügen. Wenn Sie das Betriebssystem Microsoft Windows® XP oder Windows Server® 2003 verwenden, werden die Windows Vista–spezifischen Sicherheitseinstellungen nicht in der GPMC angezeigt.

Zum Implementieren des Sicherheitsentwurfs müssen Sie drei Hauptaufgaben ausführen:

1.  Erstellen der Unternehmensclient-Umgebung

2.  Verknüpfen der Domänenrichtlinie „VSG EC Domain Policy“ mit der Domäne mithilfe der Gruppenrichtlinien-Verwaltungskonsole

3.  Überprüfen der Ergebnisse in der Gruppenrichtlinien-Verwaltungskonsole

In diesem Abschnitt des Kapitels werden diese Aufgaben und Verfahren sowie die Funktionsweise des Skripts „GPOAccelerator.wsf“ beschrieben, das automatisch die empfohlenen Gruppenrichtlinienobjekte erstellt.

##### Das Skript „GPOAccelerator.wsf“

Das wichtigste Tool, das durch die Datei „Windows Vista Security Guide.msi“ installiert wird, ist das Skript „GPOAccelerator.wsf“. Die Hauptfunktion dieses Skripts ist das automatische Erstellen aller Gruppenrichtlinienobjekte, die Sie zum Ausführen dieser Anleitungen benötigen. Sie müssen nicht mit großem Zeitaufwand manuell Richtlinieneinstellungen bearbeiten und Vorlagen anwenden. Für die Clientcomputer in der Unternehmensclient-Umgebung erstellt das Skript die folgenden vier Gruppenrichtlinienobjekte:

-   **VSG EC Domain Policy** für die Domäne.

-   **VSG EC Users Policy** für Benutzer.

-   **VSG EC Desktop Policy** für Desktopcomputer.

-   **VSG EC Laptop Policy** für Laptopcomputer.

**Wichtig**:   Um den Sicherheitsentwurf in diesem Handbuch für die Unternehmensclient-Umgebung erfolgreich implementieren zu können, müssen Sie den Entwurf unbedingt umfassend testen, bevor Sie ihn in der Produktionsumgebung bereitstellen.

Verwenden Sie das Skript „GPOAccelerator.wsf“ für die folgenden Aufgaben:

-   **Testen des Entwurfs in einer Testumgebung**. Erstellen Sie in der Testumgebung mit dem Skript „GPOAccelerator.wsf“ eine Organisationseinheitsstruktur, erstellen Sie die Gruppenrichtlinienobjekte, und erstellen Sie dann die automatische Verknüpfung zwischen den Gruppenrichtlinienobjekten und den Organisationseinheiten. Nach Abschluss der Testphase der Implementierung können Sie das Skript in der Produktionsumgebung verwenden.

-   **Bereitstellen des Entwurfs in einer Produktionsumgebung**. Wenn Sie anfangen, die Lösung in der Produktionsumgebung zu implementieren, müssen Sie zunächst eine geeignete Organisationseinheitsstruktur erstellen oder eine vorhandene Gruppe von Organisationseinheiten ändern. Sie können dann mit dem Skript „GPOAccelerator.wsf“ die Gruppenrichtlinienobjekte erstellen und die neuen Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten in der Umgebung verknüpfen.

##### Testen des Entwurfs in einer Testumgebung

Die mit diesem Handbuch bereitgestellten Gruppenrichtlinienobjekte wurden intensiv getestet. Sie müssen jedoch unbedingt eigene Tests in Ihrer Umgebung durchführen. Um Zeit zu sparen, können Sie mit dem Skript „GPOAccelerator.wsf“ die vorgeschriebenen Gruppenrichtlinienobjekte und die empfohlene Organisationseinheitsstruktur erstellen und die GPOs und die Organisationseinheiten dann automatisch verknüpfen.

#### Aufgabe 1: Erstellen der Unternehmensclient-Umgebung

Das Skript „GPOAccelerator.wsf“ befindet sich im folgenden Ordner: Windows Vista Security Guide\\
GPOAccelerator Tool. Dieser wird von der Microsoft Windows Installer-Datei (MSI-Datei) erstellt.

**Hinweis:   **Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

**So erstellen Sie die Gruppenrichtlinienobjekte und verknüpfen sie mit den entsprechenden Organisationseinheiten in der Testumgebung**

1.  Melden Sie sich als Domänenadministrator an einem Computer mit Windows Vista an, der mit Active Directory der Domäne hinzugefügt wurde, in der Sie die Gruppenrichtlinienobjekte erstellen.

2.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide**.

3.  Öffnen Sie den Ordner **GPOAccelerator Tool\\Security Group Policy Objects**.

4.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Domänenadministratorrechten zu öffnen.

    **Hinweis:**   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /Enterprise /LAB** ein, und drücken Sie dann die EINGABETASTE.

6.  Klicken Sie im Meldungsfeld **Click Yes to continue,** **or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

    **Hinweis:**   Dieser Schritt kann einige Minuten in Anspruch nehmen.

7.  Klicken Sie im Meldungsfeld **The** **Enterprise Lab Environment is created** (Die Unternehmenstestumgebung wurde erstellt) auf **OK**.

8.  Klicken Sie im Meldungsfeld **Make sure to link the Enterprise Domain GPO to your domain** (Gruppenrichtlinienobjekt für Unternehmensdomäne mit der Domäne verknüpfen) auf **OK**, und führen Sie dann die Schritte in der nächsten Aufgabe aus, um die Domänenrichtlinie „VSG EC Domain Policy“ zu verknüpfen.

    **Hinweis:**   Die Gruppenrichtlinie auf Domänenebene enthält Einstellungen, die auf alle Computer und Benutzer in der Domäne angewendet werden. Sie müssen entscheiden können, wann das Domänen-GPO verknüpft wird, da dieses Gruppenrichtlinienobjekt auf *alle* Benutzer und Computer angewendet wird. Aus diesem Grund wird das Domänen-GPO vom Skript „GPOAccelerator.wsf“ nicht automatisch mit der Domäne verknüpft.

#### Aufgabe 2: Verknüpfen der Domänenrichtlinie „VSG EC Domain Policy“ mit der Domäne mithilfe der GPMC

Sie können nun das Domänen-Gruppenrichtlinienobjekt mit der Domäne verknüpfen. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Domänenrichtlinie „VSG EC Domain Policy“ mit der Domäne verknüpfen.

**So verknüpfen Sie die Domänenrichtlinie „VSG EC Domain Policy“**

1.  Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen**. (Sie können auch die Windows-Logo-Taste + R drücken.)

2.  Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK**.

3.  Klicken Sie in der Domänenstruktur mit der rechten Maustaste auf die Domäne, und klicken Sie dann auf **Vorhandenes Gruppenrichtlinienobjekt verknüpfen**.

4.  Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG EC Domain Policy**, und klicken Sie dann auf **OK**.

5.  Wählen Sie im Detailbereich **VSG EC Domain Policy** aus, und klicken Sie dann auf die Schaltfläche **Verknüpfung an den Anfang verschieben**.

**Wichtig:**   Stellen Sie sicher, dass für **VSG EC Domain Policy** die Option **Verknüpfungsreihenfolge** auf **1** festgelegt ist. Wenn dies nicht der Fall ist, überschreiben andere mit der Domäne verknüpfte Gruppenrichtlinienobjekte, z. B. das Gruppenrichtlinienobjekt für die Standarddomänenrichtlinie, die Einstellungen des *Windows Vista-Sicherheitshandbuchs*.

#### Aufgabe 3: Überprüfen der Ergebnisse mithilfe der Gruppenrichtlinien-Verwaltungskonsole

Mit der GPMC können Sie die Ergebnisse des Skripts überprüfen. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Gruppenrichtlinienobjekte und die Struktur der Organisationseinheiten überprüfen können, die vom Skript „GPOAccelerator.wsf“ erstellt wurden.

**So überprüfen Sie die Ergebnisse des Skripts „GPOAccelerator.wsf“**

1.  Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen**.

2.  Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK**.

3.  Klicken Sie auf die entsprechende Struktur, klicken Sie auf **Domänen**, und klicken Sie dann auf die Domäne.

4.  Klicken Sie auf **Vista Security Guide EC Client OU** (EC-Client-Organisationseinheit für Vista Security Guide), erweitern Sie diese Organisationseinheit, und klicken Sie dann auf die fünf Organisationseinheiten darunter, um sie zu öffnen.

5.  Stellen Sie sicher, dass die Organisationseinheitsstruktur und die Verknüpfungen der Gruppenrichtlinienobjekte mit der folgenden Abbildung übereinstimmen.

    ![](images/Dd443680.VSGF0104(de-de,TechNet.10).gif)

    **Abbildung 1.4 GPMC-Ansicht der Organisationseinheitsstruktur und Verknüpfungen der Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt wurden**

Alle Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt werden, enthalten sämtliche in diesem Handbuch empfohlene Einstellungen. Sie können nun mit dem Tool „Active Directory-Benutzer und -Computer“ den Entwurf testen, indem Sie Benutzer und Computer in die entsprechenden Organisationseinheiten verschieben. Details zu den Einstellungen der einzelnen Gruppenrichtlinienobjekte finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

##### Bereitstellen des Entwurfs in einer Produktionsumgebung

Um Zeit zu sparen, können Sie mit dem Skript „GPOAccelerator.wsf“ die Gruppenrichtlinienobjekte für die Unternehmensclient-Umgebung erstellen. Sie können dann die Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten in der vorhandenen Struktur verknüpfen. In größeren Domänen mit einer größeren Anzahl von Organisationseinheiten müssen Sie beachten, wie Sie die vorhandene Organisationseinheitsstruktur zum Bereitstellen der Gruppenrichtlinienobjekte verwenden.

Wenn möglich, sollten Sie Computer-Organisationseinheiten von Benutzer-Organisationseinheiten trennen. Laptop- und Desktopcomputer sollten ebenfalls jeweils in eigenen Organisationseinheiten organisiert werden. Wenn das Erstellen einer solchen Struktur in Ihrer Umgebung nicht möglich ist, müssen Sie die Gruppenrichtlinienobjekte möglicherweise ändern. In Anhang A finden Sie Informationen zu den Einstellungen, die Ihnen dabei helfen können, die erforderlichen Änderungen zu ermitteln.

**Hinweis:**   Wie im vorhergehenden Abschnitt beschrieben, können Sie das Skript „GPOAccelerator.wsf“
mit der Option **/LAB** ausführen, um in einer Testumgebung die Beispiel-Organisationseinheitsstruktur zu erstellen. Bei Umgebungen mit einer flexiblen Organisationseinheitsstruktur kann diese Option jedoch auch in einer Produktionsumgebung zum Erstellen einer einfachen Organisationseinheitsstruktur und zum automatischen Verknüpfen der Gruppenrichtlinienobjekte verwendet werden. Sie können die Organisationseinheitsstruktur dann manuell an die Anforderungen Ihrer Umgebung anpassen.

#### Aufgabe 1: Erstellen der Gruppenrichtlinienobjekte

Sie erstellen die in diesem Handbuch beschriebenen Gruppenrichtlinienobjekte für Unternehmensclients mit dem Skript „GPOAccelerator.wsf“. Das Skript „GPOAccelerator.wsf“ befindet sich in folgendem Ordner: Windows Vista Security Guide\\GPOAccelerator Tool. Dieser wird von der Microsoft Windows Installer-Datei (MSI-Datei) erstellt.

**Hinweis:**   Sie können das Verzeichnis „GPOAccelerator Tool“ einfach von einem Computer, auf dem das Verzeichnis installiert ist, auf einen anderen Computer kopieren, auf dem Sie das Skript verwenden möchten. Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

**So erstellen Sie die Gruppenrichtlinienobjekte in einer Produktionsumgebung**

1.  Melden Sie sich als Domänenadministrator an einem Computer mit Windows Vista an, der mit Active Directory der Domäne hinzugefügt wurde, in der Sie die Gruppenrichtlinienobjekte erstellen.

2.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3.  Öffnen Sie den Ordner **GPOAccelerator Tool\\Security Group Policy Objects**.

4.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Domänenadministratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /Enterprise** ein, und drücken Sie dann die EINGABETASTE.

6.  Klicken Sie im Meldungsfeld **Click Yes to continue,** **or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

    **Hinweis:**   Dieser Schritt kann einige Minuten in Anspruch nehmen.

7.  Klicken Sie im Meldungsfeld **The Enterprise GPOs are created** (Die Unternehmens-Gruppenrichtlinienobjekte wurden erstellt) auf **OK**.

8.  Klicken Sie im Meldungsfeld **Make sure to link the Enterprise GPOs to the appropriate OUs** (Unternehmens-Gruppenrichtlinienobjekte mit den entsprechenden OUs verknüpfen) auf **OK**.

#### Aufgabe 2: Überprüfen der Ergebnisse mithilfe der Gruppenrichtlinien-Verwaltungskonsole

Mithilfe der GPMC können Sie sicherstellen, dass das Skript alle Gruppenrichtlinienobjekte erfolgreich erstellt hat. Im Folgenden wird beschrieben, wie Sie mit der GPMC auf einem Clientcomputer mit Windows Vista die Gruppenrichtlinienobjekte überprüfen können, die vom Skript „GPOAccelerator.wsf“ erstellt wurden.

**So überprüfen Sie die Ergebnisse des Skripts „GPOAccelerator.wsf“**

1.  Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen**.

2.  Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK**.

3.  Klicken Sie auf die entsprechende Struktur, klicken Sie auf **Domänen**, und klicken Sie dann auf die Domäne.

4.  Klicken Sie auf **Gruppenrichtlinienobjekte**, erweitern Sie den Eintrag, und stellen Sie sicher, dass alle vier VSG EC-Gruppenrichtlinienobjekte wie in der folgenden Abbildung dargestellt erstellt wurden.

    ![](images/Dd443680.VSGF0105(de-de,TechNet.10).gif)

    **Abbildung 1.5 GPMC-Ansicht der Gruppenrichtlinienobjekte für Unternehmensclients, die vom Skript „GPOAccelerator.wsf“ erstellt wurden**

Sie können nun mit der GPMC die einzelnen Gruppenrichtlinienobjekte mit den entsprechenden Organisationseinheiten verknüpfen. In der letzten Aufgabe dieses Verfahrens wird dies erläutert.

#### Aufgabe 3: Verknüpfen der Gruppenrichtlinienobjekte mit den Organisationseinheiten mithilfe der Gruppenrichtlinien-Verwaltungskonsole

Im Folgenden wird beschrieben, wie Sie diese Aufgabe mithilfe der GPMC auf einem Clientcomputer mit Windows Vista ausführen.

**So verknüpfen Sie die Gruppenrichtlinienobjekte in einer Produktionsumgebung**

1.  Klicken Sie auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, klicken Sie auf **Zubehör**, und klicken Sie dann auf **Ausführen**.

2.  Geben Sie im Textfeld **Öffnen** die Zeichenfolge **gpmc.msc** ein, und klicken Sie dann auf **OK**.

3.  Klicken Sie in der Domänenstruktur mit der rechten Maustaste auf die Domäne, und klicken Sie dann auf **Vorhandenes Gruppenrichtlinienobjekt verknüpfen**.

4.  Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG EC Domain Policy**, und klicken Sie dann auf **OK**.

5.  Wählen Sie im Detailbereich **VSG EC Domain Policy** aus, und klicken Sie dann auf die Schaltfläche **Verknüpfung an den Anfang verschieben**.

    **Wichtig:**   Stellen Sie sicher, dass für **VSG EC Domain Policy** die Option **Verknüpfungsreihenfolge** auf **1** festgelegt ist. Wenn dies nicht der Fall ist, überschreiben andere mit der Domäne verknüpfte Gruppenrichtlinienobjekte, z. B. das Gruppenrichtlinienobjekt für die Standarddomänenrichtlinie, die Einstellungen des *Windows* *Vista-Sicherheitshandbuchs*.

6.  Klicken Sie mit der rechten Maustaste auf den Knoten „Windows Vista Users OU“, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen** aus.

7.  Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG EC Users Policy**, und klicken Sie dann auf **OK**.

8.  Klicken Sie mit der rechten Maustaste auf den Knoten **Desktop OU**, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen** aus.

9.  Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG EC Desktop Policy**, und klicken Sie dann auf **OK**.

10. Klicken Sie mit der rechten Maustaste auf den Knoten **Laptop OU**, und wählen Sie dann die Option **Vorhandenes Gruppenrichtlinienobjekt verknüpfen** aus.

11. Klicken Sie im Dialogfeld **Gruppenrichtlinienobjekt auswählen** auf das Gruppenrichtlinienobjekt **VSG EC Laptop Policy**, und klicken Sie dann auf **OK**.

12. Wiederholen Sie diese Schritte für alle weiteren erstellten Benutzer- oder Computer-Organisationseinheiten, um diese zusätzlichen Organisationseinheiten mit den entsprechenden Gruppenrichtlinienobjekten zu verknüpfen.

**Hinweis:**   Sie können ein Gruppenrichtlinienobjekt, das sich unter dem Knoten „Gruppenrichtlinienobjekte“ befindet, in eine Organisationseinheit ziehen. Drag & Drop-Vorgänge sind jedoch nur innerhalb einer Domäne möglich.

**So bestätigen Sie die Gruppenrichtlinienobjekt-Verknüpfungen mithilfe der GPMC**

-   Erweitern Sie den Knoten **Gruppenrichtlinienobjekte**, wählen Sie das Gruppenrichtlinienobjekt aus, klicken Sie im Detailbereich auf die Registerkarte **Bereich**, und notieren Sie dann die Informationen in den Spalten **Verknüpfung aktiviert** und **Pfad**.

– Oder –

-   Wählen Sie die Organisationseinheit aus, klicken Sie dann im Detailbereich auf die Registerkarte **Verknüpfte Gruppenrichtlinienobjekte**, und notieren Sie die Informationen in den Spalten **Verknüpfung aktiviert** und **Gruppenrichtlinienobjekt**.

**Hinweis:**   Sie können mit der GPMC die Verknüpfungen der Gruppenrichtlinienobjekte auch aufheben oder ggf. löschen. Löschen Sie anschließend entweder mithilfe der GPMC oder dem MMC-Snap-In „Active Directory-Benutzer und -Computer“ alle nicht mehr benötigten Organisationseinheiten. Wenn Sie alle Active Directory-Änderungen rückgängig machen möchten, die vom Skript „GPOAccelerator.wsf“ vorgenommen wurden, müssen Sie manuell die Dateien „EC-VSGAuditPolicy.cmd“, „EC-ApplyAuditPolicy.cmd“ und „EC-AuditPolicy.txt“ aus der Freigabe NETLOGON auf einem der Domänencontroller löschen. Weitere Informationen zum vollständigen Entfernen der Implementierung der Überwachungsrichtlinien finden Sie im Abschnitt zu Überwachungsrichtlinien in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

Alle Gruppenrichtlinienobjekte, die vom Skript „GPOAccelerator.wsf“ erstellt werden, enthalten sämtliche in diesem Handbuch empfohlene Einstellungen. Sie können nun mit dem Tool „Active Directory-Benutzer und -Computer“ den Entwurf testen, indem Sie Benutzer und Computer in die entsprechenden Organisationseinheiten verschieben. Details zu den Einstellungen der einzelnen Gruppenrichtlinienobjekte finden Sie in Anhang A, „Sicherheitsrelevante Gruppenrichtlinieneinstellungen“.

##### Migrieren von Gruppenrichtlinienobjekten in eine andere Domäne (Optional)

Wenn Sie in dieser Lösung die Gruppenrichtlinienobjekte geändert oder eigene Gruppenrichtlinienobjekte erstellt haben und diese in mehreren Domänen verwenden möchten, müssen Sie die Gruppenrichtlinienobjekte migrieren. Für das Migrieren eines in einer Domäne funktionierenden Gruppenrichtlinienobjekts in eine andere Domäne ist etwas Planung erforderlich, das grundlegende Verfahren ist jedoch relativ einfach. Bei der Planung sind im Hinblick auf Daten bei Gruppenrichtlinienobjekten zwei wichtige Aspekte zu beachten:

-   **Komplexe Daten**. Die Daten, aus denen ein Gruppenrichtlinienobjekt besteht, sind komplex und werden an mehreren Speicherorten gespeichert. Durch die Verwendung der GPMC zum Migrieren eines Gruppenrichtlinienobjekts wird sichergestellt, dass alle relevanten Daten ordnungsgemäß migriert werden.

-   **Domänenspezifische Daten**. Einige Daten in einem Gruppenrichtlinienobjekt können domänenspezifisch sein und sind daher möglicherweise ungültig, wenn Sie sie direkt in eine andere Domäne kopieren. Zum Beheben dieses Problems werden in der GPMC Migrationstabellen verwendet, mit denen Sie domänenspezifische Daten in einem Gruppenrichtlinienobjekt bei der Migration auf neue Werte aktualisieren können. Dies ist nur erforderlich, wenn das Gruppenrichtlinienobjekt Sicherheits-IDs (SIDs) oder UNC-Pfade (Universal Naming Convention) enthält, die für eine Domäne spezifisch sind.

Weitere Informationen zum Migrieren von Gruppenrichtlinienobjekten finden Sie in der Hilfe zur Gruppenrichtlinien-Verwaltungskonsole. Im Whitepaper [Migrating GPOs Across Domains with GPMC](http://www.microsoft.com/windowsserver2003/gpmc/migrgpo.mspx) (engl.) finden Sie ebenfalls weitere Informationen zu diesem Thema.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Das GPOAccelerator-Tool

Die Tools und Vorlagen zu diesem Handbuch umfassen Skripts und Sicherheitsvorlagen. Dieser Abschnitt enthält Hintergrundinformationen zu diesen Ressourcen. Das wichtigste Tool, mit dem das Hauptskript für diesen Sicherheitsleitfaden ausgeführt wird, ist „GPOAccelerator.wsf“. Die Datei befindet sich im Ordner „Windows Vista Security Guide\\GPOAccelerator Tool\\Security Group Policy Objects“. Außerdem enthält dieser Abschnitt Informationen darüber, wie Sie die GPMC zur Anzeige der Einstellungen für Gruppenrichtlinienobjekte einrichten, sowie über die Unterverzeichnisstruktur und die Dateitypen, die zu diesem Handbuch gehören. Die Datei „Windows Vista Security Guide Settings.xls“, die ebenfalls mit diesem Handbuch geliefert wird, stellt weitere Ressourcen bereit, mit denen Sie Einstellungswerte vergleichen können.

#### Erweiterungen für Gruppenrichtlinien-Verwaltungskonsole und Sicherheitskonfigurations-Editor

In der in diesem Handbuch vorgestellten Lösung werden Einstellungen für Gruppenrichtlinienobjekte verwendet, die nicht in der Standardbenutzeroberfläche für die Gruppenrichtlinien-Verwaltungskonsole in Windows Vista oder im Sicherheitskonfigurations-Editor (Security Configuration Editor, SCE) angezeigt werden. Diese Einstellungen verfügen über das Präfix **MSS:** und wurden vom Microsoft Solutions for Security-Team für vorhergehende Sicherheitsleitfäden entwickelt.

**Wichtig**:   Die SCE-Erweiterungen und das Skript **GPOAccelerator.wsf** sind für die Ausführung auf einem Windows Vista-basierten Computer konzipiert. Diese Tools funktionieren nicht ordnungsgemäß, wenn Sie versuchen, sie auf einem Computer mit Windows XP oder Windows Server 2003 auszuführen.

Daher müssen Sie diese Tools erweitern, so dass Sie die Sicherheitseinstellungen anzeigen und ggf. ändern können. Hierzu aktualisiert das Skript „GPOAccelerator.wsf“ beim Erstellen der Gruppenrichtlinienobjekte automatisch den Computer. Wenn Sie die Gruppenrichtlinienobjekte des *Windows* *Vista-Sicherheitshandbuchs* von einem anderen Computer mit Windows Vista aus verwalten möchten, aktualisieren Sie den Sicherheitskonfigurations-Editor auf diesem Computer wie folgt.

**So ändern Sie den Sicherheitskonfigurations-Editor zum Anzeigen von MSS-Einstellungen**

1.  Stellen Sie sicher, dass die folgenden Voraussetzungen erfüllt sind:

    -   Der Computer wurde mit Active Directory der Domäne hinzugefügt, in der die Gruppenrichtlinienobjekte erstellt wurden.

    -   Das *Windows* *Vista-Sicherheitshandbuch*-Verzeichnis **GPOAccelerator** **Tool** wurde installiert.

    **Hinweis:**   Sie können das Verzeichnis „GPOAccelerator Tool“ einfach von einem Computer, auf dem das Verzeichnis installiert ist, auf einen anderen Computer kopieren, auf dem Sie das Skript verwenden möchten. Der Ordner „GPOAccelerator Tool“ und die entsprechenden Unterordner müssen sich auf dem lokalen Computer befinden, damit das Skript wie im folgenden Verfahren beschrieben ausgeführt wird.

2.  Melden Sie sich am Computer als Administrator an.

3.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

4.  Öffnen Sie den Ordner GPOAccelerator Tool\\Security Group Policy Objects.

5.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

6.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /ConfigSCE** ein, und drücken Sie dann die EINGABETASTE.

7.  Klicken Sie im Meldungsfeld **Click Yes to continue,** **or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

8.  Klicken Sie im Meldungsfeld **The** **Security Configuration Editor is updated** (Der Sicherheitskonfigurations-Editor wurde aktualisiert) auf **OK**.

**Wichtig**:   Dieses Skript ändert den Sicherheitskonfigurations-Editor nur insofern, dass MSS-Einstellungen angezeigt werden. Es werden keine Gruppenrichtlinienobjekte oder Organisationseinheiten erstellt.

Mit dem folgenden Verfahren werden die zusätzlichen MSS-Sicherheitseinstellungen entfernt, und das SCE-Tool wird auf die Standardeinstellungen in Windows Vista zurückgesetzt.

**So setzen Sie das SCE-Tool auf die Standardeinstellungen in Windows Vista zurück**

1.  Melden Sie sich am Computer als Administrator an.

2.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3.  Öffnen Sie den Ordner GPOAccelerator Tool\\Security Group Policy Objects.

4.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /ResetSCE** ein, und drücken Sie dann die EINGABETASTE.

6.  Klicken Sie im Meldungsfeld **Click Yes to continue,** **or No to exit the script** (Fortfahren mit „Ja“, Skript beenden mit „Nein“) auf **Yes** (Ja).

    **Hinweis:**   Bei Durchführen dieser Schritte wird der Sicherheitskonfigurations-Editor auf dem Computer auf die Standardeinstellungen in Windows Vista zurückgesetzt. Alle zum Sicherheitskonfigurations-Editor hinzugefügten Einstellungen werden entfernt. Dies hat nur Auswirkungen auf die Fähigkeit zur Anzeige der Einstellungen im Sicherheitskonfigurations-Editor. Konfigurierte Einstellungen für Gruppenrichtlinienobjekte bleiben unverändert.

7.  Klicken Sie im Meldungsfeld **The** **Security Configuration Editor is updated** (Der Sicherheitskonfigurations-Editor wurde aktualisiert) auf **OK**.

#### Vorherige Sicherheitseinstellungen

Es werden Sicherheitsvorlagen bereitgestellt, damit Sie, falls Sie eigene Richtlinien erstellen möchten, nicht die mit diesem Handbuch gelieferten Richtlinien verwenden oder ändern müssen, sondern die relevanten Sicherheitseinstellungen importieren können. Sicherheitsvorlagen sind Textdateien, die Werte für Sicherheitseinstellungen enthalten. Sie sind Unterkomponenten von Gruppenrichtlinienobjekten. Sie können die Richtlinieneinstellungen in den Sicherheitsvorlagen im MMC-Snap-In „Gruppenrichtlinienobjekt-Editor“ ändern. Im Gegensatz zu älteren Versionen des Windows-Betriebssystems umfasst Windows Vista keine vordefinierten Sicherheitsvorlagen. Sie können die vorhandenen Sicherheitsvorlagen bei Bedarf jedoch weiter verwenden.

Sicherheitsvorlagen sind in der Windows Installer-Datei (MSI-Datei) enthalten, die mit diesem Handbuch geliefert wird. Die folgenden Vorlagen für die Unternehmensclient-Umgebung befinden sich im Ordner „GPOAccelerator Tool\\Security Templates“:

-   VSG EC Desktop.inf

-   VSG EC Domain.inf

-   VSG EC Laptop.inf

**Wichtig:**   Sie benötigen die Sicherheitsvorlagen nicht zum Bereitstellen der in diesem Handbuch beschriebenen Lösung. Die Vorlagen stellen eine Alternative zur GPMC-basierten Lösung dar und betreffen lediglich Computersicherheitseinstellungen unter **Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen**. Sie können beispielsweise keine Einstellungen für Internet Explorer oder Windows Firewall in den Gruppenrichtlinienobjekten mit einer Sicherheitsvorlage verwalten. Außerdem sind keine Benutzereinstellungen eingeschlossen.

##### Verwenden von Sicherheitsvorlagen

Wenn Sie die Sicherheitsvorlagen verwenden möchten, müssen Sie zunächst den Sicherheitskonfigurations-Editor erweitern, damit benutzerdefinierte MSS-Sicherheitseinstellungen in der Benutzeroberfläche angezeigt werden. Das Verfahren wird weiter oben in diesem Kapitel unter „Erweiterungen für Gruppenrichtlinien-Verwaltungskonsole und Sicherheitskonfigurations-Editor“ ausführlich beschrieben. Wenn Sie die Vorlagen anzeigen können, können Sie sie anhand des folgenden Verfahrens in die Gruppenrichtlinienobjekte importieren, die Sie für Ihren Bedarf erstellt haben.

**So importieren Sie eine Sicherheitsvorlage in ein Gruppenrichtlinienobjekt**

1.  Öffnen Sie im Gruppenrichtlinienobjekt-Editor das zu ändernde Gruppenrichtlinienobjekt. In der GPMC klicken Sie hierzu mit der rechten Maustaste auf das Gruppenrichtlinienobjekt und anschließend auf **Bearbeiten**.

2.  Navigieren Sie im Gruppenrichtlinienobjekt-Editor zum Ordner **Windows-Einstellungen**.

3.  Erweitern Sie den Ordner **Windows-Einstellungen**, und wählen Sie dann **Sicherheitseinstellungen** aus.

4.  Klicken Sie mit der rechten Maustaste auf den Ordner **Sicherheitseinstellungen**, und klicken Sie anschließend auf **Richtlinie importieren**.

5.  Navigieren Sie zum Ordner **Security Templates** im Ordner **Windows Vista Security Guide**.

6.  Wählen Sie die Sicherheitsvorlage aus, die Sie importieren möchten, und klicken Sie dann auf **Öffnen**.

    Durch den letzten Schritt dieses Verfahrens werden die Einstellungen aus der Datei in das Gruppenrichtlinienobjekt importiert.

Mit den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen können Sie auch die lokale Sicherheitsrichtlinie auf eigenständigen Clientcomputern mit Windows Vista ändern. Das Skript „GPOAccelerator.wsf“ vereinfacht den Prozess zum Anwenden der Vorlagen.

**So wenden Sie die Sicherheitsvorlagen zum Erstellen einer lokalen Gruppenrichtlinie auf einem eigenständigen Clientcomputer mit Windows Vista an**

1.  Melden Sie sich als Administrator auf einem Computer mit Windows Vista an.

2.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3.  Öffnen Sie den Ordner GPOAccelerator Tool\\Security Group Policy Objects.

4.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /Enterprise /Desktop** oder **cscript GPOAccelerator.wsf /Enterprise /Laptop** ein, und drücken Sie dann die EINGABETASTE.

    Durch dieses Verfahren werden die lokalen Sicherheitsrichtlinieneinstellungen mit den Werten in den Sicherheitsvorlagen für die Unternehmensclient-Umgebung geändert.

**So setzen Sie die lokale Gruppenrichtlinie auf die Standardeinstellungen in Windows Vista zurück**

1.  Melden Sie sich als Administrator auf einem Clientcomputer mit Windows Vista an.

2.  Klicken Sie auf dem Desktop auf die Windows Vista-Schaltfläche **Start**, klicken Sie auf **Alle Programme**, und klicken Sie dann auf **Windows Vista Security Guide** (Windows Vista-Sicherheitshandbuch)

3.  Öffnen Sie den Ordner GPOAccelerator Tool\\Security Group Policy Objects.

4.  Klicken Sie mit der rechten Maustaste auf die Datei **Command-line Here.cmd**, und klicken Sie dann auf **Als Administrator ausführen**, um eine Eingabeaufforderung mit Administratorrechten zu öffnen.

    **Hinweis**:   Wenn Sie aufgefordert werden, Anmeldeinformationen einzugeben, geben Sie den Benutzernamen und das Kennwort ein, und drücken Sie dann die EINGABETASTE.

5.  Geben Sie an der Eingabeaufforderung **cscript GPOAccelerator.wsf /Restore** ein, und drücken Sie dann die EINGABETASTE.

    Durch dieses Verfahren werden die lokalen Sicherheitsrichtlinieneinstellungen auf die Standardwerte in Windows Vista zurückgesetzt.

#### Unterverzeichnisse und Dateien

Beim Ausführen der Windows Installer-Datei (MSI-Datei) wird auf Ihrem Computer standardmäßig der Ordner **Windows Vista Security Guide\\GPOAccelerator Tool** an einem von Ihnen angegebenen Speicherort erstellt. Die MSI-Datei erstellt die folgende Unterverzeichnisstruktur im Ordner **GPOAccelerator Tool** sowie die in der folgenden Tabelle beschriebenen Dateien.

**Tabelle 1.1 Unterverzeichnisse, Dateien und Beschreibungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Unterverzeichnis\Datei</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">SCE Update<br />
\Restore_SCE_to_Default.vbs</td>
<td style="border:1px solid black;">Ein Skript, das den Sicherheitskonfigurations-Editor auf Windows Vista-Standardwerte zurücksetzt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SCE Update<br />
\Sceregvl_Vista.inf.txt</td>
<td style="border:1px solid black;">Die Windows Vista-SCEREGVL.INF-Standarddatei, die den Sicherheitskonfigurations-Editor auf die Originalwerte zurücksetzt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SCE Update<br />
\Strings-sceregvl.txt</td>
<td style="border:1px solid black;">Eine Textdatei mit erforderlichen Zeichenfolgenwerten zum Hinzufügen von MSS-Einstellungen zum Sicherheitskonfigurations-Editor.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SCE Update<br />
\Update_SCE_with_MSS_Regkeys.vbs</td>
<td style="border:1px solid black;">Ein Skript, mit dem der Sicherheitskonfigurations-Editor zum Einbeziehen von MSS-Einstellungen geändert wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SCE Update<br />
\Sce.reg</td>
<td style="border:1px solid black;">Eine Registrierungsdatei mit den Standardregistrierungswerten für den Sicherheitskonfigurations-Editor.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SCE Update<br />
\Values-sceregvl.txt</td>
<td style="border:1px solid black;">Eine Textdatei mit den erforderlichen Werten zum Anzeigen von Registrierungseinstellungen im Sicherheitskonfigurations-Editor.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Group Policy Objects<br />
\Command-line here.cmd</td>
<td style="border:1px solid black;">Ein Batchdatei, die eine Eingabeaufforderung in dem Pfad öffnet, von dem aus sie gestartet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Group Policy Objects<br />
\GPOAccelerator.wsf</td>
<td style="border:1px solid black;">Das Haupttool, das ein Skript zum Implementieren der empfohlenen Anleitungen ausführt.<br />

<img src="images/Dd443680.warning(de-de,TechNet.10).gif" /><strong>Achtung:</strong>
Führen Sie das Skript erst aus, wenn Sie alle Informationen in diesem Kapitel gelesen haben.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\CreateEnvironmentFromXML.wsf</td>
<td style="border:1px solid black;">Das Skript, das die Gruppenrichtlinienobjekte und die Organisationseinheitsstruktur erstellt.<br />

<img src="images/Dd443680.warning(de-de,TechNet.10).gif" /><strong>Achtung:</strong>
Ändern Sie diese Datei nicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GPMCFiles<br />
\EC-VSG-GPOs.xml</td>
<td style="border:1px solid black;">Eine XML-Datei, mit der die GPMC die Unternehmens-Gruppenrichtlinienobjekte erstellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\EC-VSG-GPOs-LAB.xml</td>
<td style="border:1px solid black;">Eine XML-Datei, mit der die GPMC die Unternehmens-Gruppenrichtlinienobjekte und die Beispiel-Organisationseinheitsstruktur erstellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GPMCFiles<br />
\SSLF-VSG-GPOs.xml</td>
<td style="border:1px solid black;">Eine XML-Datei, mit der die GPMC die Unternehmens-Gruppenrichtlinienobjekte erstellt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\SSLF-VSG-GPOs-LAB.xml</td>
<td style="border:1px solid black;">Eine XML-Datei, mit der die GPMC die Gruppenrichtlinienobjekte für die Hochsicherheitsumgebung und die empfohlene Organisationseinheitsstruktur erstellt.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GPMCFiles<br />
\EC-VSGAuditPolicy.txt</td>
<td style="border:1px solid black;">Eine Textdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\EC-VSGAuditPolicy.cmd</td>
<td style="border:1px solid black;">Eine Befehlsdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GPMCFiles<br />
\EC-VSGApplyAuditPolicy.cmd</td>
<td style="border:1px solid black;">Eine Befehlsdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\SSLF-VSGAuditPolicy.txt</td>
<td style="border:1px solid black;">Eine Textdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GPMCFiles<br />
\SSLF-VSGAuditPolicy.cmd</td>
<td style="border:1px solid black;">Eine Befehlsdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GPMCFiles<br />
\SSLF-VSGApplyAuditPolicy.cmd</td>
<td style="border:1px solid black;">Eine Befehlsdatei, die bei der in diesem Handbuch enthaltenen detaillierten Implementierung der Überwachungsrichtlinien verwendet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates</td>
<td style="border:1px solid black;">Der Ordner mit den .inf-Dateien für Sicherheitsvorlagen, mit denen Sie einige der in diesem Handbuch vorgeschriebenen Sicherheitseinstellungen implementieren können.
<strong>Hinweis:</strong>   Microsoft empfiehlt, die vorgeschriebenen Gruppenrichtlinienobjekte mithilfe des mit diesem Handbuch bereitgestellten Skripts zu erstellen. Die bereitgestellten Sicherheitsvorlagen können jedoch beim Sichern von eigenständigen Computern eine Hilfe darstellen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Templates<br />
\EC-VSG Desktop.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für Desktopcomputer in Unternehmensumgebungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates<br />
\EC-VSG Domain.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für Domänen in Unternehmensumgebungen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Templates<br />
\EC-VSG Laptop.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für Laptopcomputer in Unternehmensumgebungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates<br />
\SSLF-VSG Desktop.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für SSLF-Desktops</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Templates<br />
\SSLF-VSG Domain.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für SSLF-Domänen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates<br />
\SSLF-VSG Laptop.inf</td>
<td style="border:1px solid black;">Sicherheitsvorlage für SSLF-Laptops</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Templates<br />
\Vista Default Security.cmd</td>
<td style="border:1px solid black;">Eine Befehlsdatei, die beim Zurücksetzen der lokalen Sicherheitsrichtlinie auf die Windows Vista-Standardeinstellungen verwendet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates<br />
\Vista Default Security.inf</td>
<td style="border:1px solid black;">Eine Sicherheitsdatei, die beim Zurücksetzen der lokalen Sicherheitsrichtlinie auf die Windows Vista-Standardeinstellungen verwendet wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Security Templates<br />
\Vista Default Security.sdb</td>
<td style="border:1px solid black;">Eine Sicherheitsdatenbankdatei, die beim Zurücksetzen der lokalen Sicherheitsrichtlinie auf die Windows Vista-Standardeinstellungen verwendet wird.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Security Templates<br />
\Vista Local Security.sdb</td>
<td style="border:1px solid black;">Eine Sicherheitsdatenbankdatei, die beim Anwenden der Sicherheitsvorlagen dieses Handbuchs auf einem Computer verwendet wird.</td>
</tr>
</tbody>
</table>
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Weitere Informationen
  
Die folgenden Links bieten weitere Informationen zu sicherheitsbezogenen Themen zu Windows Vista:
  
-   [Administering Group Policy with Group Policy Management Console Abstract](http://go.microsoft.com/fwlink/?linkid=14320) (engl.)
  
-   [Enterprise Management with the Group Policy Management Console](http://www.microsoft.com/windowsserver2003/gpmc/default.mspx) (engl.)
  
-   [Loopbackverarbeitung von Gruppenrichtlinien](http://support.microsoft.com/kb/231287)
  
-   [Migrating GPOs Across Domains with GPMC](http://www.microsoft.com/windowsserver2003/gpmc/migrgpo.mspx) (engl.)
  
-   [*Verständnis der Gruppenrichtlinienfunktionen*](http://www.microsoft.com/germany/technet/datenbank/articles/600539.mspx)
  
-   [*Verwendung des Assistenten zum Zuweisen der Objektverwaltung*](http://www.microsoft.com/germany/technet/datenbank/articles/600542.mspx)
  
-   [Summary of New or Expanded Group Policy Settings](http://www.microsoft.com/technet/windowsvista/library/gpol/2b8dc2fd-eafe-4c74-914c-ec101133feb4.mspx?mfr=true) (engl.)
  
-   [Windows-Hilfe und -Anweisungen](http://windowshelp.microsoft.com/windows/de-de/default.mspx)
  
-   [Microsoft Windows Vista Security Advancements](http://www.microsoft.com/presspass/newsroom/security/vistasecurity.mspx) (engl.)
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### In diesem Beitrag
  
-   [Übersicht](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx)  
-   Kapitel 1: Implementieren der Sicherheitsbasis  
-   [Kapitel 2: Schutz vor Malware](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx)  
-   [Kapitel 3: Schutz von vertraulichen Daten](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/protect_sensitive_data.mspx)  
-   [Kapitel 4: Anwendungskompatibilität](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/application_compatibility.mspx)  
-   [Kapitel 5: Hochsicherheit (SSLF)](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/specialized_security.mspx)  
-   [Anhang A: Sicherheitsrelevante Gruppenrichtlinieneinstellungen](http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/security_group_policy_settings.mspx)
  
**Download**
  
[Windows Vista-Sicherheitshandbuch herunterladen](http://go.microsoft.com/fwlink/?linkid=74028) (engl.)
  
**Update Notifications**
  
[Melden Sie sich an, um über Updates und neue Versionen informiert zu werden.](http://go.microsoft.com/fwlink/?linkid=54982) (engl.)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare und Anregungen.](mailto:secwish@microsoft.com?subject=windows%20vista%20security%20guide) (engl.)

 
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
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/default.mspx"><img src="images/Dd443680.pageLeft(de-de,TechNet.10).gif" /></a>5 von 7<a href="http://www.microsoft.com/germany/technet/prodtechnol/windowsvista/secprot/sicherheitshandbuch/defend_against_malware.mspx"><img src="images/Dd443680.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
