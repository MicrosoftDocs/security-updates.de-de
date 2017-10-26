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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Name</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Anwendungsname</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimale Hauptversionsnummer der Anwendung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimale Nebenversionsnummer der Anwendung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMinBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimale Buildversionsnummer der Anwendung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMinRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Minimale Revisionsnummer der Anwendung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxMajor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximale Hauptversionsnummer der Anwendung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxMinor</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximale Nebenversionsnummer der Anwendung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionMaxBuild</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximale Buildversionsnummer der Anwendung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">VersionMaxRevision</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Maximale Revisionsnummer der Anwendung</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beschreibung</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Anwendungsbeschreibung</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_AsynchronousQueue  
-----------------------
  
In der folgenden Tabelle werden Informationen zur Nachrichtenwarteschlange aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">AsyncQueueID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">QueueName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Pfad zur Nachrichtenwarteschlange</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_CaType  
------------
  
In der folgenden Tabelle werden Informationen zu Zertifikatstypen aufgelistet, die für Clients ausgestellt werden.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Die ID des Zertifikats</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Entweder Desktop, MobileDevice oder Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterConfiguration  
--------------------------
  
In der folgenden Tabelle werden Informationen zum aktuellen Server-Lizenzgeberzertifikat aufgelistet, das sich in der Tabelle DRMS\_LicensorCertificate befindet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">CurrentLicensorCertID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Das aktive Lizenzgeberzertifikat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterPolicies  
---------------------
  
In der folgenden Tabelle werden Informationen zu den Speicherorten für die Clusterrichtlinien aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PolicyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">ID der Richtlinie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PolicyName</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Name der Richtlinie</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PolicyData</td>
<td style="border:1px solid black;">sql_variant</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Richtliniendaten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_ClusterServer  
-------------------
  
In der folgenden Tabelle werden Informationen zu den Servern im Cluster aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ServerID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Server-ID</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ServerName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht angegeben</td>
<td style="border:1px solid black;">Computername für den Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_GICExclusionList  
----------------------
  
In der folgenden Tabelle werden Informationen zu den ausgeschlossenen Rechtekontozertifikaten aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PublicKeyIndex</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Bytes des öffentlichen Schlüssels</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">UserID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Index für die Benutzer-ID</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">ExpirationDate</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Datum, an dem das Rechtekontozertifikat abläuft</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Beschreibung</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Name, der dem Schlüssel für das ausgeschlossene Rechtekontozertifikat zugeordnet wurde</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorCertificate  
-------------------------
  
In der folgenden Tabelle werden Informationen zum aktiven Server-Lizenzgeberzertifikat aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_CertID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">ID der Richtlinie</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">ID-Typ des Schlüsselpaars</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">ID-GUID des Schlüsselpaars</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Zeiger auf das tatsächliche Zertifikat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_LicensorPrivateKey  
------------------------
  
Die folgende Tabelle enthält Informationen zum privaten Schlüssel des aktiven Server-Lizenzgeberzertifikats.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PrivateKeyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">ID-Typ des Schlüsselpaars</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">ID-GUID des Schlüsselpaars</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PrivateKey</td>
<td style="border:1px solid black;">varbinary(2048)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Binärdarstellung des Schlüssels</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CSP</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Name des Kryptographiedienstanbieters</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CSPType</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ des Kryptographiedienstanbieters</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">KeyContainerName</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nicht angegeben</td>
<td style="border:1px solid black;">Name des Schlüsselcontainers</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">KeyNumber</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Schlüsselnummer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_PassportDenyList  
----------------------
  
In der folgenden Tabelle werden Informationen zu Microsoft® .NET Passport-Konten aufgelistet, denen Lizenzen verweigert werden sollen.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">DenyID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DenyAddressPattern</td>
<td style="border:1px solid black;">nvarchar(500)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Benutzername/Domänenname</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_Plugin  
------------
  
In der folgenden Tabelle werden Informationen zu Plug-Ins aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ des Plug-Ins</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">NameSpace</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Namespace für das Plug-In</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginName</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Name des Plug-Ins</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Ordinal</td>
<td style="border:1px solid black;">Int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Sequenznummer, unter der das Plug-In ausgeführt wird</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Path</td>
<td style="border:1px solid black;">nvarchar(512)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Pfad zur DLL-Datei</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">ObjectTypeName</td>
<td style="border:1px solid black;">nvarchar(50)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Nicht verwendet</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DebugMode</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Gibt an, ob ein Plug-In im Debugmodus ausgeführt werden soll</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">PublicKey</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Öffentlicher Schlüssel des Plug-Ins</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Version</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Version des Plug-Ins</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_AllowedPluginVersions  
---------------------------
  
In der folgenden Tabelle werden Informationen zu den Plug-In-Versionen aufgelistet, denen eine Teilnahme am RMS-System gestattet ist.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">RowID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">VersionInfo</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nicht angegeben</td>
<td style="border:1px solid black;">Version des Plug-Ins</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginProperties  
----------------------
  
In der folgenden Tabelle werden Informationen zu den Plug-In-Eigenschaften aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PropertyID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Plug-In-ID, zu der die Eigenschaft gehört</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">PropertyName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Der Eigenschaftenname für die Konfigurationsdaten</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PropertyValue</td>
<td style="border:1px solid black;">text</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Der Eigenschaftenwert für die Konfigurationsdaten</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_PluginType  
----------------
  
In der folgenden Tabelle werden Informationen zum Plug-In-Typ aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">PluginTypeID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">PluginTypeName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Name des Plug-Ins</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_RightsTemplate  
--------------------
  
In der folgenden Tabelle werden Informationen zu den Vorlagen für Benutzerrechterichtlinien aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Guid</td>
<td style="border:1px solid black;">nvarchar(128) (PK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">GUID der Vorlage für Benutzerrechterichtlinien</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">TemplateData</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Dieses Feld enthält Daten zur XrML-Vorlage.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedCertificateAuthorities  
-----------------------------------
  
In der folgenden Tabelle werden Informationen zu vertrauenswürdigen Zertifizierungsstellen aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(1,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">ID des Zertifikats</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertificateGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">GUID des Zertifikats</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CaTypeID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Typ der Zertifizierungsstelle</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedEmailDomains  
-------------------------
  
In der folgenden Tabelle werden Informationen zu E-Mail-Domänen aufgelistet, die in der RMS-Umgebung als vertrauenswürdig gelten.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">ID</td>
<td style="border:1px solid black;">int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">int (FK)t</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">s_EmailDomainName</td>
<td style="border:1px solid black;">nvarchar(256)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Liste der E-Mail-Domänennamen, die für die vertrauenswürdige Benutzerdomäne gültig sind.</td>
</tr>
</tbody>
</table>
  
DRMS\_TrustedIdentityDomain  
---------------------------
  
In der folgenden Tabelle werden Informationen zu vertrauenswürdigen Benutzerdomänen und Veröffentlichungsdomänen aufgelistet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_TrustedIdentityDomainID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Interner Index</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_DomainType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Typ der Domäne</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">CertGUIDType</td>
<td style="border:1px solid black;">nvarchar(64)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Typ der Zertifikats-GUID</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">CertGUID</td>
<td style="border:1px solid black;">nvarchar(128)</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">GUID des Zertifikats</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">ID des Zertifikats</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">i_allowSID</td>
<td style="border:1px solid black;">int</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">SID der Domäne</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">S_friendlyname</td>
<td style="border:1px solid black;">nvarchar(255)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Anzeigename für Zertifikat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">dt_DateUpdated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Aktualisierungszeitstempel</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">dt_DateCreated</td>
<td style="border:1px solid black;">datetime</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Erstellungszeitstempel</td>
</tr>
</tbody>
</table>
  
DRMS\_XrML\_Certificate  
-----------------------
  
In der folgenden Tabelle werden Informationen zu den XrML-Server-Lizenzgeberzertifikaten aufgelistet, auf die in der Tabelle DRMS\_LicensorCertificate verwiesen wird. Außerdem wird die Zertifikatkette zugeordnet.
  
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
<th style="border:1px solid black;" >Name</th>
<th style="border:1px solid black;" >Datentyp</th>
<th style="border:1px solid black;" >NULL-Werte</th>
<th style="border:1px solid black;" >Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">i_CertificateID</td>
<td style="border:1px solid black;">Int (PK)</td>
<td style="border:1px solid black;">IDENTITY(100,1) Nicht NULL</td>
<td style="border:1px solid black;">Zeiger auf das tatsächliche Zertifikat</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">s_Certificate</td>
<td style="border:1px solid black;">ntext</td>
<td style="border:1px solid black;">Nicht NULL</td>
<td style="border:1px solid black;">Zeiger auf das tatsächliche Zertifikat</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">i_ParentCertificateID</td>
<td style="border:1px solid black;">int (FK)</td>
<td style="border:1px solid black;">NULL</td>
<td style="border:1px solid black;">Zeiger auf das tatsächliche Zertifikat</td>
</tr>
</tbody>
</table>