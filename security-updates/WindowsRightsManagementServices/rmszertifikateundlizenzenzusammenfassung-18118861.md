---
TOCTitle: 'RMS-Zertifikate und -Lizenzen – Zusammenfassung'
Title: 'RMS-Zertifikate und -Lizenzen – Zusammenfassung'
ms:assetid: '637ccfca-318e-4346-85b5-0945b058fb9c'
ms:contentKeyID: 18118861
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747595(v=WS.10)'
---

RMS-Zertifikate und -Lizenzen – Zusammenfassung
===============================================

In der folgenden Tabelle werden die in RMS verwendeten Zertifikate und Lizenzen aufgelistet. Sie werden ausführlich in den anderen Themen dieses Abschnitts erläutert.

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
<th>Zertifikat oder Lizenz</th>
<th>Zweck</th>
<th>Inhalt</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Server-Lizenzgeberzertifikate</p></td>
<td style="border:1px solid black;"><p>Das für Lizenzierungsserver ausgestellte Server-Lizenzgeberzertifikat erteilt das Recht zum Ausstellen von Folgendem:</p>
<ul>  
<li>Veröffentlichungslizenzen<br />  
<br />  
</li>  
<li>Nutzungslizenzen<br />  
<br />  
</li>  
<li>Client-Lizenzgeberzertifikate<br />  
<br />  
</li>  
<li>Vorlagen für Benutzerrechterichtlinien<br />  
<br />  
</li>  
</ul>  
<p>Das für den Stammzertifizierungscluster ausgestellte Server-Lizenzgeberzertifikat erteilt zusätzlich das Recht zum Ausstellen von Folgendem:</p>  
<ul>  
<li>Rechtekontozertifikate für Clients<br />  
<br />  
</li>  
<li>Server-Lizenzgeberzertifikate für Lizenzierungsserver<br />  
<br />  
</li>
</ul></td>
<td style="border:1px solid black;"><p>Das für einen Lizenzierungsserver ausgestellte Server-Lizenzgeberzertifikat enthält den öffentlichen Schlüssel des Lizenzierungsservers.</p>
<p>Das für den Stammzertifizierungsserver ausgestellte Server-Lizenzgeberzertifikat enthält den öffentlichen Schlüssel des Stammzertifizierungsservers.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Client-Lizenzgeberzertifikate</p></td>
<td style="border:1px solid black;"><p>Erteilen einem Benutzer das Recht, RMS-geschützten Inhalt zu veröffentlichen, ohne dass er mit dem Firmennetzwerk verbunden ist.</p></td>
<td style="border:1px solid black;"><p>Enthalten den öffentlichen Schlüssel des Zertifikats sowie dessen privaten Schlüssel, der mit dem öffentlichen Schlüssel des Benutzers verschlüsselt wird, der das Zertifikat angefordert hat. Enthalten außerdem den öffentlichen Schlüssel des Servers, der das Zertifikat ausgestellt hat.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RMS-Computerzertifikate</p></td>
<td style="border:1px solid black;"><p>Identifizieren Computer oder Geräte, denen das RMS-System vertraut.</p></td>
<td style="border:1px solid black;"><p>Enthalten den öffentlichen Schlüssel des aktivierten Computers. Der entsprechende private Schlüssel befindet sich in der Lockbox dieses Computers.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Rechtekontozertifikate</p></td>
<td style="border:1px solid black;"><p>Identifizieren einen Benutzer im Zusammenhang mit einem bestimmten Computer oder Gerät.</p></td>
<td style="border:1px solid black;"><p>Enthalten den öffentlichen Schlüssel des Benutzers sowie dessen privaten Schlüssel, der mit dem öffentlichen Schlüssel des aktivierten Computers verschlüsselt wird.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Veröffentlichungslizenzen</p></td>
<td style="border:1px solid black;"><p>Geben die Rechte an, die für einen RMS-geschützten Inhalt gelten.</p></td>
<td style="border:1px solid black;"><p>Enthalten den symmetrischen Inhaltsschlüssel zum Entschlüsseln des Inhalts, der mit dem öffentlichen Schlüssel des Servers, der die Lizenz ausgegeben hat, verschlüsselt wurde.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Nutzungslizenzen</p></td>
<td style="border:1px solid black;"><p>Geben die Rechte an, die für den RMS-geschützten Inhalt in Bezug auf einen bestimmten authentifizierten Benutzers gelten.</p></td>
<td style="border:1px solid black;"><p>Enthalten den symmetrischen Inhaltsschlüssel zum Entschlüsseln der Inhalte, der mit dem öffentlichen Schlüssel des Benutzers verschlüsselt wird.</p></td>
</tr>  
</tbody>  
</table>
