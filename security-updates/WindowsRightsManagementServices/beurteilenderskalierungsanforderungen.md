---
TOCTitle: Beurteilen der Skalierungsanforderungen
Title: Beurteilen der Skalierungsanforderungen
ms:assetid: '89f0138c-946d-47d7-a286-041d4d9606a8'
ms:contentKeyID: 18118918
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747663(v=WS.10)'
---

Beurteilen der Skalierungsanforderungen
=======================================

Um zu ermitteln, ob ein einzelner oder mehrere Server eingesetzt werden sollen, muss ermittelt werden, wie viele Benutzer die RMS-Bereitstellung nutzen, und wie viele Dateien zu schützen sein werden.

So werden durchschnittliche Nutzungsanforderungen ermittelt. In jedem Fall müssen auch für Nutzungsspitzen Vorkehrungen getroffen werden, die etwa um das Dreifache über normalen Anforderungen liegen werden.

Darüber hinaus sind Fehlertoleranz und Standards der Diensteverfügbarkeit des Unternehmens zu berücksichtigen.

Für die Ermittlung eines Maßstabs wurde RMS mit einem Server mit 2,4-GHz Pentium 4 mit Koprozessor und 1 GB RAM getestet. In dieser Konfiguration lieferte der RMS-Server etwa 50 Lizenzen pro Sekunde.

Sie können die folgenden Zahlen während der Kapazitätsplanung verwenden, um die Anforderungen für ein RMS-System zu bestimmen.

<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transaktion</th>
<th style="border:1px solid black;" >Vorkommen</th>
<th style="border:1px solid black;" >Client-Server-Bandbreitenverwendung (KB)</th>
<th style="border:1px solid black;" >Server-Client-Bandbreitenverwendung (KB)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lizenzanforderung</td>
<td style="border:1px solid black;">Wiederholt für jeden Benutzer und für jeden Inhalt</td>
<td style="border:1px solid black;">64</td>
<td style="border:1px solid black;">18</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Rechtekontozertifizierung</td>
<td style="border:1px solid black;">Ausschließlich bei RMS-Initialisierungsverkehr</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">16</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Clientregistrierung</td>
<td style="border:1px solid black;">Ausschließlich bei RMS-Initialisierungsverkehr</td>
<td style="border:1px solid black;">17</td>
<td style="border:1px solid black;">16</td>
</tr>
</tbody>
</table>
  
Zusätzlich kann der Active Directory-Abfrageverkehr einen Einfluss auf den Netzwerkdurchsatz haben. Dies ist jedoch üblicherweise kein Faktor, wenn RMS-Server in der Nähe der Server mit dem globalen Katalog positioniert werden. Die Ausnahme hierzu wäre, wenn ein Versagen aller Server mit globalen Katalogen an einem Standort ein Failover bei einem anderen Standort über eine Verbindung hervorrufen würde, die nicht die gleiche Kapazität besitzt.
  
In der folgenden Tabelle sind Basisdaten zur Bandbreitennutzung durch RMS-Transaktionen aufgeführt, mit deren Hilfe der Effekt des Abfrageverkehrs von Active Directory innerhalb des Organisationsnetzwerks ermittelt werden kann.
  
<p></p>
<table style="border:1px solid black;">
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Transaktion</th>
<th style="border:1px solid black;" >Bandbreitennutzung – RMS an globalen Katalog (Byte)</th>
<th style="border:1px solid black;" >Bandbreitennutzung – Globaler Katalog an RMS (Byte)</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Herstellen von RMS-Verbindungen (ldap_bind)</td>
<td style="border:1px solid black;">1600</td>
<td style="border:1px solid black;">200</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Auswertung der RMS-Gruppenzugehörigkeit (ldap_search)</td>
<td style="border:1px solid black;">200</td>
<td style="border:1px solid black;">100</td>
</tr>
</tbody>
</table>
  
Wenn diese Referenztabellen verwendet werden, sollte sichergestellt werden, dass die Menge aus dem Inhalt der Bereitstellung verwendet wird. Wenn ein Benutzer beispielsweise 15 Gruppen angehört, wären 200 Byte für eine Suchanfrage aus RMS nötig sowie 1500 Byte (100 Byte \* 15) für die Antwort vom globalen Katalog.
  
Die Planung der Kapazitäten sollte auf den geschätzten Anforderungslasten für Inhaltslizenzen basieren, da diese die Mehrheit der Operationen darstellen, die RMS ausführt. Die Eingabe/Ausgabe-Geschwindigkeit und der Umsatz des Laufwerks sind keine kritischen Faktoren für RMS, da Lizenzanforderungen nicht datenintensiv sind und vollständig mit Cache-Daten auskommen.
  
Die CPU-Verwendung ist die wichtigste Variable beim Ermitteln des Serverdurchsatzes. Die Auswahl der geeigneten Prozessoren ist daher wesentlich. Speicheranforderungen auf RMS-Servern wachsen mit der Serverbelastung, insbesondere wenn diese den maximalen Umsatz des Servers übersteigt. In diesem Fall erstellt Internetinformationsdienste (Internet Information Services oder IIS) eine Warteschlange für eingehende Anforderungen im Arbeitsspeicher, bis der Server die Anforderungen verarbeiten kann. Basierend auf der Begrenzung für die in IIS konfigurierbare Warteschlange werden eingehende Anforderungen nicht mehr in die Warteschlange aufgenommen. Die Anforderungen werden verworfen, wenn die Warteschlange die angegebene maximale Länge erreicht.
  
Die werkseitig eingestellten Speicheranforderungen von RMS für ein Belastungsmuster sollten die Größe des physikalischen Speichers nicht überschreiten. Die Gesamtarbeitsspeichergröße wird hauptsächlich durch erforderlichen Zwischenspeicher bei Gruppenerweiterungsoperationen erhöht. Es wird mindestens 1 GB RAM für jeden Server empfohlen, der RMS ausführt.
  
Jeder RMS-Server kann eine bestimmte Anzahl von Clientanfragen in einem bestimmten Zeitraum verarbeiten; etwa 30 bis 50 Lizenzen pro Sekunde. Das Hinzufügen von Servern vergrößert daher linear die Gesamtkapazität eines Clusters für die Lizenzausstellung und bietet eine höhere Zuverlässigkeit. Skalierbarkeit ist daher nicht nur für jeden einzelnen Server sondern auch für die Anzahl von bereitgestellten Servern empfehlenswert. Die folgenden Konfigurationsbeispiele verdeutlichen, wie mithilfe dieser Schätzungen die Skalierungsanforderungen für die RMS-Bereitstellung berechnet werden kann.
  
-   Konfiguration für leichte Nutzung  

    Manche Organisationen haben nur recht geringe Nutzungsanforderungen an RMS. Beispiel: Eine Organisation mit 5.000 Benutzern, von denen 500 regelmäßig RMS für das Schützen von E-Mail-Inhalten verwenden, geht davon aus, dass ein durchschnittlicher Benutzer pro Stunde 3 E-Mail-Nachrichten schützt. Auf der Basis dieser Bedingungen müssten RMS-Server etwa 1.500 Lizenzen pro Stunde bereitstellen, also 0,42 Lizenzen pro Sekunde. Hierbei handelt es sich um die durchschnittliche Verwendungsanforderung. Die Multiplikation dieser Zahl mit dem Faktor 3 ergibt die maximale Verwendungsanforderung von 1,25 Lizenzen pro Sekunde.  

    Basierend auf dieser Berechnung kann die Verwendung als sehr gering bewertet werden. Für diese Organisation bietet sich daher die Bereitstellung eines einzelnen Servers mit RMS an.  
-   Konfiguration für mittelschwere Nutzung  

    Viele Organisationen verfügen über recht große Benutzergruppen mit moderaten Verwendungsanforderungen. Beispiel: Eine Organisation mit 40.000 Benutzern, von denen 20.000 regelmäßig RMS für das Schützen von Inhalten verwenden, geht davon aus, dass ein durchschnittlicher Benutzer pro Stunde 7 E-Mail-Nachrichten und 1 Dokument schützt. Auf der Basis dieser Bedingungen müssten RMS-Server etwa 160.000 Lizenzen pro Stunde bereitstellen, also 44,4 Lizenzen pro Sekunde. Hierbei handelt es sich um die durchschnittliche Verwendungsanforderung. Die Multiplikation dieser Zahl mit dem Faktor 3 ergibt die maximale Verwendungsanforderung von 133.3 Lizenzen pro Sekunde.  

    Aus dieser Berechnung ergibt sich eine moderate Verwendung. Die Bereitstellung von 3 Servern mit RMS deckt in diesem Fall die aktuellen Benutzeranforderungen ab. Bei einer Anzahl von 6 Servern mit RMS können die aktuellen Benutzeranforderungen und mögliche zukünftige Skalierungsanforderungen erfüllt werden.  
-   Konfiguration für schwere Nutzung  

    Größere Organisationen verfügen häufig über extrem große Benutzergruppen mit hohen Verwendungsanforderungen. Beispiel: Eine Organisation mit 150.000 Benutzern, von denen 105.000 regelmäßig RMS für das Schützen von Inhalten verwenden, geht davon aus, dass ein durchschnittlicher Benutzer pro Stunde 15 E-Mail-Nachrichten und 3 Dokumente schützt. Auf der Basis dieser Bedingungen müssten RMS-Server etwa 1.890.000 Lizenzen pro Stunde bereitstellen, also 525 Lizenzen pro Sekunde. Hierbei handelt es sich um die durchschnittliche Verwendungsanforderung. Die Multiplikation dieser Zahl mit dem Faktor 3 ergibt die maximale Verwendungsanforderung von 1575 Lizenzen pro Sekunde. 
     
    Aus dieser Berechnung ergeben sich sehr hohe Verwendungsanforderungen. Die Bereitstellung von 32 Servern mit RMS deckt in diesem Fall die aktuellen Benutzeranforderungen ab. Bei einer Anzahl von 51 Servern mit RMS könnten die aktuellen Benutzeranforderungen und mögliche zukünftige Skalierungsanforderungen erfüllt werden.
  
Wenn Ihre Berechnungen 30 bis 50 zu liefernde Lizenzen pro Sekunde ergeben, ist gewöhnlich ein weiterer Server mit RMS erforderlich.
