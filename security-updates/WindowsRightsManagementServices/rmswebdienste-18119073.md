---
TOCTitle: 'RMS-Webdienste'
Title: 'RMS-Webdienste'
ms:assetid: 'ed8dbb2e-0590-4502-afc4-54f66b96d515'
ms:contentKeyID: 18119073
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747728(v=WS.10)'
---

RMS-Webdienste
==============

RMS stellt die Serverkomponente eines RMS-Systems bereit. Dessen Kernfunktionen werden als Satz von Microsoft® ASP.NET-Webdiensten implementiert, die unter Microsoft® Internetinformationsdienste (Internet Information Services, IIS) ausgeführt werden. Die RMS-Webdienste werden über die SOAP-Schnittstelle oder über .NET Remoting verfügbar gemacht.

Die Webdienste bieten:

-   Unterregistrierung von Servern
-   Kontozertifizierung vertrauenswürdiger Entitäten
-   Lizenzierung von durch Rechte geschützten Informationen
-   Verwaltungsfunktionen für RMS

In der folgenden Tabelle werden die RMS-Webdienste genauer beschrieben.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Dienst</th>
<th>Beschreibung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Unterregistrierung</p></td>
<td style="border:1px solid black;"><p>Stellt Servern in rein lizenzierenden Clustern untergeordnete Server-Lizenzgeberzertifikate bereit. Mit diesen Zertifikaten kann der rein lizenzierende Cluster Veröffentlichungs- und Nutzungslizenzen ausgeben.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Kontozertifizierung</p></td>
<td style="border:1px solid black;"><p>Stellt Benutzern Rechtekontozertifikate bereit. Diese Zertifikate benötigen die Benutzer zum Abrufen von Veröffentlichungs- und Nutzungslizenzen, damit sie durch Rechte geschützte Inhalte verfassen und abrufen können.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Aktivierungsproxy</p></td>
<td style="border:1px solid black;"><p>Dieser Dienst wird aus Gründen der Kompatibilität mit Clients bereitgestellt, auf denen RMS Version 1 installiert ist. Der Dienst leitet Computeraktivierungsanforderungen an den Microsoft-Aktivierungsdienst weiter und gibt Lockboxes und RMS-Computerzertifikate an Clients mit RMS Version 1 zurück. RMS-Clients mit Service Pack 1 (SP1) oder später verwenden diesen Dienst nicht.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Veröffentlichen</p></td>
<td style="border:1px solid black;"><p>Stellt Veröffentlichungslizenzen aus, die es Verfassern erlauben, durch Rechte geschützte Inhalte zu erstellen und zu verteilen. Stellt außerdem Client-Lizenzgeberzertifikate aus, mit denen Benutzer auch ohne Verbindung zum internen Netzwerk, auf dem RMS gehostet wird, Inhalte veröffentlichen können, die durch Rechte geschützt sind.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>Lizenzierung</p></td>
<td style="border:1px solid black;"><p>Stellt Nutzungslizenzen aus, mit denen Benutzer durch Rechte geschützte Inhalte abrufen können.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Verwaltung</p></td>
<td style="border:1px solid black;"><p>Ermöglicht dem Administrator die Verwaltung von RMS.</p></td>
</tr>  
<tr class="odd">
<td style="border:1px solid black;"><p>DrmRemote</p></td>
<td style="border:1px solid black;"><p>Ermöglicht es den Webdiensten, durch Verfügbarmachen von .NET Remoting untereinander und mit anderen Komponenten des RMS-Systems zu kommunizieren.</p></td>
</tr>  
<tr class="even">
<td style="border:1px solid black;"><p>Außerbetriebsetzung</p></td>
<td style="border:1px solid black;"><p>Hebt den Schutz von mit Rechten geschützten Inhalten auf und gibt die Inhalte an den Client zurück. Dieser Dienst wird zwar vom RMS-Setupprogramm installiert, das zugehörige virtuelle Stammverzeichnis in IIS muss aber erst vom Administrator aktiviert werden. Bei Aktivierung dieses Diensts werden alle anderen Dienste deaktiviert.</p></td>
</tr>  
</tbody>  
</table>
  
Zusätzlich zu den Webdiensten installiert RMS auch einen Protokollierungslistenerdienst. Jeder Webdienst sendet protokollierte Daten an die Warteschlange für Protokollierungsnachrichten. Der Protokollierungslistenerdienst leitet dann die protokollierten Daten von der Warteschlange an die Protokollierungsdatenbank weiter.
  
Die Webdienstanwendungen befinden sich in den virtuellen IIS-Verzeichnissen. Diese virtuellen Verzeichnisse werden auf jedem RMS-Server unter der Website installiert, die Sie während der Bereitstellung ausgewählt haben.
  
Die Authentifizierung und der Zugriff werden für jedes virtuelle Verzeichnis separat konfiguriert. Außerdem wird der Zugriff auch für jeden Webdienst separat konfiguriert. Informationen zu den Sicherheitseinstellungen für virtuelle Verzeichnisse und Webdienstdateien finden Sie weiter unten unter [Unterstützung der Internetinformationsdienste für RMS](https://technet.microsoft.com/bd4dc69f-1e4e-4e95-9ae2-c925d8a14d4c).
  
Weitere Informationen zu den einzelnen Webdiensten finden Sie weiter unten unter [RMS-Softwarekomponenten](https://technet.microsoft.com/e38a840e-f390-48fd-8354-50108a64f5ca).
