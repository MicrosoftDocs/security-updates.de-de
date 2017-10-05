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

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Bedingung</th>
<th style="border:1px solid black;" >Empfehlung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Große Anzahl von Desktops, die RMS verwenden</td>
<td style="border:1px solid black;">Sie können mit Windows Update, einem Skript oder einer Softwareverteilungsmethode wie Systems Management Server (SMS) oder mit einer Gruppenrichtlinie die Clientsoftware von Microsoft Windows RMS installieren und aktivieren.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Viele Clientanforderungen</td>
<td style="border:1px solid black;">Mithilfe eines Lastenausgleichsservers, des Netzwerklastenausgleichsdienstes (Network Load Balancing oder NLB) oder eines Hardwarelastenausgleichs können Anforderungen über den Cluster verteilt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Zwei Netzwerkadapter mit virtueller IP-Adressen-Zuweisung, sowohl für Extranet- als auch Intranet-Anforderungen</td>
<td style="border:1px solid black;">Stellen Sie sicher, dass alle DNS-Registrierungen, mit deren Hilfe virtuelle IP-Adressen auf dem Extranet dargestellt werden sollen, auch für die Darstellung im Intranet verantwortlich sind.
Wenn die DNS-Registrierung nicht über das Intranet erfolgt, schlagen interne Nutzungslizenzanforderungen fehl. Wenn die DNS-Ressourcendatensätze nicht verändert werden können, ist es möglich, die Hosttabelle aller Server des Clusters zu verändern. Auf diesem Wege kann der URL des Clusters der entsprechenden virtuellen IP-Adresse zugeordnet werden. Vor der Bereitstellung von RMS ist eine DNS-Registrierung erforderlich. Wenn Sie RMS bereits bereitgestellt haben, müssen Sie die Bereitstellung beenden und dann den Bereitstellungsprozess erneut ausführen.</td>
</tr>
</tbody>
</table>
