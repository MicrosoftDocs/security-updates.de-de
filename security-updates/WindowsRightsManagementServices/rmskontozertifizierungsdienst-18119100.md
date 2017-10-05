---
TOCTitle: 'RMS-Kontozertifizierungsdienst'
Title: 'RMS-Kontozertifizierungsdienst'
ms:assetid: 'fb294969-850e-44b4-8f6a-ca5d5cec1bf1'
ms:contentKeyID: 18119100
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747802(v=WS.10)'
---

RMS-Kontozertifizierungsdienst
==============================

Der Kontozertifizierungsdienst wird nur auf dem RMS-Stammcluster ausgeführt. Der Kontozertifizierungsdienst erstellt Rechtekontozertifikate, mit denen Benutzerkonten bestimmten Computern zugeordnet werden. Ein Rechtekontozertifikat ermöglicht einem Benutzer das Veröffentlichen oder Abrufen von durch Rechte geschützten Inhalten auf einem bestimmten Computer.

Die Anwendungsdatei für den Kontozertifizierungsdienst, Certification.asmx, befindet sich im virtuellen Verzeichnis Certification von IIS (Internet Information Services oder Internetinformationsdienste).

Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Benutzer oder Gruppe</th>
<th style="border:1px solid black;" >Standardberechtigung</th>
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
