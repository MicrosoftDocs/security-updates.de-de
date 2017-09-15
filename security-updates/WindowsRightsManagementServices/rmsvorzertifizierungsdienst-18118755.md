---
TOCTitle: 'RMS-Vorzertifizierungsdienst'
Title: 'RMS-Vorzertifizierungsdienst'
ms:assetid: '09957294-167f-4f98-88e9-ae90fbeb26c1'
ms:contentKeyID: 18118755
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720191(v=WS.10)'
---

RMS-Vorzertifizierungsdienst
============================

Der Vorzertifizierungsdienst wird nur auf dem RMS-Stammcluster ausgeführt. Über diesen Dienst kann ein Server ein Rechtekontozertifikat für einen Benutzer anfordern. Darüber hinaus ist der Dienst für die Entwicklung benutzerdefinierter Anwendungen vorgesehen. Einige Beispiele, die diesen Dienst verwenden, sind Microsoft Exchange Server 2007 und Microsoft Office SharePoint Server 2007.

Die Anwendungsdatei für den Vorzertifizierungsdienst, Precertification.asmx, befindet sich im virtuellen Verzeichnis Certification von IIS (Internet Information Services oder Internetinformationsdienste).

Weitere Informationen zum Entwickeln benutzerdefinierter Anwendungen finden Sie in der Dokumentation zur Microsoft-Diensttechnologie für die Windows-Rechteverwaltung in der MSDN-Bibliothek [http://go.microsoft.com/fwlink/?LinkId=32972](http://go.microsoft.com/fwlink/?linkid=32972).

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
