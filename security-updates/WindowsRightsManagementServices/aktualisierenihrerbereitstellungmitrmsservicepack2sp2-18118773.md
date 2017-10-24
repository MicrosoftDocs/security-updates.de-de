---
TOCTitle: 'Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 2 (SP2)'
Title: 'Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 2 (SP2)'
ms:assetid: '27ee06a1-f467-4a6c-b662-45ddb5f8c13e'
ms:contentKeyID: 18118773
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720225(v=WS.10)'
---

Aktualisieren Ihrer Bereitstellung mit RMS Service Pack 2 (SP2)
===============================================================

Dieser Abschnitt enthält Informationen zum Installieren von Microsoft® Windows® Rights Management Services (RMS) mit Service Pack 2 (SP2) in Unternehmen, in denen bereits eine RMS-Bereitstellung vorhanden ist. Die Aktualisierung von RMS-Bereitstellungen mit SP2 ist nur bei Unternehmen erforderlich, in denen RMS bereits bereitgestellt ist. Unternehmen, bei denen RMS zum ersten Mal bereitgestellt werden soll, können RMS mit SP2 unter Verwendung der im Thema zum Planen einer RMS-Bereitstellung ([http://go.microsoft.com/fwlink/?LinkId=74999](http://go.microsoft.com/fwlink/?linkid=74999)) (möglicherweise in englischer Sprache) und im Thema zum Bereitstellen eines RMS-Systems ([http://go.microsoft.com/fwlink/?LinkID=75000](http://go.microsoft.com/fwlink/?linkid=75000)) (möglicherweise in englischer Sprache) in dieser Dokumentationssammlung genannten Richtlinien bereitstellen.

Sie können RMS mit SP2 installieren, ohne die vorhandene Installation von RMS mit SP1 entfernen zu müssen. Das Setupprogramm für RMS mit SP2 erkennt, dass RMS mit SP1 installiert ist, und fügt nach Bedarf die zusätzlichen Features und Einstellungen hinzu.

| ![](images/Cc720225.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                         |
|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Ein Upgradepfad von der RMS-Serverkomponente ohne Service Pack auf RMS mit SP2 wird nicht unterstützt. Wenn Sie die RMS-Serverkomponente ohne das Service Pack verwenden, müssen Sie erst das SP1 installieren, bevor Sie mit dem Upgrade auf SP2 beginnen können. Für die RMS-Clientkomponente bestehen keine derartigen Upgradebeschränkungen. |

**Behandelte Themen**

-   [Vorbereiten auf das RMS mit SP2-Update](#bkmk_preparingforsp2update)
-   [Ausführen des RMS mit SP2-Updates](#bkmk_performingsp2update)
-   [Aktualisieren von Clustern](#bkmk_updateclusters)
-   [Aktualisieren von RMS-Clients](#bkmk_updateclients)
-   [Interoperabilität mit RMS Version 1.0](#bkmk_interop)
-   [Entfernen von RMS mit SP2](#bkmk_removingrms)


Vorbereiten auf das RMS mit SP2-Update
--------------------------------------

Das RMS mit SP2-Update ist so ausgelegt, dass Sie RMS unterbrechungsfrei weiter ausführen können. Bevor Sie mit dem Upgrade des RMS-Clusters beginnen, sollten Sie jedoch Folgendes tun:

-   Erstellen Sie eine Sicherungskopie der Konfigurationsdatenbank und des privaten RMS-Schlüssels. Weitere Informationen dazu finden Sie im Abschnitt zu Systemsicherungen für RMS ([http://go.microsoft.com/fwlink/?LinkId=75001](http://go.microsoft.com/fwlink/?linkid=75001)) (möglicherweise in englischer Sprache) in dieser Dokumentationssammlung.
-   Wenn Sie einen softwarebasierten privaten Schlüssel verwenden, sorgen Sie dafür, dass Sie das Kennwort für den privaten RMS-Schlüssel zur Hand haben.
-   Erstellen Sie eine Sicherungskopie der Protokollierungsdatenbank, sofern Sie die bisher protokollierten Statistiken behalten möchten.
-   Stellen Sie sicher, dass auf den Clients und Servern die neuesten wichtigen Updates und Sicherheitsupdates für das Betriebssystem installiert sind. Klicken Sie dazu auf **Start** und dann auf **Windows Update**, und führen Sie die Anweisungen auf dem Bildschirm aus.

Ausführen des RMS mit SP2-Updates
---------------------------------

Wenn der Assistent für das Setup von Windows Rights Management Services mit Service Pack 2 die vorhandene RMS-Installation erkennt, prüft er die vorhandene RMS mit SP1-Installation und fügt nur neue Dateien hinzu bzw. ersetzt die Dateien, die für RMS mit SP2 geändert werden müssen. Wenn Sie RMS bereits erfolgreich ausführen, müssen Sie nach dem Installieren von RMS mit SP2 keine zusätzlichen Konfigurationsschritte vornehmen, um RMS weiter verwenden zu können.

Aktualisieren von Clustern
--------------------------

Wenn Sie RMS in einer Clusterkonfiguration installiert haben, sollten Sie die Aktualisierung der Cluster so planen, dass sie sich so wenig wie möglich auf die Installation auswirkt. Berücksichtigen Sie bei der Planung, wie RMS mit SP2 in Ihrem Unternehmen am besten zu implementieren ist, folgende Überlegungen:

-   Es hat sich bewährt, RMS mit SP2 immer nur in einem Teil eines Clusters zu installieren, da das Upgrade des Clusters auf diese Weise vorhersehbarer wird und die Gefahr geringer ist, dass es während des Upgrades zu einer Verlangsamung des Diensts kommt.
-   Wenn mehrere RMS-Cluster vorhanden sind, sollten Sie das Upgrade zunächst auf den Stammzertifizierungsclustern vornehmen und erst dann die unterregistrierten Lizenzierungscluster upgraden.
-   Wenn Sie die gesamtstrukturübergreifende Gruppenerweiterung verwenden, können Sie die Cluster in den Gesamtstrukturen unabhängig voneinander upgraden, ohne dass dadurch die RMS-Server daran gehindert werden, die Gruppenmitgliedschaft gesamtstrukturübergreifend zu erweitern.
-   Die Serverkomponenten von RMS mit SP2, RMS mit SP1 und RMS Version 1.0 können nur dann nebeneinander existieren, wenn sie sich in verschiedenen Active Directory-Gesamtstrukturen befinden. Das gleichzeitige Vorhandensein verschiedener Versionen von RMS-Servern in ein und demselben Cluster wird nicht empfohlen.
-   Das Setup-Paket für RMS mit SP2 kann auch für die Installation einer völlig neuen Bereitstellung von RMS mit SP2 auf einem Server verwendet werden – RMS mit SP1 wird in diesem Fall nicht vorausgesetzt.

Aktualisieren von RMS-Clients
-----------------------------

In Windows Update und im Microsoft Download Center steht ein neuer RMS mit SP2-Client zur Verfügung. Das Setup-Paket für den RMS mit SP2-Client kann auch zum Installieren einer völlig neuen Version des RMS mit SP2-Clients auf einem Computer verwendet werden – der RMS 1.0-Client wird in diesem Fall nicht vorausgesetzt. Der RMS mit SP2-Client bietet Rückwärtskompatibilität und kann so auch mit RMS-fähigen Anwendungen eingesetzt werden, die RMS Version 1.0 benötigen.

Weitere Informationen zum Aktualisieren und Installieren des RMS-Clients finden Sie im Thema zum Verteilen des RMS-Clients ([http://go.microsoft.com/fwlink/?LinkId=75070](http://go.microsoft.com/fwlink/?linkid=75070)) (möglicherweise in englischer Sprache).

Interoperabilität mit RMS Version 1.0
-------------------------------------

Da RMS mit SP2 viele Verbesserungen bei der Funktionalität und Arbeitsgeschwindigkeit bietet, sollten Sie dessen Installation im Rahmen Ihres nächsten Upgradezyklus einplanen. Auch wenn RMS-Server und -Clients, auf denen RMS mit SP2 ausgeführt wird, in vollem Umfang mit RMS-Servern und -Clients funktionieren, auf denen RMS mit SP2 nicht ausgeführt wird, sollten bei einem Einsatz in gemischten Umgebungen die folgenden Unterschiede berücksichtigt werden:

-   Nur Server, auf denen RMS mit SP1 und später ausgeführt wird, unterstützen Offlineregistrierungen.
-   Nur Clients, auf denen RMS mit SP1 und später ausgeführt wird, sind selbstaktivierend.
-   Der folgenden Tabelle können Sie entnehmen, welche Funktionen in gemischten Umgebungen unterstützt werden:

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Version der RMS-Serverkomponente</th>
<th style="border:1px solid black;" >Unterstützte Features bei RMS 1.0-Clients</th>
<th style="border:1px solid black;" >Unterstützte Features bei RMS SP2-Clients</th>
<th style="border:1px solid black;" >Unterstützte Features in gemischten Clientumgebungen</th>
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
SP2-Clients sind selbstaktivierend,
RMS 1.0-Clients müssen über das Internet aktiviert werden</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">SP2</td>
<td style="border:1px solid black;">Alle bisherigen Features
Offlineregistrierung des Servers
Keine Selbstaktivierung der Clients</td>
<td style="border:1px solid black;">Alle SP1-Features
Offlineregistrierung des Servers
Selbstaktivierung der Clients
Serverlockbox
Microsoft SQL Server™ 2005 wird ab Werk unterstützt</td>
<td style="border:1px solid black;">Alle bisherigen Features plus SP2-Features
Offlineregistrierung des Servers
SP2-Clients sind selbstaktivierend,
RMS 1.0-Clients müssen über das Internet aktiviert werden</td>
</tr>
</tbody>
</table>
<p></p> 

Entfernen von RMS mit SP2
-------------------------

Wenn auf dem RMS-Server nach dem Installieren von RMS mit SP2 wieder die vorherige Konfiguration hergestellt werden soll, können Sie RMS mit SP2 mithilfe der Option **Software** in der Systemsteuerung wieder vom Server entfernen.