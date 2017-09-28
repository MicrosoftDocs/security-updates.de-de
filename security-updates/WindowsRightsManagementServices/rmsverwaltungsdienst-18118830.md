---
TOCTitle: 'RMS-Verwaltungsdienst'
Title: 'RMS-Verwaltungsdienst'
ms:assetid: '4bd3e142-f0f6-40e9-a160-deab28ce5b88'
ms:contentKeyID: 18118830
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747560(v=WS.10)'
---

RMS-Verwaltungsdienst
=====================

Der Verwaltungsdienst wird auf dem RMS-Stammcluster sowie auf allen Lizenzierungsclustern ausgeführt. Der Verwaltungsdienst hostet die Verwaltungswebsite und ermöglicht Ihnen die Verwaltung von RMS.

Die Anwendungsdatei des Verwaltungsdienstes, Default.aspx, befindet sich im virtuellen Verzeichnis „Admin“ unter *RMS-Website*\\\_wmcs\\Admin. Dabei steht *RMS-Website* für den Namen der Website, auf der Sie RMS bereitgestellt haben.

Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Benutzer oder Gruppe</th>
<th>Standardberechtigung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Administratoren</td>
<td style="border:1px solid black;">Vollzugriff</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS-Dienstgruppe</td>
<td style="border:1px solid black;">Lesen und Ausführen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SYSTEM</td>
<td style="border:1px solid black;">Vollzugriff</td>
</tr>
</tbody>
</table>
