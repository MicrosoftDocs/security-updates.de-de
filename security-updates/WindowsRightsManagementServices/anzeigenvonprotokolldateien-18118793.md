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
<td style="border:1px solid black;">HostMachineName</td>
<td style="border:1px solid black;">Der Computer, der die Anforderung verarbeitet hat.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">HostMachineRequestId</td>
<td style="border:1px solid black;">Identifiziert diese Anforderung eindeutig auf diesem Computer. Die Kombination aus HostMachineName und HostMachineRequestId identifiziert die Anforderung eindeutig im Cluster.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestTime</td>
<td style="border:1px solid black;">Die Uhrzeit in UTC (Coordinated Universal Time, Greenwich Mean Time), zu der die Anforderung einging.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestPath</td>
<td style="border:1px solid black;">Relativer URL zur ASMX-Datei. Beispiel: /_wmcs/licensing/License.asmx.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestType</td>
<td style="border:1px solid black;">Name der aufgerufenen Webmethode. Beispiel: AcquireLicense.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">RequestUserAddress</td>
<td style="border:1px solid black;">Die Quell-IP-Adresse des Anfordernden</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RequestUserAgent</td>
<td style="border:1px solid black;">Wert des Benutzer-Agenten des HTTP-Headers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedState</td>
<td style="border:1px solid black;">Gibt an, ob die HTTP-Verbindung authentifiziert wurde (True/False).</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SecureConnectionState</td>
<td style="border:1px solid black;">Gibt an, ob es sich um eine SSL-Verbindung handelt (True/False).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">AuthenticatedId</td>
<td style="border:1px solid black;">Anmeldename für authentifizierte Anforderungen. Ist leer, wenn AuthenticatedState=False.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ReceivedXrMLDocument</td>
<td style="border:1px solid black;">Das vom Anfordernden empfangene XrML-Dokument.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ReceivedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Die Ausstellerkette des empfangenen XrML-Dokuments.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">IssuedXrMLDocument</td>
<td style="border:1px solid black;">Das an den Anfordernden zurückgegebene XrML-Dokument.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">IssuedXrMLDocumentIssuerChain</td>
<td style="border:1px solid black;">Die Ausstellerkette des ausgestellten XrML-Dokuments.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">SuccessOrFailure</td>
<td style="border:1px solid black;">Gibt an, ob die Anforderung erfolgreich war oder fehlgeschlagen ist (Succeeded/Failed).</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Metadaten</td>
<td style="border:1px solid black;">Metadatenfeld</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ErrorInformation</td>
<td style="border:1px solid black;">Beschreibende Fehlermeldung, wenn ein Fehler auftritt.</td>
</tr>
</tbody>
</table>
