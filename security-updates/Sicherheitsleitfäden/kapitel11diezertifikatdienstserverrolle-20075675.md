---
TOCTitle: 'Kapitel 11: Die Zertifikatdienstserverrolle'
Title: 'Kapitel 11: Die Zertifikatdienstserverrolle'
ms:assetid: '7488b1dc-eb9b-4f4a-b597-b84d87717b57'
ms:contentKeyID: 20075675
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Dd443732(v=TechNet.10)'
---

Windows Server 2003-Sicherheitshandbuch
=======================================

### Kapitel 11: Die Zertifikatdienstserverrolle

Aktualisiert: 27.12.2005

##### Auf dieser Seite

[](#eiaa)[Überblick](#eiaa)  
[](#ehaa)[Einstellungen für Überwachungsrichtlinien](#ehaa)  
[](#egaa)[Zuweisen von Benutzerrechten](#egaa)  
[](#efaa)[Sicherheitsoptionen](#efaa)  
[](#eeaa)[Ereignisprotokolleinstellungen](#eeaa)  
[](#edaa)[Zusätzliche Registrierungseinträge](#edaa)  
[](#ecaa)[Zusätzliche Sicherheitseinstellungen](#ecaa)  
[](#ebaa)[Erstellen der Richtlinie mithilfe des SCW](#ebaa)  
[](#eaaa)[Zusammenfassung](#eaaa)

### Überblick

Dieses Kapitel enthält Anweisungen für die Absicherung von Servern in Ihrer Umgebung, auf denen Microsoft® Windows Server™ 2003 mit Service Pack 1 (SP1) und Microsoft-Zertifikatdienste ausgeführt werden. Obwohl dieses Kapitel alle Informationen für ein erfolgreiches Absichern dieser Servertypen enthält, sind darin keine detaillierten Informationen zur Erstellung einer sicheren Zertifikatdienstinfrastruktur in Ihrer Umgebung oder zur Bereitstellung einer Zertifizierungsstelle (CA) enthalten. Diese Themen werden in der Produktdokumentation zu Windows Server 2003 ausführlich behandelt. Sie werden darüber hinaus im *Windows Server 2003 Ressource Kit* sowie in Whitepapers diskutiert, die auf der Microsoft-Website verfügbar sind. Weitere Informationen finden Sie im Begleithandbuch [*Sichern von Wireless LANs mit Zertifikatsdiensten*](http://go.microsoft.com/fwlink/?linkid=14843), das unter http://go.microsoft.com/fwlink/?LinkId=14843 verfügbar ist.

Die Einstellungen in diesem Kapitel werden durch Gruppenrichtlinien konfiguriert und angewendet. Ein Gruppenrichtlinienobjekt (GPO), das die Richtlinie für die Mitgliedsserver-Baseline unterstützt, kann mit den jeweiligen die Zertifizierungsstellenserver enthaltenden Organisationseinheiten verknüpft werden, um die für diese Serverrollen erforderlichen Sicherheitseinstellungsänderungen bereitzustellen. In diesem Kapitel werden nur die Richtlinieneinstellungen erläutert, die von der Richtlinie für die Mitgliedsserver-Baseline abweichen.

Sofern möglich, werden diese Richtlinieneinstellungen in einer inkrementellen Gruppenrichtlinienvorlage gesammelt, die auf die Zertifizierungsstellenserver-Organisationseinheit angewendet wird. Einige Einstellungen in diesem Kapitel können nicht durch Gruppenrichtlinien angewendet werden. Ausführliche Informationen zur Konfiguration dieser manuellen Einstellungen werden bereitgestellt.

Der Name der Zertifizierungsstellenserver-Sicherheitsvorlage für die Unternehmensclient-Umgebung lautet „Unternehmensclient - Zertifizierungsstellenserver.inf“. Dabei handelt es sich um die inkrementelle Zertifizierungsstellenserver-Vorlage, die zum Erstellen eines neuen Gruppenrichtlinienobjekts verwendet wird, das mit der Zertifizierungsstellenserver-Organisationseinheit in der jeweiligen Umgebung verknüpft wird. In Kapitel 2, „Absicherungsmechanismen von Windows Server 2003“, finden Sie ausführliche Anweisungen, die Ihnen beim Erstellen von Organisationseinheiten und Gruppenrichtlinien und beim darauf folgenden Import der entsprechenden Sicherheitsvorlage in die einzelnen Gruppenrichtlinienobjekte helfen.

Informationen zu den Einstellungen in der Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Informationen zu sämtlichen Standardeinstellungen finden Sie im Begleithandbuch [*Bedrohungen und Gegenmaßnahmen: Sicherheitseinstellungen für Windows Server 2003 und Windows XP*](https://technet.microsoft.com/de-de/library/fb31fa9b-58c8-4b6c-aa93-f49128e79916(v=TechNet.10))*,* das unter *http://www.microsoft.com/germany/technet/sicherheit/topics/serversecurity/tcg/tcgch00.mspx* verfügbar ist.

**Hinweis**: Die Einstellungsempfehlungen für die Zertifikatdienstserverrolle wurden nur für die Unternehmensclient-Umgebung geprüft. Aus diesem Grund sind die Informationen zum Denial-of-Service (DoS), die für die meisten anderen Serverrollen in diesem Handbuch angegeben wurden, in diesem Kapitel nicht enthalten.

Sie können u. U. die Microsoft Internet Information Services (IIS) auf einigen der Zertifikatdienstserver in Ihrer Umgebung installieren, damit diese Server Zertifizierungsstellenzertifikate und Zertifikatssperrlisten (Certificate Revocation List, CRL) verteilen können. IIS wird auch zum Hosten jener Webregistrierungsseiten der Zertifikatdienstserver verwendet, die Microsoft Windows®-fremden Clients das Registrieren von Zertifikaten ermöglichen. Bevor Sie die Anweisungen in diesem Kapitel befolgen, stellen Sie sicher, dass Sie mit der Installation von IIS vertraut sind, die in Kapitel 9, „Die Webserverrolle“, dieses Handbuchs beschrieben wird. Wenn Sie IIS in ihren Zertifizierungsstellen installieren, muss die für Kapitel 9 entwickelte Sicherheitskonfigurationsvorlage auf die Zertifikatdienstserver angewendet werden, bevor Sie die in diesem Kapitel empfohlenen Einstellungen konfigurieren.

**Hinweis**: In vereinfachten Umgebungen kann der ausstellende Zertifizierungsstellenserver verwendet werden, um den Webserver, das Zertifizierungsstellenzertifikat und die CRL-Downloadpunkte zu hosten. In Ihrer Umgebung sollten Sie jedoch u. U. einen separaten Webserver verwenden, um die Sicherheit Ihrer Zertifizierungsstellen zu verbessern.

IIS wird verwendet, um die Registrierungsseiten des Zertifikatservers zur Verfügung zu stellen und Zertifizierungsstellenzertifikate und CRL-Downloadpunkte für Windows-fremde Clients zu verteilen. Es wird empfohlen, IIS nicht auf dem Stammzertifizierungsstellenserver zu installieren. Sie sollten IIS nach Möglichkeit nicht auf Ihrer ausstellenden Zertifizierungsstelle oder einer Zwischenzertifizierungsstelle in Ihrer Umgebung ausführen. Es ist sicherer, wenn Sie die Internet-Downloadpunkte für Zertifizierungsstellenzertifikate und CRLs auf einem anderen Server als dem Zertifizierungsstellenserver hosten. Viele Zertifikatbenutzer (interne und externe), die CRLs oder Zertifizierungsstellen-Ketteninformationen abrufen müssen, sollten u. U. keinen Zugriff auf die Zertifizierungsstelle erhalten. Sie können Benutzer allerdings nicht von der Zertifizierungsstelle fern halten, wenn Sie darauf die Downloadpunkte bereitstellen.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Einstellungen für Überwachungsrichtlinien

Die Einstellungen für Überwachungsrichtlinien für Zertifikatdienstserver in den in diesem Handbuch definierten Unternehmensclient-Umgebungen werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen der Richtlinie für die Mitgliedsserver-Baseline wird sichergestellt, dass alle relevanten Sicherheitsüberwachungsinformationen auf sämtlichen Zertifikatdienstservern erfasst werden.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Zuweisen von Benutzerrechten

Die Einstellungen zum Zuweisen von Benutzerrechten für Zertifikatdienstserver in der Unternehmensclient-Umgebung werden ebenfalls über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie in Kapitel 4, „Richtlinie für die Mitgliedsserver-Baseline“. Durch die Einstellungen für die Richtlinie für die Mitgliedsserver-Baseline wird sichergestellt, dass der entsprechende Zugriff auf Zertifikatdienstserver in einem Unternehmen einheitlich konfiguriert wird.

[](#mainsection)[Zum Seitenanfanq](#mainsection)

### Sicherheitsoptionen

Der Gruppenrichtlinienabschnitt zu Sicherheitsoptionen wird verwendet, um Sicherheitseinstellungen für Computer zu aktivieren oder zu deaktivieren, wie z. B. das digitale Signieren von Daten, die Namen des Administrator- und des Gastkontos, den Zugriff auf Disketten- und CD-ROM-Laufwerke, das Verhalten bei der Treiberinstallation sowie die Anmeldeaufforderungen.

Die Sicherheitsoptionen können unter Windows Server 2003 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:

**Computerkonfiguration\\Windows-Einstellungen\\Sicherheitseinstellungen\\Lokale Richtlinien\\**
**Sicherheitsoptionen**

Die folgende Tabelle enthält die empfohlenen Sicherheitsoptionseinstellungen für die Zertifikatdienstserverrolle in der Unternehmensclient-Umgebung. Ausführliche Informationen zur Einstellung werden im Text im Anschluss an die Tabelle bereitgestellt.

**Tabelle 11.1: Empfohlene Sicherheitsoptionseinstellungen**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Einstellung</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden</td>
<td style="border:1px solid black;">Aktiviert</td>
</tr>
</tbody>
</table>
  
#### Systemkryptografie: FIPS-konformen Algorithmus für Verschlüsselung, Hashing und Signatur verwenden
  
Durch diese Richtlinieneinstellung wird festgelegt, ob der TLS/SSL-Sicherheitsdienst nur die Verschlüsselungssammlung TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA unterstützt. Die Unterstützung dieser Verschlüsselungssammlung bedeutet, dass der Dienst das TLS-Protokoll nur als Client und als Server unterstützt (falls zutreffend).
  
Der TLS/SSL-Sicherheitsdienst verwendet folgende Algorithmen:
  
-   Den dreifachen DES-Verschlüsselungsalgorithmus (3DES) für die TLS-Verkehrverschlüsselung
  
-   Den auf öffentlichen Schlüsseln basierenden RSA-Algorithmus für TLS-Schlüsselaustausch und -Authentifizierung (RSA ist eine Verschlüsselungstechnologie, die von RSA Data Security, Inc. entwickelt wurde.)
  
-   Den SHA 1-Hashingalgorithmus für die TLS-Hashinganforderungen

Für den EFS-Dienst (Encrypting File System, verschlüsselndes Dateisystem) unterstützt der TLS/SSL-Sicherheitsdienst nur den dreifachen DES-Verschlüsselungsalgorithmus, um Dateidaten zu verschlüsseln, die im NTFS-Dateisystem von Windows gespeichert werden. Standardmäßig verwendet der EFS-Dienst den DESX-Algorithmus für die Verschlüsselung von Dateidaten.
  
Wenn Sie diese Richtlinieneinstellung aktivieren, verwenden Computer in dieser Serverrolle in Ihrer Umgebung die leistungsstärksten Algorithmen, die für die digitale Verschlüsselung sowie das Hashing und das Signieren zur Verfügung stehen. Durch die Verwendung dieser Algorithmen werden Risiken verringert, da sie unautorisierte Benutzer am Missbrauch digital verschlüsselter oder signierter Daten hindern.
  
Deshalb ist die Einstellung **Systemkryptografie: IPS-konformen Algorithmus für Verschlüsselung,** **Hashingund Signatur verwenden** für die Unternehmensclient-Umgebung auf **Aktiviert** gesetzt.
  
**Hinweis**: Clientcomputer, auf denen diese Richtlinieneinstellung aktiviert ist, können mit Servern, die diese Algorithmen nicht unterstützen, nicht über digital verschlüsselte oder signierte Protokolle kommunizieren. Die Netzwerkclientcomputer, die diese Algorithmen nicht unterstützen, können keine Server verwenden, die diese Algorithmen für die Netzwerkkommunikation erfordern. Viele Apache-basierte Webserver sind z. B. nicht für eine Unterstützung der TLS-Protokolle konfiguriert.
  
Wenn Sie diese Einstellung aktivieren, müssen Sie auch den Internet Explorer für TLS konfigurieren. Öffnen Sie zu diesem Zweck das Dialogfeld **Internetoptionen** im Menü **Extras** von Internet Explorer, klicken Sie auf die Registerkarte **Erweitert**, gehen Sie zum Ende der Liste **Einstellungen**, und aktivieren Sie danach das Kontrollkästchen **TLS 1.0 verwenden**. Sie können diese Konfiguration auch über die Gruppenrichtlinie oder mithilfe des Internet Explorer-Administratorkits vornehmen.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Ereignisprotokolleinstellungen
  
Die Ereignisprotokolleinstellungen für Zertifikatdienstserver in der Unternehmensclient-Umgebung werden über die Richtlinie für die Mitgliedsserver-Baseline konfiguriert. Weitere Informationen zur Richtlinie für die Mitgliedsserver-Baseline finden Sie im Kapitel 4, „Die Richtlinie für die Mitgliedsserver-Baseline“.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusätzliche Registrierungseinträge
  
Zusätzliche Registrierungseinträge wurden für die Vorlagendatei „Unternehmensclient - Zertifizierungsstellenserver.inf“ erstellt. Diese Einträge sind nicht in den administrativen Vorlagedateien (.adm) für die in diesem Handbuch beschriebene Unternehmensclient-Umgebung definiert. Die .adm-Dateien definieren die Systemrichtlinien und -beschränkungen für die Desktop-, Shell- und Sicherheitseinstellungen für Windows Server2003 mit SP1.
  
Die zusätzlichen Registrierungseinträge sind zur Automatisierung ihrer Implementierung in der Sicherheitsvorlage konfiguriert. Wenn die inkrementelle Gruppenrichtlinie für Zertifikatdienste für diese Umgebung entfernt wird, werden die Einstellungen nicht automatisch entfernt. Sie müssen mit einem Programm zum Bearbeiten der Registrierung (wie Regedt32.exe) manuell geändert werden.
  
Die Registrierungseinträge können unter Windows Server 2003 im Gruppenrichtlinienobjekt-Editor in folgendem Verzeichnis konfiguriert werden:
  
**MACHINE\\SYSTEM\\CurrentControlSet\\Services\\CertSvc\\Configuration**
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusätzliche Sicherheitseinstellungen
  
Die folgenden Zugriffssteuerungslisten (ACLs) werden empfohlen und können über die Gruppenrichtlinie zugewiesen werden. Diese ACLs sind jedoch nicht in den in diesem Handbuch bereitgestellten Sicherheitsvorlagen enthalten, da der Datenbankpfad und die Protokolle sich von Server zu Server unterscheiden. Ihr Zertifikatdienstserver kann z. B. ein Laufwerk C:\\, D:\\ und E:\\ aufweisen. Im folgenden Abschnitt wird beschrieben, wie diese Richtlinieneinstellungen manuell implementiert werden können.
  
#### Zugriffssteuerungslisten des Dateisystems
  
Die Dateien, die nicht durch Zugriffssteuerungslisten geschützt sind, können von autorisierten Benutzern, die lokal oder über ein Netzwerk auf diese Dateien zugreifen können, leicht angezeigt, geändert oder gelöscht werden. Obwohl Dateien mithilfe von Zugriffssteuerungslisten geschützt werden können, kann durch die Verschlüsselung der Dateien ein viel höheres Maß an Sicherheit erzielt werden, insbesondere dann, wenn es sich um Dateien handelt, die nur von einem einzelnen Benutzer verwendet werden.
  
In der folgenden Tabelle sind die Zugriffssteuerungslisten des Dateisystems für Zertifikatdienstserver in der Unternehmensclient-Umgebung enthalten, die auf Windows Server 2003 basieren. In dieser Umgebung verwenden die Zertifikatdienstserver das Laufwerk **D:\\CertSrv** als Zertifikatdatenbankverzeichnis, und die Datenbankprotokolle werden im Standardordner **%SystemRoot%\\system32\\CertLog** gespeichert. Sie können die Protokolle auch vom Systemlaufwerk in ein physisch getrenntes, gespiegeltes Laufwerk verschieben, wie z. B. **E:\\CertLog**. Das separate Speichern der Datenbank und der Protokolle auf verschiedenen physischen Laufwerken ist keine Sicherheitsanforderung, wird aber als Schutz vor Laufwerksausfällen und zur Verbesserung der Leistung empfohlen. Die Standardinstallationsordner der Zertifikatdienste **%SystemRoot%\\system32\\CertLog** und **%SystemRoot%\\system32\\CertSrv** weisen standardmäßig die richtigen Zugriffssteuerungslisten auf, die in der folgenden Tabelle dargestellt werden.
  
**Tabelle 11.2: Zugriffssteuerungslisten des Dateisystems**

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Pfad der Zugriffssteuerungsliste in der Benutzeroberfläche</th>
<th style="border:1px solid black;" >Unternehmensclient</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">%SystemRoot%\system32\CertLog (auf alle Unterordner übertragen)</td>
<td style="border:1px solid black;">Administratoren (Vollzugriff)
SYSTEM (Vollzugriff)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">%SystemRoot%\system32\CertSrv (auf alle Unterordner übertragen)</td>
<td style="border:1px solid black;">Administratoren (Vollzugriff)
SYSTEM (Vollzugriff)
Benutzer (Lesen und Ausführen, Ordnerinhalte anzeigen, Lesen)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">D:\CertLog</td>
<td style="border:1px solid black;">Administratoren (Vollzugriff)
SYSTEM (Vollzugriff)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">D:\CertLog</td>
<td style="border:1px solid black;">Administratoren (Vollzugriff)
SYSTEM (Vollzugriff)
Benutzer (Lesen und Ausführen, Ordnerinhalte anzeigen, Lesen)</td>
</tr>
</tbody>
</table>
 

Aufgrund der Bedeutung der Sicherheit von Zertifizierungsstellen wird die Dateiüberwachung in den Zertifikatdienstordnern aktiviert, die in der obigen Tabelle aufgeführt sind. Die Überwachungseinträge sind wie in der folgenden Tabelle dargestellt konfiguriert:

**Tabelle 11.3: Konfiguration der Datei- und Registrierungsüberwachung für Zertifikatdienste**

 
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Dateipfad oder Registrierungspfad</th>
<th style="border:1px solid black;" >Überwachungstyp</th>
<th style="border:1px solid black;" >Überwachungseinstellung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">%SystemRoot%\system32\CertLog</td>
<td style="border:1px solid black;">Fehlgeschlagen</td>
<td style="border:1px solid black;">Jeder (Vollzugriff)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">%SystemRoot%\system32\CertSrv</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Jeder (Ändern)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">D:\CertLog</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Jeder (Ändern)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">D:\CertLog</td>
<td style="border:1px solid black;">Erfolg</td>
<td style="border:1px solid black;">Jeder (Ändern)</td>
</tr>
</tbody>
</table>
  
Durch diese Richtlinieneinstellungen werden sämtliche fehlgeschlagenen Zugriffe (Lesen oder Ändern) von jedem Benutzer sowie sämtliche erfolgreichen Änderungen von Benutzern überwacht.
  
#### Sichern von bekannten Konten
  
Windows Server 2003 mit SP1 verfügt über eine Reihe vordefinierter Benutzerkonten, die nicht gelöscht, aber umbenannt werden können. Die zwei bekanntesten vordefinierten Konten in Windows Server 2003 sind die Konten „Gast“ und „Administrator“.
  
Das Konto „Gast“ ist auf Mitgliedsservern und Domänencontrollern standardmäßig deaktiviert. Diese Konfiguration sollte nicht geändert werden. Viele verschiedene schädliche Codes verwenden das vordefinierte Administratorkonto bei einem ersten Versuch, einen Server anzugreifen. Daher sollte das vordefinierte Administratorkonto umbenannt und seine Beschreibung geändert werden, damit Angriffen von Remoteservern vorgebeugt wird, bei denen die Angreifer versuchen, dieses bekannte Konto zu nutzen.
  
Die Auswirkung dieser Konfigurationsänderung hat sich in den letzten Jahren nach dem Auftreten von Angriffstools verringert, die durch Angabe der Sicherheits-ID (SID) des vordefinierten Administratorkontos dessen wahren Namen in Erfahrung bringen und dadurch Zugriff auf den Server erhalten. Eine Sicherheits-ID ist ein Wert, der jeden Benutzer, jede Gruppe, jedes Computerkonto und jede Anmeldesitzung bei einem Netzwerk eindeutig identifiziert. Die Sicherheits-ID dieses vordefinierten Kontos kann nicht geändert werden. Ihre Betriebsgruppen können allerdings versuchte Angriffe auf dieses Administratorkonto überwachen, wenn Sie es umbenennen und mit einem eindeutigen Namen versehen.
  
**So sichern Sie bekannte Konten auf Zertifizierungsstellenservern**
  
-   Benennen Sie die Administrator- und Gastkonten in jeder Domäne und auf jedem Server um, und ändern Sie die zugehörigen Kennwörter zu langen und komplexen Werten.
  
-   Verwenden Sie auf jedem Server verschiedene Namen und Kennwörter. Wenn auf allen Domänen und Servern die gleichen Kontonamen und -kennwörter verwendet werden, kann ein Angreifer, der sich Zugriff zu einem Mitgliedsserver verschafft hat, auch auf alle anderen Server zugreifen.
  
-   Ändern Sie die Standardkontobeschreibungen, um eine einfache Identifizierung der Konten zu verhindern.
  
-   Notieren Sie sich diese Änderungen an einem sicheren Ort.
  
    **Hinweis**: Das vordefinierte Administratorkonto kann durch eine Gruppenrichtlinie umbenannt werden. Diese Richtlinieneinstellung wurde in den mit diesem Handbuch bereitgestellten Sicherheitsvorlagen nicht implementiert, da jede Organisation Ihren eigenen eindeutigen Namen für dieses Konto auswählen sollte. Sie können jedoch die Einstellung **Konten: Administratorkonto umbenennen** so konfigurieren, dass Administratorkonten in der Unternehmensclient-Umgebungen umbenannt werden. Diese Richtlinieneinstellung ist Teil der Einstellungen für die Sicherheitsoptionen eines Gruppenrichtlinienobjekts.
  
#### Sichern von Dienstkonten
  
Konfigurieren Sie einen Dienst für die Ausführung im Sicherheitskontext eines Domänenkontos nur, wenn es sich nicht vermeiden lässt. Bei einem physischen Zugriff auf den Server könnten Domänenkontenkennwörter leicht durch Abbilden von geheimen LSA-Schlüsseln aufgedeckt werden. Weitere Informationen zum Sichern von Dienstkonten finden Sie im [Planungshandbuch für die Dienste- und Dienstekontensicherheit](http://www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx) (in englischer Sprache) unter www.microsoft.com/technet/security/topics/serversecurity/serviceaccount/default.mspx.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Erstellen der Richtlinie mithilfe des SCW
  
Zum Bereitstellen der notwendigen Sicherheitseinstellungen müssen Sie sowohl den Sicherheitskonfigurations-Assistenten (SCW) sowie die im Rahmen der herunterladbaren Version dieses Handbuchs verfügbaren Sicherheitsvorlagen verwenden, um eine Serverrichtlinie zu erstellen.
  
Wenn Sie Ihre eigene Richtlinie erstellen, müssen Sie die Abschnitte „Registrierungseinstellungen“ und „Überwachungsrichtlinie“ überspringen. Diese Einstellungen werden von den Sicherheitsvorlagen für die von Ihnen gewählte Umgebung bereitgestellt. Dieser Ansatz ist nötig um sicherzustellen, dass die in den Vorlagen angebotenen Richtlinienelemente Vorrang vor den vom SCW konfigurierten Elementen haben.
  
Es empfiehlt sich, das Betriebssystem zu Beginn der Konfigurationsarbeit neu zu installieren. Dadurch wird sichergestellt, dass keine älteren Einstellungen oder Software von früheren Konfigurationen verwendet werden. Wenn möglich, sollten Sie ähnliche Hardware wie in Ihrer Bereitstellungsumgebung verwenden, um eine möglichst hohe Kompatibilität zu gewährleisten. Die neue Installation wird als *Referenzcomputer* bezeichnet.
  
Während der Erstellung einer Serverrichtlinie entfernen Sie wahrscheinlich die Dateiserverrolle aus der Liste mit den erkannten Rollen. Diese Rolle wird häufig auf Servern konfiguriert, die sie nicht benötigen. Sie könnte als Sicherheitsrisiko betrachtet werden. Um die Dateiserverrolle für Server zu aktivieren, die sie benötigen, können Sie zu einem späteren Zeitpunkt eine zweite Richtlinie anwenden.
  
**So erstellen Sie die Richtlinie für Zertifikatdienstserver**
  
1.  Erstellen Sie auf einem neuen Referenzcomputer eine neue Installation von Windows Server 2003 mit SP1.
  
2.  Installieren Sie die Komponente für den Sicherheitskonfigurations-Assistenten (SCW) auf dem Computer, indem Sie auf „Systemsteuerung“, „Software“ und „Windows-Komponenten hinzufügen/entfernen“ klicken.
  
3.  Schließen Sie den Computer an die Domäne an, die sämtliche Sicherheitseinstellungen von den übergeordneten Organisationseinheiten übernehmen.
  
4.  Installieren und konfigurieren Sie nur die obligatorischen Anwendungen, die sich auf allen Servern mit dieser Rolle befinden. Dazu zählen z. B. rollenspezifische Dienste, Software- und Verwaltungsagenten, Bandsicherungsagenten sowie Antiviren- und Antispywaredienstprogramme.
  
5.  Starten Sie die grafische Benutzeroberfläche des SCW, wählen die Option zum **Erstellen einer neuen Richtlinie**, und verweisen Sie auf den Referenzcomputer.
  
6.  Stellen Sie sicher, dass die ermittelten Serverrollen auf Ihre Umgebung zutreffen, wie z. B. die Zertifikatdienstserverrolle.
  
7.  Stellen Sie sicher, dass die erkannten Clientfunktionen für Ihre Umgebung geeignet sind.
  
8.  Stellen Sie sicher, dass die erkannten Verwaltungsfunktionen für Ihre Umgebung geeignet sind.
  
9.  Stellen Sie sicher, dass von der Baseline benötigte zusätzliche Dienste, wie etwa Sicherungsagenten oder Antivirensoftware, erkannt werden.
  
10. Entscheiden Sie, wie nicht festgelegte Dienste in Ihrer Umgebung zu behandeln sind. Um eine verbesserte Sicherheit zu erzielen, können Sie diese Richtlinieneinstellung auf **Deaktivieren** setzen. Es empfiehlt sich, diese Konfiguration vor ihrer Bereitstellung auf dem Produktionsnetzwerk zu testen, da es bei der Ausführung von zusätzlichen Diensten auf den Produktionsservern, die auf dem Referenzcomputer nicht dupliziert wurden, zu Problemen kommen kann.
  
11. Achten Sie darauf, dass das Kontrollkästchen zum Überspringen des Abschnittsim Abschnitt „Netzwerksicherheit“ deaktiviert ist, und klicken Sie dann auf **Weiter**. Die zuvor ermittelten Ports und Anwendungen sind als Ausnahmen für die Windows-Firewall konfiguriert.
  
12. Aktivieren Sie im Abschnitt „Registrierungseinstellungen“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
13. Aktivieren Sie im Abschnitt „Überwachungsrichtlinie“ das Kontrollkästchen zum Überspringen des Abschnitts,und klicken Sie dann auf **Weiter.** Die Richtlinieneinstellungen werden aus der bereitgestellten INF-Datei importiert.
  
14. Schließen Sie die entsprechende Sicherheitsvorlage mit ein (z. B. „Unternehmensclient - Zertifizierungsstellenserver.inf“).
  
15. Speichern Sie die Richtlinie unter einem geeigneten Namen (z. B. Zertifikatdienste.xml).
  
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
  
     `scwcmd transform /p:<PathToPolicy.xml> /g:<GPODisplayName>`

     und drücken Sie anschließend die Eingabetaste. Beispiel:

     `scwcmd transform /p:"C:\Windows\Security\msscw\Policies\Certificate Services.xml"  /g:"Certificate Services Policy"`
    
    
    **Hinweis**: Die an der Eingabeaufforderung einzugebenden Daten werden hier aufgrund von Anzeigebeschränkungen in mehreren Zeilen angezeigt. Die Daten sollten jedoch in einer Zeile eingegeben werden.
  
2.  Verknüpfen Sie mithilfe der Gruppenrichtlinien-Verwaltungskonsole das neu erstellte Gruppenrichtlinienobjekt mit der jeweiligen Organisationseinheit.
  
Beachten Sie, dass für eine erfolgreiche Durchführung dieses Verfahrens die Windows-Firewall auf dem lokalen Computer aktiviert sein muss, wenn die SCW-Sicherheitsrichtliniendatei Windows-Firewall-Einstellungen enthält. Um zu überprüfen, ob die Windows-Firewall aktiviert ist, öffnen Sie die Systemsteuerung, und doppelklicken Sie auf **Windows-Firewall**.
  
Anschließend sollten Sie eine endgültige Prüfung vornehmen, um sicherzustellen, dass das Gruppenrichtlinienobjekt die gewünschten Einstellungen anwendet. Prüfen Sie zum Abschluss dieses Verfahrens, dass die entsprechenden Einstellungen vorgenommen wurden und die Funktionalität nicht beeinträchtigt ist.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### Zusammenfassung
  
In diesem Kapitel wurden die Richtlinieneinstellungen behandelt, die in den drei in diesem Handbuch definierten Umgebungen zur Absicherung von Zertifikatdienstservern verwendet werden können, auf denen Windows Server 2003 mit SP1 ausgeführt wird. Die Einstellungen werden über ein Gruppenrichtlinienobjekt (GPO) konfiguriert und angewendet, das die Richtlinie für die Mitgliedsserver-Baseline unterstützt. Gruppenrichtlinienobjekte können zur Erhöhung der Sicherheit mit den jeweiligen die Zertifikatdienstserver enthaltenden Organisationseinheiten verknüpft werden.
  
#### Weitere Informationen
  
Die folgenden Links bieten zusätzliche Informationen zur Absicherung von Servern, auf denen Windows Server 2003 mit SP1 und Zertifikatdienste ausgeführt werden.
  
-   Eine gute Einführung in PKI-Konzepte und die Funktionen der Windows 2000-Zertifikatdienste finden Sie im Artikel „[Einführung in die Infrastruktur öffentlicher Schlüssel von Windows 2000](http://www.microsoft.com/technet/archive/windows2000serv/evaluate/featfunc/pkiintro.mspx)“ (in englischer Sprache) unter http://www.microsoft.com/technet/archive/windows2000serv/evaluate/featfunc/pkiintro.mspx.
  
-   Eine Beschreibung der verbesserten PKI-Funktionen von Windows Server 2003 und Windows XP finden Sie in „[PKI-Verbesserungen in Windows XP Professional und Windows Server 2003](http://www.microsoft.com/technet/prodtechnol/winxppro/plan/pkienh.mspx)“ (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/winxppro/plan/pkienh.mspx.
  
-   Weitere Hintergrundinformationen zu wichtigen PKI-Konzepten finden Sie auf der Seite [Infrastruktur öffentlicher Schlüssel](http://www.microsoft.com/technet/prodtechnol/windowsserver2003/library/serverhelp/32aacfe8-83af-4676-a45c-75483545a978.mspx) (in englischer Sprache) unter www.microsoft.com/technet/prodtechnol/windowsserver2003/library/ServerHelp/32aacfe8-83af-4676-a45c-75483545a978.mspx.
  
[](#mainsection)[Zum Seitenanfanq](#mainsection)
  
### In diesem Beitrag
  
-   [Überblick](https://technet.microsoft.com/de-de/library/303c53d5-6b76-46e1-8ee3-7d8c99891129(v=TechNet.10))  
-   [Kapitel 1: Einführung in das Windows Server 2003-Sicherheitshandbuch](https://technet.microsoft.com/de-de/library/b0015e61-fe4e-4523-a875-ef8b971da55c(v=TechNet.10))  
-   [Kapitel 2: Absicherungsmechanismen von Windows Server 2003](https://technet.microsoft.com/de-de/library/015a5e65-1d76-48df-9657-6fe516a5095a(v=TechNet.10))  
-   [Kapitel 3: Die Domänenrichtlinie](https://technet.microsoft.com/de-de/library/70e3e562-9517-4fb9-b617-ef7854a0f03c(v=TechNet.10))  
-   [Kapitel 4: Die Richtlinie für die Mitgliedsserver-Baseline](https://technet.microsoft.com/de-de/library/7fd4e7b6-32b3-4fe8-a323-7c01d0c86c51(v=TechNet.10))  
-   [Kapitel 5: Die Richtlinie für die Domänencontroller-Baseline](https://technet.microsoft.com/de-de/library/f86f67bd-c150-4d0d-ad85-ff13a01afb01(v=TechNet.10))  
-   [Kapitel 6: Die Infrastrukturserverrolle](https://technet.microsoft.com/de-de/library/5914ba9b-2fe2-4886-8171-a908521836ec(v=TechNet.10))  
-   [Kapitel 7: Die Dateiserverrolle](https://technet.microsoft.com/de-de/library/2b1536d0-9610-4fb5-93b4-72f62d9e2ff3(v=TechNet.10))  
-   [Kapitel 8: Die Druckserverrolle](https://technet.microsoft.com/de-de/library/a37f44cf-85b3-4ae6-8e32-0cd877c5e9ee(v=TechNet.10))  
-   [Kapitel 9: Die Webserverrolle](https://technet.microsoft.com/de-de/library/835865cd-ff71-43e6-88bf-91f5b35a00b9(v=TechNet.10))  
-   [Kapitel 10: Die IAS-Serverrolle](https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10))  
-   Kapitel 11: Die Zertifikatdienstserverrolle  
-   [Kapitel 12: Die Bastion-Hostrolle](https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10))  
-   [Kapitel 13: Zusammenfassung](https://technet.microsoft.com/de-de/library/4a4cf96c-802d-4aef-9478-da3242f961da(v=TechNet.10))  
-   [Anhang A: Sicherheitstools und Formate](https://technet.microsoft.com/de-de/library/e15ff47c-bd77-4b34-9b58-c3f3fba2d135(v=TechNet.10))  
-   [Anhang B: Zu berücksichtigende Schlüsseleinstellungen](https://technet.microsoft.com/de-de/library/ff6d4718-4179-4f5a-a09d-50d75e9f32e6(v=TechNet.10))  
-   [Anhang C: Zusammenfassung der Einstellungen für Sicherheitsvorlagen](https://technet.microsoft.com/de-de/library/3a17dffb-0395-4656-ada8-28e3954307f5(v=TechNet.10))  
-   [Anhang D: Testen des Windows Server 2003-Sicherheitshandbuchs](https://technet.microsoft.com/de-de/library/2698b276-4c42-4a18-9930-3d69974746f8(v=TechNet.10))  
-   [Danksagungen](https://technet.microsoft.com/de-de/library/3ec7641e-0d9e-45a2-b3b2-b2a08960d871(v=TechNet.10))
  
**Download**
  
[Holen Sie sich das Windows Server 2003-Sicherheitshandbuch (engl.)](http://go.microsoft.com/fwlink/?linkid=14846&clcid=0x409)
  
**Benachrichtigung über Neuerungen**
  
[Melden Sie sich an, um sich über Updates und neue Versionen zu informieren](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx)
  
**Feedback**
  
[Senden Sie uns Ihre Kommentare oder Vorschläge](mailto:secwish@microsoft.com?subject=windows%20server%202003%20security%20guide)
<br/>
 
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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/library/605c5b8e-d007-41c2-92a6-9260fe571bc7(v=TechNet.10)"><img src="images/Dd443732.pageLeft(de-de,TechNet.10).gif" /></a>12 von 19<a href="https://technet.microsoft.com/de-de/library/cb056f68-1a74-4a6a-ac25-5629fefe7cbb(v=TechNet.10)"><img src="images/Dd443732.pageRight(de-de,TechNet.10).gif" /></a></td>
</tr>
</tbody>
</table>