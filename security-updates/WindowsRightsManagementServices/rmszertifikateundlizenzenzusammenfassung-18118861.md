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
<td style="border:1px solid black;">Server-Lizenzgeberzertifikate</td>
<td style="border:1px solid black;">Das für Lizenzierungsserver ausgestellte Server-Lizenzgeberzertifikat erteilt das Recht zum Ausstellen von Folgendem:
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
Das für den Stammzertifizierungscluster ausgestellte Server-Lizenzgeberzertifikat erteilt zusätzlich das Recht zum Ausstellen von Folgendem:
<ul>
<li>Rechtekontozertifikate für Clients<br />
<br />
</li>
<li>Server-Lizenzgeberzertifikate für Lizenzierungsserver<br />
<br />
</li>
</ul></td>
<td style="border:1px solid black;">Das für einen Lizenzierungsserver ausgestellte Server-Lizenzgeberzertifikat enthält den öffentlichen Schlüssel des Lizenzierungsservers.
Das für den Stammzertifizierungsserver ausgestellte Server-Lizenzgeberzertifikat enthält den öffentlichen Schlüssel des Stammzertifizierungsservers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Client-Lizenzgeberzertifikate</td>
<td style="border:1px solid black;">Erteilen einem Benutzer das Recht, RMS-geschützten Inhalt zu veröffentlichen, ohne dass er mit dem Firmennetzwerk verbunden ist.</td>
<td style="border:1px solid black;">Enthalten den öffentlichen Schlüssel des Zertifikats sowie dessen privaten Schlüssel, der mit dem öffentlichen Schlüssel des Benutzers verschlüsselt wird, der das Zertifikat angefordert hat. Enthalten außerdem den öffentlichen Schlüssel des Servers, der das Zertifikat ausgestellt hat.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RMS-Computerzertifikate</td>
<td style="border:1px solid black;">Identifizieren Computer oder Geräte, denen das RMS-System vertraut.</td>
<td style="border:1px solid black;">Enthalten den öffentlichen Schlüssel des aktivierten Computers. Der entsprechende private Schlüssel befindet sich in der Lockbox dieses Computers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rechtekontozertifikate</td>
<td style="border:1px solid black;">Identifizieren einen Benutzer im Zusammenhang mit einem bestimmten Computer oder Gerät.</td>
<td style="border:1px solid black;">Enthalten den öffentlichen Schlüssel des Benutzers sowie dessen privaten Schlüssel, der mit dem öffentlichen Schlüssel des aktivierten Computers verschlüsselt wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Veröffentlichungslizenzen</td>
<td style="border:1px solid black;">Geben die Rechte an, die für einen RMS-geschützten Inhalt gelten.</td>
<td style="border:1px solid black;">Enthalten den symmetrischen Inhaltsschlüssel zum Entschlüsseln des Inhalts, der mit dem öffentlichen Schlüssel des Servers, der die Lizenz ausgegeben hat, verschlüsselt wurde.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Nutzungslizenzen</td>
<td style="border:1px solid black;">Geben die Rechte an, die für den RMS-geschützten Inhalt in Bezug auf einen bestimmten authentifizierten Benutzers gelten.</td>
<td style="border:1px solid black;">Enthalten den symmetrischen Inhaltsschlüssel zum Entschlüsseln der Inhalte, der mit dem öffentlichen Schlüssel des Benutzers verschlüsselt wird.</td>
</tr>
</tbody>
</table>
