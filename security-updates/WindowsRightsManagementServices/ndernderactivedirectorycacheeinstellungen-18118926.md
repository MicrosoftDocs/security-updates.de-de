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

 
<table style="border:1px solid black;">
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Typ</th>
<th style="border:1px solid black;" >Standardwert</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrincipalCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximale Anzahl von Prinzipalen sowie von deren E-Mail-Adressen und SIDs, die im Cache zwischengespeichert werden können.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Gültigkeitszeitraum der zwischengespeicherten Informationen für Prinzipale.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupIDCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximale Anzahl von Gruppen sowie von deren E-Mail-Adressen und SIDs, die im Cache zwischengespeichert werden können.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIDCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Gültigkeitszeitraum der zwischengespeicherten Informationen für Gruppenmitgliedschaft.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembershipCacheMax</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">1,000</td>
<td style="border:1px solid black;">Maximale Anzahl von Kontakten, die Mitglieder einer Gruppe sind, die im Cache gespeichert werden können.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupMembershipCacheExpireMinutes</td>
<td style="border:1px solid black;">DWORD</td>
<td style="border:1px solid black;">12</td>
<td style="border:1px solid black;">Gültigkeitszeitraum der zwischengespeicherten Informationen für Kontakte, die Mitglieder einer Gruppe sind.</td>
</tr>
</tbody>
</table>
  
| ![](images/Cc747586.Caution(WS.10).gif)Vorsicht                                                                                                                                         |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Durch falsches Bearbeiten der Registrierung kann das System schwerwiegend beschädigt werden. Deshalb sollten Sie alle wichtigen Daten auf dem Computer sichern, bevor Sie Änderungen an der Registrierung vornehmen. |
  
| ![](images/Cc747586.note(WS.10).gif)Hinweis                                                                                                                                                                                                                                                                           |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Die Registrierungeinträge **PrincipalCacheExpireMinutes**, **GroupIDCacheExpireMinutes**, **GroupMembershipCacheExpireMinutes** und **ContactMembersofGroupCacheExpireMinutes** steuern auch die Cacheablaufzeit für den lokalen Active Directory-Cache; dieser ist in der Datenbank der Verzeichnisdienste auf Ihrem Datenbankserver gespeichert. |
