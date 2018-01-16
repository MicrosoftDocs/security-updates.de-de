---
TOCTitle: 'Schritt 1: Überprüfen der Installationsanforderungen für WSUS'
Title: 'Schritt 1: Überprüfen der Installationsanforderungen für WSUS'
ms:assetid: '57d7f8ec-1523-4485-9967-604be9ba2aac'
ms:contentKeyID: 18127465
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720547(v=WS.10)'
---

Schritt 1: Überprüfen der Installationsanforderungen für WSUS
=============================================================

In diesem Handbuch sind Anweisungen zum Installieren von Microsoft Windows Server Update Services (WSUS) unter Microsoft Windows Server 2003-Betriebssystemen (mit Ausnahme von Web Edition und allen 64-Bit-Versionen) enthalten. Wenn auf Ihrem Server Microsoft Windows 2000 Server ausgeführt wird und Sie weitere Informationen benötigen, informieren Sie sich im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache).

Die folgenden Grundinstallationsanforderungen gelten für Installationen mit den Standardoptionen. Hardware- und Softwareanforderungen für weitere Installationen können Sie dem Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache) entnehmen.

Für einen Server mit bis zu 500 Clients gelten die folgenden Hardwarempfehlungen:

-   1 GHz-Prozessor
-   1 GB RAM

Softwareanforderungen
---------------------

Zum Installieren von WSUS mit den Standardoptionen muss Folgendes auf dem Computer installiert sein. Weitere Informationen zu den Softwareanforderungen für WSUS finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" (möglicherweise in englischer Sprache). Wenn für eines dieser Updates nach Abschluss der Installation ein Neustart des Computers erforderlich ist, sollten Sie Ihren Server neu starten, bevor Sie WSUS installieren.

-   Microsoft Internetinformationsdienste (IIS) 6.0 Anweisungen zum Installieren von IIS finden Sie im Whitepaper "Bereitstellen von Microsoft Windows Server Update Services" oder im Hilfe- und Supportcenter von Windows Server 2003 (möglicherweise in englischer Sprache).
-   Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003. Sie erhalten diese Software im [Download Center](http://go.microsoft.com/fwlink/?linkid=47358) unter **http://go.microsoft.com/fwlink/?LinkId=47358** (möglicherweise in englischer Sprache).
    Alternativ können Sie auch zu **http://www.windowsupdate.com** gehen und unter "Wichtige Updates und Service Packs" nach "Installieren von Microsoft .NET Framework 1.1 Service Pack 1 für Windows Server 2003" (möglicherweise in englischer Sprache) suchen.
-   Intelligenter Hintergrundübertragungsdienst (BITS) 2.0 BITS 2.0 für Windows Server 2003 steht derzeit nicht im Download Center zur Verfügung. Sie erhalten diese Software auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=47357) zu Windows Server Update Services Open Evaluation unter **http://go.microsoft.com/fwlink/?LinkId=39496** (möglicherweise in englischer Sprache).

> [!NOTE]
> Zum Installieren von WSUS ist Datenbanksoftware erforderlich. Sie ist hier jedoch nicht aufgeführt, da die Standardinstallation von WSUS unter Windows Server 2003 die Datenbanksoftware Windows SQL Server™ 2000 Desktop Engine (WMSDE) beinhaltet. 

Festplattenanforderungen und -empfehlungen
------------------------------------------

Zum Installieren von WSUS muss das Dateisystem auf dem Server folgende Anforderungen erfüllen:

-   Die Systempartition und die Partition, auf der WSUS installiert wird, müssen mit dem NTFS-Dateisystem formatiert sein.
-   Für die Systempartition ist mindestens 1 GB freier Speicher erforderlich.
-   Für den Datenträger, auf dem WSUS Inhalt speichert, sind mindestens 6 GB freier Speicher erforderlich; 30 GB werden empfohlen.
-   Für den Datenträger, auf dem WSUS Setup Windows SQL Server 2000 Desktop Engine (WMSDE) speichert, sind mindestens 2 GB freier Speicher erforderlich.

Anforderungen für die automatischen Updates
-------------------------------------------

Die automatischen Updates sind die WSUS-Clientkomponente. Für die automatischen Updates bestehen keine Hardwareanforderungen außer einer Netzwerkverbindung. Sie können die automatischen Updates mit WSUS auf Computern unter folgenden Betriebssystemen verwenden:

-   Microsoft Windows 2000 Professional mit Service Pack 3 (SP3) oder Service Pack 4 (SP4), Windows 2000 Server mit SP3 oder SP4 oder Windows 2000 Advanced Server mit SP3 oder SP4.
-   Microsoft Windows XP Professional mit oder ohne Service Pack 1 oder Service Pack 2.
-   Microsoft Windows Server 2003 Standard Edition, Windows Server 2003 Enterprise Edition, Windows Server 2003 Datacenter Edition oder Windows Server 2003 Web Edition.
