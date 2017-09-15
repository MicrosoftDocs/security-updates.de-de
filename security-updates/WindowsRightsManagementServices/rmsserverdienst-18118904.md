---
TOCTitle: 'RMS-Serverdienst'
Title: 'RMS-Serverdienst'
ms:assetid: '772d0a89-c9fb-4430-9434-38cd5add1e86'
ms:contentKeyID: 18118904
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747566(v=WS.10)'
---

RMS-Serverdienst
================

Der Serverdienst wird nur auf dem RMS-Stammcluster ausgeführt. Der Server stellt eine von einem Client gestellte Anforderung durch Onlineveröffentlichung dar, um ein Server-Lizenzgeberzertifikat abzurufen.

Die Anwendungsdatei für den Serverdienst, Server.asmx, befindet sich im virtuellen Verzeichnis Certification von IIS (Internet Information Services oder Internetinformationsdienste).

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
