---
TOCTitle: 'Kapitel 6: Die Infrastrukturserverrolle'
Title: 'Kapitel 6: Die Infrastrukturserverrolle'
ms:assetid: '5914ba9b-2fe2-4886-8171-a908521836ec'
ms:contentKeyID: 20075670
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443727(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 6: Die Infrastrukturserverrolle

Aktualisiert : Januar 1, 1

##### Auf dieser Seite

[](#ehaa)[Überblick](#ehaa)
[](#egaa)[Einstellungen für Überwachungsrichtlinien](#egaa)
[](#efaa)[Einstellungen zum Zuweisen von Benutzerrechten](#efaa)
[](#eeaa)[Sicherheitsoptionen](#eeaa)
[](#edaa)[Ereignisprotokolleinstellungen](#edaa)
[](#ecaa)[Zusätzliche Sicherheitseinstellungen](#ecaa)
[](#ebaa)[Erstellen der Richtlinie mithilfe des SCW](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

In diesem Kapitel werden die Richtlinieneinstellungen erklärt, die in den drei in diesem Handbuch definierten Umgebungen zum Absichern von Infrastrukturservern, auf denen Microsoft® Windows Server™ 2003 mit Service Pack 1 (SP1) ausgeführt wird, verwendet werden können. In diesem Handbuch sind mit Infrastrukturservern Server gemeint, der DHCP-Dienste oder Microsoft-WINS-Funktionen bereitstellen.

Die meisten Einstellungen in diesem Kapitel werden durch Gruppenrichtlinien konfiguriert und angewendet. Ein Gruppenrichtlinienobjekt (GPO), das die Richtlinie für die Mitgliedsserver-Baseline (MSBP) unterstützt, kann mit den entsprechenden die Infrastrukturserver enthaltenden Organisationseinheiten (OUs) verknüpft werden, um die Sicherheit der Server zu erhöhen. In diesem Kapitel werden nur die Richtlinieneinstellungen erläutert, die von der Richtlinie für die Mitgliedsserver-Baseline abweichen.

Sofern möglich, werden diese Richtlinieneinstellungen in einem inkrementellen Gruppenrichtlinienobjekt gesammelt, das auf die Infrastrukturserver-Organisationseinheit angewendet wird. Einige Einstellungen in diesem Kapitel können nicht durch Gruppenrichtlinien angewendet werden. Ausführliche Informationen zur Konfiguration dieser manuellen Einstellungen werden bereitgestellt.

Die folgende Tabelle zeigt die Namen der Sicherheitsvorlagen für Infrastrukturserver für die drei in diesem Handbuch definierten Umgebungen. Diese Vorlagen stellen die Richtlinieneinstellungen für die inkrementelle Infrastrukturservervorlage bereit, die wiederum zum Erstellen eines neuen GPO verwendet wird, das mit der Infrastrukturserver-Organisationseinheit in der jeweiligen Umgebung verknüpft ist. In Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, finden Sie ausführliche Anweisungen, die Ihnen beim Erstellen von Organisationseinheiten und Gruppenrichtlinien und beim darauf folgenden Import der entsprechenden Sicherheitsvorlage in die einzelnen Gruppenrichtlinienobjekte helfen.

**Tabelle 6.1: Sicherheitsvorlagen und Richtlinien für Infrastrukturserver**

 
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
<td style="border:1px solid black;">Älterer Client - Infrastrukturserver.inf</td>
<td style="border:1px solid black;">Unternehmensclient - Infrastrukturserver.inf</td>
<td style="border:1px solid black;">Hochsicher - Infrastrukturserver.inf</td>
</tr>
</tbody>
</table>
  
Informationen zu den Einstellungen in der Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Informationen zu sämtlichen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen für Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))*,*das unter *http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx* erhältlich ist.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Einstellungen für Überwachungsrichtlinien
  
Die Einstellungen für Überwachungsrichtlinien für Infrastrukturserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie wird die Protokollierung für die relevanten Sicherheitsüberwachungsinformationen auf Infrastrukturservern aktiviert.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Einstellungen zum Zuweisen von Benutzerrechten
  
Die Zuweisungen von Benutzerrechten für Infrastrukturserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie werden die Zuweisungen von Benutzerrechten auf allen Infrastrukturenservern einheitlich konfiguriert.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Sicherheitsoptionen
  
Die Einstellungen für Sicherheitsoptionen für Infrastrukturserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie werden die relevanten Sicherheitsoptionseinstellungen auf allen Infrastrukturenservern einheitlich konfiguriert.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Ereignisprotokolleinstellungen
  
Die Ereignisprotokolleinstellungen für Infrastrukturserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusätzliche Sicherheitseinstellungen
  
Die von der Richtlinie für die Mitgliedsserver-Baseline angewendeten Sicherheitseinstellungen erhöhen die Sicherheit von Infrastrukturservern deutlich. In diesem Abschnitt werden einige zusätzliche Einstellungen in Betracht gezogen. Die Einstellungen in diesem Abschnitt können nicht über Gruppenrichtlinien konfiguriert werden, sondern müssen auf allen Infrastrukturservern manuell konfiguriert werden.
  
#### Konfigurieren der DHCP-Protokollierung
  
Standardmäßig protokolliert der DHCP-Dienst nur das Starten und Herunterfahren als Ereignis im Ereignisprotokoll. Führen Sie die folgenden Schritte aus, um ein detaillierteres Protokoll auf dem DHCP-Server zu aktivieren:
  
1.  Klicken Sie im DHCP-Verwaltungstool mit der rechten Maustaste auf den DHCP-Server.
  
2.  Wählen Sie **Eigenschaften** aus.
  
3.  Klicken Sie auf der Registerkarte **Allgemein** des Dialogfelds **Eigenschaften** auf **DHCP-Überwachungsprotokollierung aktivieren**.
  
Nach dem Ausführen dieser Schritte erstellt der DHCP-Server in folgendem Verzeichnis eine Protokolldatei:
  
**%systemroot%\\system32\\dhcp\\**
  
Die Informationen zum DHCP-Client sind in Protokolldateien oft schwer zu finden, weil die meisten Protokolle nur die Computernamen und keine IP-Adressen speichern. Die DHCP-Überwachungsprotokolle stellen ein zusätzliches Tool für das Auffinden der Quellen interner Angriffe oder unbeabsichtigter Aktivitäten bereit.
  
Die Informationen in diesen Protokollen sind jedoch nicht absolut sicher, da sowohl Hostnamen als auch MAC-Adressen (Media Access Control) gefälscht und vorgetäuscht werden können. (Beim Spoofing wird bei einer Übertragung ein anderer Benutzer als Sender angezeigt, als der Benutzer, der die Übertragung tatsächlich ausgeführt hat.) Die durch diese Informationen entstandenen Vorteile überwiegen jedoch die Nachteile in Form der durch eine aktivierte Protokollierung auf einem DHCP-Server verursachten Kosten. Beim Nachverfolgen des Einsatzes einer bestimmten IP-Adresse kann es sehr nützlich sein, mehr als nur eine IP-Adresse und einen Computernamen zu haben.
  
Standardmäßig besitzen die Gruppen **Server-Operatoren** und **Authentifizierte Benutzer** Leseberechtigungen für die DHCP-Protokolldateien. Um die Integrität der von einem DHCP-Server protokollierten Informationen zu wahren, wird empfohlen, den Zugriff auf diese Protokolle auf die Serveradministratoren zu beschränken. Die Gruppen **Server-Operatoren** und **Authentifizierte Benutzer** sollten aus der Zugriffssteuerungsliste (ACL) des Ordners **%systemroot%\\system32\\dhcp\\** entfernt werden.
  
Theoretisch könnten die DHCP-Überwachungsprotokolle die Festplatte füllen, auf der sie gespeichert sind. Die Standardkonfiguration für die Einstellung der **DHCP-Überwachungsprotokollierung** stellt daher sicher, dass die Protokollierung angehalten wird, wenn weniger als 20 MB freier Speicherplatz auf dem Server verfügbar sind. Diese Standardkonfiguration ist für Server in den meisten Umgebungen ausreichend. Sie können sie jedoch ändern, wenn Sie genügend Speicherplatz für andere Anwendungen auf dem Server sicherstellen möchten. Informationen zum Ändern dieser Konfiguration finden Sie auf der Seite [DhcpLogMinSpaceOnDisk](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/depkit/f7802dce-3ff9-406a-b3e6-c0c6b3ed4941.mspx) im Windows Server 2003 Tech Center unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/  
DepKit/f7802dce-3ff9-406a-b3e6-c0c6b3ed4941.mspx.
  
#### Schützen vor DHCP-DoS-Angriffen
  
Da DHCP-Server wichtige Ressourcen sind, die den Clientzugriff auf das Netzwerk sicherstellen, können sie Hauptziele für einen DoS-Angriff darstellen. Wenn ein DHCP-Server angegriffen wird und nicht in der Lage ist, DHCP-Anforderungen zu verarbeiten, können die DHCP-Clients möglicherweise keine Leases mehr abrufen. Diese Clients verlieren dann ihre vorhandenen IP-Leases und können nicht mehr auf das Netzwerk zugreifen.
  
Es wäre nicht sehr schwierig, ein Angriffstoolskript zu schreiben, das alle verfügbaren Adressen auf einem DHCP-Server anfordert. Ein solches Skript würde den Vorrat an verfügbaren IP-Adressen für nachfolgende legitime Abfragen von DHCP-Clients erschöpfen. Ein böswilliger Benutzer kann auch alle DHCP-IP-Adressen im Netzwerkadapter eines von diesen Adressen verwalteten Computers konfigurieren, wodurch der DHCP-Server IP-Adressenkonflikte in seinem Bereich feststellen und keine DHCP-Leases mehr zuordnen würde.
  
Darüber hinaus könnte ein DoS-Angriff (z. B. eine CPU-Überlastung oder ein Füllen des Anforderungspuffers des DHCP-Empfängers), der die Möglichkeit des DHCP-Servers, auf legitimen Verkehr zu antworten, erschöpft, es wie bei allen anderen Netzwerkdiensten für Clients unmöglich machen, Leases oder Erneuerungen anzufordern. Diese Art von Problem kann durch eine entsprechende Gestaltung der DHCP-Dienste vermieden werden.
  
Sie können DHCP-Server paarweise konfigurieren und die empfohlene Vorgehensweise der 80-20-Regel befolgen, d. h. der Bereich des DHCP-Servers wird auf mehrere Server aufgeteilt, sodass 80 % der Adressen von einem DHCP-Server verteilt werden und 20 % von einem anderen. Dadurch werden die Auswirkungen von Angriffen dieser Art verringert. Diese Konfigurationsempfehlungen sollen auch sicherstellen, dass Clients im Falle eines Serverausfalls weiterhin IP-Adressenkonfigurationen erhalten. Weitere Informationen zur 80-20-Regel und das DHCP-Protokoll finden Sie auf der Seite [DHCP](http://www.microsoft.com/resources/documentation/windows/2000/server/reskit/en-us/default.asp?url=/resources/documentation/windows/2000/server/reskit/en-us/cnet/cncb_dhc_klom.asp) im Windows 2000 Server Resource Kit unter www.microsoft.com/resources/documentation/Windows/2000/server/  
reskit/en-us/cnet/cncb\_dhc\_klom.asp.
  
**Hinweis**: Die im Windows 2000 Server Resource Kit beschriebene 80-20-Regel gilt auch für DHCP-Dienste in Windows Server 2003 mit SP1.
  
#### Sichern von bekannten Konten
  
Windows Server 2003 mit SP1 verfügt über eine ganze Reihe von vordefinierten Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.
  
Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Daher sollten Sie das vordefinierte Administratorkonto umbenennen und seine Beschreibung ändern, damit sie Angriffen von Remoteservern vorbeugen und Angreifer dieses bekannte Konto nicht nutzen können.
  
Die Auswirkung dieser Konfigurationsänderung hat sich in den letzten Jahren nach dem Auftreten von Angriffstools verringert, die durch Angabe der Sicherheits-ID (SID) des vordefinierten Administratorkontos dessen wahren Namen in Erfahrung bringen und dadurch Zugriff auf den Server erhalten. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf dieses Administratorkonto überwachen, wenn Sie es umbenennen und mit einem eindeutigen Namen versehen.
  
**So sichern Sie bekannte Konten auf Infrastrukturservern**
  
-   Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie die zugehörigen Kennwörter zu langen und komplexen Werten.
  
-   Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server mit dem gleichen Kontonamen und Kennwort zugreifen.
  
-   Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.
  
-   Notieren Sie die vorgenommenen Änderungen, und bewahren Sie diese Informationen an einem sicheren Ort auf.
  
    **Hinweis**: Das vordefinierte Administratorkonto kann durch Gruppenrichtlinien umbenannt werden. Diese Richtlinieneinstellung wurde in den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen nicht implementiert, da jede Organisation Ihren eigenen eindeutigen Namen für dieses Konto auswählen sollte. Sie können jedoch die Einstellung **Konten: Administratorkonto umbenennen** so konfigurieren, dass Administratorkonten in den drei in diesem Handbuch definierten Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.
  
#### Sichern von Dienstkonten
  
Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Erstellen der Richtlinie mithilfe des SCW
  
Zum Bereitstellen der notwendigen Sicherheitseinstellungen müssen Sie sowohl den Sicherheitskonfigurations-Assistenten (SCW) sowie die im Rahmen der herunterladbaren Version dieses Handbuchs verfügbaren Sicherheitsvorlagen verwenden, um eine Serverrichtlinie zu erstellen.
  
Wenn Sie Ihre eigene Richtlinie erstellen, müssen Sie die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ überspringen. Diese Richtlinieneinstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den vom SCW konfigurierten Elementen haben.
  
Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie das Betriebssystem auf ähnlicher Hardware wie der bei der Bereitstellung verwendeten installieren, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.
  
Während der Erstellung einer Serverrichtlinie entfernen Sie wahrscheinlich die Dateiserverrolle aus der Liste mit den erkannten Rollen. Diese Rolle wird häufig auf Servern konfiguriert, die sie nicht benötigen. Sie könnte als Sicherheitsrisiko betrachtet werden. Um die Dateiserverrolle für Server zu aktivieren, die sie benötigen, können Sie zu einem späteren Zeitpunkt eine zweite Richtlinie anwenden.
  
**So erstellen Sie die Infrastrukturserverrichtlinie**
  
1.  Erstellen Sie auf einem neuen Referenzcomputer eine neue Installation von Windows Server 2003 mit SP1.
  
2.  Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.
  
3.  Schließen Sie den Computer an die Domäne an, die sämtliche Sicherheitseinstellungen von den übergeordneten Organisationseinheiten übernehmen.
  
4.  Installieren und konfigurieren Sie nur die obligatorischen Anwendungen, die sich auf allen Servern mit dieser Rolle befinden. Dazu zählen z. B. rollenspezifische Dienste, Software- und Verwaltungsagenten, Bandsicherungsagenten sowie Antiviren- und Antispywaredienstprogramme.
  
5.  Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.
  
6.  Stellen Sie sicher, dass die ermittelten Serverrollen auf Ihre Umgebung zutreffen, wie z. B. die Rollen der DHCP-Server und WINS-Server.
  
7.  Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.
  
8.  Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.
  
9.  Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.
  
10. Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.
  
11. Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter**. Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.
  
12. Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
13. Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
14. Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. „Unternehmensclient - Infrastrukturserver.inf“).
  
15. Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Infrastrukturserver.xml).
  
#### Testen der Richtlinie mithilfe des SCW
  
Nach dem Erstellen und Speichern der Richtlinie empfiehlt es sich unbedingt, sie in Ihrer Testumgebung bereitzustellen. Im Idealfall werden Ihre Testserver die gleiche Hardware- und Softwarekonfiguration wie Ihre Produktionsserver aufweisen. Mit diesem Ansatz können Sie mögliche Probleme, wie etwa das Vorhandensein unerwarteter Dienste, die von bestimmten Hardwaregeräten benötigt werden, ermitteln und beheben.
  
Zum Testen der Richtlinie gibt es zwei Möglichkeiten. Sie können die standardmäßigen SCW-Bereitstellungsgeräte verwenden oder mithilfe eines Gruppenrichtlinienobjekts Richtlinien anwenden.
  
Beim Verfassen der Richtlinien sollten Sie zunächst die Verwendung der standardmäßigen SCW-Bereitstellungsgeräte in Betracht ziehen. Sie können eine Richtlinie mit dem SCW jeweils auf einen einzelnen Server oder mithilfe von Scwcmd auf eine ganze Servergruppe anwenden. Mithilfe der standardmäßigen Bereitstellungsmethode können Sie aus SCW bereitgestellte Richtlinien einfach zurücknehmen. Dies erweist sich als außerordentlich nützlich, wenn Sie im Testverfahren mehrere Änderungen an Ihren Richtlinien vornehmen.
  
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
 scwcmd transform /p:"C:\\Windows\\Security\\msscw\\Policies\\Infrastructure.xml" /g:"Infrastructure Policy"  
```
  
    **Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.
  
2.  Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der jeweiligen Organisationseinheit.
  
Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall**.
  
Anschließend sollten Sie eine endgültige Prüfung vornehmen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Richtlinieneinstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Richtlinieneinstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurden die Richtlinieneinstellungen behandelt, die in den drei in diesem Handbuch definierten Umgebungen für DHCP- und WINS-Server verwendet werden können, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die meisten Einstellungen für diese Rollen werden über die Richtlinie für die Mitgliedsserver-Baseline angewendet. Das Hauptziel beim Erstellen eines Infrastrukturrichtlinienobjekts für die DHCP- und WINS-Server besteht darin sicherzustellen, dass die notwendigen Dienste für diese Rollen voll funktionsfähig und umfassend geschützt sind.
  
Obwohl die Richtlinie für die Mitgliedsserver-Baseline ein hohes Maß an Sicherheit bietet, wurden in diesem Kapitel auch andere Überlegungen zu Rollen für Infrastrukturenserver erläutert. Zu diesen Überlegungen zählt in erster Linie die Erstellung von Protokolldateien.
  
#### Weitere Informationen
  
Die folgenden Links bieten weitere Informationen zur Absicherung von Infrastrukturservern, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
  
-   Informationen dazu, welche Änderungen die DHCP-Protokollierung in Windows Server 2003 erfahren hat, finden Sie im Microsoft Knowledge Base-Artikel „[Änderungen bei der DHCP-Protokollierung unter Windows Server 2003](http://support.microsoft.com/kb/328891/en-us)“ (in englischer Sprache) unter http://support.microsoft.com/kb/328891/en-us.
  
-   Weitere Informationen zu DHCP finden Sie auf der Seite [Dynamic Host Configuration Protocol](http://www.microsoft.com/resources/documentation/windows/2000/server/reskit/en-us/default.asp?url=/resources/documentation/windows/2000/server/reskit/en-us/cnet/cncb_dhc_klom.asp) (in englischer Sprache) unter www.microsoft.com/resources/documentation/Windows/2000/server/reskit/en-us/cnet/cncb\_dhc\_klom.asp.
  
-   Weitere Informationen zu WINS finden Sie unter „[Windows 2000 Server Windows Internet Naming Service (WINS) Overview](http://www.microsoft.com/technet/archive/windows2000serv/evaluate/featfunc/nt5wins.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/archive/windows2000serv/evaluate/featfunc/nt5wins.mspx.
  
-   Informationen zum Installieren von WINS in Windows Server 2003 finden Sie auf der Seite „[Installieren und Verwalten von WINS-Servern](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/a29d0a59-8bdd-4a82-a980-b53bd72fcb0e.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/a29d0a59-8bdd-4a82-a980-b53bd72fcb0e.mspx.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))  
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))  
-   Kapitel 6: Die Infrastrukturserverrolle  
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
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))  
-   [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
  
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10)"><img src="images/Dd443727.pageLeft(de-de,TechNet.10).gif" /></a> 7 von 19 <a href="https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10)"><img src="images/Dd443727.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>
