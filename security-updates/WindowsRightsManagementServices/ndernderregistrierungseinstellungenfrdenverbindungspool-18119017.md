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

<p> </p>
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
<td style="border:1px solid black;"><p>GC</p></td>
<td style="border:1px solid black;"><p>Zeichenfolge</p></td>
<td style="border:1px solid black;"><p>name-1, ..., name-n</p></td>
<td style="border:1px solid black;"><p>Durch Komma getrennte Liste der globalen Kataloge (mithilfe von DNS-Namen). Bei Einsatz dieses Schlüssels kann RMS nur die angegebenen globalen Kataloge verwenden.</p></td>
<td style="border:1px solid black;"><p>Wenn RMS keine Abfrageliste erstellen soll, geben Sie mit dieser Einstellung die zu verwendenden globalen Kataloge an.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>MinGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Mindestanzahl der globalen Kataloge, die verfügbar sein müssen, bevor RMS gestartet werden kann.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>MaxGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>15</p></td>
<td style="border:1px solid black;"><p>Höchstanzahl der globalen Kataloge, die der Algorithmus für die Topologieerkennung zur Abfrageliste hinzufügen soll.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ThreshHoldAlive</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Mindestanzahl der Verbindungen, die aktiv sein sollten, bevor die Suchdienste mit der Suche nach globalen Katalogen beginnen, die zur Abfrageliste hinzugefügt werden sollen, damit RMS Anforderungen annehmen kann.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>RetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie oft eine unterbrochene Verbindung wiederholt werden soll, bevor sie als nicht reagierend deklariert wird.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TimeRetryDown</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>300</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie viele Sekunden gewartet werden soll, bevor eine unterbrochene Verbindung wiederholt wird.</p></td>
<td style="border:1px solid black;"><p>Eine Änderung dieser Standardeinstellung sollte nur unter ungewöhnlichen Umständen erforderlich sein.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TimeRetrySlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>30</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie viele Sekunden gewartet werden soll, bevor eine langsame Verbindung erneut versucht wird.</p></td>
<td style="border:1px solid black;"><p>Eine Änderung dieser Standardeinstellung sollte nur unter ungewöhnlichen Umständen erforderlich sein.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WtRoundRobin</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1</p></td>
<td style="border:1px solid black;"><p>Gewichtung von Round-Robin während des Lastenausgleichs.</p></td>
<td style="border:1px solid black;"><p>Die relative Bedeutung von Round-Robin beim Lastenausgleich. 1 ist der niedrigste Wert.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>WtThreadCount</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>100</p></td>
<td style="border:1px solid black;"><p>Gewichtung der Threadanzahl pro Verbindung während des Lastenausgleichs.</p></td>
<td style="border:1px solid black;"><p>Die relative Bedeutung einer geringen Threadanzahl.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>WtSlow</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>Gewichtung der langsamen Verbindung während des Lastenausgleichs.</p></td>
<td style="border:1px solid black;"><p>Die relative Bedeutung der nicht langsamen Verbindung.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TimeOutForGC</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie viele Sekunden gewartet werden soll, bevor eine Anforderung zum Hinzufügen eines globalen Katalogs zur Abfrageliste das Zeitlimit überschreitet.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>LdapTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>5</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie viele Sekunden gewartet werden soll, bevor LDAP-APIs das Zeitlimit überschreiten.</p></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>TopDownExpansionLDAPTimeOut</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>40</p></td>
<td style="border:1px solid black;"><p>Gibt an, wie viele Sekunden gewartet werden soll, bevor hierarchische LDAP-Erweiterungsabfragen das Zeitlimit überschreiten.</p></td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747660.Caution(WS.10).gif)Vorsicht                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Durch falsches Bearbeiten der Registrierung kann das System schwerwiegend beschädigt werden. Deshalb sollten Sie alle wichtigen Daten auf dem Computer sichern, bevor Sie Änderungen an der Registrierung vornehmen. |
