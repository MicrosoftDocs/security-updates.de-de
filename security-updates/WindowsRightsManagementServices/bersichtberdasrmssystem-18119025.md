---
TOCTitle: 'Übersicht über das RMS-System'
Title: 'Übersicht über das RMS-System'
ms:assetid: 'cbd14635-e17e-42b8-9fd8-6fdce42ffe07'
ms:contentKeyID: 18119025
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747671(v=WS.10)'
---

Übersicht über das RMS-System
=============================

Dieses Thema enthält Informationen dazu, wie die RMS-Webdienste und RMS-Clienttechnologien in einem RMS-System zusammenarbeiten.

In der folgenden Tabelle werden die Arten von Servern aufgelistet, die zu einer RMS-Bereitstellung gehören, und ihre Funktionen beschrieben. Weitere Informationen zur Bereitstellung finden Sie unter „Bereitstellen eines RMS-Systems“ in dieser Dokumentationssammlung.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Server oder Cluster</th>
<th>Funktion</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Stammzertifizierung</p></td>
<td style="border:1px solid black;"><p>Führt folgende RMS-Dienste aus:</p>
<ul>  
<li><strong>Unterregistrierung</strong>. Führt die Unterregistrierung eines Lizenzierungsservers aus.<br />  
<br />  
</li>  
<li><strong>Aktivierungsproxy</strong>. Dient als Internet-Proxy für Clientanforderungen für Lockboxes und RMS-Computerzertifikate.<br />  
<br />  
</li>  
<li><strong>Zertifizierung</strong>. Stellt Rechtekontozertifikate aus.<br />  
<br />  
</li>  
<li><strong>Veröffentlichung</strong>. Stellt Veröffentlichungslizenzen aus.<br />  
<br />  
</li>  
<li><strong>Lizenzierung</strong>. Stellt Nutzungslizenzen aus.<br />  
<br />  
</li>  
</ul>
<p>Jede Bereitstellung muss mindestens einen Stammzertifizierungsserver oder -cluster einschließen. In einer Active Directory-Gesamtstruktur kann es nur einen Stammzertifizierungscluster geben.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Lizenzierung (optional)</p></td>
<td style="border:1px solid black;"><p>Führt folgende RMS-Dienste aus:</p>
<ul>  
<li><strong>Veröffentlichung</strong>. Stellt Veröffentlichungslizenzen aus.<br />  
<br />  
</li>  
<li><strong>Lizenzierung</strong>. Stellt Nutzungslizenzen aus.<br />  
<br />  
</li>  
</ul>
<p>Lizenzierungsserver werden zur Unterstützung einzelner Abteilungen oder zum Verschieben von Lizenzierungsanforderungen vom Stammzertifizierungscluster bereitgestellt. Lizenzierungsserver sind optional.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Datenbankserver, wie z. B. SQL Server</p></td>
<td style="border:1px solid black;"><ul>
<li>Führt die RMS-Datenbanken für Konfiguration, Protokollierung und Verzeichnisdienste aus.<br />  
<br />  
</li>  
<li>Speichert Rechtekontozertifikate in der Konfigurationsdatenbank des Stammzertifizierungsclusters.<br />  
<br />  
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Domänencontroller und globaler Katalog</p></td>
<td style="border:1px solid black;"><ul>
<li>Stellt Benutzerauthentifizierung und Verzeichnisdienste bereit.<br />  
<br />  
</li>  
<li>Speichert den Pfad für die Suche nach Diensten des Stammzertifizierungsclusters.<br />  
<br />  
</li>
</ul></td>
</tr>
</tbody>
</table>
<p> </p>

RMS verwendet die von Microsoft gehosteten Registrierungs- und Aktivierungsdienste, um einen gemeinsamen Vertrauensstamm für das System bereitzustellen. Weitere Informationen hierzu finden Sie unter „[RMS-Vertrauenshierarchie](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)“ weiter unten in diesem Thema.

Im folgenden Diagramm sind die unterschiedlichen Komponenten eines RMS-Systems und deren Rollen im System dargestellt. Pfeile stehen für Anforderungen und Antworten, die zwischen diesen Komponenten übergeben werden.

![](images/Cc747671.29138741-d45c-459b-8ead-b9bc3f708dd5(WS.10).gif)

Weitere Informationen zu den einzelnen Komponenten finden Sie unter „[RMS-Softwarekomponenten](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca)“ weiter unten in diesem Thema.
