---
TOCTitle: 'FIPS-Kompatibilitätsfragen für RMS'
Title: 'FIPS-Kompatibilitätsfragen für RMS'
ms:assetid: '720bdace-dcd8-431e-b0fa-01193782fe0b'
ms:contentKeyID: 18118948
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747551(v=WS.10)'
---

FIPS-Kompatibilitätsfragen für RMS
==================================

Rights Management Services (RMS) Version 1.0 Service Pack 1 (SP1) ist auf den effektiven Einsatz in Unternehmen ausgerichtet, bei denen FIPS-geprüfte Kryptographiefunktionen notwendig sind.

Die US-amerikanische Datenverarbeitungsnorm Federal Information Processing Standard 140-1 (FIPS 140-1) und die Nachfolgenorm FIPS 140-2 liefern Richtgrößen für die Implementierung von Kryptographiesoftware. Hier werden bewährte Verfahren für die Implementierung von Kryptographiealgorithmen, den Umgang mit wichtigen Material- und Datenpuffern sowie für die Arbeit mit dem Betriebssystem genannt.

RMS kann als Bestandteil eines FIPS-konformen Systems implementiert werden und so ein Mittel zum Schutz vertraulicher Daten bilden.

-   Die FIPS-geprüften Kryptographiedienstanbieter schränken die Funktionen wie folgt ein: **TLS\_RSA\_WITH\_3DES\_EDE\_CBC\_SHA**. Durch diese Einschränkung ist der Sicherheitskanalanbieter gezwungen, in jedem Fall das strengere Protokoll TLS 1.0 (Transport Layer Security) auszuhandeln. Unter Umständen muss Internet Explorer für die Unterstützung von TLS konfiguriert werden. Zahlreiche Webserver von Drittanbietern unterstützen TLS jedoch nicht. Weitere Informationen zu diesem Punkt finden Sie im Knowledge Base-Artikel 811834 auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=43614).

Falls Sie den softwarebasierten Schutz des privaten Schlüssels verwenden, lassen Sie den privaten RMS-Schlüssel von einem der beiden standardmäßigen Kryptographiedienstanbieter von Microsoft (Cryptographic Services Provider, CSP) schützen. Diese CSPs haben sich der Prüfung gemäß FIPS 140-1 bzw. FIPS 140-2 unterzogen. Kunden, bei denen die Sicherheit eine bedeutende Rolle spielt, sollten zum Schutz der privaten Schlüssel für die RMS-Server auf Hardwaresicherheitsmodule zurückgreifen (z. B. von nCipher oder IBM). Werden HSMs verwendet, muss der entsprechende CSP ausgewählt werden, um das HSM nutzen zu können. Hierbei muss das System ggf. neu gestartet werden. Weitere Informationen zu diesem Punkt finden Sie im Knowledge Base-Artikel 811834 auf der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=44138).

Bei der Implementierung des RMS-Systems sollten Sie wie folgt vorgehen:

-   Beachten Sie die NSA-Richtlinien für FIPS-konforme Kryptographie in Windows.
-   Aktivieren Sie die lokale Sicherheitsrichtlinie für die FIPS-konforme Kryptographie.
-   Stellen Sie Clients und Server mit RMS SP1 in der obigen Arbeitsumgebung bereit.
-   Aktivieren Sie das TLS-Protokoll (Transport Layer Security) in den Internetinformationsdiensten auf dem RMS-Server.
-   Aktivieren Sie das TLS-Protokoll (Transport Layer Security) in Internet Explorer auf den Clients.
-   Aktivieren Sie das SQL-TDS-Protokoll (Tabular Data Stream), das beim Windows TLS/SSL-Sicherheitsanbieter zwischen den SQL-Clients und SQL Server auf dem Datenbankserver eingesetzt wird.
-   Konfigurieren Sie SQL so, dass TSL/SSL obligatorisch ist.
