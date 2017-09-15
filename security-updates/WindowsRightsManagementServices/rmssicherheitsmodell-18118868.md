---
TOCTitle: 'RMS-Sicherheitsmodell'
Title: 'RMS-Sicherheitsmodell'
ms:assetid: '665db831-366d-4dca-9bb3-cc2912481fe1'
ms:contentKeyID: 18118868
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747598(v=WS.10)'
---

RMS-Sicherheitsmodell
=====================

Im Rahmen seiner Operationen erhält RMS (Rights Management Services oder Dienste für die Rechteverwaltung) Zugriff auf verschiedene Ressourcen, einschließlich des Datenbankservers, Active Directory, der Nachrichtenwarteschlange und der lokalen Festplatte. Darüber erstellt RMS-Setup bestimmte Ressourcen, die für seine Operationen erforderlich sind, wie z. B. SOAP-Einträge, Webseiten, Warteschlangen für Protokollierungsnachrichten usw., und stellt sie dar. RMS-Setup konfiguriert DACLs (Discretionary Access Control Lists oder freigegebene Zugriffssteuerungslisten) für die Ressourcen, die es erstellt und darstellt, und konfiguriert außerdem die IIS-Authentifizierung für jede Ressource.

Dieser Abschnitt enthält Informationen darüber, wie RMS die Sicherheit für die von ihm verwendeten Ressourcen konfiguriert und wie es während der unterschiedlichen Phasen seiner Operationen Zugriff auf die Ressourcen erhält: Setup, Bereitstellung und Normalbetrieb.

Dieser Abschnitt behandelt die folgenden Themen:

-   [RMS-Sicherheitsgruppen](https://technet.microsoft.com/25749a83-8c12-48ec-96ad-296d31fd55d4)
-   [Sicherheitsmodi für RMS](https://technet.microsoft.com/d7792293-5bb2-4232-9d48-e81e87ab6219)
-   [Sicherheit während des RMS-Setups](https://technet.microsoft.com/0a3d40b2-f27e-4e63-baff-a9c8433f5f91)
-   [Sicherheit während der Bereitstellung](https://technet.microsoft.com/9f1282c5-5642-4870-a9a4-c3a485f8ff76)
-   [Sicherheit während der normalen RMS-Operationen](https://technet.microsoft.com/98f3d584-6320-4aa1-9959-7133cfdb6df7)
