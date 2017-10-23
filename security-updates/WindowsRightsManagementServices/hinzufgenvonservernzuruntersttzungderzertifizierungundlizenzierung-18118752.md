---
TOCTitle: Hinzufügen von Servern zur Unterstützung der Zertifizierung und Lizenzierung
Title: Hinzufügen von Servern zur Unterstützung der Zertifizierung und Lizenzierung
ms:assetid: '089ceb62-2a96-444f-ab42-1d5deaabd0c3'
ms:contentKeyID: 18118752
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720189(v=WS.10)'
---

Hinzufügen von Servern zur Unterstützung der Zertifizierung und Lizenzierung
============================================================================

Nachdem der erste Server als Stamminstallation von RMS bereitgestellt wurde, können Sie zusätzliche Server zur Unterstützung von Zertifizierungs- und Lizenzierungsdiensten einrichten, wie etwa:

-   Sie können einen Server als Mitglied eines Stammzertifizierungsclusters hinzufügen, um eine erweiterte Unterstützung der Zertifizierungs- und Lizenzierungsdienste bereitzustellen. Ein zu diesem Cluster hinzugefügter Server verwendet dieselbe Konfiguration und dieselben Datenbanken wie der Stammzertifizierungsserver.
-   Sie können einen separaten Lizenzierungsserver als eigenständigen Server oder als Teil eines Lizenzierungsserverclusters einrichten. Er ist im Stammzertifizierungsserver unterregistriert und erhält sein Server-Lizenzgeberzertifikat über die Lizenzierungsdienste des Stammzertifizierungsservers. Alle an den Lizenzierungsserver gestellten Clientanforderungen nach Zertifizierungsdiensten werden an den Zertifizierungsserver weitergeleitet. Der Lizenzierungsserver kann Nutzungslizenzen und Veröffentlichungslizenzen ausstellen, ohne die Anforderung an den Stammzertifizierungsserver weiterzuleiten.

Die von Ihnen bereitgestellte Option ist von der Größe der Organisation und der Implementierung der Redundanz, Skalierung, Unterstützung des Lastenausgleichs und Sicherheit abhängig. Wenn Sie weitere Server mit RMS bereitstellen, um einen zunehmenden Zertifizierungs-, Lizenzierungs- und Veröffentlichungsbedarf zu erfüllen, sollten Sie Server mit RMS als Mitglieder des Stammzertifizierungsclusters bereitstellen, damit Sie die Redundanz und den Lastenausgleich auf allen Servern einrichten können. Sie können Zertifizierungsserver gruppieren und die Verarbeitung von Lizenzierungs- und Veröffentlichungsdiensten verteilen, indem Sie die Lizenzierungsserver – die auch für den Lastenausgleich gruppiert werden können – unterregistrieren lassen; es ist jedoch nicht möglich, für den Lastenausgleich eines unterregistrierten Lizenzierungsclusters einen Stammzertifizierungscluster heranzuziehen.

Die folgenden Themen bieten einen Leitfaden für diese Aufgabe:

-   [Für Installation und Bereitstellung erforderliche Rollen, Berechtigungen und Rechte](#bkmk_1)
-   [Bereitstellungsprozesse für zusätzliche Zertifizierungs- und Lizenzierungsserver](#bkmk_2)
-   [Einrichten der Cluster und des Lastenausgleichs](#bkmk_3)

Für Installation und Bereitstellung erforderliche Rollen, Berechtigungen und Rechte
-----------------------------------------------------------------------------------

Beim Installieren und Bereitstellen zusätzlicher Server werden die gleichen Rollen, Berechtigungen und Rechte benötigt wie beim Einrichten des ersten Servers. Darüber hinaus benötigen Sie auch die Berechtigung vom Stammzertifizierungsserver, einen separaten Lizenzierungsserver einzurichten. Dies wird als Unterregistrierung bezeichnet. Der Stammzertifizierungsserver wird durch die Discretionary Access Control Lists (= DACL) der Datei SubEnrollService.asmx gesteuert. Mitglieder der RMS Service Group (RMS-Dienstgruppe), einschließlich des RMS-Dienstkontos, das von Ihnen im Rahmen der Bereitstellung des Stammzertifizierungsservers festgelegt wird, sind zur Durchführung einer Unterregistrierung berechtigt. Weitere Informationen finden Sie unter [Einrichten von Zertifizierungs- und Lizenzierungsdiensten auf dem ersten Server](https://technet.microsoft.com/cce29a2f-984f-48ed-9187-0eb68286ec5b) an früherer Stelle dieses Themas.

Bereitstellungsprozesse für zusätzliche Zertifizierungs- und Lizenzierungsserver
--------------------------------------------------------------------------------

Das Hinzufügen von Servern zu Zertifizierungs- und Lizenzierungsclustern erfordert, dass der Server den Bereitstellungsprozess abschließt. Der Bereitstellungsprozess variiert je nach der Art des bereitzustellenden Servers.

-   Wenn Sie einen separaten Lizenzierungsserver bereitstellen, müssen Sie genauso wie für einen Stammzertifizierungsserver eine Konfigurationsdatenbank, ein RMS-Dienstkonto, einen Cluster-URL sowie die Informationen zum Schutz des privaten Schlüssels festlegen. Sie geben aber jedoch keine Sperrrichtlinie für ein Server-Lizenzgeberzertifikat an, da dies Richtlinie vom Stammzertifizierungsserver gesteuert wird.
-   Wird der Server als Teil eines Clusters bereitgestellt, müssen Sie bei der Bereitstellung lediglich das RMS-Dienstkonto, die Konfigurationsdatenbank und das Kennwort zum Schutz des privaten Schlüssels festlegen, bzw. denselben Kryptographiedienstanbieter und privaten Schlüssel wie der vorhandene Cluster verwenden. Alle Server in einem Cluster verfügen über dasselbe Server-Lizenzgeberzertifikat und Serverschlüsselpaar.

| ![](images/Cc720189.Important(WS.10).gif)Wichtig                                                                                                                                              |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Beginnen Sie mit der Installation von RMS auf anderen Servern erst dann, wenn Sie die Einrichtung von RMS auf dem ersten Server – einschließlich der Installation und Bereitstellung dieses Servers – abgeschlossen haben. |

Nach der Installation und Bereitstellung eines zusätzlichen Servers wird dieser automatisch als Teil des Clusters konfiguriert. Wenn Sie allerdings Lastenausgleich aktiviert haben, müssen Sie die Lastenausgleichssoftware für den Einsatz mit dem neuen Server konfigurieren.

Einrichten der Cluster und des Lastenausgleichs
-----------------------------------------------

RMS wurde zur Unterstützung von Servergruppen konzipiert. Durch die Erstellung von RMS-Serverclustern erzielen Sie größere Skalierbarkeit, erhöhte Zuverlässigkeit und verbesserten Lastenausgleich der RMS-Bereitstellung.

**Erstellen von Clustern**

Wenn Sie einen Cluster einrichten möchten, beginnen Sie zunächst mit einem Stammzertifizierungsserver oder einem Lizenzierungsserver. Für alle folgenden Server in den einzelnen Clustern installieren Sie RMS auf dem neuen Server, wechseln Sie zur Seite **Globale Verwaltung** und klicken danach auf **Diesen Server zu einem Cluster hinzufügen**, um die nötigen Ressourcen bereitzustellen und den Server dem Stammzertifizierungscluster oder Lizenzierungscluster hinzuzufügen.

Legen Sie den Datenbanknamen für den Cluster fest, zu dem Sie einen Server hinzufügen möchten.

**Lastenausgleichscluster**

Der Lastenausgleich wird bei RMS nicht automatisch implementiert. Sie können Hardware- oder Softwarelastenausgleich verwenden, einschließlich des Netzwerklastenausgleichs, um die Lasten über alle RMS-Server hinweg auszugleichen.

Die folgenden Themen bieten weitere Informationen hierzu:

-   Weitere Informationen über die Unterschiede zwischen den Zertifizierungs- und Lizenzierungsdiensten finden Sie unter „Überblick über das RMS-System“ im Abschnitt „Technische Referenz für RMS“ dieser Dokumentationssammlung.
-   Weitere Informationen über die Art der Zuordnung von Serverbereitstellungen hinsichtlich der Verfügbarkeit und Leistung Ihrer Organisation finden Sie unter „Bereitstellen von Redundanz und Lastenausgleich“ im Abschnitt „Planen einer RMS-Bereitstellung“ dieser Dokumentationssammlung.
-   Weitere Informationen zur Vorgehensweise bei der Festlegung der Anzahl von Servern, die für die Bereitstellung von RMS in Ihrer Organisation erforderlich sind, finden Sie unter „Beurteilen der Skalierungsanforderungen“ im Abschnitt „Planen einer RMS-Bereitstellung“ dieser Dokumentationssammlung.
-   Weitere Informationen zur Vorgehensweise bei der Implementierung der IT-Sicherheit im Rahmen Ihrer RMS-Bereitstellung finden Sie unter [Sichern der RMS-Bereitstellung](https://technet.microsoft.com/6de8b636-a824-4844-aefc-f26347abfc14) in diesem Thema.
-   Weitere Informationen zur Vorgehensweise bei der Installation von RMS finden Sie unter „So installieren Sie RMS mit Service Pack 1“ im Abschnitt „Ausführen eines RMS-Servers“ dieser Dokumentationssammlung.
    Sie können RMS außerdem über eine Eingabeaufforderung installieren. Weitere Informationen dazu finden Sie unter „RMS-Installation mithilfe einer Eingabeaufforderung“ im Abchnitt „Ausführen eines RMS-Servers“ dieser Dokumentationssammlung.
-   Weitere Informationen zur Vorgehensweise bei der Bereitstellung eines Lizenzierungsservers finden Sie unter „So stellen Sie einen Lizenzierungsserver bereit“ im Abschnitt „Ausführen eines RMS-Servers“ dieser Dokumentationssammlung.
-   Weitere Informationen über die Vorgehensweise bei der Bereitstellung zusätzlicher Server in einem Cluster finden Sie unter „So fügen Sie einen Server zu einem Cluster hinzu“ im Abschnitt „Ausführen eines RMS-Servers“ dieser Dokumentationssammlung.