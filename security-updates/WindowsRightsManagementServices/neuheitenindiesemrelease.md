---
TOCTitle: Neuheiten in diesem Release
Title: Neuheiten in diesem Release
ms:assetid: 'c68ec6fd-0ff5-467e-85a8-a53b9f089de3'
ms:contentKeyID: 18119002
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747748(v=WS.10)'
---

Neuheiten in diesem Release
===========================

Die Dienste für die Rechteverwaltung (Rights Management Services oder RMS) mit Service Pack 1 ( SP1) bieten Unterstützung für die folgenden Features:

-   **Registrieren des RMS-Servers ohne Internetkonnektivität des Servers**. In der Vorgängerversion musste der RMS-Server eine Verbindung zum Internet herstellen, um sich beim Microsoft-Registrierungsdienst zu registrieren und das Stammserver-Lizenzgeberzertifikat zu erhalten. In RMS SP1 muss das Stammserver-Lizenzgeberzertifikat weiterhin beim Microsoft-Registrierungsdienst angefordert werden. Die Anforderung kann jedoch über einen anderen Computer mit Internetanschluss erfolgen und das Zertifikat nach der Bereitstellung von RMS auf den RMS-Server importiert werden.
-   **Clients aktivieren sich selbst**. In der Vorgängerversion mussten die Computerzertifikate und Lockboxen für die Clientcomputer vom Microsoft-Aktivierungsdienst heruntergeladen werden. Bei RMS SP1 ist keine Verbindung mehr zum Microsoft-Aktivierungsdienst erforderlich.
-   **Unterstützung für mehr Arten von Clients.** In dieser Version kann der RMS-Server zur Unterstützung von Clients auf mobilen Geräten und Serverdiensten verwendet werden. Als RMS-Server-Administrator können Sie steuern, ob der Server diesen Clients ein Zertifikat erteilt oder nicht, wenn die Clients versuchen, Ihre Dienste zu nutzen.
-   **Unterstützung für Vorlagen in mehreren Sprachen**. In der Vorgängerversion war die Vorlagensprache von der Spracheinstellung für Internet Explorer abhängig. In dieser Version können Sie auf der Website für die RMS-Verwaltung angeben, welche Sprache zur Erstellung von Vorlagen verwendet werden soll.
-   **Unterstützung für die Clientauthentifizierung mit Smartcards**. In dieser Version kann der RMS-Client zur Authentifizierung beim RMS-Server für den Erhalt von Rechtekontozertifikaten (Rights Account Certificates oder RACs) und Nutzungslizenzen Anmeldeinformationen verwenden, die als x.509-Zertifikate auf Smartcards gespeichert sind.