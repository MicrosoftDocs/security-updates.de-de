---
TOCTitle: 'Datenbank der RMS-Verzeichnisdienste'
Title: 'Datenbank der RMS-Verzeichnisdienste'
ms:assetid: '6f6b8586-5d17-4a40-94a3-4dc738195301'
ms:contentKeyID: 18118875
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747617(v=WS.10)'
---

Datenbank der RMS-Verzeichnisdienste
====================================

Der Datenbankserver hostet die Datenbank der Verzeichnisdienste, die Informationen zu Benutzern, IDs (wie z. B. E-Mail-Adressen), Sicherheits-IDs (SID), Gruppenmitgliedschaften und anderen IDs enthält. Diese Informationen werden durch LDAP-Abfragen ermittelt, die vom RMS-Lizenzierungsdienst an den globalen Katalog von Active Directory gestellt werden. Weitere Informationen zu diesem Prozess und seinem Zweck finden Sie unter „[Active Directory-Cache für RMS](https://technet.microsoft.com/c721a2eb-2fe9-4346-b426-3cc169b97265)“ weiter unten in diesem Thema.

Die RMS Service Group (RMS-Dienstgruppe) verfügt über die Berechtigungen Ausführen für die gespeicherten Prozeduren in der Datenbank der Verzeichnisdienste.

In der folgenden Tabelle werden die Active Directory-Attribute aufgelistet, die in den Datenbanktabellen der Verzeichnisdienste gespeichert sind.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Tabelle</th>
<th>Attribut</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">GroupAliases</td>
<td style="border:1px solid black;"><ul>
<li>GroupName: der Alias für die Gruppe<br />
<br />
</li>
<li>GroupID: die eindeutige ID für diese Gruppe<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">GroupIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>GroupDN: der definierte Active Directory-Name für diese Gruppe<br />
<br />
</li>
<li>GroupID: die eindeutige ID für diese Gruppe<br />
<br />
</li>
<li>Expiration: das Datum und die Uhrzeit, an dem bzw. zu der die Gültigkeit der für diese Gruppe gespeicherten Informationen abläuft<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">GroupMembership</td>
<td style="border:1px solid black;"><ul>
<li>GroupID: die eindeutige ID für diese Gruppe<br />
<br />
</li>
<li>ParentID: die eindeutige ID für die Gruppe, der diese Gruppe angehört<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalAliases</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalName: ein Aliasname für den Prinzipal<br />
<br />
</li>
<li>PrincipalID: die eindeutige ID für diesen Prinzipal<br />
<br />
</li>
</ul></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PrincipalIdentifiers</td>
<td style="border:1px solid black;"><ul>
<li>PrincipalID: die eindeutige ID für diesen Prinzipal<br />
<br />
</li>
<li>Expiration: das Datum und die Uhrzeit, an dem bzw. zu der die Gültigkeit der für diesen Prinzipal gespeicherten Informationen abläuft<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrincipalMembership</td>
<td style="border:1px solid black;">Jede Tabellenzeile schließt die eindeutige ID eines Prinzipals und die eindeutige ID der Gruppe ein, die dem Prinzipal angehört.
<ul>
<li>PrincipalID: die eindeutige ID für diesen Prinzipal<br />
<br />
</li>
<li>ParentID: die eindeutige ID einer Gruppe, der dieser Prinzipal angehört<br />
<br />
</li>
</ul></td>
</tr>
</tbody>
</table>
