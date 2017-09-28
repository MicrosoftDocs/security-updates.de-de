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
