---
TOCTitle: Sperrung in Vorlagen für Benutzerrechterichtlinien
Title: Sperrung in Vorlagen für Benutzerrechterichtlinien
ms:assetid: '287c5b92-fcb5-4295-9c2b-4e37e643beb2'
ms:contentKeyID: 18118775
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720226(v=WS.10)'
---

Sperrung in Vorlagen für Benutzerrechterichtlinien
==================================================

Sperrbedingungen werden in Vorlagen für Benutzerrechterichtlinien angegeben. Die dafür in eine Vorlage für Benutzerrechterichtlinien eingegebenen Werte werden in einem XrML-Tag REFRESH (in der Veröffentlichungslizenz erfasst, die für die Vorlage ausgestellt wird. Die dann vom Server ausgestellte Nutzungslizenz enthält ebenfalls das REFRESH-Tag.

In der folgenden Tabelle werden die Parameter für das REFRESH-Tag aufgelistet.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Parameter</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Die Sperrlisten-ID.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ADDRESS</td>
<td style="border:1px solid black;">Der URL oder UNC-Pfad, über den die Sperrliste erhalten werden kann.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Der öffentliche Schlüssel des Sperrlistenausstellers. Er entspricht dem privaten Schlüssel, mit dem die Sperrliste signiert wurde.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">INTERVALTIME</td>
<td style="border:1px solid black;">Das maximale Alter der Sperrliste (in Tagen). Wenn die Sperrliste im Cache älter ist, als in INTERVALTIME festgelegt, ruft RMS-Client die aktuellste Version der Liste über den URL, der unter ADDRESS aufgeführt ist. Damit wird sichergestellt, dass immer die aktuellste Sperrliste verwendet wird.</td>
</tr>
</tbody>
</table>
  
Weitere Informationen zum Erstellen von Benutzerrechterichtlinien finden Sie in dieser Dokumentationssammlung unter „Betreiben eines RMS-Servers“ im Abschnitt „Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien“.
