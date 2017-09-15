---
TOCTitle: 'Kapitel 7: Die Dateiserverrolle'
Title: 'Kapitel 7: Die Dateiserverrolle'
ms:assetid: '2b1536d0-9610-4fb5-93b4-72f62d9e2ff3'
ms:contentKeyID: 20075671
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443728(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 7: Die Dateiserverrolle

Aktualisiert: 27.12.2005

##### Auf dieser Seite

[](#ehaa)[Überblick](#ehaa)
[](#egaa)[Einstellungen für Überwachungsrichtlinien](#egaa)
[](#efaa)[Zuweisen von Benutzerrechten](#efaa)
[](#eeaa)[Sicherheitsoptionen](#eeaa)
[](#edaa)[Ereignisprotokolleinstellungen](#edaa)
[](#ecaa)[Zusätzliche Sicherheitseinstellungen](#ecaa)
[](#ebaa)[Erstellen der Richtlinie mithilfe des SCW](#ebaa)
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Die Absicherung von Dateiservercomputern unter Microsoft® Windows Server™ 2003 mit Service Pack 1 (SP1) kann sich als Herausforderung erweisen, da die grundlegenden von diesem Server bereitgestellten Dienste SMB (Server Message Block)- und CIFS (Common Internet File System)-Protokolle erfordern. Diese Protokolle können nicht authentifizierte Benutzer mit umfangreichen Informationen versorgen und sind in hochsicheren Windows-Umgebungen häufig deaktiviert. Es ist jedoch für Benutzer und Administratoren schwierig, auf Dateiserver zuzugreifen, wenn diese Protokolle deaktiviert sind.

Die meisten Richtlinieneinstellungen in diesem Kapitel werden durch die Gruppenrichtlinie konfiguriert und angewendet. Ein Gruppenrichtlinienobjekt (GPO), das die Richtlinie für die Mitgliedsserver-Baseline unterstützt, kann mit den jeweiligen die Dateiserver enthaltenden Organisationseinheiten verknüpft werden, um die für diese Serverrollen erforderlichen Sicherheitseinstellungen bereitzustellen. In diesem Kapitel werden nur die Richtlinieneinstellungen erläutert, die von der Richtlinie für die Mitgliedsserver-Baseline abweichen.

Sofern möglich, werden diese Richtlinieneinstellungen in einem inkrementellen Gruppenrichtlinienobjekt gesammelt, das auf die Dateiserver-Organisationseinheit angewendet wird. Einige Richtlinieneinstellungen in diesem Kapitel können nicht durch Gruppenrichtlinien angewendet werden. Ausführliche Informationen zur Konfiguration dieser manuellen Richtlinieneinstellungen werden bereitgestellt.

Die folgende Tabelle enthält die Namen der Sicherheitsvorlagen der Dateiserver für die drei in diesem Handbuch definierten Umgebungen. Diese Vorlagen stellen die Einstellungen für die inkrementelle Dateiservervorlage bereit, die wiederum zum Erstellen eines neuen Gruppenrichtlinienobjekts verwendet wird, das mit der Dateiserver-Organisationseinheit in der jeweiligen Umgebung verknüpft ist. In Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, finden Sie ausführliche Anweisungen, die Ihnen beim Erstellen von Organisationseinheiten und Gruppenrichtlinien und beim darauf folgenden Import der entsprechenden Sicherheitsvorlage in die einzelnen Gruppenrichtlinienobjekte helfen.

**Tabelle 7.1: Dateiserver-Sicherheitsvorlagen**

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Älterer Client</p></th>
<th><p>Unternehmensclient</p></th>
<th><p>Hochsicher (SSLF)</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Älterer Client - Dateiserver.inf</p></td>
<td style="border:1px solid black;"><p>Unternehmensclient - Dateiserver.inf</p></td>
<td style="border:1px solid black;"><p>Hochsicher - Dateiserver.inf</p></td>
</tr>  
</tbody>  
</table>
  
Informationen zu den Einstellungen in der Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Informationen zu sämtlichen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen für Windows Server 2003 und Windows XP*](http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx)*,* das unter *http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx* erhältlich ist.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Einstellungen für Überwachungsrichtlinien
  
Die Einstellungen für Überwachungsrichtlinien für Dateiserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie wird die Protokollierung der Sicherheitsüberwachungsinformationen auf allen Dateiservern aktiviert.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zuweisen von Benutzerrechten
  
Die Einstellungen für die Zuweisung von Benutzerrechten für Dateiserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie werden die Zuweisungen von Benutzerrechten auf allen Dateiservern einheitlich konfiguriert.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Sicherheitsoptionen
  
Die Einstellungen für die Sicherheitsoptionen für Dateiserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für diese Richtlinie werden die relevanten Sicherheitsoptionen auf allen Dateiservern einheitlich konfiguriert.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Ereignisprotokolleinstellungen
  
Die Ereignisprotokolleinstellungen für Dateiserver in den drei in diesem Handbuch definierten Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusätzliche Sicherheitseinstellungen
  
Obwohl die durch die Richtlinie für die Mitgliedsserver-Baseline angewendeten Sicherheitseinstellungen die Dateiserversicherheit bedeutend erhöhen, werden in diesem Abschnitt einige zusätzliche Überlegungen erörtert. Die Einstellungen in diesem Abschnitt können jedoch nicht über die Gruppenrichtlinie implementiert werden und müssen daher auf allen Dateiservern manuell durchgeführt werden.
  
#### Sichern von bekannten Konten
  
Windows Server 2003 mit SP1 verfügt über eine ganze Reihe von vordefinierten Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.
  
Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Daher sollten Sie das vordefinierte Administratorkonto umbenennen und seine Beschreibung ändern, damit sie Angriffen von Remoteservern vorbeugen und Angreifer dieses bekannte Konto nicht nutzen können.
  
Die Auswirkung dieser Konfigurationsänderung hat sich in den letzten Jahren nach dem Auftreten von Angriffstools verringert, die durch Angabe der Sicherheits-ID (SID) des vordefinierten Administratorkontos dessen wahren Namen in Erfahrung bringen und dadurch Zugriff auf den Server erhalten. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf dieses Administratorkonto überwachen, wenn Sie es umbenennen und mit einem eindeutigen Namen versehen.
  
**So sichern Sie bekannte Konten auf Dateiservern**
  
-   Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie danach die zugehörigen Kennwörter zu langen und komplexen Werten.
  
-   Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server zugreifen.
  
-   Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.
  
-   Notieren Sie die vorgenommenen Änderungen, und bewahren Sie diese Informationen an einem sicheren Ort auf.
  
    **Hinweis**: Das vordefinierte Administratorkonto kann durch eine Gruppenrichtlinie umbenannt werden. Diese Einstellung wurde in den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen nicht implementiert, da jede Organisation einen eindeutigen Namen für dieses Konto auswählen sollte. Sie können jedoch die Einstellung **Konten: Administratorkonto umbenennen** so konfigurieren, dass Administratorkonten in den drei in diesem Handbuch definierten Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.
  
#### Sichern von Dienstkonten
  
Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Erstellen der Richtlinie mithilfe des SCW
  
Zum Bereitstellen der notwendigen Sicherheitseinstellungen müssen Sie sowohl den Sicherheitskonfigurations-Assistenten (SCW) sowie die im Rahmen der herunterladbaren Version dieses Handbuchs verfügbaren Sicherheitsvorlagen verwenden, um eine Serverrichtlinie zu erstellen.
  
Wenn Sie Ihre eigene Richtlinie erstellen, müssen Sie die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ überspringen. Diese Einstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den vom SCW konfigurierten Elementen haben.
  
Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie das Betriebssystem auf ähnlicher Hardware wie der bei der Bereitstellung verwendeten installieren, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.
  
**So erstellen Sie die Dateiserverrichtlinie**
  
1.  Erstellen Sie auf einem neuen Referenzcomputer eine neue Installation von Windows Server 2003 mit SP1.
  
2.  Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.
  
3.  Schließen Sie den Computer an die Domäne an, die sämtliche Sicherheitseinstellungen von den übergeordneten Organisationseinheiten übernehmen.
  
4.  Installieren und konfigurieren Sie nur die obligatorischen Anwendungen, die sich auf allen Servern mit dieser Rolle befinden. Dazu zählen z. B. rollenspezifische Dienste, Software- und Verwaltungsagenten, Bandsicherungsagenten sowie Antiviren- und Antispywaredienstprogramme.
  
5.  Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.
  
6.  Stellen Sie sicher, dass die ermittelten Serverrollen auf Ihre Umgebung zutreffen, wie z. B. die Dateiserverrolle.
  
7.  Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.
  
8.  Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.
  
9.  Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.
  
10. Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.
  
11. Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter**. Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.
  
12. Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
13. Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
14. Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. „Unternehmensclient - Dateiserver.inf“).
  
15. Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Dateiserver.xml).
  
#### Testen der Richtlinie mithilfe des SCW
  
Nach dem Erstellen und Speichern der Richtlinie empfiehlt es sich unbedingt, sie in Ihrer Testumgebung bereitzustellen. Im Idealfall werden Ihre Testserver die gleiche Hardware- und Softwarekonfiguration wie Ihre Produktionsserver aufweisen. Mit diesem Ansatz können Sie mögliche Probleme, wie etwa das Vorhandensein unerwarteter Dienste, die von bestimmten Hardwaregeräten benötigt werden, ermitteln und beheben.
  
Zum Testen der Richtlinie gibt es zwei Möglichkeiten. Sie können die standardmäßigen SCW-Bereitstellungsgeräte verwenden oder mithilfe eines Gruppenrichtlinienobjekts Richtlinien anwenden.
  
Beim Verfassen der Richtlinien sollten Sie zunächst die Verwendung der standardmäßigen SCW-Bereitstellungsgeräte in Betracht ziehen. Sie können eine Richtlinie mit der SCW-Benutzeroberfläche jeweils auf einen einzelnen Server oder mithilfe von Scwcmd auf eine ganze Servergruppe anwenden. Mithilfe der standardmäßigen Bereitstellungsmethode können Sie aus SCW bereitgestellte Richtlinien einfach zurücknehmen. Dies erweist sich als außerordentlich nützlich, wenn Sie im Testverfahren mehrere Änderungen an Ihren Richtlinien vornehmen.
  
Die Richtlinie wird getestet, um sicherzustellen, dass ihre Anwendung auf den Zielservern keine negativen Auswirkungen auf wichtige Funktionen hat. Nach Übernahme der Konfigurationsänderungen müssen Sie zunächst die Kernfunktionalität des Computers überprüfen. Ist der Server z. B. als Zertifizierungsstelle (CA) konfiguriert, müssen Sie sicherstellen, dass Clients Zertifikate anfordern und erhalten bzw. eine Zertifikatsperrliste herunterladen können usw.
  
Wenn Sie mit der Konfiguration von Richtlinien vertraut sind, können Sie Scwcmd verwenden, um wie im folgenden Verfahren veranschaulicht die Richtlinien in Gruppenrichtlinienobjekte umzuwandeln.
  
Weitere Informationen zum Testen von SCW-Richtlinien finden Sie im [Deployment Guide for the Security Configuration Wizard](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/scwdeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/  
library/SCWDeploying/5254f8cd-143e-4559-a299-9c723b366946.mspx**sowie in der [Security Configuration Wizard Documentation](http://go.microsoft.com/fwlink/?linkid=43450) unter http://go.microsoft.com/fwlink/?linkid=43450 (jeweils in englischer Sprache).
  
#### Umwandeln und Bereitstellen der Richtlinie
  
Nachdem Sie die Richtlinie gründlich getestet haben, führen Sie folgende Schritte aus, um sie in ein Gruppenrichtlinienobjekt umzuwandeln und bereitzustellen:
  
1.  Geben Sie an der Eingabeaufforderung folgenden Befehl ein:
  
    ```  
 scwcmd transform /p:&lt;PathToPolicy.xml&gt; /g:&lt;GPODisplayName&gt;  
```
  
    und drücken Sie anschließend die Eingabetaste. Beispiel:
  
    ```  
 scwcmd transform /p:"C:\\Windows\\Security\\msscw\\Policies\\File Server.xml" /g:"File Server Policy"  
```
  
    **Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.
  
2.  Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der jeweiligen Organisationseinheit.
  
Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall**.
  
Anschließend sollten Sie eine endgültige Prüfung vornehmen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Einstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Einstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurden die Richtlinieneinstellungen behandelt, die in den drei in diesem Handbuch definierten Umgebungen für Dateiserver verwendet werden können, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die meisten Richtlinieneinstellungen werden durch ein Gruppenrichtlinienobjekt angewendet, das zur Ergänzung der Richtlinie für die Mitgliedsserver-Baseline entwickelt wurde. Gruppenrichtlinienobjekte können zur Erhöhung der Sicherheit mit den jeweiligen die Dateiserver enthaltenden Organisationseinheiten verknüpft werden.
  
Einige Richtlinieneinstellungen können durch die Gruppenrichtlinie nicht angewendet werden. Für diese Richtlinieneinstellungen wurden Informationen für die manuelle Konfiguration bereitgestellt.
  
#### Weitere Informationen
  
Die folgenden Links bieten zusätzliche Informationen zur Absicherung von Dateiservern, auf denen Windows Server 2003 mit SP1 ausgeführt wird.
  
-   Weitere Informationen zu Dateiservern finden Sie im Artikel „[Technischer Überblick über Windows Server 2003-Dateidienste](http://www.microsoft.com/windowsserver2003/techinfo/overview/file.mspx)“ (in englischer Sprache) unter www.microsoft.com/windowsserver2003/techinfo/overview/file.mspx.
  
-   Weitere Informationen zu DFS finden Sie im Whitepaper „[Verteiltes Dateisystem](http://www.microsoft.com/windows2000/techinfo/howitworks/fileandprint/dfsnew.asp)“ (in englischer Sprache) unter www.microsoft.com/windows2000/techinfo/howitworks/fileandprint/dfsnew.asp.
  
-   Weitere Informationen zu FRS finden Sie im Thema „[Dateireplikationsdienst](http://www.microsoft.com/windowsserversystem/storage/storservices.mspx#egbaaa)“ (in englischer Sprache) unter www.microsoft.com/windowsserversystem/storage/storservices.mspx\#EGBAAA.
  
[](#mainsection)[Zum Seitenanfang](#mainsection)
  
##### In diesem Beitrag
  
-   [Überblick](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/sgch00.mspx)  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch01.mspx)  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch02.mspx)  
-   [Kapitel 3: Die Domänenrichtlinie](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch03.mspx)  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch04.mspx)  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch05.mspx)  
-   [Kapitel 6: Die Infrastrukturserverrolle](http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch06.mspx)  
-   Kapitel 7: Die Dateiserverrolle  
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
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch06.mspx"><img src="images/Dd443728.pageLeft(de-de,TechNet.10).gif" /></a> 8 von 19 <a href="http://www.microsoft.com/germany/technet/sicherheit/prodtech/windowsserver2003/w2003hg/s3sgch08.mspx"><img src="images/Dd443728.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>  
</tbody>  
</table>
