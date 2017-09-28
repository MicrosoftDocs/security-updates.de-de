---
TOCTitle: 'RMS-Aktivierungsproxydienst'
Title: 'RMS-Aktivierungsproxydienst'
ms:assetid: '6b9d33ef-466b-405b-a768-54e5615d6770'
ms:contentKeyID: 18118865
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747608(v=WS.10)'
---

RMS-Aktivierungsproxydienst
===========================

Alle in RMS Version 1.0 gestellten Computeraktivierungsanforderungen werden vom Aktivierungsproxydienst verarbeitet, der nur auf dem RMS-Stammcluster ausgeführt wird. Sie müssen erst einen Clientcomputer aktivieren, damit er mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) zum Veröffentlichen oder Abrufen von durch Rechte geschützte Inhalte verwendet werden kann. Öffnen Sie RMS mit Service Pack 1. Der Client ist „selbstaktivierend“ und benötigt deshalb nicht den Aktivierungsproxyserver oder den Microsoft-Aktivierungsdienst, um eine Lockbox und ein Computerzertifikat zu erzeugen.

Der Aktivierungsproxydienst leitet Computeraktivierungsanforderungen von Clients mit RMS Version 1.0 an den Microsoft-Aktivierungsservice weiter, der seinerseits eine für diesen Benutzer und diesen Computer speziell angepasste Lockbox und ein übereinstimmendes RMS-Computerzertifikat erzeugt. Anschließend leitet der Aktivierungsproxydienst diese Objekte an den anfordernden Client zurück.

Die Anwendungsdatei für den Aktivierungsproxydienst, Activation.asmx, befindet sich im virtuellen Verzeichnis Certification von IIS (Internet Information Services oder Internetinformationsdienste). Die Standardzugriffsteuerungsliste bei diesem Dienst wird in folgender Tabelle gezeigt:

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
<td style="border:1px solid black;"><p>Gäste</p></td>
<td style="border:1px solid black;"><p>Lesen und Ausführen</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RMS-Dienstgruppe</p></td>
<td style="border:1px solid black;"><p>Lesen und Ausführen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Vollzugriff</p></td>
</tr>
</tbody>
</table>
