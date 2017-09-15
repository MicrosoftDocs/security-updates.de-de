---
TOCTitle: 'Verwalten von Server-Lizenzgeberzertifikaten'
Title: 'Verwalten von Server-Lizenzgeberzertifikaten'
ms:assetid: '549979ad-13ee-4abc-8281-3e002a5a9561'
ms:contentKeyID: 18118845
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720272(v=WS.10)'
---

Verwalten von Server-Lizenzgeberzertifikaten
============================================

Server-Lizenzgeberzertifikate laufen nach dem angegebenen Zeitraum ab. Dieser Zeitraum beträgt normalerweise ein Jahr. Sie müssen als lokaler Administrator angemeldet sein, um ein Server-Lizenzzertifikat zu erneuern. Beim Erneuern des Server-Lizenzgeberzertifikats für den Stammzertifizierungscluster sendet RMS eine Anforderung zur Erneuerung dieses Zertifikats an den Microsoft-Registrierungsdienst. Wenn Sie das Zertifikat für einen Lizenzierungsserver erneuern, sendet RMS die Erneuerungsanforderung an den Stammzertifizierungsserver, der das ablaufende Zertifikat ausgestellt hat.

Es gibt drei von RMS im Systemereignisprotokoll veröffentlichte Ereignisse, die Sie überwachen sollten. Diese Ereignisse teilen Ihnen mit, dass das Erneuerungsdatum des Server-Lizenzgeberzertifikats bevorsteht oder dass das Zertifikat abgelaufen ist. In der folgenden Tabelle sind die Ereignis-IDs und -namen aufgeführt:

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th>Ereignis-ID</th>
<th>Ereignisname</th>
<th>Ereignistyp</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>16</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneMonthEvent</p></td>
<td style="border:1px solid black;"><p>Warnung: Der Dienst ist weiterhin wie üblich funktionsfähig.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>17</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiresInOneWeekEvent</p></td>
<td style="border:1px solid black;"><p>Warnung: Der Dienst ist weiterhin wie üblich funktionsfähig.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>18</p></td>
<td style="border:1px solid black;"><p>LicensorCertExpiredEvent</p></td>
<td style="border:1px solid black;"><p>Fehler: Der Dienst wurde deaktiviert.</p></td>
</tr>  
</tbody>  
</table>
