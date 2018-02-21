---
TOCTitle: Identifizieren von Kernkomponenten
Title: Identifizieren von Kernkomponenten
ms:assetid: 'c9ec225b-0e51-42f5-aff6-0aecb62e3b27'
ms:contentKeyID: 18119011
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747751(v=WS.10)'
---

Identifizieren von Kernkomponenten
==================================

Wenn Sie die passende Topologie ermitteln möchten, müssen Sie zunächst die Kernkomponenten einer RMS-Bereitstellung und ihre Funktion kennen. Die folgende Liste identifiziert die Server, die Bestandteil der RMS-Bereitstellung sind:

-   Stammzertifizierungsserver Der Stammzertifizierungsserver ist die erste Komponente einer RMS-Bereitstellung; alle weiteren Komponenten hängen von ihr ab. Der Stammzertifizierungsserver führt alle RMS-Dienste aus, einschließlich des Kontozertifizierungsdienstes, mit dem Rechtekontozertifikate für RMS-Clients innerhalb der Organisation bereitgestellt werden. In jeder Active Directory-Gesamtstruktur kann nur ein Stammzertifizierungsserver vorhanden sein. Sie können jedoch der Installation mehrere Server hinzufügen, um so einen Stammzertifizierungscluster zu erzeugen, was Redundanz und Lastenausgleich bietet. Alle Server eines Stammzertifizierungsclusters verwenden dieselbe Konfigurationsdatenbank, die bei der ursprünglichen Bereitstellung eines Zertifizierungsservers innerhalb der Installation definiert wurde.
-   Lizenzierungsserver Ein Lizenzierungsserver ist optional und stellt keinen Teil des Stammzertifizierungsclusters dar. Der Lizenzierungsserver ist jedoch dem Stammzertifizierungsserver untergeordnet. Ein Lizenzierungsserver hängt hinsichtlich der Zertifizierungsdienste und sonstiger Dienste vom Stammzertifizierungsserver ab – er kann keine Kontozertifizierungsdienste bereitstellen. Der Lizenzierungsserver bietet jedoch Lizenzierungsdienste für Veröffentlichungs- und Nutzungslizenzen. Um Redundanz und Lastenausgleich zu gewährleisten, können der Installation mehrere Server hinzugefügt werden, was einen Lizenzierungscluster erzeugt. Alle Server eines Lizenzierungsclusters verwenden dieselbe Konfigurationsdatenbank, die bei der ersten Bereitstellung eines Lizenzierungsservers innerhalb des Clusters definiert wurde.
-   Server, die Infrastrukturkomponenten ausführen Zusätzliche Server in der Bereitstellung können die erforderliche Infrastruktur bereitstellen. Hierzu zählen Komponenten wie z. B. SQL Server 2000 und Active Directory. Der Bereitstellungsort dieser Komponenten sowie die Anzahl der hierzu erforderlichen Server hängen von den jeweiligen Anforderungen ab.

Die für eine Organisation entworfene RMS-Topologie muss der Bereitstellung all dieser Komponenten Rechnung tragen.