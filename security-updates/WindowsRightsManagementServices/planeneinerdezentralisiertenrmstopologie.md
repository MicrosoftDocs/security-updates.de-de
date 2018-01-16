---
TOCTitle: 'Planen einer dezentralisierten RMS-Topologie'
Title: 'Planen einer dezentralisierten RMS-Topologie'
ms:assetid: '8773a1e0-6ac3-41f5-9866-5890cef08d04'
ms:contentKeyID: 18118913
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747657(v=WS.10)'
---

Planen einer dezentralisierten RMS-Topologie
============================================

Es ist unter Umständen erforderlich, einen oder mehrere Lizenzierungsserver bereitzustellen, die nicht Bestandteil des Stammzertifizierungsclusters sind. Dies geschieht häufig für Abteilungen, die direkte Kontrolle über das Ausstellen von Veröffentlichungs- und Nutzungslizenzen benötigen. Ein Beispiel wäre eine Rechtsabteilung mit Sicherheitsanforderungen, die eine direkte Kontrolle der Abteilung über die Lizenzvergabe erforderlich machen. Der Stammzertifizierungscluster stellt den Kontozertifizierungsdienst für die Lizenzierungsserver bereit. Die Kombination aus Stammzertifizierungscluster und mindestens einer Lizenzierungsserverinstallation wird auch als dezentrale Topologie bezeichnet.

Es ist zu beachten, dass Lizenzierungsserver genau wie der Stammzertifizierungsserver in Clustern bereitgestellt werden können. Darüber hinaus nutzt ein Lizenzierungscluster – ebenfalls analog zu einem Stammzertifizierungscluster – einen eigenen Lastenausgleichsdienst. Jeder Lizenzierungsserver oder Lizenzierungscluster verwendet eine separate SQL Server-Instanz, um die Konfigurations- und Protokollierungsdatenbanken für diesen Server oder Cluster bereitzustellen.

Es ist zwar möglich, eine RMS-Installation so einzurichten, dass sie nur die Zertifizierungsdienste über die Stamminstallation und den gesamten Lizenzierungsdienst über einen oder mehrere Lizenzierungsserver oder -cluster ausführt, doch dies ist eher ungewöhnlich. Üblicherweise würde eher die Anzahl der physikalischen Server im Stammzertifizierungscluster erhöht, um den Leistungs- und Redundanzanforderungen zu entsprechen, als dass separate Lizenzierungsserver bereitgestellt würden. Nur für den Fall, dass Abteilungen die Lizenzierung ermöglicht werden soll, wäre eine andere Topologie denkbar. Im folgenden Diagramm wird diese Bereitstellung verdeutlicht.

![](images/Cc747657.01fa5a85-5711-41aa-932a-124049d34186(WS.10).gif)

Das Einrichten einer dezentralen Topologie kann die Verwaltungskosten für eine Organisation erhöhen, da eine dezentralisierte Topologie von Natur aus komplexer als eine Standardtopologie ist. Wenn eine Organisation über mehrere Lizenzierungscluster und Strukturen verfügt, ist es möglicherweise erforderlich, auf den RMS-Clientcomputern die Registrierung aktiv zu erzwingen, damit gewährleistet ist, dass Lizenzierungsanforderungen über den korrekten RMS-Server verlaufen. Darüber hinaus können bei domänenübergreifenden Topologien Vertrauensprobleme auftreten. Daher ist es erforderlich, die Domänen genauer zu konfigurieren, damit RMS-geschützte Inhalte überhaupt abgerufen werden können.

Dienstverbindungspunkte in einer dezentralisierten Topologie
------------------------------------------------------------

Wenn ein RMS-Server bereitgestellt wird, wird ein Cluster-URL zur Active Directory-Struktur über einen Dienstverbindungspunkt (Service Connection Point = SCP) hinzugefügt. Es gibt je einen SCP für den Stammzertifizierungscluster und für jeden Lizenzierungscluster, der in der Struktur bereitgestellt wurde. Der SCP muss beim Stammzertifizierungscluster registriert werden, bevor ein Lizenzierungscluster bereitgestellt werden kann. Wenn ein Lizenzierungscluster bereitgestellt wird, sucht der Unterregistrierungsvorgang den Stammzertifizierungscluster im Netzwerk über den URL, und nutzt diesen auch für das Erwerben von Serverlizenzgeberzertifikaten.

Wenn statt eines einfachen Stammzertifizierungsservers ein Cluster verwendet wird, muss jeder Teilserver des Clusters über einen gemeinsamen URL virtuell erreichbar sein.

Virtuelle Adressierung kann auf verschiedenen Wegen ermöglicht werden, beispielsweise über Round-Robin-DNS, den Netzwerklastenausgleichsdienst, Hardwarelösungen, u.v.m. Die Nutzung virtueller Adressen bedeutet Lastenausgleich zwischen den Server und verhindert, dass Lizenzierung und Veröffentlichung von nur einem Server abhängen.

RMS verwendet den gemeinsamen URL für den Lizenzerwerb sowie für das Veröffentlichen des Wertes, über den Endbenutzer-Computer zuständige RMS-Cluster in Active Directory oder bei der Registrierung aufrufen. Kein Endbenutzercomputer erfordert direkten Zugriff auf einen einzelnen Server im Cluster.