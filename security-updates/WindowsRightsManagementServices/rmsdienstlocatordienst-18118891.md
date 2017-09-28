---
TOCTitle: 'RMS-Dienstlocatordienst'
Title: 'RMS-Dienstlocatordienst'
ms:assetid: '6f410cc9-5d5b-4df3-bf4f-7b13811eb52f'
ms:contentKeyID: 18118891
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747548(v=WS.10)'
---

RMS-Dienstlocatordienst
=======================

Der Dienstlocatordienst wird sowohl auf RMS-Stamm- als auch auf Lizenzierungsclustern ausgeführt. Der Dienstlocatordienst stellt die Dienstverbindungs-URL des Clusters für Active Directory bereit, so dass er von RMS-fähigen Clients gesucht werden kann.

Die Anwendungsdatei für den Dienstlocatordienst, ServiceLocator.asmx, befindet sich in den virtuellen Verzeichnissen Certification und Licensing von IIS (Internet Information Services oder Internetinformationsdienste).

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
<tr class="even">
<td style="border:1px solid black;">Benutzer</td>
<td style="border:1px solid black;">Lesen und Ausführen</td>
</tr>
</tbody>
</table>
