---
TOCTitle: Planen der Clusteranforderungen für RMS
Title: Planen der Clusteranforderungen für RMS
ms:assetid: 'ec4023eb-4d39-4551-9789-c8a2d973a55b'
ms:contentKeyID: 18119088
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747792(v=WS.10)'
---

Planen der Clusteranforderungen für RMS
=======================================

Wenn Sie RMS in einer Clusterkonfiguration einsetzen, sollten Sie sicherstellen, dass Sie für die folgenden Bedingungen innerhalb Ihrer Organisation ein Konzept entwickelt haben.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Bedingung</th>
<th>Empfehlung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Große Anzahl von Desktops, die RMS verwenden</p></td>
<td style="border:1px solid black;"><p>Sie können mit Windows Update, einem Skript oder einer Softwareverteilungsmethode wie Systems Management Server (SMS) oder mit einer Gruppenrichtlinie die Clientsoftware von Microsoft Windows RMS installieren und aktivieren.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Viele Clientanforderungen</p></td>
<td style="border:1px solid black;"><p>Mithilfe eines Lastenausgleichsservers, des Netzwerklastenausgleichsdienstes (Network Load Balancing oder NLB) oder eines Hardwarelastenausgleichs können Anforderungen über den Cluster verteilt werden.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Zwei Netzwerkadapter mit virtueller IP-Adressen-Zuweisung, sowohl für Extranet- als auch Intranet-Anforderungen</p></td>
<td style="border:1px solid black;"><p>Stellen Sie sicher, dass alle DNS-Registrierungen, mit deren Hilfe virtuelle IP-Adressen auf dem Extranet dargestellt werden sollen, auch für die Darstellung im Intranet verantwortlich sind.</p>
<p>Wenn die DNS-Registrierung nicht über das Intranet erfolgt, schlagen interne Nutzungslizenzanforderungen fehl. Wenn die DNS-Ressourcendatensätze nicht verändert werden können, ist es möglich, die Hosttabelle aller Server des Clusters zu verändern. Auf diesem Wege kann der URL des Clusters der entsprechenden virtuellen IP-Adresse zugeordnet werden. Vor der Bereitstellung von RMS ist eine DNS-Registrierung erforderlich. Wenn Sie RMS bereits bereitgestellt haben, müssen Sie die Bereitstellung beenden und dann den Bereitstellungsprozess erneut ausführen.</p></td>
</tr>
</tbody>
</table>
