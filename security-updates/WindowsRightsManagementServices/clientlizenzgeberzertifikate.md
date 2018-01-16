---
TOCTitle: 'Client-Lizenzgeberzertifikate'
Title: 'Client-Lizenzgeberzertifikate'
ms:assetid: 'bfb36387-3e15-4cde-8b8f-482219569a64'
ms:contentKeyID: 18118995
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747744(v=WS.10)'
---

Client-Lizenzgeberzertifikate
=============================

Ein Client-Lizenzgeberzertifikat erteilt einem Autor die Berechtigung, RMS-geschützten Inhalt zu veröffentlichen, ohne dass eine Verbindung zum Firmennetzwerk besteht.

Der Autor sendet von einem Clientcomputer aus eine Clientregistrierungsanforderung an den Stammzertifizierungsserver oder einen Lizenzierungsserver, um ein Client-Lizenzgeberzertifikat zu erhalten. Der Server gibt dann ein Client-Lizenzgeberzertifikat für den betreffenden Computer zurück.

Ein Client-Lizenzgeberzertifikat enthält den öffentlichen Schlüssel des Clientlizenzgebers zusammen mit dessen privatem Schlüssel. Dieser wird mit dem öffentlichen Schlüssel des Autors verschlüsselt, der das Zertifikat angefordert hat. Das Client-Lizenzgeberzertifikat enthält außerdem den öffentlichen Schlüssel des Servers, der das Zertifikat ausgestellt hat. Dieser Schlüssel wird mit dem privaten Schlüssel desselben Servers signiert. Der private Schlüssel des Clientlizenzgebers wird zum Signieren von Veröffentlichungslizenzen verwendet, die vom Autor erstellt werden.