---
TOCTitle: Stilllegen von Servern
Title: Stilllegen von Servern
ms:assetid: '52005e2e-9563-4ba0-906c-3cc76f9c378f'
ms:contentKeyID: 18118838
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747568(v=WS.10)'
---

Stilllegen von Servern
======================

Es kann Situationen geben, in denen ein RMS-Server stillgelegt werden muss. Im Folgenden finden Sie einige Beispiele für solche Situationen:

-   Geräteprobleme oder Updates, die ein Ersetzen von bestimmten Servern zur Folge haben.
-   Eine Verringerung des Lizenzierungs- und Veröffentlichungsverkehrs, der zur Außerbetriebsetzung einiger Server führt.
-   Rechtliche Anforderungen zum Entfernen von Servern von bestimmten Orten, die zur Außerbetriebssetzung eines gesamten Clusters führen.
-   Die Fusion oder der Verkauf von Divisionen oder anderen Teilen einer Organisation, die bzw. der zu einem Transfer von Vermögenswerten führt.
-   Die Fusion einer Organisation mit einer anderen Organisation, bei der ebenfalls RMS ausgeführt wird, und die zu einer Redundanz beider RMS-Installationen führt.

Bevor Sie einen Server stilllegen, sollten Sie eine Sicherungskopie aller von diesem Server verwendeten RMS-Datenbanken, insbesondere der Konfigurationsdatenbank, erstellen. Weitere Informationen zum Sichern von Datenbanken finden Sie unter „Sichern und Wiederherstellen des RMS-Systems“ im Abschnitt „Planen einer RMS-Bereitstellung“ in dieser Dokumentationssammlung. .

Nach dem Sichern der Datenbanken können Sie den Server entfernen. Die Anforderungen an das Entfernen eines RMS-Servers hängen von der Rolle des Servers und der Topologie der RMS-Installation ab:

-   **Entfernen eines einzelnen Servers aus einem Cluster**. Wenn der RMS-Server, der stillgelegt werden soll, in einem Cluster enthalten ist, in dem weiterhin RMS-Server aktiviert und erforderlich sind, müssen Sie zum Entfernen des einzelnen RMS-Servers aus dem Cluster die Bereitstellung von RMS auf dem stillzulegenden Server beenden. Sie können auch RMS von diesem Server deinstallieren, die Hardware aus dem Cluster entfernen und die Datenbanken archivieren.
    | ![](images/Cc747568.note(WS.10).gif)Hinweis                                                                                                           |
    |------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Sie müssen vor dem Deinstallieren von RMS lediglich die Bereitstellung der Server im Stammzertifizierungscluster beenden. Bei Lizenzierungsservern ist dieser Prozess nicht nötig. |

-   **Stilllegen eines eigenständigen Servers**. Führen Sie die folgenden Schritte aus, wenn es sich bei dem stillzulegenden RMS-Server um einen eigenständigen RMS-Server handelt (er gehört dann keinem aus mehreren Servern bestehenden Cluster an), der durch einen neuen Server ersetzt werden soll: Beenden Sie die Bereitstellung des vorhandenen RMS-Servers, und deinstallieren Sie RMS. Entfernen Sie den Server aus dem Netzwerk, installieren Sie RMS umgehend auf dem Ersatzserver, und stellen Sie diesen bereit. Konfigurieren Sie den neuen RMS-Server so, dass er den gleichen URL und die gleiche Konfigurationsdatenbank wie der stillgelegte RMS-Server verwendet. Bedenken Sie, dass Benutzer die vom stillgelegten Server veröffentlichten Inhalte erst wieder abrufen können, wenn der Ersatzserver installiert und bereitgestellt wurde.
    | ![](images/Cc747568.Important(WS.10).gif)Wichtig                                                                                                                                                                                                                |
    |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
    | Wenn der zu ersetzende RMS-Server ein Hardwaresicherheitsmodul verwendet, müssen Sie die Sicherheitsumgebung auf den neuen Server übertragen, bevor Sie RMS auf diesem installieren und bereitstellen. Anleitungen hierzu finden Sie in der Dokumentation zu Ihrem Hardwaresicherheitsmodul. |

-   **Ersetzen einer RMS-Installation durch eine andere, vorhandene RMS-Installation**. In einigen Situationen muss möglicherweise eine RMS-Installation stillgelegt und durch eine andere, vorhandene RMS-Installation ersetzt werden, z. B. bei der Fusion zweier Unternehmen, die beide RMS ausführen.

Wenn Sie die Bereitstellung eines Servers beenden und diesen deinstallieren, wird er aus der Tabelle „ClusterServer“ der Konfigurationsdatenbank entfernt, und die Datenbank der Verzeichnisdienste wird aus SQL Server gelöscht. Weitere Anleitungen zum Beenden der Bereitstellung von RMS und zur Deinstallation des Programms finden Sie nachstehend unter „[So beenden Sie die Bereitstellung von RMS](https://technet.microsoft.com/9fa63daa-5fb9-4afd-8371-b38248619857)“ und „[So deinstallieren Sie RMS](https://technet.microsoft.com/885e3b4f-ea32-466f-9f7f-d8440b0f7c28)“.