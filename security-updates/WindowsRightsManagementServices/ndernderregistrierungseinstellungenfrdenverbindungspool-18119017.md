---
TOCTitle: Ändern der Registrierungseinstellungen für den Verbindungspool
Title: Ändern der Registrierungseinstellungen für den Verbindungspool
ms:assetid: 'c61d91db-a1ad-4ca5-a492-015da629afbc'
ms:contentKeyID: 18119017
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747660(v=WS.10)'
---

Ändern der Registrierungseinstellungen für den Verbindungspool
==============================================================

Zur Verbesserung der Systemleistung können Sie die Eigenschaften des von RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendeten Active Directory-LDAP-Verbindungspools (Lightweight Directory Access Protocol) mithilfe von Registrierungsschlüsseleinträgen festlegen.

Auf Computern mit der 32-Bit-Version von Windows Server 2003 ist der folgende Registrierungsschlüssel der vollständige Unterschlüsselpfad für die Registrierungseinstellungen des Verbindungspools:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0**

Auf Computern mit der 64-Bit-Version von Windows Server 2003 ist der folgende Registrierungsschlüssel der vollständige Unterschlüsselpfad für die Registrierungseinstellungen des Verbindungspools:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0**

In der folgenden Tabelle werden die Einträge aufgelistet, die Sie hinzufügen können, um die Standardeinstellungen des Active Directory-Verbindungspools außer Kraft zu setzen. Die angezeigten Werte sind die Standardwerte. Weitere Informationen zum Erstellen einer Abfrageliste und Verwenden dieser Einstellungen in RMS finden Sie oben unter „Optimieren der Einstellungen für den Active Directory-Verbindungspool“.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th>Name</th>
<th>Typ</th>
<th>Standardwert</th>
<th>Beschreibung</th>
<th>Anmerkungen</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GC</td>
<td style="border:1px solid black;">Zeichenfolge</td>
<td style="border:1px solid black;">name-1, ..., name-n</td>
<td style="border:1px solid black;">Durch Komma getrennte Liste der globalen Kataloge (mithilfe von DNS-Namen). Bei Einsatz dieses Schlüssels kann RMS nur die angegebenen globalen Kataloge verwenden.</td>
<td style="border:1px solid black;">Wenn RMS keine Abfrageliste erstellen soll, geben Sie mit dieser Einstellung die zu verwendenden globalen Kataloge an.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">MinGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Mindestanzahl der globalen Kataloge, die verfügbar sein müssen, bevor RMS gestartet werden kann.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">MaxGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">15</td>
<td style="border:1px solid black;">Höchstanzahl der globalen Kataloge, die der Algorithmus für die Topologieerkennung zur Abfrageliste hinzufügen soll.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ThreshHoldAlive</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Mindestanzahl der Verbindungen, die aktiv sein sollten, bevor die Suchdienste mit der Suche nach globalen Katalogen beginnen, die zur Abfrageliste hinzugefügt werden sollen, damit RMS Anforderungen annehmen kann.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">RetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Gibt an, wie oft eine unterbrochene Verbindung wiederholt werden soll, bevor sie als nicht reagierend deklariert wird.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TimeRetryDown</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">300</td>
<td style="border:1px solid black;">Gibt an, wie viele Sekunden gewartet werden soll, bevor eine unterbrochene Verbindung wiederholt wird.</td>
<td style="border:1px solid black;">Eine Änderung dieser Standardeinstellung sollte nur unter ungewöhnlichen Umständen erforderlich sein.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeRetrySlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">30</td>
<td style="border:1px solid black;">Gibt an, wie viele Sekunden gewartet werden soll, bevor eine langsame Verbindung erneut versucht wird.</td>
<td style="border:1px solid black;">Eine Änderung dieser Standardeinstellung sollte nur unter ungewöhnlichen Umständen erforderlich sein.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtRoundRobin</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1</td>
<td style="border:1px solid black;">Gewichtung von Round-Robin während des Lastenausgleichs.</td>
<td style="border:1px solid black;">Die relative Bedeutung von Round-Robin beim Lastenausgleich. 1 ist der niedrigste Wert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">WtThreadCount</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">100</td>
<td style="border:1px solid black;">Gewichtung der Threadanzahl pro Verbindung während des Lastenausgleichs.</td>
<td style="border:1px solid black;">Die relative Bedeutung einer geringen Threadanzahl.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">WtSlow</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Gewichtung der langsamen Verbindung während des Lastenausgleichs.</td>
<td style="border:1px solid black;">Die relative Bedeutung der nicht langsamen Verbindung.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TimeOutForGC</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Gibt an, wie viele Sekunden gewartet werden soll, bevor eine Anforderung zum Hinzufügen eines globalen Katalogs zur Abfrageliste das Zeitlimit überschreitet.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">LdapTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">5</td>
<td style="border:1px solid black;">Gibt an, wie viele Sekunden gewartet werden soll, bevor LDAP-APIs das Zeitlimit überschreiten.</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">TopDownExpansionLDAPTimeOut</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">40</td>
<td style="border:1px solid black;">Gibt an, wie viele Sekunden gewartet werden soll, bevor hierarchische LDAP-Erweiterungsabfragen das Zeitlimit überschreiten.</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Vorsicht                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Durch falsches Bearbeiten der Registrierung kann das System schwerwiegend beschädigt werden. Deshalb sollten Sie alle wichtigen Daten auf dem Computer sichern, bevor Sie Änderungen an der Registrierung vornehmen. |
