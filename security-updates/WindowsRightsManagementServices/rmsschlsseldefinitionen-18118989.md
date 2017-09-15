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

<p> </p>
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
<td style="border:1px solid black;"><p>Serverschlüssel</p></td>
<td style="border:1px solid black;"><p><strong>Öffentlicher Schlüssel</strong></p>
<p>Verschlüsselt den in der Veröffentlichungslizenz angegebenen Inhaltsschlüssel, so dass nur der RMS-Server den Inhaltsschlüssel abrufen und Nutzungslizenzen für diese Veröffentlichungslizenz ausstellen kann.</p>  
<p><strong>Privater Schlüssel</strong></p>
<p>Signiert alle vom Server ausgestellten Zertifikate und Lizenzen.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Computerschlüssel</p></td>
<td style="border:1px solid black;"><p><strong>Öffentlicher Schlüssel</strong></p>
<p>Verschlüsselt den privaten Schlüssel eines Rechtekontozertifikats.</p>  
<p><strong>Privater Schlüssel</strong></p>
<p>Entschlüssel ein Rechtekontozertifikat.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Client-Lizenzgeberschlüssel</p></td>
<td style="border:1px solid black;"><p><strong>Öffentlicher Schlüssel</strong></p>
<p>Verschlüsselt den symmetrischen Inhaltsschlüssel in den von ihm ausgestellten Veröffentlichungslizenzen.</p>  
<p><strong>Privater Schlüssel</strong></p>
<p>Signiert Veröffentlichungslizenzen, die lokal ausgestellt werden, während der Benutzer nicht mit dem Netzwerk verbunden ist.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Benutzerschlüssel</p></td>
<td style="border:1px solid black;"><p><strong>Öffentlicher Schlüssel</strong></p>
<p>Verschlüsselt den in einer Nutzungslizenz angegebenen Inhaltsschlüssel, so dass nur ein bestimmter Benutzer den RMS-geschützten Inhalt mit Hilfe dieser Lizenz abrufen kann.</p>  
<p><strong>Privater Schlüssel</strong></p>
<p>Ermöglicht einem Benutzer das Abrufen von RMS-geschütztem Inhalt.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Inhaltsschlüssel</p></td>
<td style="border:1px solid black;"><p>Verschlüsselt RMS-geschützten Inhalt, wenn der Autor ihn veröffentlicht.</p></td>
</tr>  
</tbody>  
</table>
