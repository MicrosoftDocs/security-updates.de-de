---
TOCTitle: 'Zertifizierungstabellen der RMS-Konfigurationsdatenbank'
Title: 'Zertifizierungstabellen der RMS-Konfigurationsdatenbank'
ms:assetid: 'd392663a-1a46-42f6-a71d-f0f2c1843566'
ms:contentKeyID: 18119023
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747760(v=WS.10)'
---

Zertifizierungstabellen der RMS-Konfigurationsdatenbank
=======================================================

Dieses Thema beschreibt die Zertifizierungstabellen in der RMS-Konfigurationsdatenbank (Rights Management Services oder Dienste für die Rechteverwaltung). Die Tabellen enthalten Informationen zu den Rechtekontozertifikaten, die für Benutzer dieser Installation ausgestellt werden.

UD\_Machines
------------

In der folgenden Tabelle werden Informationen zu den Hardware-IDs für alle Computer aufgelistet.

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
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_PubKeyHash</p></td>
<td style="border:1px solid black;"><p>binary(20)</p></td>
<td style="border:1px solid black;"><p>(20) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Hash der Hardware-ID</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</p></td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
In der folgenden Tabelle werden Informationen zu den Microsoft .NET Passport-Daten von Benutzern aufgelistet.
  
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
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i64_Puid</p></td>
<td style="border:1px solid black;"><p>bigint</p></td>
<td style="border:1px solid black;"><p>(50) NULL</p></td>
<td style="border:1px solid black;"><p>.NET Passport-Benutzer-ID</p></td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
In der folgenden Tabelle werden zertifizierte Benutzer mit den entsprechenden Computerinformationen verknüpft.
  
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
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_MachineId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</p></td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
In der folgenden Tabelle werden Informationen zu den Benutzerdaten aufgelistet.
  
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
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_KeyData</p></td>
<td style="border:1px solid black;"><p>varbinary(2000)</p></td>
<td style="border:1px solid black;"><p>(2000) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Verschlüsselter Benutzerschlüssel (öffentlich/privat)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_KeyDataLength</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Länge des unverschlüsselten Schlüssels (öffentlich/privat)</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>b_PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Benutzerschlüssel (öffentlich)</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_EncryptionDbId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Index zum Lizenzgeberzertifikat, mit dem das Schlüsselpaar (öffentlich/privat) verschlüsselt wird</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nicht angegeben</p></td>
<td style="border:1px solid black;"><p>Nicht verwendet</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_Expiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Ablaufdatum des Benutzerschlüssels</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_TemporaryExpiration</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Ablaufdatum und -uhrzeit für die temporäre Verwendung des Schlüssels</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>f_Modified</p></td>
<td style="border:1px solid black;"><p>bit</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Nicht verwendet</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_Quota</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Aktuelle Kontingentebene für den Benutzer</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_WaitDays</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Anzahl von Tagen, bevor zusätzliche Kontingentanforderungen erfolgreich abgeschlossen werden können</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_LastConsumption</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Datum und Uhrzeit der letzten zusätzlichen Benutzerzertifizierung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_CreateDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</p></td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
In der folgenden Tabelle werden die IDs aller authentifizierten und zertifizierten Windows-Benutzer aufgelistet.
  
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
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>i_UserId</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Sid</p></td>
<td style="border:1px solid black;"><p>Sid</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Sicherheits-ID (SID) des Benutzers</p></td>
</tr>
</tbody>
</table>
