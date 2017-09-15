---
TOCTitle: 'Ändern der Active Directory-Cacheeinstellungen'
Title: 'Ändern der Active Directory-Cacheeinstellungen'
ms:assetid: '8789a7a5-2065-4fae-9104-e0a70f1f2fb6'
ms:contentKeyID: 18118926
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747586(v=WS.10)'
---

Ändern der Active Directory-Cacheeinstellungen
==============================================

Die Einstellungen in der Registrierung geben die Anzahl von Einträgen an, die im Active Directory-Cache gespeichert werden sollen. Sie können diese Einstellungen ändern, um die Antwortzeit bei Clientanforderungen zu verbessern. Weitere Informationen hierzu finden Sie oben unter „Optimieren der Leistung der Verzeichnisdienste“. Sie können auch den Gültigkeitszeitraum für Informationen angeben, die im Cache zwischengespeichert werden.

Auf Computern mit der 32-Bit-Version von Windows Server 2003 ist der folgende Registrierungsschlüssel der vollständige Unterschlüsselpfad für die Cacheeinträge:

**HKEY\_LOCAL\_MACHINE\\Software\\Microsoft\\DRMS\\1.0\\DirectoryServices**

Auf Computern mit der 64-Bit-Version von Windows Server 2003 ist der folgende Registrierungsschlüssel der vollständige Unterschlüsselpfad für die Cacheeinträge:

**HKEY\_LOCAL\_MACHINE\\SoftwareWOW6432Node\\Microsoft\\DRMS\\1.0\\DirectoryServices**

In der folgenden Tabelle werden die Einträge aufgelistet, die das Verhalten des Speichercaches steuern.

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
<th>Name</th>
<th>Typ</th>
<th>Standardwert</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>PrincipalCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>Maximale Anzahl von Prinzipalen sowie von deren E-Mail-Adressen und SIDs, die im Cache zwischengespeichert werden können.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>PrincipalCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>Gültigkeitszeitraum der zwischengespeicherten Informationen für Prinzipale.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>GroupIDCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>Maximale Anzahl von Gruppen sowie von deren E-Mail-Adressen und SIDs, die im Cache zwischengespeichert werden können.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>GroupIDCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>Gültigkeitszeitraum der zwischengespeicherten Informationen für Gruppenmitgliedschaft.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>GroupMembershipCacheMax</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>1,000</p></td>
<td style="border:1px solid black;"><p>Maximale Anzahl von Kontakten, die Mitglieder einer Gruppe sind, die im Cache gespeichert werden können.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>GroupMembershipCacheExpireMinutes</p></td>
<td style="border:1px solid black;"><p>DWORD</p></td>
<td style="border:1px solid black;"><p>12</p></td>
<td style="border:1px solid black;"><p>Gültigkeitszeitraum der zwischengespeicherten Informationen für Kontakte, die Mitglieder einer Gruppe sind.</p></td>
</tr>  
</tbody>  
</table>
  
| ![](images/Cc747586.Caution(WS.10).gif)Vorsicht                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Durch falsches Bearbeiten der Registrierung kann das System schwerwiegend beschädigt werden. Deshalb sollten Sie alle wichtigen Daten auf dem Computer sichern, bevor Sie Änderungen an der Registrierung vornehmen. |
  
| ![](images/Cc747586.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                           |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Die Registrierungeinträge **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** und **ContactMembersofGroupCacheExpireMinutes** steuern auch die Cacheablaufzeit für den lokalen Active Directory-Cache; dieser ist in der Datenbank der Verzeichnisdienste auf Ihrem Datenbankserver gespeichert. |
