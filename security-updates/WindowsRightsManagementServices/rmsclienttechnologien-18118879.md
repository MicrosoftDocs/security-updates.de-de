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
<td style="border:1px solid black;">RMS-fähige Anwendungen</td>
<td style="border:1px solid black;">Erforderlich, um RMS-geschützten Inhalt zu erstellen und zu veröffentlichen. Anwendungen können entweder spezielle für RMS entwickelt werden, oder es können vorhandene Anwendungen für die Verwendung mit RMS angepasst werden.</td>
<td style="border:1px solid black;">Nicht von Microsoft stammende Entwickler.</td>
<td style="border:1px solid black;">RMS-fähige Anwendungen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RMS-Computerzertifikate</td>
<td style="border:1px solid black;">Identifizieren einen bestimmten Computer als vertrauenswürdig für RMS.</td>
<td style="border:1px solid black;">Aktivierungsdienst für RMS Version 1.0. Es ist kein Dienst erforderlich, um mit RMS SP1 ein Computerzertifikat zu erhalten.</td>
<td style="border:1px solid black;">RMS-Computerzertifikate</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lockboxes</td>
<td style="border:1px solid black;">Enthalten den privaten Schlüssel des Computers sowie ein entsprechendes Zertifikat mit dem öffentlichen Schlüssel des Computers.</td>
<td style="border:1px solid black;">Aktivierungsdienst für RMS Version 1.0. Es ist kein Dienst erforderlich, um mit RMS SP1 eine Lockbox zu erhalten. Die Lockbox enthält den privaten Computerschlüssel. Dies ist der Kernsicherheitsprinzipal für das Verschlüsseln und Entschlüsseln.</td>
<td style="border:1px solid black;">Lockboxes</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rechtekontozertifikate</td>
<td style="border:1px solid black;">Identifizieren einen bestimmten Benutzer als vertrauenswürdig für RMS.</td>
<td style="border:1px solid black;">Rechtekontozertifizierungsdienst</td>
<td style="border:1px solid black;">Rechtekontozertifikate</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Client-Lizenzgeberzertifikate</td>
<td style="border:1px solid black;">Ermöglichen einem Benutzer das Veröffentlichen von RMS-geschütztem Inhalt, während er nicht mit dem Netzwerk verbunden ist.
(Optional)</td>
<td style="border:1px solid black;">RMS-Veröffentlichungsdienst.</td>
<td style="border:1px solid black;">Client-Lizenzgeberzertifikate</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Veröffentlichungslizenzen</td>
<td style="border:1px solid black;">Definieren die Nutzungsrechte für einen bestimmten Inhalt.</td>
<td style="border:1px solid black;">Diese Lizenz kann vom RMS-Veröffentlichungsdienst bzw. im Falle von Offlineveröffentlichung vom Clientlizenzgeber ausgestellt werden.</td>
<td style="border:1px solid black;">Veröffentlichungslizenzen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Nutzungslizenzen</td>
<td style="border:1px solid black;">Ermöglichen einem Benutzer das Abrufen von RMS-geschütztem Inhalt.</td>
<td style="border:1px solid black;">RMS-Lizenzierungsdienst.</td>
<td style="border:1px solid black;">Nutzungslizenzen</td>
</tr>
</tbody>
</table>
