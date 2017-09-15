---
TOCTitle: Hinzufügen von Servern zu einer vorhandenen Installation
Title: Hinzufügen von Servern zu einer vorhandenen Installation
ms:assetid: '7f3598ff-cd19-4daa-aa65-877f7f95a8ec'
ms:contentKeyID: 18118905
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747648(v=WS.10)'
---

Hinzufügen von Servern zu einer vorhandenen Installation
========================================================

Sie können Server bei Bedarf zu einer RMS-Installation (Rights Management Services oder Dienste für die Rechteverwaltung) hinzufügen, um eine erhöhte Nachfrage zu erfüllen oder Server zu ersetzen, die stillgelegt werden sollen. Jede RMS-Installation muss mindestens einen Stammzertifizierungsserver umfassen und kann wahlweise weitere Stammzertifizierungsserver in einem Cluster einschließen. Jede RMS-Installation kann außerdem eigenständige oder gruppierte Lizenzierungsserver einschließen.

Sie können Server mit einer der folgenden Methoden zu einer RMS-Installation hinzufügen:

-   Hinzufügen eines oder mehrerer Server(s) mit RMS zu einem Stammzertifizierungscluster.
-   Hinzufügen eines neuen eigenständigen Lizenzierungsservers.
-   Hinzufügen eines oder mehrerer Server(s) mit RMS zu einem Lizenzierungscluster.

**Hinzufügen von Stammzertifizierungsservern**

In den meisten Fällen lässt sich die Verfügbarkeit und Redundanz einer Bereitstellung am besten durch Hinzufügen eines oder mehrerer Server mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) zu einem Stammzertifizierungscluster erhöhen. Ein Stammzertifizierungscluster besteht aus einem oder mehreren Stammzertifizierungsservern. Stammzertifizierungsserver stellen im Gegensatz zu Lizenzierungsservern, die nur Lizenzierungs- und Veröffentlichungsdienste bereitstellen, alle RMS-Dienste bereit.

Während der Installation und Bereitstellung können Sie einen Server zu einem Cluster hinzufügen. In diesem Fall wird der neue RMS-Server automatisch als Mitglied des Clusters konfiguriert. Detaillierte Anweisungen zum Installieren und Bereitstellen eines RMS-Servers, der zum Stammzertifizierungscluster hinzugefügt werden soll, finden Sie nachstehend unter [So installieren Sie RMS mit Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d) und [So fügen Sie einen Server zu einem Cluster hinzu](https://technet.microsoft.com/db635238-5528-4bec-9cc6-8244e2b3d733).

Wenn Sie einen Cluster zum ersten Mal erstellen, müssen Sie neben diesem Bereitstellungsschritt bei Bedarf Software oder Hardware für die Verwendung von Clustern und Lastenausgleich einrichten. Wenn Sie bereits einen Cluster implementiert haben, müssen Sie die Lastenausgleichssoftware oder -hardware so konfigurieren, dass sie mit dem neuen Mitglied des Clusters funktionsfähig ist.

**Hinzufügen von Lizenzierungsservern**

Ein Lizenzierungsserver stellt im Gegensatz zum Stammzertifizierungsserver, der alle RMS-Dienste (Rights Management Services oder Dienste für die Rechteverwaltung) bereitstellt, nur Lizenzierungs- und Veröffentlichungsdienste bereit.

Lizenzierungsserver sind optional und werden meist zum Erfüllen spezifischer Lizenzierungsanforderungen bereitgestellt, wie z. B. die folgenden:

-   Unterstützung von eindeutigen Anforderungen einer Abteilung an die Rechteverwaltung. Eine Gruppe in einer Organisation kann beispielsweise andere Sicherheitsanforderungen an die Rechteverwaltung haben als der Rest der Organisation und wünscht möglicherweise die volle Kontrolle über die Implementierung der Lizenzierung für ihre Gruppe. Da in einer Gesamtstruktur nur ein Stammzertifizierungsserver zulässig ist, ist das Einrichten eines separaten Stammzertifizierungsservers daher nicht angebracht. In diesem Fall könnten Sie einen Lizenzierungsserver oder -cluster einrichten, der für den Bedarf dieser Gruppe dediziert ist. Sie können dann die Benutzerrechterichtlinie für diesen Lizenzierungsserver oder -cluster separat einrichten.
-   Unterstützung der Rechteverwaltung für externe Geschäftspartner im Rahmen eines Extranets, das eine sichere Trennung und Nachverfolgung von Ressourcen für bestimmte Geschäftspartner erfordert. Weitere Informationen hierzu finden Sie nachstehend unter [Konfigurieren eines Extranet-URLs](https://technet.microsoft.com/88fec9ff-c96c-4d20-8856-0485e7507572).
-   Verschieben von Lizenzierungsaufgaben vom Stammzertifizierungsserver. Dies kann in Organisationen, die (statt über einen Stammzertifizierungscluster) nur über einen einzelnen Stammzertifizierungsserver verfügen, zu Leistungsvorteilen führen.

Für die meisten Zwecke sollten Sie RMS-Server zum Stammzertifizierungscluster hinzufügen, damit Sie Redundanz und Lastenausgleich für alle Server in der Bereitstellung nutzen können. Zwar können Lizenzierungsserver zum Übernehmen der Verarbeitung von Lizenzierungs- und Veröffentlichungsanforderungen verwendet werden, diese Server ermöglichen aber kein Lastenausgleich mit dem Stammzertifizierungscluster. Sofern keine spezielle Anforderung für die Bereitstellung separater Lizenzierungsserver vorliegt, ist es besser, alle RMS-Server zu Mitgliedern des Stammzertifizierungsclusters zu machen und so einen Lastenausgleich zu ermöglichen.

Detaillierte Anweisungen zum Installieren und Bereitstellen eines RMS-Lizenzierungsservers finden Sie nachstehend unter [So installieren Sie RMS mit Service Pack 1](https://technet.microsoft.com/dab20175-a690-43f8-b943-768d289daa0d) und [So stellen Sie einen Lizenzierungsserver bereit](https://technet.microsoft.com/4d67b898-0ba9-4eef-ab7d-ee0ca55a688e).
