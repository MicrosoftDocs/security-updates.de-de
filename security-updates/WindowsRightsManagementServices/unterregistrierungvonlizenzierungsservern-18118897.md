---
TOCTitle: Unterregistrierung von Lizenzierungsservern
Title: Unterregistrierung von Lizenzierungsservern
ms:assetid: '7bc63397-9186-464c-8824-867038adce9b'
ms:contentKeyID: 18118897
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747640(v=WS.10)'
---

Unterregistrierung von Lizenzierungsservern
===========================================

Der Prozess, bei dem Lizenzierungsserver während der Bereitstellung automatisch registriert werden, wird als Unterregistrierung bezeichnet. Wenn Sie einem Lizenzierungsservercluster einen neuen Server hinzufügen, wird jedoch keine explizite Unterregistrierung des neuen Servers ausgeführt, weil dieser das Server-Lizenzgeberzertifikat und die Konfigurationsdatenbank des Clusters verwendet.

Der Lizenzierungsserver sendet die Unterregistrierungsanforderung nicht an den Microsoft-Registrierungsdienst, sondern an den Stammzertifizierungsserver. Die Unterregistrierungsanforderung für einen Lizenzierungsserver ist identisch mit einer Registrierungsanforderung für den Stammzertifizierungsserver.

Wenn der Stammzertifizierungsserver eine Unterregistrierungsanforderung erhält, überprüft er, ob die Anforderung das ordnungsgemäße Format hat, und gibt dann eine Zertifikatkette, die die Lizenzgeberzertifikatkette des Stammzertifizierungsservers enthält, sowie ein Zertifikat zurück, das vom Stammzertifizierungsserver signiert ist. Das Zertifikat enthält den öffentlichen Serverschlüssel, der mit dem privaten Schlüssel des Stammzertifizierungsservers signiert ist. Er erteilt dem Lizenzierungsserver das Recht zum Ausstellen von Nutzungs- und Veröffentlichungslizenzen.

Das Server-Lizenzgeberzertifikat ist für die Dauer eines Jahres gültig. Der Gültigkeitszeitraum beginnt bei der Ausstellung des Zertifikats. Am Ende des Gültigkeitszeitraums kann das Zertifikat erneuert werden. Die vom Server ausgestellten Zertifikate und Lizenzen sind für die Dauer von sieben Jahren gültig. Der Gültigkeitszeitraum beginnt bei der Ausstellung des Zertifikats bzw. der Lizenz.

Standardmäßig wird der zum Verarbeiten einer Unterregistrierungsanforderung auf dem Stammzertifizierungsserver erforderliche Dienst SubEnrollService.asmx so konfiguriert, dass er alle Zugriffe ablehnt. Sie müssen deshalb die DACLs (Discretionary Access Control Lists oder freigegebene Zugriffssteuerungslisten) ändern, um dem RMS-Administrator Zugriff zu erteilen, bevor eine Anforderung verarbeitet werden kann.