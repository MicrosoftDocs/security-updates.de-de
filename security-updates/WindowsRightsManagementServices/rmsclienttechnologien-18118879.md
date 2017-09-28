---
TOCTitle: 'RMS-Clienttechnologien'
Title: 'RMS-Clienttechnologien'
ms:assetid: '6980468a-fc8c-489b-966f-2921ec268e74'
ms:contentKeyID: 18118879
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720288(v=WS.10)'
---

RMS-Clienttechnologien
======================

Clientcomputer in einer RMS-Bereitstellung verwenden die folgenden Technologien, mit denen Benutzer RMS-geschützten Inhalt erstellen, veröffentlichen und abrufen können.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th>Technologie</th>
<th>Beschreibung</th>
<th>Ausgegeben von</th>
<th>Weitere Informationen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>RMS-fähige Anwendungen</p></td>
<td style="border:1px solid black;"><p>Erforderlich, um RMS-geschützten Inhalt zu erstellen und zu veröffentlichen. Anwendungen können entweder spezielle für RMS entwickelt werden, oder es können vorhandene Anwendungen für die Verwendung mit RMS angepasst werden.</p></td>
<td style="border:1px solid black;"><p>Nicht von Microsoft stammende Entwickler.</p></td>
<td style="border:1px solid black;"><p>RMS-fähige Anwendungen</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>RMS-Computerzertifikate</p></td>
<td style="border:1px solid black;"><p>Identifizieren einen bestimmten Computer als vertrauenswürdig für RMS.</p></td>
<td style="border:1px solid black;"><p>Aktivierungsdienst für RMS Version 1.0. Es ist kein Dienst erforderlich, um mit RMS SP1 ein Computerzertifikat zu erhalten.</p></td>
<td style="border:1px solid black;"><p>RMS-Computerzertifikate</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Lockboxes</p></td>
<td style="border:1px solid black;"><p>Enthalten den privaten Schlüssel des Computers sowie ein entsprechendes Zertifikat mit dem öffentlichen Schlüssel des Computers.</p></td>
<td style="border:1px solid black;"><p>Aktivierungsdienst für RMS Version 1.0. Es ist kein Dienst erforderlich, um mit RMS SP1 eine Lockbox zu erhalten. Die Lockbox enthält den privaten Computerschlüssel. Dies ist der Kernsicherheitsprinzipal für das Verschlüsseln und Entschlüsseln.</p></td>
<td style="border:1px solid black;"><p>Lockboxes</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Rechtekontozertifikate</p></td>
<td style="border:1px solid black;"><p>Identifizieren einen bestimmten Benutzer als vertrauenswürdig für RMS.</p></td>
<td style="border:1px solid black;"><p>Rechtekontozertifizierungsdienst</p></td>
<td style="border:1px solid black;"><p>Rechtekontozertifikate</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Client-Lizenzgeberzertifikate</p></td>
<td style="border:1px solid black;"><p>Ermöglichen einem Benutzer das Veröffentlichen von RMS-geschütztem Inhalt, während er nicht mit dem Netzwerk verbunden ist.</p>
<p>(Optional)</p></td>
<td style="border:1px solid black;"><p>RMS-Veröffentlichungsdienst.</p></td>
<td style="border:1px solid black;"><p>Client-Lizenzgeberzertifikate</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Veröffentlichungslizenzen</p></td>
<td style="border:1px solid black;"><p>Definieren die Nutzungsrechte für einen bestimmten Inhalt.</p></td>
<td style="border:1px solid black;"><p>Diese Lizenz kann vom RMS-Veröffentlichungsdienst bzw. im Falle von Offlineveröffentlichung vom Clientlizenzgeber ausgestellt werden.</p></td>
<td style="border:1px solid black;"><p>Veröffentlichungslizenzen</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Nutzungslizenzen</p></td>
<td style="border:1px solid black;"><p>Ermöglichen einem Benutzer das Abrufen von RMS-geschütztem Inhalt.</p></td>
<td style="border:1px solid black;"><p>RMS-Lizenzierungsdienst.</p></td>
<td style="border:1px solid black;"><p>Nutzungslizenzen</p></td>
</tr>
</tbody>
</table>
