---
TOCTitle: 'RMS-Unterregistrierungsdienst'
Title: 'RMS-Unterregistrierungsdienst'
ms:assetid: '6b05e71c-5e7d-467c-9e13-35ac14d3718a'
ms:contentKeyID: 18118883
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720289(v=WS.10)'
---

RMS-Unterregistrierungsdienst
=============================

Der Unterregistrierungsdienst wird nur auf dem RMS-Stammcluster ausgeführt. Er antwortet auf Anforderungen von Server-Lizenzgeberzertifikaten, die von Lizenzierungsclustern während der Bereitstellung gesendet werden.

Die Anwendungsdatei des Unterregistrierungsdienstes, „SubEnrollService.asmx“, befindet sich im virtuellen Verzeichnis „Certification“ unter *RMS-Website*\\\_wmcs\\Certification\\. Dabei ist *RMS-Website* der Name der Website, auf der Sie RMS (Rights Management Services oder Dienste für die Rechteverwaltung) bereitgestellt haben.

Standardmäßig ist der Zugriff auf diesen Dienst auf lokale Systemkonten beschränkt. Zum Bereitstellen und Registrieren eines untergeordneten Servers in einem Lizenzierungscluster muss das Benutzerkonto des Administrators dieses Lizenzierungsservers der freigegebenen Zugriffssteuerungsdatei (DACL) SubEntrollService.asmx mit Vollzugriffsberechtigungen hinzugefügt werden.

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
<td style="border:1px solid black;"><p>SYSTEM</p></td>
<td style="border:1px solid black;"><p>Vollzugriff</p></td>
</tr>
</tbody>
</table>
