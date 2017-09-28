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
