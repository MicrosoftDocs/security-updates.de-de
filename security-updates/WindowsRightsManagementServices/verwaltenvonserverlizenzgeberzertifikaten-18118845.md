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

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Ereignis-ID</th>
<th style="border:1px solid black;" >Ereignisname</th>
<th style="border:1px solid black;" >Ereignistyp</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">16</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneMonthEvent</td>
<td style="border:1px solid black;">Warnung: Der Dienst ist weiterhin wie üblich funktionsfähig.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">LicensorCertExpiresInOneWeekEvent</td>
<td style="border:1px solid black;">Warnung: Der Dienst ist weiterhin wie üblich funktionsfähig.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">18</td>
<td style="border:1px solid black;">LicensorCertExpiredEvent</td>
<td style="border:1px solid black;">Fehler: Der Dienst wurde deaktiviert.</td>
</tr>
</tbody>
</table>