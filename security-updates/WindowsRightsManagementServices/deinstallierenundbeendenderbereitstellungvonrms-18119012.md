---
TOCTitle: Deinstallieren und Beenden der Bereitstellung von RMS
Title: Deinstallieren und Beenden der Bereitstellung von RMS
ms:assetid: 'cae1ed5b-f716-41f0-8e14-7cbfef405331'
ms:contentKeyID: 18119012
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747753(v=WS.10)'
---

Deinstallieren und Beenden der Bereitstellung von RMS
=====================================================

Es kann verschiedene Gründe für das Entfernen von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) von einem Server geben. Bei einem Stammzertifizierungsserver müssen Sie die Bereitstellung von RMS zunächst auf dem Server beenden. Dazu können Sie auf der Seite **Globale Verwaltung** des Servers, dessen Bereitstellung beendet werden soll, auf **RMS von dieser Website entfernen** klicken. Bei einem Lizenzierungsserver ist das Beenden der Bereitstellung vor der Deinstallation von RMS nicht nötig.

| ![](images/Cc747753.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                        |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie die Bereitstellung des letzten Stammzertifizierungsservers in einer Active Directory-Gesamtstruktur beenden, wird das Dienstverbindungspunktobjekt aus Active Directory entfernt. Wenn Sie die Bereitstellung dieses Servers vor der Deinstallation von RMS nicht beenden, können Sie in dieser Gesamtstruktur keinen neuen Stammzertifizierungsserver bereitstellen, bis Sie das Dienstverbindungspunktobjekt manuell aus Active Directory entfernen. |

Deinstallieren Sie als Nächstes RMS.

Wenn Sie die Bereitstellung von RMS auf einem eigenständigen Server oder auf dem letzten Server in einem Cluster beenden und das Programm deinstallieren, wird die Datenbank der Verzeichnisdienste entfernt. Die Konfigurations- und Protokollierungsdatenbanken werden nicht entfernt. Wenn Sie RMS aber auf dem Server aktualisieren oder neu installieren, wird die Protokollierungsdatenbank durch eine neue Datenbank überschrieben.

Wenn Sie die Bereitstellung von RMS auf einem Server in einem Cluster beenden und das Programm deinstallieren, werden die Konfigurations- und Protokollierungsdatenbank sowie die Datenbank der Verzeichnisdienste für den Cluster nicht entfernt. Allerdings wird die Konfigurationsdatenbanktabelle „DRMS\_ClusterServer“ aktualisiert, so dass erkennbar ist, das der Server aus dem Cluster entfernt wurde.

Weitere Informationen zum Stilllegen von Servern und den dabei zu beachtenden Punkten finden Sie oben unter [Stilllegen von Servern](https://technet.microsoft.com/52005e2e-9563-4ba0-906c-3cc76f9c378f).