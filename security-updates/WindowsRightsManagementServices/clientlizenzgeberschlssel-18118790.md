---
TOCTitle: 'Client-Lizenzgeberschlüssel'
Title: 'Client-Lizenzgeberschlüssel'
ms:assetid: '28781125-2692-4ff9-99b1-e09227d72966'
ms:contentKeyID: 18118790
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720221(v=WS.10)'
---

Client-Lizenzgeberschlüssel
===========================

Autoren können Client-Lizenzgeberzertifikate anfordern, mit denen Sie RMS-geschützte Inhalte veröffentlichen lassen können, selbst wenn Sie nicht mit dem RMS-fähigen Netzwerk verbunden sind. Ein Client-Lizenzgeberzertifikat verfügt über ein Schlüsselpaar von 1024-Bit-RSA-Schlüsseln.

Der RMS-Client verwendet den öffentlichen Schlüssel des Client-Lizenzgeberzertifikats, wenn er eine Veröffentlichungslizenz für die folgenden Aufgaben ausstellt:

-   Verschlüsseln des symmetrischen Inhaltsschlüssels
-   Signieren von Veröffentlichungslizenzen, die lokal ausgestellt werden, während der Benutzer nicht mit dem Netzwerk verbunden ist
