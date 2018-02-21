---
TOCTitle: 'Planen einer RMS-Standardtopologie'
Title: 'Planen einer RMS-Standardtopologie'
ms:assetid: 'fec3201e-201f-4faf-910e-fa44132af83d'
ms:contentKeyID: 18119082
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747755(v=WS.10)'
---

Planen einer RMS-Standardtopologie
==================================

Die Standardtopologie von RMS besteht aus mindestens einem physikalischen Server, der als Stammzertifizierungscluster dient. Dieser Cluster wird für die Zertifizierung, Lizenzierung und Veröffentlichung in der Organisation verwendet. Für alle Bereitstellungen – ausgenommen sehr kleine Bereitstellungen – werden im Allgemeinen mehrere physische Server als Cluster hinter einem einzelnem URL konfiguriert. Dieser Cluster wird erzeugt durch Bereitstellung des ersten Servers zur Erstellung des Stammzertifizierungsservers und anschließendes Hinzufügen von Servern zum Clustern, bis die Anzahl von Stammzertifizierungsservern erreicht wurde, die für die Unterstützung der erwarteten Aktivität erforderlich ist. In der folgenden Abbildung wird diese Topologie dargestellt.

![](images/Cc747755.a3332719-4d25-4694-a89a-7c31fd97ca3b(WS.10).gif)

Wenn Sie Server zu einem Cluster zusammenfügen, verwenden diese gemeinsame Konfigurations- und Protokollierungsdatenbanken. Hierbei handelt es sich um SQL Server-Datenbanken. SQL Server kann entweder auf dem Stammzertifizierungsserver oder einem separaten Server gespeichert sein.

Lastenausgleich wird für alle Server im Stammzertifizierungscluster eingerichtet. Alle Anforderungen von Zertifikaten und Lizenzen werden an den Stammzertifizierungscluster über den gemeinsamen URL geleitet, der während der Konfiguration des ersten Clusterservers festgelegt wurde.

Wenn nur ein geringe Anzahl von Clients unterstützt wird, kann RMS auf einem einzelnen Server mit einer lokalen Datenbank eingerichtet werden. Der Server ist für alle Zertifizierungen und Lizenzierungen in der Organisation verantwortlich. Diese Konfiguration bietet nur eine einzelne Fehlerquelle. Sie sollten daher regelmäßige Datensicherungen der Konfiguration ausführen.