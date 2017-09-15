---
TOCTitle: 'Aktivieren der RMS-Unterstützung für Serverdienste'
Title: 'Aktivieren der RMS-Unterstützung für Serverdienste'
ms:assetid: '6288323c-0638-41b6-bef8-67a7c9433424'
ms:contentKeyID: 18118858
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747593(v=WS.10)'
---

Aktivieren der RMS-Unterstützung für Serverdienste
==================================================

RMS kann auch Rechte-Kontozertifikate bereitstellen und Lizenzen für RMS-fähige Serveranwendungen verwenden. Es gibt eine Reihe von Dingen, auf die Sie bei der Konfiguration von Serverdiensten achten sollten:

-   Freigegebene Zugriffssteuerungslisten (Discretionary Access Control Lists, DACLs) auf den RMS-Pipelines verwenden standardmäßig die sichersten Einstellungen. Sie müssen die DACL bei der Verwendung von RMS-Serverdiensten bearbeiten.
-   Wenn der RMS-Client auf einem Server unter Windows 2003 installiert und die verstärkte Sicherheitskonfiguration aktiviert ist, müssen Sie die RMS-Cluster-URL der Zone vertrauenswürdiger Sites des Internet Explorers hinzufügen.
-   Viele Serverdienste verwenden erweiterte Active Directory-Verzeichnisdienstfunktionalität, die nur verfügbar ist, wenn alle Active Directory-Domänencontroller Windows Server 2003 ausführen. Wenn Sie einen dieser Serverdienste verwenden (z. B. Microsoft Office SharePoint Server 2007 oder Microsoft Exchange Server 2007), sollten alle Domänencontroller Windows Server 2003 ausführen und die Funktionsebenen der Active Directory-Domänen und -Gesamtstrukturen auf Windows Sever 2003 Ebene sein.

Standard-Zugriffssteuerungsliste (Discretionary Access Control List oder DACL) auf Serverzertifizierungspipeline
----------------------------------------------------------------------------------------------------------------

Anwendungen wie Microsoft Office SharePoint Server 2007 oder Microsoft Exchange Server 2007 sind RMS-fähig und können Lizenzen für Benutzer anfordern. In einer RMS-Standardinstallation ist die DACL der RMS-Serverzertifizierungspipeline eingeschränkt, was bedeutet, dass eine Anwendung für ihre Benutzer keine Zertifikate und Lizenzen einholen kann. Wenn Sie jedoch eine RMS-fähige Anwendung für diese Computer besitzen, können Sie diese Anwendung im Hinblick auf eine Teilnahme am RMS-System aktivieren, indem Sie die DACLs auf der RMS-Serverzertifizierungspipeline konfigurieren.

RMS-fähige Serveranwendung verwenden die Datei ServerCertification.asmx, um eine Verbindung mit dem RMS-Zertifizierungsdienst herzustellen.

Bei der Erstellung dieser Dateien durch RMS sind ihre DACLs so eingestellt, dass der Zugriff nur über Systemprozesse erfolgen kann. Sie sollten eine Active Directory-Sicherheitsgruppe für Serverdienste erstellen und dieser Gruppe dann Active Directory-Objekte der Computer hinzufügen, die Lizenzen für ihre Benutzer anfordern.

Nach dem Erstellen der Gruppen können Sie die freigegebenen Zugriffssteuerungslisten (DACL) für die Datei ServerCertification.asmx ändern, um der Gruppe auf diesem Dienst die Berechtigung Lesen & Ausführen zu gewähren. Außerdem muss die RMS Service Group (RMS-Dienstgruppe) der DACL zugewiesen werden, und zwar mit der Berechtigung zum Lesen & Ausführen.

| ![](images/Cc747593.note(WS.10).gif)Hinweis                                                                           |
|----------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn es mehr als einen RMS-Server im Cluster gibt, muss die DACL in der Datei ServerCertifiation.asmx auf jedem Server im Cluster geändert werden. |

Für Microsoft Exchange Server 2007 muss das Active Directory-Computerobjekt jedes Exchange-Bridgeheadservers der Serverdienstgruppe hinzugefügt werden. Andernfalls kann der Exchange-Bridgeheadserver keine Lizenzen für Benutzer anfordern, die die E-Mail erhielten.

Für Office SharePoint Server 2007 müssen Sie die Active Directory-Computerobjekte des Servers, auf dem Office SharePoint Server 2007 ausgeführt wird, der Serverdienstgruppe hinzufügen. Wenn Ihr Office SharePoint Server 2007-Server auf die Verwendung des Standardservers in Active Directory eingestellt ist, müssen Sie die RMS Service Group (RMS-Dienstgruppe) und die für Serverdienste erstellte Gruppe der Datei ServiceLocater.asmx hinzufügen und die Berechtigung zum Lesen & Ausführen zulassen.

| ![](images/Cc747593.Important(WS.10).gif)Wichtig                                                                                                                                                                             |
|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Internetinformationsdienste (IIS) müssen nach Änderungen an der DACL in den Dateien ServerCertification.asmx und ServiceLocater.asmx neu gestartet werden. Zum Zurücksetzen der IIS führen Sie den Befehl **iisreset** über eine Eingabeaufforderung aus. |
