---
TOCTitle: Softwareanforderungen für RMS
Title: Softwareanforderungen für RMS
ms:assetid: '17faf2ad-2366-4a92-98a5-766e20a0f741'
ms:contentKeyID: 18118827
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720201(v=WS.10)'
---

Softwareanforderungen für RMS
=============================

Die folgende Tabelle zeigt die Softwareanforderungen zum Ausführen von RMS-Servern.

###  

<p> </p>
<table style="border:1px solid black;">
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Software</th>
<th>Anforderung</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><p>Betriebssystem</p></td>
<td style="border:1px solid black;"><p>Jede Microsoft Windows Server® 2003 Edition außer Web Edition.</p></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Dateisystem</p></td>
<td style="border:1px solid black;"><p>Das NTFS-Dateisystem wird empfohlen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Betriebssystemkomponenten</p></td>
<td style="border:1px solid black;"><ul>
<li>Message Queuing (auch als MSMQ bezeichnet) mit aktivierter Active Directory®-Verzeichnisdienstintegration.<br />
<br />
</li>
<li>Internet Information Services (IIS) mit aktivierter Komponente ASP.NET.<br />
<br />
</li>
<li>Microsoft .NET Framework 1.1<br />
<br />
</li>
</ul></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><p>Active Directory®-Directory-Dienst</p></td>
<td style="border:1px solid black;"><p>RMS muss in einer Active Directory-Domäne installiert werden, in der auf allen Domänencontrollern Windows Server 2000 mit Service Pack 3 (SP3) oder höher ausgeführt wird. Alle Benutzer und Gruppen, die RMS zum Abrufen und Veröffentlichen von Inhalt verwenden, müssen über eine in Active Directory konfigurierte E-Mail-Adresse verfügen.</p></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><p>Datenbankserver</p></td>
<td style="border:1px solid black;"><p>RMS erfordert eine Datenbank und gespeicherte Verfahren zum Ausführen von Operationen. Sie können Microsoft SQL Server 2000 mit SP3a oder höher bzw. Microsoft SQL Server 2005 verwenden. Zum Testen oder Bereitstellen auf einem einzelnen Computer kann Microsoft SQL Server Desktop Engine (MSDE 2000) mit SP3 oder Microsoft SQL Server 2005 Express Edition verwendet werden.</p></td>
</tr>
</tbody>
</table>
  
Wenn Sie RMS in einer Umgebung mit mehreren Active Directory-Gesamtstrukturen bereitstellen, müssen Sie universelle Active Directory-Gruppen verwenden, damit die Gruppenmitgliedschaft auf den globalen Katalogen repliziert wird. Für die Erstellung von universellen Gruppen muss Ihre Domänenfunktionsebene mindestens die systemeigene Funktionsebene von Windows 2000 eingestellt und die Gesamtstrukturfunktionsebene auf Windows Server 2003 heraufgestuft sein.
  
Sie sollten MSDE 2000 oder Microsoft SQL Server 2005 Express Edition nur in Testumgebungen zur Unterstützung von RMS-Datenbanken verwenden, da weder MSDE 2000 noch Microsoft SQL Server 2005 Express Edition Netzwerkschnittstellen unterstützen. Darüber hinaus wird in den Nutzungsbedingungen für MSDE 2000 bzw. Microsoft SQL Server 2005 Express Edition angegeben, dass SQL Server-Clienttools nicht zur Bearbeitung einer MSDE 2000- oder Microsoft SQL Server 2005 Express Edition-Datenbank verwendet werden können. Aufgrund dieser Einschränkung können Sie weder Protokollierungsinformationen anzeigen noch in der Konfigurationsdatenbank gespeicherte Daten ändern.
  
Wenn Sie nicht ASP.NET-Version 1.1 auf dem Server installiert haben, unterscheidet sich der Installationsvorgang je nachdem, ob Sie die 32-Bit-Version von Windows Server 2003 oder die 64-Bit-Version von Windows Server 2003 ausführen.
  
Bei Ausführung der 32-Bit-Version von Windows Server 2003 sind für die Installation und Aktivierung von ASP.NET-Version 1.1 folgende Anweisungen zu beachten:
  
1.  Klicken Sie in der **Systemsteuerung** auf **Software**, und klicken Sie danach auf **Windows-Komponenten hinzufügen/entfernen**.  
2.  Klicken Sie auf **Anwendungsserver** und danach auf **Details**.  
3.  Wählen Sie im Assistenten für Windows-Komponenten **ASP.NET**.  
4.  Wenn ASP.NET 1.1 zwar installiert, aber nicht als IIS-Webdiensterweiterung zugelassen ist:  
    -   Öffnen Sie den Internetinformationsdienste-Manager.  
    -   Klicken Sie auf **IIS-Webdiensterweiterung**, wählen Sie ASP.NET, Version 1.1.4322, und klicken Sie danach auf **Zulassen**.
  
Bei Ausführung der 64-Bit-Version von Windows Server 2003 sind für die Installation und Aktivierung von ASP.NET-Version 1.1 folgende Anweisungen zu beachten:
  
1.  Installieren Sie .NET Framework 1.1, in dem die Installation von ASP.NET 1.1 enthalten ist. Sie können Microsoft .NET Framework Version 1.1 Redistributable Package vom Microsoft Download Center ([http://go.microsoft.co](http://go.microsoft.com/fwlink/?linkid=69985)) herunterladen.  
2.  Öffnen Sie den Internetinformationsdienste-Manager.  
3.  Klicken Sie auf IIS-Webdiensterweiterung, wählen Sie ASP.NET, Version 1.1.4322, und klicken Sie danach auf Zulassen.
  
Wenn Sie RMS mit einer 64-Bit-Version von Windows Server 2003 ausführen, müssen Sie folgende Anweisungen befolgen, damit IIS mit RMS eingesetzt werden kann:
  
1.  Klicken Sie auf **Start**, und klicken Sie danach auf **Ausführen**.  
2.  Geben Sie unter **Öffnen** den folgenden Befehl ein, und drücken Sie danach die Eingabetaste.
  
**"cscript %SystemDrive%\\inetpub\\AdminScripts\\adsutil.vbs set w3svc/AppPools/Enable32bitAppOnWin64 1"**
  
RMS ist nicht für .NET Framework Version 2.0 ausgelegt. Eine Parallelinstallation wird zwar unterstützt, Sie müssen jedoch sicherstellen, dass ASP.NET für die Verwendung von ASP.NET v1.1.4322 konfiguriert ist. Sie haben zwei Möglichkeiten, um eine erfolgreiche Parallelinstallation sicherzustellen:
  
-   Installieren Sie .NET Framework Version 2.0, bevor Sie den RMS-Server installieren.  
-   Stellen Sie die ASP.NET Version auf Version 1.1.4322 auf der Standardwebsite in IIS mithilfe folgenden Befehls zurück:
  
**"%SystemRoot%\\Microsoft.NET\\Framework\\v1.1.4322\\aspnet\_regiis -s w3svc/1/root"**
  
Weitere Informationen zu Active Directory, Message Queuing und IIS finden Sie im Windows Server 2003 Hilfe- und Supportcenter.
  
| ![](images/Cc720201.Caution(WS.10).gif)Vorsicht                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |  
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| Sie können den RMS-Server auf der Standardwebsite oder einer beliebigen anderen Website bereitstellen, die Sie zuvor in IIS definiert haben. Aus Sicherheitsgründen sollten Sie diesen Server nicht verwenden, um zusätzliche Websites oder Dienste auszuführen. Dies könnte dazu führen, dass mehrere Anwendungen und Dienste unter demselben Konto wie RMS (besonders das Konto „Lokales System“) ausgeführt werden. Hierdurch werden die privaten Schlüssel möglicherweise in dafür nicht vorgesehenen Operationen angezeigt. Der RMS-Server sollte nicht auf derselben Website wie Microsoft Office SharePoint Server 2007 bereitgestellt werden. RMS kann nicht mit Kerberos-Authentifizierung verwendet werden. Durch das Bereitstellen des RMS-Servers auf einer Website wird Kerberos-Authentifizierung für diesen Server deaktiviert. Wenn RMS nicht zur Verwendung von ASP.NET v1.1.4322 konfiguriert ist, werden keine Informationen in der Protokollierungsdatenbank protokolliert, was zu Datenverlust führt. |
  
Siehe auch  
----------
  
####  
  
[Planen der Datenbankserver-Infrastruktur](https://technet.microsoft.com/b12354bd-3143-4d1f-b5aa-450c4550653c)
