---
TOCTitle: 'RMS-Veröffentlichungsdienst'
Title: 'RMS-Veröffentlichungsdienst'
ms:assetid: '4c0c8fe3-695c-4b2c-a2d3-cab9b52bbb25'
ms:contentKeyID: 18118837
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720267(v=WS.10)'
---

RMS-Veröffentlichungsdienst
===========================

Der Veröffentlichungsdienst, mit dem Veröffentlichungslizenzen ausgegeben werden, wird auf dem RMS-Stammcluster sowie auf allen Lizenzierungsclustern ausgeführt. Veröffentlichungslizenzen definieren die Richtlinie, unter der Nutzungslizenzen geliefert werden können.

Die Anwendungsdatei für den Veröffentlichungsdienst, Publish.asmx, befindet sich im virtuellen Verzeichnis Licensing von IIS (Internet Information Services oder Internetinformationsdienste).

Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

###  

<p> </p>
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
<td style="border:1px solid black;"><p>Administratoren</p></td>
<td style="border:1px solid black;"><p>Vollzugriff</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RMS-Dienstgruppe</p></td>
<td style="border:1px solid black;"><p>Lesen und Ausführen</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Vollzugriff</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Benutzer</p></td>
<td style="border:1px solid black;"><p>Lesen und Ausführen</p></td>
</tr>
</tbody>
</table>
