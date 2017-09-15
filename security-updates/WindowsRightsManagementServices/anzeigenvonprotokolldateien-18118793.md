---
TOCTitle: Anzeigen von Protokolldateien
Title: Anzeigen von Protokolldateien
ms:assetid: '2dc9ed54-76d8-4721-ba93-194845de726a'
ms:contentKeyID: 18118793
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720228(v=WS.10)'
---

Anzeigen von Protokolldateien
=============================

Je nachdem, wie Sie RMS bereitgestellt haben, werden Protokolldateien in einem Datenbankserver wie dem SQL Server- oder der Microsoft® SQL Server 2000 Desktop Engine-Datenbank (MSDE 2000) gespeichert. Sie können Filter schreiben, mit denen sich die in den Protokolldateien gespeicherten Informationen reduzieren lassen. Anleitungen hierzu finden Sie in der Hilfe zu SQL Server Enterprise Manager.

Die Größe eines typischen Protokolleintrags beträgt etwa 300 Bytes. In der folgenden Tabelle werden die protokollierten Felder beschrieben.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Feld</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>HostMachineName</p></td>
<td style="border:1px solid black;"><p>Der Computer, der die Anforderung verarbeitet hat.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>HostMachineRequestId</p></td>
<td style="border:1px solid black;"><p>Identifiziert diese Anforderung eindeutig auf diesem Computer. Die Kombination aus HostMachineName und HostMachineRequestId identifiziert die Anforderung eindeutig im Cluster.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestTime</p></td>
<td style="border:1px solid black;"><p>Die Uhrzeit in UTC (Coordinated Universal Time, Greenwich Mean Time), zu der die Anforderung einging.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RequestPath</p></td>
<td style="border:1px solid black;"><p>Relativer URL zur ASMX-Datei. Beispiel: /_wmcs/licensing/License.asmx.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestType</p></td>
<td style="border:1px solid black;"><p>Name der aufgerufenen Webmethode. Beispiel: AcquireLicense.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>RequestUserAddress</p></td>
<td style="border:1px solid black;"><p>Die Quell-IP-Adresse des Anfordernden</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>RequestUserAgent</p></td>
<td style="border:1px solid black;"><p>Wert des Benutzer-Agenten des HTTP-Headers.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>AuthenticatedState</p></td>
<td style="border:1px solid black;"><p>Gibt an, ob die HTTP-Verbindung authentifiziert wurde (True/False).</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SecureConnectionState</p></td>
<td style="border:1px solid black;"><p>Gibt an, ob es sich um eine SSL-Verbindung handelt (True/False).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>AuthenticatedId</p></td>
<td style="border:1px solid black;"><p>Anmeldename für authentifizierte Anforderungen. Ist leer, wenn AuthenticatedState=False.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ReceivedXrMLDocument</p></td>
<td style="border:1px solid black;"><p>Das vom Anfordernden empfangene XrML-Dokument.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>ReceivedXrMLDocumentIssuerChain</p></td>
<td style="border:1px solid black;"><p>Die Ausstellerkette des empfangenen XrML-Dokuments.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>IssuedXrMLDocument</p></td>
<td style="border:1px solid black;"><p>Das an den Anfordernden zurückgegebene XrML-Dokument.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>IssuedXrMLDocumentIssuerChain</p></td>
<td style="border:1px solid black;"><p>Die Ausstellerkette des ausgestellten XrML-Dokuments.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>SuccessOrFailure</p></td>
<td style="border:1px solid black;"><p>Gibt an, ob die Anforderung erfolgreich war oder fehlgeschlagen ist (Succeeded/Failed).</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Metadaten</p></td>
<td style="border:1px solid black;"><p>Metadatenfeld</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>ErrorInformation</p></td>
<td style="border:1px solid black;"><p>Beschreibende Fehlermeldung, wenn ein Fehler auftritt.</p></td>
</tr>  
</tbody>  
</table>
