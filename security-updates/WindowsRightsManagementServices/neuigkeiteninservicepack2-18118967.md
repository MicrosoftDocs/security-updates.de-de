---
TOCTitle: Neuigkeiten in Service Pack 2
Title: Neuigkeiten in Service Pack 2
ms:assetid: 'a944cb73-d900-42bb-b7aa-92916dead408'
ms:contentKeyID: 18118967
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747629(v=WS.10)'
---

Neuigkeiten in Service Pack 2
=============================

RMS (Rights Management Services, Rechteverwaltungsdienst) mit Service Pack 2 (SP2) bietet Unterstützung für die folgenden Features:

-   **Native Unterstützung für Microsoft® SQL Server™ 2005**. In vorherigen RMS-Versionen konnte RMS nur mit zusätzlichem Aufwand mit SQL Server 2005 genutzt werden. Informationen dazu, wie diese Problemumgehung aussieht, finden Sie in Artikel 913372 in der Microsoft Knowledge Base ([http://go.microsoft.com/fwlink/?LinkId=68638](http://go.microsoft.com/fwlink/?linkid=68638)) (möglicherweise in englischer Sprache). In RMS mit SP2 wurde dieses Problem behoben.
-   **Microsoft Office SharePoint® Server 2007**. In dieser Version wird Office SharePoint Server 2007 unterstützt. Die Office SharePoint Server 2007-Dokumentbibliothek weist Dokumenten beim Herunterladen automatisch RMS-Berechtigungen auf der Basis der Office SharePoint Server 2007-Rechte zu. Dies wird erreicht, indem der RMS mit SP2-Client auf dem Office SharePoint Server 2007-Server installiert wird. Es wird nicht empfohlen, die Serverkomponente von RMS mit SP2 und Office SharePoint Server 2007 auf ein und demselben Computer zu installieren.
-   **Mehr Sicherheit bei den Nachrichten an die Protokollierungsdatenbank**. In dieser Version werden alle Message Queuing-Nachrichten von den RMS-Servern an die RMS-Protokollierungsdatenbank digital signiert.
-   **Vergrößerung der Serverbatchgrößen**. In dieser Version können RMS-fähige Anwendungen mit einer einzigen Lizenzanfrage beim RMS-Server mehrere Nutzungslizenzen für unterschiedliche Benutzerkonten abrufen. Dadurch erhöht sich die Arbeitsgeschwindigkeit, denn es entfällt der Aufwand, der für die Verarbeitung mehrerer Lizenzanforderungen für ein und denselben durch Rechte geschützten Inhalt erforderlich ist.
-   **Verbesserte gesamtstrukturübergreifende Gruppenerweiterung**. In dieser Version erfolgt die gesamtstrukturübergreifende Gruppenerweiterung in Form einer SOAP-Anforderung (Simple Object Access-Protokoll) an einen neuen ASP.NET-Webdienst, der auf dem RMS-Server ausgeführt wird.
