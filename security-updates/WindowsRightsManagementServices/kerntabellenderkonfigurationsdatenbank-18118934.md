---
TOCTitle: Kerntabellen der Konfigurationsdatenbank
Title: Kerntabellen der Konfigurationsdatenbank
ms:assetid: '8f9e15a2-92bc-41f7-a4fd-329567afb142'
ms:contentKeyID: 18118934
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747676(v=WS.10)'
---

Kerntabellen der Konfigurationsdatenbank
========================================

Dieses Thema beschreibt die Kerntabellen der RMS-Konfigurationsdatenbank.

DRMS\_ApplicationExclusionList
------------------------------

In der folgenden Tabelle werden Informationen zu ausgeschlossenen Anwendungen aufgelistet.

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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Name</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Anwendungsname</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimale Hauptversionsnummer der Anwendung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimale Nebenversionsnummer der Anwendung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMinBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimale Buildversionsnummer der Anwendung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMinRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Minimale Revisionsnummer der Anwendung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxMajor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximale Hauptversionsnummer der Anwendung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxMinor</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximale Nebenversionsnummer der Anwendung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionMaxBuild</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximale Buildversionsnummer der Anwendung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>VersionMaxRevision</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Maximale Revisionsnummer der Anwendung</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Beschreibung</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Anwendungsbeschreibung</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
In der folgenden Tabelle werden Informationen zur Nachrichtenwarteschlange aufgelistet.
  
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
<td style="border:1px solid black;"><p>AsyncQueueID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>QueueName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Pfad zur Nachrichtenwarteschlange</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
In der folgenden Tabelle werden Informationen zu Zertifikatstypen aufgelistet, die für Clients ausgestellt werden.
  
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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Die ID des Zertifikats</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Entweder Desktop, MobileDevice oder Server</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
In der folgenden Tabelle werden Informationen zum aktuellen Server-Lizenzgeberzertifikat aufgelistet, das sich in der Tabelle DRMS\_LicensorCertificate befindet.
  
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
<td style="border:1px solid black;"><p>CurrentLicensorCertID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Das aktive Lizenzgeberzertifikat</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
In der folgenden Tabelle werden Informationen zu den Speicherorten für die Clusterrichtlinien aufgelistet.
  
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
<td style="border:1px solid black;"><p>PolicyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID der Richtlinie</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PolicyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Name der Richtlinie</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PolicyData</p></td>
<td style="border:1px solid black;"><p>sql_variant</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Richtliniendaten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
In der folgenden Tabelle werden Informationen zu den Servern im Cluster aufgelistet.
  
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
<td style="border:1px solid black;"><p>ServerID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Server-ID</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ServerName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht angegeben</p></td>
<td style="border:1px solid black;"><p>Computername für den Server</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
In der folgenden Tabelle werden Informationen zu den ausgeschlossenen Rechtekontozertifikaten aufgelistet.
  
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
<td style="border:1px solid black;"><p>PublicKeyIndex</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Bytes des öffentlichen Schlüssels</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>UserID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Index für die Benutzer-ID</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>ExpirationDate</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Datum, an dem das Rechtekontozertifikat abläuft</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Beschreibung</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Name, der dem Schlüssel für das ausgeschlossene Rechtekontozertifikat zugeordnet wurde</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
In der folgenden Tabelle werden Informationen zum aktiven Server-Lizenzgeberzertifikat aufgelistet.
  
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
<td style="border:1px solid black;"><p>i_CertID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID der Richtlinie</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID-Typ des Schlüsselpaars</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID-GUID des Schlüsselpaars</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Zeiger auf das tatsächliche Zertifikat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Die folgende Tabelle enthält Informationen zum privaten Schlüssel des aktiven Server-Lizenzgeberzertifikats.
  
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
<td style="border:1px solid black;"><p>PrivateKeyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID-Typ des Schlüsselpaars</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID-GUID des Schlüsselpaars</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PrivateKey</p></td>
<td style="border:1px solid black;"><p>varbinary(2048)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Binärdarstellung des Schlüssels</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CSP</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Name des Kryptographiedienstanbieters</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CSPType</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ des Kryptographiedienstanbieters</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>KeyContainerName</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nicht angegeben</p></td>
<td style="border:1px solid black;"><p>Name des Schlüsselcontainers</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>KeyNumber</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Schlüsselnummer</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
In der folgenden Tabelle werden Informationen zu Microsoft® .NET Passport-Konten aufgelistet, denen Lizenzen verweigert werden sollen.
  
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
<td style="border:1px solid black;"><p>DenyID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DenyAddressPattern</p></td>
<td style="border:1px solid black;"><p>nvarchar(500)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Benutzername/Domänenname</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
In der folgenden Tabelle werden Informationen zu Plug-Ins aufgelistet.
  
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
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ des Plug-Ins</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>NameSpace</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Namespace für das Plug-In</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginName</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Name des Plug-Ins</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Ordinal</p></td>
<td style="border:1px solid black;"><p>Int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Sequenznummer, unter der das Plug-In ausgeführt wird</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Path</p></td>
<td style="border:1px solid black;"><p>nvarchar(512)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Pfad zur DLL-Datei</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>ObjectTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(50)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Nicht verwendet</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DebugMode</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Gibt an, ob ein Plug-In im Debugmodus ausgeführt werden soll</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>PublicKey</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Öffentlicher Schlüssel des Plug-Ins</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Version</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Version des Plug-Ins</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
In der folgenden Tabelle werden Informationen zu den Plug-In-Versionen aufgelistet, denen eine Teilnahme am RMS-System gestattet ist.
  
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
<td style="border:1px solid black;"><p>RowID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>VersionInfo</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nicht angegeben</p></td>
<td style="border:1px solid black;"><p>Version des Plug-Ins</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
In der folgenden Tabelle werden Informationen zu den Plug-In-Eigenschaften aufgelistet.
  
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
<td style="border:1px solid black;"><p>PropertyID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Plug-In-ID, zu der die Eigenschaft gehört</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>PropertyName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Der Eigenschaftenname für die Konfigurationsdaten</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PropertyValue</p></td>
<td style="border:1px solid black;"><p>text</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Der Eigenschaftenwert für die Konfigurationsdaten</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
In der folgenden Tabelle werden Informationen zum Plug-In-Typ aufgelistet.
  
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
<td style="border:1px solid black;"><p>PluginTypeID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>PluginTypeName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Name des Plug-Ins</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
In der folgenden Tabelle werden Informationen zu den Vorlagen für Benutzerrechterichtlinien aufgelistet.
  
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
<td style="border:1px solid black;"><p>Guid</p></td>
<td style="border:1px solid black;"><p>nvarchar(128) (PK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>GUID der Vorlage für Benutzerrechterichtlinien</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>TemplateData</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Dieses Feld enthält Daten zur XrML-Vorlage.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
In der folgenden Tabelle werden Informationen zu vertrauenswürdigen Zertifizierungsstellen aufgelistet.
  
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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(1,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>ID des Zertifikats</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertificateGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>GUID des Zertifikats</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CaTypeID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Typ der Zertifizierungsstelle</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
In der folgenden Tabelle werden Informationen zu E-Mail-Domänen aufgelistet, die in der RMS-Umgebung als vertrauenswürdig gelten.
  
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
<td style="border:1px solid black;"><p>ID</p></td>
<td style="border:1px solid black;"><p>int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>int (FK)t</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>s_EmailDomainName</p></td>
<td style="border:1px solid black;"><p>nvarchar(256)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Liste der E-Mail-Domänennamen, die für die vertrauenswürdige Benutzerdomäne gültig sind.</p></td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
In der folgenden Tabelle werden Informationen zu vertrauenswürdigen Benutzerdomänen und Veröffentlichungsdomänen aufgelistet.
  
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
<td style="border:1px solid black;"><p>i_TrustedIdentityDomainID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Interner Index</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_DomainType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Typ der Domäne</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>CertGUIDType</p></td>
<td style="border:1px solid black;"><p>nvarchar(64)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Typ der Zertifikats-GUID</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>CertGUID</p></td>
<td style="border:1px solid black;"><p>nvarchar(128)</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>GUID des Zertifikats</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>ID des Zertifikats</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>i_allowSID</p></td>
<td style="border:1px solid black;"><p>int</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>SID der Domäne</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>S_friendlyname</p></td>
<td style="border:1px solid black;"><p>nvarchar(255)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Anzeigename für Zertifikat</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>dt_DateUpdated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Aktualisierungszeitstempel</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>dt_DateCreated</p></td>
<td style="border:1px solid black;"><p>datetime</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Erstellungszeitstempel</p></td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
In der folgenden Tabelle werden Informationen zu den XrML-Server-Lizenzgeberzertifikaten aufgelistet, auf die in der Tabelle DRMS\_LicensorCertificate verwiesen wird. Außerdem wird die Zertifikatkette zugeordnet.
  
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
<td style="border:1px solid black;"><p>i_CertificateID</p></td>
<td style="border:1px solid black;"><p>Int (PK)</p></td>
<td style="border:1px solid black;"><p>IDENTITY(100,1) Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Zeiger auf das tatsächliche Zertifikat</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>s_Certificate</p></td>
<td style="border:1px solid black;"><p>ntext</p></td>
<td style="border:1px solid black;"><p>Nicht NULL</p></td>
<td style="border:1px solid black;"><p>Zeiger auf das tatsächliche Zertifikat</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>i_ParentCertificateID</p></td>
<td style="border:1px solid black;"><p>int (FK)</p></td>
<td style="border:1px solid black;"><p>NULL</p></td>
<td style="border:1px solid black;"><p>Zeiger auf das tatsächliche Zertifikat</p></td>
</tr>
</tbody>
</table>
