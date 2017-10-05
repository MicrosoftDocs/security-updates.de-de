---
TOCTitle: Voraussetzungen und Prüflisten für RMS
Title: Voraussetzungen und Prüflisten für RMS
ms:assetid: '836d96ef-d0fd-4935-b595-e8dec19cbb2b'
ms:contentKeyID: 18118922
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747582(v=WS.10)'
---

Voraussetzungen und Prüflisten für RMS
======================================

Bevor Sie mit der Installation von RMS beginnen, sollten Sie die technischen Voraussetzungen zum Einsatz von RMS überprüfen. Die aufgelisteten Technologien und ein grundlegendes Verständnis derselben sind für eine erfolgreiche Bereitstellung von RMS unerlässlich. Mithilfe der folgenden Prüflisten können Sie Aufgabenlisten und Pläne für die Bereitstellung und Verwaltung von RMS erstellen:

-   [Technologievoraussetzungen](#bkmk_9)
-   [Prüflisten für die RMS-Bereitstellung](#bkmk_10)
-   [Prüflisten für die RMS-Verwaltung](#bkmk_14)

<span id="BKMK_9"></span>
Technologievoraussetzungen
--------------------------

In dieser Dokumentationssammlung werden Informationen geboten, die Ihnen Einblick in die Funktionsweise von RMS, die Planung und Durchführung einer Bereitstellung für Ihre Organisation und die Verwaltung des Systems im Geschäftsalltag geben sollen. Dabei wird davon ausgegangen, dass Sie über Kenntnisse in folgenden Bereichen verfügen:

-   Bereitstellung und Verwaltung von Windows Server 2003
-   Bereitstellung und Verwaltung von Active Directory
-   Bereitstellung und Verwaltung von Microsoft® Internetinformationsdienste 6.0 (Internet Information Services oder IIS)
-   Verwaltung von Microsoft® SQL Server™ 2000
-   PKI-Basiskonzepte (Public Key Infrastructure)
-   Servernetzwerk und -sicherheit

Weitere Informationen über diese Themen finden Sie unter „Zusätzliche Ressourcen“ im Abschnitt [Betreiben eines RMS-Servers](http://go.microsoft.com/fwlink/?linkid=42495) in dieser Dokumentationssammlung.

<span id="BKMK_10"></span>
Prüflisten für die RMS-Bereitstellung
-------------------------------------

In diesem Abschnitt werden Prüflisten für die folgenden Bereitstellungsaufgaben behandelt:

-   [Bereitstellen einer Installation mit einem einzelnen Server](#bkmk_11)
-   [Bereitstellen von Stammzertifizierungs- und Lizenzierungsclustern](#bkmk_12)
-   [Gesamtstrukturübergreifendes Bereitstellen von RMS](#bkmk_13)

Weitere Informationen über das Bereitstellen von RMS finden Sie unter [Bereitstellen eines RMS-Systems](http://go.microsoft.com/fwlink/?linkid=42494) in dieser Dokumentationssammlung.

<span id="BKMK_11"></span>
Bereitstellen einer Installation mit einem einzelnen Server
-----------------------------------------------------------

Zum Bereitstellen eines einzelnen RMS-Servers verwenden Sie die folgende Prüfliste.

###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu Konzepten und Planung</td>
<td style="border:1px solid black;">„Vorbereitung für eine RMS-Bereitstellung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lesen der Informationen zu Systemanforderungen und Überprüfen der Verfügbarkeit aller erforderlichen Hardware- und Softwarekomponenten.</td>
<td style="border:1px solid black;">„Infrastrukturelle Voraussetzungen für RMS“ unter <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planen einer RMS-Bereitstellung</a>
„Planen der Infrastruktur des Datenbankservers“ unter <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planen einer RMS-Bereitstellung</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Einrichten der Infrastruktur, einschließlich erforderlicher Hardware- und Softwarekomponenten, administrativer Konten und Unterstützung von SMS oder Gruppenrichtlinie.</td>
<td style="border:1px solid black;">„Vorbereitung für eine RMS-Bereitstellung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Installieren und Konfigurieren von RMS auf dem Server</td>
<td style="border:1px solid black;">„Einrichten von Zertifizierungs- und Lizenzierungsdiensten auf dem ersten Server“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Testen der Bereitstellung.</td>
<td style="border:1px solid black;">„Einrichten einer Testumgebung“ in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Implementieren von RMS in der Produktionsumgebung</td>
<td style="border:1px solid black;">„Festlegen des Umfangs der RMS-Implementierung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_12"></span>
Bereitstellen von Stammzertifizierungs- und Lizenzierungsclustern  
-----------------------------------------------------------------
  
Verwenden Sie die folgenden Prüflisten zum Bereitstellen der Stammzertifizierungs- und Lizenzierungscluster.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu Konzepten und Planung</td>
<td style="border:1px solid black;">„Vorbereitung für eine RMS-Bereitstellung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Lesen der Informationen zu Systemanforderungen und Überprüfen der Verfügbarkeit aller erforderlichen Hardware- und Softwarekomponenten</td>
<td style="border:1px solid black;">„Infrastrukturelle Voraussetzungen für RMS“ unter <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planen einer RMS-Bereitstellung</a>
„Planen der Infrastruktur des Datenbankservers“ unter <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planen einer RMS-Bereitstellung</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu dem Bereitstellungsplan zum besseren Verständnis der Topologie und der zu installierenden Komponenten.</td>
<td style="border:1px solid black;">„Festlegen der RMS-Topologie“ unter <a href="http://go.microsoft.com/fwlink/?linkid=37537">Planen einer RMS-Bereitstellung</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Einrichten der Infrastruktur, einschließlich erforderlicher Hardware- und Softwarekomponenten, administrativer Konten und Unterstützung von SMS oder Gruppenrichtlinie.</td>
<td style="border:1px solid black;">„Vorbereitung für eine RMS-Bereitstellung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Installieren und Konfigurieren von RMS auf den Servern, die nicht Teil des Stammzertifizierungsclusters sind</td>
<td style="border:1px solid black;">„Einrichten von Zertifizierungs- und Lizenzierungsdiensten auf dem ersten Server“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a>
„Hinzufügen von Servern zur Unterstützung der Zertifizierung und Lizenzierung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Installieren und Konfigurieren von RMS auf den Servern, die Teil des Stammzertifizierungsclusters sind</td>
<td style="border:1px solid black;">„Einrichten von Zertifizierungs- und Lizenzierungsdiensten auf dem ersten Server“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a>
„Hinzufügen von Servern zur Unterstützung der Zertifizierung und Lizenzierung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Einrichten des Lastenausgleichs</td>
<td style="border:1px solid black;">„Erweitern der grundlegenden Infrastruktur zur Unterstützung von Clustern“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Testen der Bereitstellung.</td>
<td style="border:1px solid black;">„Einrichten einer Testumgebung“ in <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Implementieren von RMS in der Produktionsumgebung</td>
<td style="border:1px solid black;">„Definieren des Umfangs der RMS-Implementierung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_13"></span>
Gesamtstrukturübergreifendes Bereitstellen von RMS  
--------------------------------------------------
  
Verwenden Sie die folgenden Prüflisten zum gesamtstrukturübergreifenden Bereitstellen von RMS.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu Konzepten und Planung</td>
<td style="border:1px solid black;">„Vorbereitung für eine RMS-Bereitstellung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Konfigurieren der erforderlichen Berechtigungen basierend auf dem Vertrauensmodell.</td>
<td style="border:1px solid black;">„Gesamtstrukturübergreifendes Bereitstellen von RMS“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Einrichten der entsprechenden Active Directory-Attribute für die Gesamtstrukturen</td>
<td style="border:1px solid black;">„Gesamtstrukturübergreifendes Bereitstellen von RMS“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_14"></span>
Prüflisten für die RMS-Verwaltung  
---------------------------------
  
In diesem Abschnitt werden Prüflisten für die folgenden Verwaltungsaufgaben behandelt:
  
-   [Implementieren von Vorlagen für Benutzerrechterichtlinien](#bkmk_15)  
-   [Bereitstellen von neuen RMS-Clients](#bkmk_16)  
-   [Hinzufügen von vertrauenswürdigen Benutzerdomänen](#bkmk_17)  
-   [Hinzufügen von vertrauenswürdigen Veröffentlichungsdomänen](#bkmk_18)
  
Weitere Informationen zum Verwalten von RMS finden Sie unter [Betreiben eines RMS-Servers](http://go.microsoft.com/fwlink/?linkid=42495) in dieser Dokumentationssammlung.
  
<span id="BKMK_15"></span>
Implementieren von Vorlagen für Benutzerrechterichtlinien  
---------------------------------------------------------
  
Verwenden Sie die folgende Prüfliste zum Implementieren einer Vorlage für Benutzerrechterichtlinien.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu relevanten Konzepten.</td>
<td style="border:1px solid black;">„Vorlagen für Benutzerrechterichtlinien“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische Referenz für RMS</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Angeben des Speicherorts der Vorlage für Benutzerrechterichtlinien</td>
<td style="border:1px solid black;">„So geben Sie den Speicherort von Vorlagen für Benutzerrechterichtlinien an“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Erstellen der Vorlage für Benutzerrechterichtlinien</td>
<td style="border:1px solid black;">„Erstellen und Ändern von Vorlagen für Benutzerrechterichtlinien“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a>
„So fügen Sie eine Vorlage für Benutzerrechterichtlinien hinzu“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Verteilen der Vorlage für Benutzerrechterichtlinien</td>
<td style="border:1px solid black;">„Verteilen von Vorlagen für Benutzerrechterichtlinien“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_16"></span>
Bereitstellen von neuen RMS-Clients  
-----------------------------------
  
Verwenden Sie die folgende Prüfliste zum Bereitstellen einer neuen Version des RMS-Clients.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu relevanten Konzepten.</td>
<td style="border:1px solid black;">„Planung der Client-Verteilung“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42494">Bereitstellen eines RMS-Systems</a>
„Ausschließen von Lockbox-Versionen“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Um eine Aktualisierung der aktuellsten Client-Version zu erzwingen, müssen Sie die zu aktualisierende Lockbox-Version ausschließen.</td>
<td style="border:1px solid black;">„So schließen Sie Lockbox-Versionen aus“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_17"></span>
Hinzufügen von vertrauenswürdigen Benutzerdomänen  
-------------------------------------------------
  
Verwenden Sie die folgende Prüfliste zum Hinzufügen einer vertrauenswürdigen Benutzerdomäne.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu relevanten Konzepten.</td>
<td style="border:1px solid black;">„Vertrauenswürdige Benutzerdomänen“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische Referenz für RMS</a>
„Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Erhalten des Server-Lizenzgeberzertifikats der Benutzerdomäne, die hinzugefügt werden soll. (Das Zertifikat muss von dem Administrator der zu vertrauenden Installation bereitgestellt werden.) Hinzufügen der Benutzerdomäne zur Installation.</td>
<td style="border:1px solid black;">„So fügen Sie eine vertrauenswürdige Benutzerdomäne hinzu“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
</tbody>
</table>
  
<span id="BKMK_18"></span>
Hinzufügen von vertrauenswürdigen Veröffentlichungsdomänen  
----------------------------------------------------------
  
Verwenden Sie die folgende Prüfliste zum Hinzufügen einer vertrauenswürdigen Veröffentlichungsdomäne.
  
###  

 
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th style="border:1px solid black;" >Schritt</th>
<th style="border:1px solid black;" >Verweis</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;">Lesen der Informationen zu relevanten Konzepten.</td>
<td style="border:1px solid black;">„Vertrauenswürdige Veröffentlichungsdomänen“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42496">Technische Referenz für RMS</a>
„Hinzufügen und Entfernen von vertrauenswürdigen Veröffentlichungsdomänen“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Abrufen des verschlüsselten Server-Lizenzgeberzertifikats und des privaten Schlüssels der Veröffentlichungsdomäne, die hinzugefügt werden soll. Anschließendes Hinzufügen der Veröffentlichungsdomäne zur Installation.</td>
<td style="border:1px solid black;">„So fügen Sie eine vertrauenswürdige Veröffentlichungsdomäne hinzu“ unter <a href="http://go.microsoft.com/fwlink/?linkid=42495">Ausführen eines RMS-Servers</a></td>
</tr>
</tbody>
</table>
