---
TOCTitle: Tabellen für die Protokollierungsdatenbank
Title: Tabellen für die Protokollierungsdatenbank
ms:assetid: '7ab2104c-b12d-4807-8a4b-bcabb145ff9b'
ms:contentKeyID: 18118908
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747569(v=WS.10)'
---

Tabellen für die Protokollierungsdatenbank
==========================================

Dieser Abschnitt beschreibt die Tabellen der RMS-Protokollierungsdatenbank (Rights Management Services oder Dienste für die Rechteverwaltung).

DRMS\_Log\_Master
-----------------

In der folgenden Tabelle wird ein Eintrag für jeden Protokollierungsdatensatz aufgelistet.

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
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Eindeutige ID für den Protokollierungsdatensatz</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_HostMachineName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Server, der den Datensatz generiert hat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_HostMachineRequestId</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Anforderungs-ID</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_RequestTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Datum und Uhrzeit der Anforderung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestPath</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>URL-Pfad der Anforderung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ der Anforderung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_RequestUserAddress</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>IP-Adresse des Clients</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_RequestUserAgent</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Benutzer-Agent-Kopfzeile des Clients</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Authentifizierungsstatus der Anforderung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_SecureConnectionState</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>SSL-Schutz der Anforderung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_AuthenticatedId</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID des authentifizierten Benutzers</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ReceivedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Vom Client in der Anforderung empfangenes XrML</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_IssuedXrML</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>In der Anforderung ausgestellte XrML-Lizenz</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Metadata</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Metadaten</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_SuccessOrFailure</p></td>
<td style="border:1px solid black;"><p>nvarchar(32)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erfolg oder Fehlschlagen der Anforderung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_ErrorInformation</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Fehlerdaten</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_LogCreateTime</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Uhrzeit der Protokollerstellung</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Detail  
-----------------
  
In der folgenden Tabelle werden zusätzliche Daten für einen Protokollierungsdatensatz aufgelistet. Normalerweise werden die XrML-Daten in dieser Tabelle protokolliert.
  
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
<td style="border:1px solid black;"><p>i_LogDetailID</p></td>
<td style="border:1px solid black;"><p>int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1)</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_LogID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL (FK)</p></td>
<td style="border:1px solid black;"><p>ID des übergeordneten Protokollierungsdatensatzes</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_Name</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Name der Eigenschaft</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Value</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Wert der Eigenschaft</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Log\_Filter  
-----------------
  
In der folgenden Tabelle werden die Felder aufgelistet, die vom Protokollierungslistenerdienst protokolliert werden.
  
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
<td style="border:1px solid black;"><p>i_ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_FieldName</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Name des Feldes</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_FieldDescription</p></td>
<td style="border:1px solid black;"><p>nvarchar(1024)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Beschreibung des Feldes</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_IsIncluded</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Gibt an, ob das Feld protokolliert wird</p></td>
</tr>
</tbody>
</table>
