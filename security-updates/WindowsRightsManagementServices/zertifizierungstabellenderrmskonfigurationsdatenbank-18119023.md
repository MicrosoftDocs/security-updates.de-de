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
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PubKeyHash</td>
<td style="border:1px solid black;">binary(20)</td>
<td style="border:1px solid black;">(20) Nicht NULL</td>
<td style="border:1px solid black;">Hash der Hardware-ID</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</td>
</tr>
</tbody>
</table>
  
UD\_PassportAuthIdentities  
--------------------------
  
In der folgenden Tabelle werden Informationen zu den Microsoft .NET Passport-Daten von Benutzern aufgelistet.
  
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
<th>Name</th>
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i64_Puid</td>
<td style="border:1px solid black;">bigint</td>
<td style="border:1px solid black;">(50) NULL</td>
<td style="border:1px solid black;">.NET Passport-Benutzer-ID</td>
</tr>
</tbody>
</table>
  
UD\_UserMachine  
---------------
  
In der folgenden Tabelle werden zertifizierte Benutzer mit den entsprechenden Computerinformationen verknüpft.
  
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
<th>Name</th>
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_MachineId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</td>
</tr>
</tbody>
</table>
  
UD\_Users  
---------
  
In der folgenden Tabelle werden Informationen zu den Benutzerdaten aufgelistet.
  
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
<th>Name</th>
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_KeyData</td>
<td style="border:1px solid black;">varbinary(2000)</td>
<td style="border:1px solid black;">(2000) Nicht NULL</td>
<td style="border:1px solid black;">Verschlüsselter Benutzerschlüssel (öffentlich/privat)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_KeyDataLength</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Länge des unverschlüsselten Schlüssels (öffentlich/privat)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">b_PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Benutzerschlüssel (öffentlich)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_EncryptionDbId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Index zum Lizenzgeberzertifikat, mit dem das Schlüsselpaar (öffentlich/privat) verschlüsselt wird</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nicht angegeben</td>
<td style="border:1px solid black;">Nicht verwendet</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_Expiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Ablaufdatum des Benutzerschlüssels</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_TemporaryExpiration</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Ablaufdatum und -uhrzeit für die temporäre Verwendung des Schlüssels</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">f_Modified</td>
<td style="border:1px solid black;">bit</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Nicht verwendet</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_Quota</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Aktuelle Kontingentebene für den Benutzer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_WaitDays</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Anzahl von Tagen, bevor zusätzliche Kontingentanforderungen erfolgreich abgeschlossen werden können</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_LastConsumption</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Datum und Uhrzeit der letzten zusätzlichen Benutzerzertifizierung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_CreateDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Datum und Uhrzeit, an dem bzw. zu der der Eintrag zur Tabelle hinzugefügt wurde</td>
</tr>
</tbody>
</table>
  
UD\_Windows AuthIdentities  
--------------------------
  
In der folgenden Tabelle werden die IDs aller authentifizierten und zertifizierten Windows-Benutzer aufgelistet.
  
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
<th>Name</th>
<th>Datentyp</th>
<th>NULL-Werte</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_UserId</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Sid</td>
<td style="border:1px solid black;">Sid</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Sicherheits-ID (SID) des Benutzers</td>
</tr>
</tbody>
</table>
