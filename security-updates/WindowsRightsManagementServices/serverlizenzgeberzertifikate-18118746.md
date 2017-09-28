---
TOCTitle: 'Server-Lizenzgeberzertifikate'
Title: 'Server-Lizenzgeberzertifikate'
ms:assetid: '0b35fbcd-25a9-4587-898d-9a30fd1d3c5b'
ms:contentKeyID: 18118746
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720184(v=WS.10)'
---

Server-Lizenzgeberzertifikate
=============================

Ein Server-Lizenzgeberzertifikat gewährt einem RMS-Server die Berechtigung, Zertifikate und Lizenzen auszustellen. Wenn der erste Stammzertifizierungsserver Ihrer RMS-Bereitstellung aktiviert wird, erhält er über den Microsoft-Registrierungsdienst ein Server-Lizenzgeberzertifikat. Mit diesem Vorgang wird die Registrierung abgeschlossen. Dieses Zertifikat enthält den öffentlichen Schlüssel des Stammzertifizierungsservers und wird mit dem privaten Schlüssel des Registrierungsdienstes signiert. Andere zum Stammzertifizierungscluster hinzugefügte Server nutzen dieses Zertifikat gemeinsam.

Während der Bereitstellung erhält der erste Lizenzierungsserver eines Clusters ein Server-Lizenzgeberzertifikat über den RMS-Stammzertifizierungsserver bzw. -cluster. Dieser Vorgang nennt sich Unterregistrierung. Dieses Zertifikat enthält den öffentlichen Schlüssel des Lizenzierungsservers und wird mit dem privaten Schlüssel des Stammzertifizierungsservers oder -clusters signiert. Andere zum Lizenzierungscluster hinzugefügte Server nutzen dieses Zertifikat gemeinsam.

In der folgenden Tabelle werden die Rechte aufgelistet, die Servern durch Server-Lizenzgeberzertifikate erteilt werden.

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
<th>Recht zum Ausstellen von Folgendem</th>
<th>Server-Lizenzgeberzertifikat für einen Stammzertifizierungsserver</th>
<th>Server-Lizenzgeberzertifikat für einen Lizenzierungsserver</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Rechtekontozertifikate</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
<td style="border:1px solid black;"><p>Nein</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Veröffentlichungslizenzen</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Nutzungslizenzen</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Untergeordnete Server-Lizenzgeberzertifikate</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
<td style="border:1px solid black;"><p>Nein</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Client-Lizenzgeberzertifikate</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
<td style="border:1px solid black;"><p>Ja</p></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720184.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Für RMS sind separate Lizenzierungsserver bzw. -cluster nicht erforderlich, doch sind sie gut dafür geeignet, Lizenzierungsanforderungen vom Stammzertifizierungscluster zu übernehmen. Administratoren können außerdem Lizenzierungsserver einrichten, um den Bedürfnissen interner Organisationen gerecht zu werden, die die Veröffentlichung sicherer Inhalte direkt steuern müssen. Beispiel: In den allgemeinen Unternehmensrichtlinien, die in den Vorlagen für Benutzerrechterichtlinien des Stammzertifizierungsservers oder -clusters implementiert sind, können möglicherweise einige der von einer bestimmten Abteilung benötigen Rechte nicht angegeben werden. In diesem Fall kann die Abteilung einen separaten Lizenzierungsserver oder -cluster zum Speichern ihrer Vorlagen für Benutzerrechterichtlinien und zum Verarbeiten der Lizenzierungsanforderungen bereitstellen. |
