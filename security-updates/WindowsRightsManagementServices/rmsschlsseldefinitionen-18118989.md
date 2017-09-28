---
TOCTitle: 'RMS-Schlüsseldefinitionen'
Title: 'RMS-Schlüsseldefinitionen'
ms:assetid: 'b052305c-1db7-434a-bad9-26d704156776'
ms:contentKeyID: 18118989
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747729(v=WS.10)'
---

RMS-Schlüsseldefinitionen
=========================

In der folgenden Tabelle werden die im RMS-System verwendeten Schlüssel aufgelistet.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Schlüssel</th>
<th>Zweck</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Serverschlüssel</td>
<td style="border:1px solid black;"><strong>Öffentlicher Schlüssel</strong>
Verschlüsselt den in der Veröffentlichungslizenz angegebenen Inhaltsschlüssel, so dass nur der RMS-Server den Inhaltsschlüssel abrufen und Nutzungslizenzen für diese Veröffentlichungslizenz ausstellen kann.
<strong>Privater Schlüssel</strong>
Signiert alle vom Server ausgestellten Zertifikate und Lizenzen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Computerschlüssel</td>
<td style="border:1px solid black;"><strong>Öffentlicher Schlüssel</strong>
Verschlüsselt den privaten Schlüssel eines Rechtekontozertifikats.
<strong>Privater Schlüssel</strong>
Entschlüssel ein Rechtekontozertifikat.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Client-Lizenzgeberschlüssel</td>
<td style="border:1px solid black;"><strong>Öffentlicher Schlüssel</strong>
Verschlüsselt den symmetrischen Inhaltsschlüssel in den von ihm ausgestellten Veröffentlichungslizenzen.
<strong>Privater Schlüssel</strong>
Signiert Veröffentlichungslizenzen, die lokal ausgestellt werden, während der Benutzer nicht mit dem Netzwerk verbunden ist.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Benutzerschlüssel</td>
<td style="border:1px solid black;"><strong>Öffentlicher Schlüssel</strong>
Verschlüsselt den in einer Nutzungslizenz angegebenen Inhaltsschlüssel, so dass nur ein bestimmter Benutzer den RMS-geschützten Inhalt mit Hilfe dieser Lizenz abrufen kann.
<strong>Privater Schlüssel</strong>
Ermöglicht einem Benutzer das Abrufen von RMS-geschütztem Inhalt.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Inhaltsschlüssel</td>
<td style="border:1px solid black;">Verschlüsselt RMS-geschützten Inhalt, wenn der Autor ihn veröffentlicht.</td>
</tr>
</tbody>
</table>
