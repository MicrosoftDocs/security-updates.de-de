---
TOCTitle: Registrierung des Stammzertifizierungsservers
Title: Registrierung des Stammzertifizierungsservers
ms:assetid: 'f08bc919-f090-4843-b2ce-b40d558012ce'
ms:contentKeyID: 18119075
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747734(v=WS.10)'
---

Registrierung des Stammzertifizierungsservers
=============================================

Die Registrierung beim Microsoft-Registrierungsdienst ist für den ersten Server in einer RMS-Bereitstellung erforderlich. Dieser Server, der ein Stammzertifizierungsserver ist, kann automatisch während der Bereitstellung registriert werden, wenn er eine Internetverbindung hat, oder er kann manuell registriert werden, wenn er Teil eines abgeschlossenen Netzwerks ist. Weitere Informationen zur manuellen Serverregistrierung finden Sie unter „So registrieren Sie einen Stammzertifizierungsserver manuell“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.

Die Registrierungsanforderung verwendet folgende Eingabeparameter:

-   Ein öffentlicher 1024-Bit-Schlüssel. Dies ist der öffentliche RMS-Schlüssel.
-   Version, Name und URL des RMS-Servers, der registriert werden soll.

Der Microsoft-Registrierungsdienst verwendet die Informationen nur zum Erstellen des Server-Lizenzgeberzertifikats. Er speichert die Informationen nur für Sperrungszwecke.

Der Microsoft-Registrierungsdienst gibt eine Zertifikatskette zurück. Diese enthält die Lizenzgeberzertifikatskette des Registrierungsservers sowie ein von diesem Server signiertes Zertifikat. Das Zertifikat enthält den öffentlichen Serverschlüssel, der mit dem privaten Registrierungsschlüssel sowie der Version und dem URL des registrierten Servers signiert ist. Das Zertifikat erteilt dem Stammzertifizierungsserver das Recht, Server-Lizenzgeberzertifikate für Lizenzierungsserver sowie Rechtekontozertifikate, Client-Lizenzgeberzertifikate, Veröffentlichungs- und Nutzungslizenzen auszustellen.

Das Server-Lizenzgeberzertifikat ist für die Dauer eines Jahres gültig. Der Gültigkeitszeitraum beginnt bei der Ausstellung des Zertifikats. Am Ende des Gültigkeitszeitraums kann das Zertifikat erneuert werden. Die vom Server ausgestellten Zertifikate und Lizenzen sind für die Dauer von sieben Jahren gültig. Der Gültigkeitszeitraum beginnt bei der Ausstellung des Zertifikats bzw. der Lizenz.

Die Informationen zum Sperren des Zertifikats werden entsprechend der Angabe in der Registrierungsanforderung dem Server-Lizenzgeberzertifikat hinzugefügt. Der öffentliche Schlüssel des Microsoft-Registrierungsdienstes wird dem Zertifikat als sperrender Schlüssel hinzugefügt. Wenn darüber hinaus ein Sperrschlüssel eines Drittanbieters angegeben wird, wird auch dieser dem Zertifikat als sperrender Schlüssel hinzugefügt.
