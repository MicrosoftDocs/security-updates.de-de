---
TOCTitle: 'Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 1 (SP1)'
Title: 'Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 1 (SP1)'
ms:assetid: 'a562c4b0-15df-46db-9d61-24db74871cfa'
ms:contentKeyID: 18118976
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747714(v=WS.10)'
---

Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 1 (SP1)
===============================================================

Dieser Abschnitt enthält Informationen zum Installieren von Microsoft® Windows® Rights Management Services (RMS) Service Pack 1 (SP1) in Unternehmen, in denen bereits eine RMS-Bereitstellung vorhanden ist. Die Aktualisierung von RMS-Bereitstellungen mit SP1 ist nur in Unternehmen erforderlich, in denen RMS bereits bereitgestellt wurde. Unternehmen, bei denen RMS zum ersten Mal bereitgestellt werden soll, können RMS mit SP1 unter Verwendung der im Thema zum Planen einer RMS-Bereitstellung und im Thema zum Bereitstellen eines RMS-Systems in dieser Dokumentationssammlung genannten Richtlinien bereitstellen.

Sie können RMS SP1 installieren, ohne die vorhandene Installation von RMS entfernen zu müssen. Das Setupprogramm für RMS SP1 erkennt, dass RMS installiert ist, und fügt nach Bedarf die zusätzlichen Features und Einstellungen hinzu.

**Behandelte Themen**

-   [Vorbereiten auf das RMS SP1-Update](#bkmk_1)
-   [Ausführen des RMS SP1-Updates](#bkmk_2)
-   [Aktualisieren von Clustern](#bkmk_3)
-   [Aktualisieren von RMS-Clients](#bkmk_4)
-   [Interoperabilität mit RMS Version 1.0](#bkmk_5)
-   [Entfernen von RMS mit SP1](#bkmk_6)

<span id="BKMK_1"></span>
Vorbereiten auf das RMS SP1-Update
----------------------------------

Das RMS SP1-Update ist so ausgelegt, dass Sie RMS unterbrechungsfrei weiter ausführen können. Bevor Sie mit dem Upgrade der RMS-Server beginnen, sollten Sie jedoch Folgendes tun:

-   Erstellen Sie eine Sicherungskopie der Konfigurationsdatenbank und des privaten RMS-Schlüssels. Weitere Informationen dazu finden Sie im Abschnitt zu Systemsicherungen für RMS im Thema zum Planen einer RMS-Bereitstellung in dieser Dokumentationssammlung.
-   Sorgen Sie dafür, dass Sie das Kennwort für den privaten RMS-Schlüssel zur Hand haben.
-   Erstellen Sie eine Sicherungskopie der Protokollierungsdatenbank, sofern Sie die bisher protokollierten Statistiken behalten möchten.
-   Stellen Sie sicher, dass auf den Clients und Servern die neuesten wichtigen Updates und Sicherheitsupdates für das Betriebssystem installiert sind. Klicken Sie dazu auf **Start** und dann auf **Windows Update**, und führen Sie die Anweisungen auf dem Bildschirm aus.

<span id="BKMK_2"></span>
Ausführen des RMS SP1-Updates
-----------------------------

Wenn der Assistent für das RMS SP1-Setup erkennt, dass bereits eine RMS-Installation vorhanden ist, fügt er nur neue Dateien hinzu bzw. ersetzt die Dateien, die für RMS SP1 geändert werden müssen. Wenn Sie RMS bereits erfolgreich ausführen, müssen Sie nach dem Installieren von RMS SP1 keine zusätzlichen Konfigurationsschritte vornehmen, um RMS weiter verwenden zu können.

<span id="BKMK_3"></span>
Aktualisieren von Clustern
--------------------------

Wenn Sie RMS in einer Clusterkonfiguration installiert haben, sollten Sie die Aktualisierung der Cluster so planen, dass sie sich so wenig wie möglich auf die Installation auswirkt. Berücksichtigen Sie bei der Planung, wie RMS SP1 in Ihrem Unternehmen am besten zu implementieren ist, folgende Überlegungen:

-   Es hat sich bewährt, RMS SP1 immer nur in einem Teil eines Clusters zu installieren, da das Upgrade des Clusters auf diese Weise vorhersehbarer wird und die Gefahr geringer ist, dass es während des Upgrades zu einer Verlangsamung des Diensts kommt.
-   Wenn mehrere RMS-Cluster vorhanden sind, sollten Sie das Upgrade zunächst auf den Stammzertifizierungsclustern vornehmen und erst dann die unterregistrierten Lizenzierungscluster upgraden.
-   Wenn Sie die gesamtstrukturübergreifende Gruppenerweiterung verwenden, können Sie die Cluster in den Gesamtstrukturen unabhängig voneinander upgraden, ohne dass dadurch die RMS-Server daran gehindert werden, die Gruppenmitgliedschaft gesamtstrukturübergreifend zu erweitern.
-   Die Serverkomponenten von RMS SP1 und RMS 1.0 können parallel vorhanden sein und zusammenarbeiten.
-   Das Setup-Paket für RMS SP1 kann auch für die Installation einer völlig neuen Version von RMS mit SP1 auf einem Server verwendet werden – RMS 1.0 wird in diesem Fall nicht vorausgesetzt.

<span id="BKMK_4"></span>
Aktualisieren von RMS-Clients
-----------------------------

RMS mit SP1 enthält einen neuen RMS-Client. Das Setup-Paket für den RMS SP1-Client kann auch zum Installieren einer völlig neuen Version des RMS SP1-Clients auf einem Computer verwendet werden – der RMS 1.0-Client wird in diesem Fall nicht vorausgesetzt. Der RMS SP1-Client bietet Rückwärtskompatibilität und kann so auch mit RMS-fähigen Anwendungen eingesetzt werden, die RMS Version 1.0 benötigen.

Dieser neue RMS-Client zeichnet sich durch die folgenden Features aus:

-   Der Client muss nicht mehr über das Internet eine Verbindung zu Microsoft herstellen und eine Lockbox herunterladen.
-   Für das Installieren des RMS-Clients mithilfe eines SMS oder einer Gruppenrichtlinie werden keine Administratorrechte benötigt.
-   Der RMS SP1-Client enthält eine neue Serverlockbox (wird auch als „Serversicherheitsprozessor“ bezeichnet), mit deren Hilfe Webdienste oder serverseitige Anwendungen, wie z. B. Windows SharePoint® Services und Exchange Server 2003, RMS-fähig gemacht werden können, sodass diese Dienste RMS-geschützte Inhalte abrufen und weiterverteilen können. Diese Lockbox ist beim Einsatz in vertrauenswürdigen Serveranwendungen hochgradig leistungsfähig und skalierbar.
-   Der RMS-Client verwendet FIPS 140-2-zertifizierte kryptografische Algorithmen. Er kann daher in FIPS-konformen Umgebungen bereitgestellt werden.

<span id="BKMK_5"></span>
Interoperabilität mit RMS Version 1.0
-------------------------------------

Da RMS SP1 viele Verbesserungen bei der Funktionalität und Arbeitsgeschwindigkeit bietet, empfiehlt es sich, das SP1 zu installieren, sobald Sie Ihre Tests abgeschlossen haben. Auch wenn RMS-Server und -Clients, auf denen RMS SP1 ausgeführt wird, in vollem Umfang mit RMS-Servern und -Clients funktionieren, auf denen RMS SP1 nicht ausgeführt wird, sollten bei einem Einsatz in gemischten Umgebungen die folgenden Unterschiede berücksichtigt werden:

-   Nur Server, auf denen RMS SP1 ausgeführt wird, unterstützen Offlineregistrierungen.
-   Nur Clients, auf denen RMS SP1 ausgeführt wird, sind selbstaktivierend.
-   Der folgenden Tabelle können Sie entnehmen, welche Funktionen in gemischten Umgebungen unterstützt werden:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Version der RMS-Serverkomponente</th>
<th>Unterstützte Features bei RMS 1.0-Clients</th>
<th>Unterstützte Features bei RMS SP1-Clients</th>
<th>Unterstützte Features in gemischten Clientumgebungen (RMS 1.0 und RMS SP1)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">1.0</td>
<td style="border:1px solid black;">Alle bisherigen Features
Keine Offlineregistrierung des Servers; Server muss über das Internet registriert werden
Keine Selbstaktivierung der Clients</td>
<td style="border:1px solid black;">Alle bisherigen Features
Keine Offlineregistrierung des Servers;
Selbstaktivierung der Clients</td>
<td style="border:1px solid black;">Alle bisherigen Features
SP1-Clients sind selbstaktivierend,
RMS 1.0-Clients müssen über das Internet aktiviert werden</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP1</td>
<td style="border:1px solid black;">Alle bisherigen Features
Offlineregistrierung des Servers
Keine Selbstaktivierung der Clients</td>
<td style="border:1px solid black;">Alle SP1-Features
Offlineregistrierung des Servers
Selbstaktivierung der Clients
Serverlockbox</td>
<td style="border:1px solid black;">Alle bisherigen Features plus SP1-Features
Offlineregistrierung des Servers
SP1-Clients sind selbstaktivierend,
RMS 1.0-Clients müssen über das Internet aktiviert werden</td>
</tr>
</tbody>
</table>
 

<span id="BKMK_6"></span>
Entfernen von RMS mit SP1
-------------------------

Wenn auf dem RMS-Server nach dem Installieren von RMS SP1 die vorherige Konfiguration erneut hergestellt werden soll, können Sie RMS SP1 mithilfe der Option **Software** in derSystemsteuerung wieder vom Server entfernen.

**Hinweis**   Wenn Sie vor dem Installieren von RMS SP1 eine Sicherungskopie der Konfigurationsdatenbank erstellt haben, können Sie durch Wiederherstellen dieser Sicherung sämtliche Änderungen, die durch RMS SP1 vorgenommen wurden, rückgängig machen. Wenn Sie keine Sicherungskopie der Konfigurationsdatenbank erstellt haben, können Sie u. U. in der wiederhergestellten RMS-Installation die Konfigurationsdatenbank aus der RMS SP1-Installation verwenden. Die wiederhergestellte RMS-Installation ignoriert dann die zusätzlichen Felder, die der Konfigurationsdatenbank bei der RMS SP1-Installation hinzugefügt wurden, da sie dafür keine Verwendung hat.
