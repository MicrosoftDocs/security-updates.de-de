---
Title: Kapitel 8: Die Druckserverrolle
TOCTitle: Kapitel 8: Die Druckserverrolle
ms:assetid: a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee
ms:mtpsurl: https://technet.microsoft.com/de-de/library/Dd443729(v=TechNet.10)
ms:contentKeyID: 20075672
---


# Windows Server 2003-Sicherheitshandbuch



### Kapitel 8: Die Druckserverrolle
Aktualisiert: 27.12.2005
 

#### Auf dieser Seite

[Überblick](#ehaa)  
[Einstellungen für Überwachungsrichtlinien](#egaa)  
[Zuweisen von Benutzerrechten](#efaa)  
[Sicherheitsoptionen](#eeaa)  
[Ereignisprotokolleinstellungen](#edaa)  
[Zusätzliche Sicherheitseinstellungen](#ecaa)  
[Erstellen der Richtlinie mithilfe des SCW](#ebaa)  
[Zusammenfassung](#eaaa)  



### Überblick

Dieses Kapitel befasst sich mit der Absicherung von Druckservern unter Microsoft® Windows Server™ 2003 mit SP1, die sich als besondere Herausforderung erweisen kann. Die wichtigsten von diesen Servern bereitgestellten Dienste erfordern SMB (Server Message Block)- und CIFS (Common Internet File System)-Protokolle, die nicht authentifizierte Benutzer mit umfassenden Informationen versorgen können. Diese Protokolle sind auf Druckservern in hochsicheren Windows-Umgebungen oft deaktiviert. Es ist jedoch für Administratoren und Benutzer schwierig, auf Druckserver zuzugreifen, wenn diese Protokolle in Ihrer Umgebung deaktiviert sind.

Die meisten Einstellungen in diesem Kapitel werden durch Gruppenrichtlinien konfiguriert und angewendet. Ein Gruppenrichtlinienobjekt (GPO), das die Richtlinie für die Mitgliedsserver-Baseline ergänzt, kann mit den jeweiligen die Druckserver enthaltenden Organisationseinheiten verknüpft werden, um die für diese Serverrollen erforderlichen Sicherheitseinstellungen bereitzustellen. In diesem Kapitel werden nur die Richtlinieneinstellungen erläutert, die von der Richtlinie für die Mitgliedsserver-Baseline abweichen.

Sofern möglich, werden diese Richtlinieneinstellungen in einer inkrementellen Gruppenrichtlinienvorlage gesammelt, die auf die Druckserver-Organisationseinheit angewendet wird. Einige Einstellungen in diesem Kapitel können nicht durch Gruppenrichtlinien angewendet werden. Ausführliche Informationen zur Konfiguration dieser manuellen Einstellungen werden bereitgestellt.

Die folgende Tabelle enthält die Namen der Sicherheitsvorlagen der Druckserver für die drei in diesem Handbuch definierten Umgebungen. Diese Vorlagen stellen die Richtlinieneinstellungen für die inkrementelle Druckservervorlage bereit, die wiederum zum Erstellen eines neuen Gruppenrichtlinienobjekts verwendet wird, das mit der Druckserver-Organisationseinheit in der jeweiligen Umgebung verknüpft ist. In Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, finden Sie ausführliche Anweisungen, die Ihnen beim Erstellen von Organisationseinheiten und Gruppenrichtlinien und beim darauf folgenden Import der entsprechenden Sicherheitsvorlage in die einzelnen Gruppenrichtlinienobjekte helfen.

**Tabelle 8.1: Druckserver-Sicherheitsvorlagen für alle drei Umgebungen**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Älterer Client - Druckserver.inf

</td>

<td style="border:1px solid black;">


Unternehmensclient - Druckserver.inf

</td>

<td style="border:1px solid black;">


Hochsicher - Druckserver.inf

</td>

</tr>

</table>


Informationen zu den Einstellungen in der Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Informationen zu sämtlichen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen für Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))*,* das unter *http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx* verfügbar ist.

**Hinweis**: Auf Druckserver, die mit der Sicherheitsvorlage „Hochsicher - Druckserver.inf“ gesichert sind, kann nur über Clientcomputer zugegriffen werden, die mit kompatiblen Einstellungen gesichert sind. Im *Windows XP-Sicherheitshandbuch* finden Sie Informationen zum Sichern von Clientcomputern mit SSLF-kompatiblen Einstellungen.

[Zum Seitenanfanq](#mainsection)  



### Einstellungen für Überwachungsrichtlinien

Die Einstellungen für Überwachungsrichtlinien für Druckserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie wird die Protokollierung der Sicherheitsüberwachungsinformationen auf allen Druckservern aktiviert.

[Zum Seitenanfanq](#mainsection)  



### Zuweisen von Benutzerrechten

Die Einstellungen für die Zuweisung von Benutzerrechten für Druckserver in den drei in dieser Anleitung definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie werden die Zuweisungen von Benutzerrechten auf allen Druckservern einheitlich konfiguriert.

[Zum Seitenanfanq](#mainsection)  



### Sicherheitsoptionen

Die meisten Sicherheitsoptionseinstellungen für Druckserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Unterschiede zwischen der Richtlinie für die Mitgliedsserver-Baseline und der Gruppenrichtlinie für Druckserver werden im folgenden Abschnitt beschrieben.


#### Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)

**Tabelle 8.2: Empfohlene Einstellungen für „Kommunikation digital signieren (immer)“**

<table style="border:1px solid black;">

<tr>

<th style="border:1px solid black;">

Einstellung

</th>

<th style="border:1px solid black;">

Älterer Client

</th>

<th style="border:1px solid black;">

Unternehmensclient

</th>

<th style="border:1px solid black;">

Hochsicher (SSLF)

</th>

</tr>

<tr>

<td style="border:1px solid black;">


Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

<td style="border:1px solid black;">


Deaktiviert

</td>

</tr>

</table>


Durch diese Richtlinieneinstellung wird festgelegt, ob die SMB-Serverkomponente die Signierung von Paketen erfordert. Das SMB-Protokoll bildet die Grundlage für die Microsoft Datei- und Druckfreigabe und weitere Netzwerkoptionen, wie z. B. Windows-Remoteverwaltung. Um Man-in-the-Middle-Angriffe, die SMB-Pakete während der Übertragung ändern, zu verhindern, unterstützt das SMB-Protokoll die digitale Paketsignierung. Durch diese Richtlinieneinstellung wird festgelegt, ob die SMB-Paketsignierung ausgehandelt werden muss, bevor eine weitere Kommunikation mit einem SMB-Client gestattet wird.

Obwohl die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** standardmäßig deaktiviert ist, aktiviert die Richtlinie für die Mitgliedsserver-Baseline diese Einstellung für Server in der Hochsicherheitsumgebung, sodass Benutzer zwar drucken, aber nicht die Druckerwarteschlange anzeigen können. Benutzer, die versuchen, die Druckerwarteschlange anzuzeigen, erhalten eine Zugriffsverweigerungsmeldung.

Die Einstellung **Microsoft-Netzwerk (Server): Kommunikation digital signieren (immer)** ist für Druckserver in allen drei in diesem Handbuch definierten Umgebungen auf **Deaktiviert** gesetzt.

[Zum Seitenanfanq](#mainsection)  



### Ereignisprotokolleinstellungen

Die Ereignisprotokolleinstellungen für Druckserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“.

[Zum Seitenanfanq](#mainsection)  



### Zusätzliche Sicherheitseinstellungen

Obwohl die durch die Richtlinie für die Mitgliedsserver-Baseline angewendeten Sicherheitseinstellungen die Sicherheit der Druckserver bedeutend erhöhen, sind einige zusätzliche Einstellungen in Betracht zu ziehen. Die Einstellungen in diesem Abschnitt können nicht durch die Gruppenrichtlinie implementiert werden und müssen daher auf allen Druckservern manuell vorgenommen werden.


#### Sichern von bekannten Konten

Microsoft Windows Server 2003 mit SP1 verfügt über eine Reihe vordefinierter Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.

Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Daher sollten Sie das vordefinierte Administratorkonto umbenennen und seine Beschreibung ändern, damit sie Angriffen von Remoteservern vorbeugen und Angreifer dieses bekannte Konto nicht nutzen können.

Die Auswirkung dieser Konfigurationsänderung hat sich in den letzten Jahren nach dem Auftreten von Angriffstools verringert, die durch Angabe der Sicherheits-ID (SID) des vordefinierten Administratorkontos dessen wahren Namen in Erfahrung bringen und dadurch Zugriff auf den Server erhalten. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf dieses Administratorkonto überwachen, wenn Sie es umbenennen und mit einem eindeutigen Namen versehen.

**So sichern Sie bekannte Konten auf Druckservern**
* Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie danach die zugehörigen Kennwörter zu langen und komplexen Werten.

* Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server zugreifen.

* Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.

* Notieren Sie die vorgenommenen Änderungen, und bewahren Sie diese Informationen an einem sicheren Ort auf.

    **Hinweis**: Das vordefinierte Administratorkonto kann durch eine Gruppenrichtlinie umbenannt werden. Diese Einstellung wurde in den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen nicht implementiert, da jede Organisation einen eindeutigen Namen für dieses Konto auswählen sollte. Die Einstellung **Konten: Administratorkonto umbenennen** kann jedoch so konfiguriert werden, dass Administratorkonten in den drei in diesem Handbuch definierten Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.



#### Sichern von Dienstkonten

Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx.

[Zum Seitenanfanq](#mainsection)  



### Erstellen der Richtlinie mithilfe des SCW

Zum Bereitstellen der notwendigen Sicherheitseinstellungen müssen Sie sowohl den Sicherheitskonfigurations-Assistenten (SCW) sowie die im Rahmen der herunterladbaren Version dieses Handbuchs verfügbaren Sicherheitsvorlagen verwenden, um eine Serverrichtlinie zu erstellen.

Wenn Sie Ihre eigene Richtlinie erstellen, müssen Sie die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ überspringen. Diese Einstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den vom SCW konfigurierten Elementen haben.

Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie ähnliche Hardware wie in Ihrer Bereitstellungsumgebung verwenden, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.

**So erstellen Sie die Druckserverrichtlinie**
1. Erstellen Sie auf einem neuen Referenzcomputer eine neue Installation von Windows Server 2003 mit SP1.

2. Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.

3. Schließen Sie den Computer an die Domäne an, die sämtliche Sicherheitseinstellungen von den übergeordneten Organisationseinheiten übernehmen.

4. Installieren und konfigurieren Sie nur die obligatorischen Anwendungen, die sich auf allen Servern mit dieser Rolle befinden. Dazu zählen z. B. rollenspezifische Dienste, Software- und Verwaltungsagenten, Bandsicherungsagenten sowie Antiviren- und Antispywaredienstprogramme.

5. Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.

6. Stellen Sie sicher, dass die ermittelten Serverrollen auf Ihre Umgebung zutreffen, wie z. B. die Druckserverrolle.

7. Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.

8. Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.

9. Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.

10. Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.

11. Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter.**   Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.

12. Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.

13. Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.

14. Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. „Unternehmensclient - Druckserver.inf“).

15. Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Druckserver.xml).


#### Testen der Richtlinie mithilfe des SCW

Nach dem Erstellen und Speichern der Richtlinie empfiehlt es sich unbedingt, sie in Ihrer Testumgebung bereitzustellen. Im Idealfall werden Ihre Testserver die gleiche Hardware- und Softwarekonfiguration wie Ihre Produktionsserver aufweisen. Mit diesem Ansatz können Sie mögliche Probleme, wie etwa das Vorhandensein unerwarteter Dienste, die von bestimmten Hardwaregeräten benötigt werden, ermitteln und beheben.

Zum Testen der Richtlinie gibt es zwei Möglichkeiten. Sie können die standardmäßigen SCW-Bereitstellungsgeräte verwenden oder mithilfe eines Gruppenrichtlinienobjekts Richtlinien anwenden.

Beim Verfassen der Richtlinien sollten Sie zunächst die Verwendung der standardmäßigen SCW-Bereitstellungsgeräte in Betracht ziehen. Sie können eine Richtlinie mit dem SCW jeweils auf einen einzelnen Server oder mithilfe von Scwcmd auf eine ganze Servergruppe anwenden. Die standardmäßige Bereitstellungsmethode bietet den Vorteil, dass bereitgestellte Richtlinien leicht vom SCW aus zurückgenommen werden können. Dies erweist sich als außerordentlich nützlich, wenn Sie im Testverfahren mehrere Änderungen an Ihren Richtlinien vornehmen.

Die Richtlinie wird getestet, um sicherzustellen, dass ihre Anwendung auf den Zielservern keine negativen Auswirkungen auf wichtige Funktionen hat. Nach Übernahme der Konfigurationsänderungen müssen Sie zunächst die Kernfunktionalität des Computers überprüfen. Ist der Server z. B. als Zertifizierungsstelle (CA) konfiguriert, müssen Sie sicherstellen, dass Clients Zertifikate anfordern und erhalten bzw. eine Zertifikatsperrliste herunterladen können usw.

Wenn Sie mit der Konfiguration von Richtlinien vertraut sind, können Sie Scwcmd verwenden, um wie im folgenden Verfahren veranschaulicht die Richtlinien in Gruppenrichtlinienobjekte umzuwandeln.

Weitere Informationen zum Testen von SCW-Richtlinien finden Sie im [Security Configuration Wizard Documentation](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/scwdeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx">Deployment Guide for the Security Configuration Wizard unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/SCWDeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx** sowie in der 


#### Umwandeln und Bereitstellen der Richtlinie

Nachdem Sie die Richtlinie gründlich getestet haben, führen Sie folgende Schritte aus, um sie in ein Gruppenrichtlinienobjekt umzuwandeln und bereitzustellen:
1. Geben Sie an der Eingabeaufforderung folgenden Befehl ein:

    `scwcmd transform /p:<PathToPolicy.xml> /g:<GPODisplayName>`

    und drücken Sie anschließend die Eingabetaste. Beispiel:
 
    ```
    scwcmd transform /p:"C:\Windows\Security\msscw\Policies\Print 
    Server.xml" /g:"Print Server Policy"
    ```

    **Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.

2. Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der jeweiligen Organisationseinheit.


Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall.**  

Anschließend sollten Sie eine endgültige Prüfung vornehmen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Einstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Einstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.

[Zum Seitenanfanq](#mainsection)  



### Zusammenfassung

In diesem Kapitel wurden die Richtlinieneinstellungen behandelt, die in den drei in diesem Handbuch definierten Umgebungen für Druckserver verwendet werden können, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die meisten Richtlinieneinstellungen werden durch ein Gruppenrichtlinienobjekt angewendet, das zur Ergänzung der Richtlinie für die Mitgliedsserver-Baseline entwickelt wurde. Gruppenrichtlinienobjekte können zur Erhöhung der Sicherheit mit den jeweiligen die Druckserver enthaltenden Organisationseinheiten verknüpft werden.

Einige Richtlinieneinstellungen können nicht über Gruppenrichtlinien angewendet werden. Für diese Richtlinieneinstellungen wurden Informationen für die manuelle Konfiguration bereitgestellt.


#### Weitere Informationen

Die folgenden Links bieten zusätzliche Informationen zur Absicherung von Druckservern, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
* Einen Überblick über Druckserver erhalten Sie im Artikel „[Technischer Überblick über Windows Server 2003-Druckdienste](http://www.microsoft.com/windowsserver2003/techinfo/overview/print.mspx)“ (in englischer Sprache), der unter folgender Adresse verfügbar ist: www.microsoft.com/windowsserver2003/techinfo/overview/print.mspx.

* Weitere Informationen zu Druckservern finden Sie im Artikel „[Neuerungen bei Datei- und Druckdiensten](http://www.microsoft.com/windowsserver2003/evaluation/overview/technologies/fileandprint.mspx)“ (in englischer Sprache) unter www.microsoft.com/windowsserver2003/evaluation/overview/technologies/  
fileandprint.mspx.

 
[Zum Seitenanfanq](#mainsection)

In diesem Beitrag
* [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))
* [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))
* [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))
* [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))
* [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))
* [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))
* [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))
* [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))
* Kapitel 8: Die Druckserverrolle
* [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))
* [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))
* [Kapitel 11: Die Zertifikatdienstserverrolle](https://technet.microsoft.com/de-de/library/7488b1dc-eb9b-4f4a-b597-b84d87717b57(v=TechNet.10))
* [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))
* [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))
* [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))
* [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))
* [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))
* [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))
* [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
 

**Download**  


[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&amp;clcid=0x409)

**Benachrichtigung über Neuerungen**  


[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)

**Feedback**  


[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows server 2003 security guide)

 

<table style="border:1px solid black;">

<tr>

<td style="border:1px solid black;">

[Zum Seitenanfanq](#mainsection)

</td>

<td style="border:1px solid black;">

[![](https://technet.microsoft.com/de-de/Dd443729.pageLeft(de-de,TechNet.10).gif "Dd443729.pageLeft(de-de,TechNet.10).gif")](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))
9 von 19[![](https://technet.microsoft.com/de-de/Dd443729.pageRight(de-de,TechNet.10).gif "Dd443729.pageRight(de-de,TechNet.10).gif")](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))

</td>

</tr>

</table>