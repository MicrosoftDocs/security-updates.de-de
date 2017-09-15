---
TOCTitle: Vorbereitungen zur Systemwiederherstellung
Title: Vorbereitungen zur Systemwiederherstellung
ms:assetid: '885c047f-1e3b-4bf5-8248-3a4505759cbb'
ms:contentKeyID: 18118916
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747659(v=WS.10)'
---

Vorbereitungen zur Systemwiederherstellung
==========================================

Das Versagen einer beliebigen Komponente des RMS-Systems, einschließlich der Internet- bzw. Intranetverbindung des RMS-Servers, des RMS-Zertifizierungsservers, der unterregistrierten RMS-Lizenzierungsserver, oder der Datenbankserver auf denen sich die RMS-Konfigurationsdatenbanken befinden, kann bedeuten, dass das System den Dienst unerwartet einstellt. Wenn ein RMS-System eingerichtet wird, ist es unerlässlich, die möglichen Auswirkungen auf die vorhandene IT-Systeme und vertrauliche Daten für den Fall abzuschätzen, das ein Systemversagen eintritt. Dementsprechend sollten auch Vorkehrungen für das effiziente Wiederherstellen der Komponente getroffen werden.

Das Versagen der Datenbankserver auf denen sich die RMS-Konfigurationsdatenbanken befinden würde als einziges dazu führen, dass kein durchgehender Zugriff auf RMS-geschützte Daten mehr möglich ist. In diesem Abschnitt wird beschrieben, welche Aspekte und Faktoren bei der Vorbereitung der Systemwiederherstellung bei RMS zu berücksichtigen sind. Dies umfasst auch die folgenden Aspekte:

-   [Internetkonnektivität](#bkmk_1)
-   [Intranetkonnektivität](#bkmk_2)
-   [Zertifizierungs- und Lizenzierungsdienste](#bkmk_3)
-   [Datenbankserver](#bkmk_4)
-   [Active Directory](#bkmk_5)

<span id="BKMK_1"></span>
Internetkonnektivität
---------------------

Wenn eine Online-Serverregistrierung verwendet wird, ist für den RMS-Server Internetkonnektivität während des Bereitstellungsvorgangs erforderlich, damit ein Serverlizenzgeberzertifikat erworben werden kann. Dies ist auch für die jährliche Erneuerung des Zertifikats von Bedeutung. Wenn der Zeitpunkt der Erneuerung bevorsteht, weist der Zertifizierungsserver darauf hin, dass das Zertifikat zu erneuern ist, indem Ereignisse im Systemereignisprotokoll ausgegeben werden. Ereignisse werden einen Monat (Ereignis-ID: 16) und eine Woche (Ereignis-ID: 17) vor Ablauf des Zertifikats, und zum Zeitpunkt des Ablaufens ausgegeben (Ereignis-ID: 18). Auf der Verwaltungswebsite für RMS wird auf der RMS-Seite „Globale Verwaltung“ ebenfalls eine Warnmeldung hinsichtlich des bevorstehenden Zertifikatsablaufs angezeigt. Wenn der RMS-Management Pack für Microsoft Operations Manager (MOM) verwendet wird, verursachen die Ablaufsereignisse einen Warnhinweis. Wenn beim RMS-Server keine Internetverbindung besteht, kann das Serverlizenzgeberzertifikat nicht mithilfe der Schaltfläche **Erneuern** auf der RMS-Verwaltungswebsite erneuert werden. In diesem Fall muss eine Offline-Registrierung für ein aktualisiertes Zertifikat durchgeführt werden.

Es hat sich bewährt, das Zertifikat einige Zeit vor dem Ablaufdatum zu erneuern. Damit können viele Probleme im Zusammenhang mit einer möglicherweise gestörten Internetverbindung am Ablaufzeitpunkt im Voraus vermieden werden. Der RMS-Server kann ohne gültiges Servicelizenzgeberzertifikat keine Dienste bereitstellen. Dies würde bedeuten, dass Benutzer keine RMS-geschützten Daten veröffentlichen und keine Nutzungslizenzen und Rechtekontozertifikate erhalten können, was beides für das Einsehen RMS-geschützter Daten erforderlich ist. Benutzer, die bereits über Nutzungslizenzen und Rechtekontozertifikate für Teile des RMS-geschützten Inhalts verfügen, können auch weiterhin auf diese Daten zugreifen, bis diese Lizenzen und Zertifikate verfallen.

<span id="BKMK_2"></span>
Intranetkonnektivität
---------------------

RMS arbeitet nach einem Client-Server-Prinzip, das auf eine vernetzte Infrastruktur angewiesen ist. Ohne ein funktionierendes Intranet können RMS-Server keine Verbindung zu erforderlichen Diensten innerhalb eines Unternehmens aufbauen, und auch nicht zu Benutzern, um diesen die Dienste zugänglich zu machen. Ohne Intranetkonnektivität können Benutzer keine Rechtekonto- oder Clientlizenzgeberzertifikate und keine Nutzungslizenzen von den RMS-Servern erhalten.

Organisationen sollten redundante Routing-Architekturen und Failover-Verknüpfungen von externen Standorten mit den RMS-Server-Standorten in Betracht ziehen.

Wenn ein Benutzer ein Clientlizenzgeberzertifikat für seinen Computer erhalten hat, kann er RMS-geschützte Daten offline veröffentlichen, sollte kein Zugriff auf einen RMS-Server möglich sein. Einige RMS unterstützende E-Mail-Anwendungen wurden so konfiguriert, dass Sie Lizenzen für die zugehörigen RMS-geschützten E-Mail-Nachrichten automatisch herunterladen, wenn das Postfach synchronisiert wird. Dementsprechend kann der Benutzer RMS-geschützte E-Mail noch lesen, wenn die Intranetverbindung nicht mehr besteht.

<span id="BKMK_3"></span>
Zertifizierungs- und Lizenzierungsdienste
-----------------------------------------

Das RMS-System nutzt insbesondere zwei virtuelle Verzeichnisse der Internetinformationsdienste (Internet Information Services = IIS) 6.0, nämlich Zertifizierungs- und Lizenzierungsdienste. Mit diesen Diensten können Benutzer ihre Computer in der RMS-Umgebung und bei RMS unterstützenden Anwendungen registrieren lassen, damit sie RMS-geschützte Daten veröffentlichen oder auf sie zugreifen können. Wenn diese Dienste nicht mehr verfügbar sind, können die Benutzer bis zur Wiederherstellung möglicherweise keinerlei Dienste abrufen.

Als Sicherheitsvorkehrung sollte daher die Erstellung von Clustern für Zertifizierungsserver und unterregistrierte Lizenzierungsserver in Betracht gezogen werden; in diesem Fall würde das Versagen eines Knotens innerhalb des Clusters die Verfügbarkeit des Dienstes nicht beeinträchtigen.

Es hat sich bewährt, zusätzliche Kapazitäten in Cluster zu integrieren, damit sich das Versagen eines Knotens nicht negativ auf die allgemeine Leistung auswirkt. Wenn der erste Zertifizierungsserver, unterregistrierte Lizenzierungsserver oder der erste unterregistrierte Lizenzierungsserver in einem Cluster installiert wird, sollten alle für die Bereitstellung verwendeten Konfigurationsoptionen und -daten sorgfältig erfasst werden.

<span id="BKMK_4"></span>
Datenbankserver
---------------

Die wichtigsten Komponenten im RMS-System sind die Datenbankserver mit den Konfigurationsdatenbanken. Jeder RMS-Server oder -Cluster speichert Konfigurations- und Protokollierungsdaten in Datenbanken. Die Konfigurationsdaten sind für den Betrieb von RMS unerlässlich. Diese Datenbanken enthalten das Serverlizenzgeberzertifikat, die bereits erstellten RMS-Benutzerrechterichtlinien und eine Liste der beim RMS-System registrierten Benutzer. Wenn kein Hardwaresicherheitsmodul für den RMS-Server verwendet wird, sind auch private und öffentliche Schlüssel des RMS-Servers hier gespeichert. Durch Sicherung der RMS-Datenbanken lassen sich frühere RMS-Installationen auf einem neuen Server wiederherstellen und ein RMS-System neu erstellen. Der Verlust einer Datenbank wirkt sich je nach Art dieser Datenbank unterschiedlich aus. In der folgenden Liste sind die Auswirkungen von konkretem Datenbankversagen aufgeführt:

-   **Konfigurationsdatenbank** Wenn diese Datenbank während des Betriebs des RMS-Servers plötzlich nicht mehr zur Verfügung steht, können die RMS-Dienste weitergeführt werden, da RMS über lokale Caches mit den nötigen Daten verfügt. Wenn jedoch ein Ereignis eintritt, durch das RMS mit der Konfigurationsdatenbank interagieren muss – beispielsweise soll ein neuer Benutzer registriert werden – tritt ein Fehler beim RMS-Dienst auf und der neue Benutzer kann nicht mit RMS-geschützten Inhalten arbeiten. Wenn eine Operation ausgeführt wird, durch die der RMS-Server Informationen aus Caches löscht – beispielsweise der Neustart des IIS-Dienstes oder eine routinemäßige Aktualisierung des lokalen Cache – funktioniert der RMS-Dienst nicht mehr. Der RMS-Server kann nicht mehr normal funktionieren, bis die Konfigurationsdatenbank wieder zur Verfügung steht.
    Wenn die Konfigurationsdatenbank beschädigt wird oder aus einem anderen Grund dauerhaft nicht mehr zur Verfügung steht, funktionieren die RMS-Server nicht mehr.
-   **Verzeichnisdienstdatenbank** Enthält Cache-Daten zu Gruppennamen und -zugehörigkeitsdaten, die dem Server mit dem globalen Katalog entnommen sind. Wenn diese Tabelle kurzzeitig nicht zur Verfügung steht, werden die RMS-Dienste nicht spürbar beeinträchtigt. Die Hauptaufgabe dieser Datenbank ist es, den Server mit dem globalen Katalog durch Redundanz abzusichern und seine Dienstebelastung zu verringern.
-   **Protokollierungsdatenbank** Wenn auf dem RMS-Server die Protokollierung aktiviert wurde, werden die Protokolle in dieser Datenbank gespeichert. Sollte die Datenbank nicht zur Verfügung stehen, werden die Protokolleinträge über den Message Queuing-Dienst (= MSMQ) des RMS-Servers bezogen und werden den gesamten verfügbaren Speicherplatz ausnutzen, es sei denn, diese Konfigurationsoption wurde deaktiviert.

Um sicher zu gehen, sollten die Datenbankserver in Clusterform vorliegen; dies bietet aktiv abrufbaren Failover-Schutz. Darüber hinaus sollten Datenbanken für RMS-Zertifizierungsserver, Lizenzierungsserver und -cluster regelmäßig gesichert werden.

Eine weitere bewährte Vorgehensweise ist es, mithilfe des Versendens des Transaktionsprotokolls stets eine sofort abrufbare Sicherungsdatenbank bereitzuhalten. Diese Vorgehensweise erfordert zwar möglicherweise zusätzliche Hardware, ermöglicht aber Organisationen, Datenbanken schneller wiederherzustellen. Microsoft IT verwendet diese Methode für die Wiederherstellung von RMS-Konfigurationsdatenbanken. Ein solches Vorgehen wird durch Auswählen des virtuellen SQL-Namens während der RMS-Bereitstellung eingeleitet. Mithilfe des virtuellen SQL-Namens kann der echte SQL-Name über das DNS (Domain Name System = Domänennamensystem) zugeordnet werden. Sollte die ursprüngliche Instanz von SQL Server nicht mehr funktionieren, kann einfach zur Sicherungsinstanz gewechselt werden, indem die Zuordnung des DNS-Namens vom Originalserver auf den Sicherungsserver geändert wird. Weitere Informationen über die interne Bereitstellung dieser Lösung bei Microsoft finden Sie in dem Fallbeispiel für die Microsoft Corporation auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=42070)(http://go.microsoft.com/fwlink/?LinkId=42070).

<span id="BKMK_5"></span>
Active Directory
----------------

RMS benötigt Active Directory für zwei wichtige Dienste: Benutzerauthentifizierung und globalen Katalogdienst Sollte Active Directory nicht zur Verfügung stehen, ist keine Benutzerauthentifizierung möglich, was bedeutet, dass keine Benutzer im RMS-System registriert werden können. Die Zertifizierungspipeline ist für den Erhalt eines Rechtekontozertifikates erforderlich. Diese Pipeline erfordert wiederum Authentifizierung. Wenn ein Benutzer über ein Rechtekontozertifikat verfügt, kann er Nutzungslizenzen ohne weitere Authentifizierung erhalten, da die Lizenzierungspipeline standardmäßig anonym ist.

Da Unternehmensentitäten über Gruppenmitgliedschaften bei Active Directory Zugriffsberechtigte für RMS-geschützte Informationen definieren, bedeutet der Verlust von Active Directory auch den Verlust der Möglichkeiten, Lizenzen zu erhalten. Standardmäßig werden Daten zur Gruppenmitgliedschaft für 15 Minuten auf dem RMS-Server im Cache aufbewahrt. Dementsprechend ist ein vorübergehender Ausfall des globalen Katalogdienstes leicht zu verschmerzen. Wenn der Zeitraum zwischen den Aktualisierungen des Cache vergrößert oder verringert werden soll, muss dazu der Registrierungsschlüssel verändert werden, der die Gültigkeitsdauer steuert. Weiter Informationen finden Sie in dieser Dokumentationssammlung unter „Betreiben eines RMS-Servers“ im Abschnitt „Ändern der Active Directory-Cacheeinstellungen“.
