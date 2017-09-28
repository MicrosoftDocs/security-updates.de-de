---
TOCTitle: 'RMS-Sperrlisten'
Title: 'RMS-Sperrlisten'
ms:assetid: '688d4dfa-c928-4b2f-8116-2f9e87d2b6f7'
ms:contentKeyID: 18118877
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720287(v=WS.10)'
---

RMS-Sperrlisten
===============

Sperrlisten geben die Inhalte, Anwendungen, Benutzer oder anderen Prinzipale an, die gesperrt wurden. Eine Organisation könnte eine in einer Sperrliste aufgeführte Entität aus einem oder mehreren der folgenden Gründe einschließen:

-   Ein privater Schlüssel ist unbekannt oder scheint unsicher zu sein.
-   Ein Besitzer fordert die Sperrung eines Schlüssels an, der unsicher zu sein scheint.
-   Ein Prinzipal ist nicht mehr gültig (beispielsweise wurde ein Mitarbeiter gekündigt).
-   Es liegt ein Problem bei der Durchsetzung von Sicherheit vor (beispielsweise ist ein für einen Clientcomputer ausgestelltes Zertifikat unsicher).
-   Eine erneute Zertifizierung ist aufgrund von Autorisierungsänderungen erforderlich.
-   Aufgrund vorhandener Sicherheitslücken in einer RMS-fähigen Anwendung kann sie nicht zum Abrufen streng vertraulichen Inhalts oder geschützten Inhalts jeglicher Art verwendet werden.
-   Zu einem früheren Zeitpunkt verteilte Inhalte sind jetzt veraltet oder zum Abrufen nicht mehr geeignet.

In der folgenden Tabelle werden die Entitäten, die in einer Sperrliste angegeben werden können, zusammen mit den Informationen zum Identifizieren der einzelnen Entitäten beschrieben.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Entität</th>
<th>Bezeichner</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Eine Gruppe von Lizenzen oder Zertifikaten</td>
<td style="border:1px solid black;">Aussteller-ID oder öffentlicher Schlüssel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Eine Gruppe von Anwendungsmanifesten</td>
<td style="border:1px solid black;">Aussteller-ID oder öffentlicher Schlüssel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Eine bestimmte Lizenz oder ein bestimmtes Zertifikat</td>
<td style="border:1px solid black;">Lizenz-ID oder Hash</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Ein bestimmtes Anwendungsmanifest</td>
<td style="border:1px solid black;">Lizenz-ID oder Hash</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ein bestimmter Prinzipal</td>
<td style="border:1px solid black;">Prinzipal-ID oder öffentlicher Schlüssel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Bestimmte Inhalte</td>
<td style="border:1px solid black;">Datei-ID</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc720287.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |  
|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Für die Sperrung und den Ausschluss werden alle Hashes im Format SHA-1 \[NIS94c\], einer Überarbeitung des SHA-Algorithmus (Secure Hash Algorithm oder Sicherer Hash-Algorithmus), angegeben, der im Secure Hash Standard (Sicherer Hash-Standard oder SHS, FIPS 180) angegeben wird. SHA-1 wird im Standard ANSI X9.30 (Teil 2) beschrieben. Zum Sperren nach Anwendungsmanifest müssen Sie entweder die Aussteller-ID, den öffentlichen Schlüssel des Ausstellers, die Lizenz-ID oder den Lizenz-Hash aus dem Anwendungsmanifest extrahieren. Anwendungsmanifeste sind jedoch Base-64-kodiert. Daher sind diese Informationen nicht in lesbarer Form verfügbar. Mit dem Client-SDK für die Rechteverwaltung (Rights Management Services oder RMS) kann ein Programm entwickelt werden, das zur Dekodierung des Anwendungsmanifests und zum Abruf der erforderlichen Informationen die Methoden **DRMConstructCertificateChain**, **DRMDeconstructCertificateChain** und **DRMDecode** verwendet. Wenn Sie nicht möchten, dass eine bestimmte Anwendung RMS-geschützte Inhalte abrufen kann, sollten Sie mithilfe eines Anwendungsausschlusses verhindern, dass der RMS-Server dieser Anwendung Nutzungslizenzen erteilt. Ein Anwendungsausschluss kann jedoch nicht verhindern, dass ein Benutzer mit einer gültigen Nutzungslizenz RMS-geschützte Inhalte entschlüsselt. Weitere Informationen zum Anwendungsausschluss finden Sie unter Ausschließen von Anwendungen im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung. |
  
Bei Sperrlisten handelt es sich um XrML-Dateien, die folgende Parameter angeben:
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Parameter</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ISSUEDTIME</td>
<td style="border:1px solid black;">Die Systemzeit, zu der die XrML-Datei erstellt wurde. Diese wird von der in einer Nutzungslizenz enthaltenen Bedingung REFRESH dazu verwendet, das Alter der Sperrliste zu bestimmen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ISSUER</td>
<td style="border:1px solid black;">Der Name, die ID und Adresse des Sperrlistenausstellers.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PUBLICKEY</td>
<td style="border:1px solid black;">Der öffentliche Schlüssel des Sperrlistenausstellers.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">REVOCATIONLIST</td>
<td style="border:1px solid black;">Der Name, der Typ und die ID jeder gesperrten Entität.</td>
</tr>
</tbody>
</table>
