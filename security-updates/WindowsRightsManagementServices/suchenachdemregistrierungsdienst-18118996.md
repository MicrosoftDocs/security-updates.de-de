---
TOCTitle: Suche nach dem Registrierungsdienst
Title: Suche nach dem Registrierungsdienst
ms:assetid: 'bbeb00bd-04e0-4df6-8615-76aa8125b620'
ms:contentKeyID: 18118996
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747737(v=WS.10)'
---

Suche nach dem Registrierungsdienst
===================================

Der erste RMS-Server, der in einer Gesamtstruktur bereitgestellt werden soll, muss eine Verbindung zum Microsoft-Registrierungsdienst herstellen, um sich zu registrieren und ein Server-Lizenzgeberzertifikat zu erhalten. Um den URL des Registrierungsdienstes zu ermitteln, sendet RMS-Setup eine UDDI-Anforderung (Universal Discovery, Description and Integration) an die [Microsoft-Website für UDDI](http://go.microsoft.com/fwlink/?linkid=14794)(http://go.microsoft.com/fwlink/?LinkId=14794). Nachfolgende Server, die als Teil des Stammzertifizierungsclusters bereitgestellt werden, müssen keine Server-Lizenzgeberzertifikate erhalten, weil sie die Konfiguration des ersten Stammzertifizierungsservers gemeinsam nutzen.
