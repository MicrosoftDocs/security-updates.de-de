---
TOCTitle: 'RMS-Clientregistrierung'
Title: 'RMS-Clientregistrierung'
ms:assetid: '9c1d07bf-7235-4694-8291-ac2e5b221f4a'
ms:contentKeyID: 18118951
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747613(v=WS.10)'
---

RMS-Clientregistrierung
=======================

Clientcomputer können beim RMS-Veröffentlichungsdienst registriert werden, damit sie ein Client-Lizenzgeberzertifikat erhalten. Mit diesem Zertifikat können Autoren RMS-geschützten Inhalt auch dann veröffentlichen, wenn sie nicht mit dem Firmennetzwerk verbunden sind. In diesem Fall werden die Veröffentlichungslizenzen, die Informationen zu den Nutzungsrechten für RMS-geschützten Inhalt enthalten, der auf diesem Computer veröffentlicht wird, nicht vom Veröffentlichungsdienst, sondern vom Clientcomputer signiert.

Der RMS-Veröffentlichungsdienst erteilt Client-Lizenzgeberzertifikate.

Die Clientregistrierung schließt die folgenden Schritten ein:

1.  Der Clientcomputer sendet das Rechtekontozertifikat des Benutzers in einer Registrierungsanforderung an den Veröffentlichungsservice, der auf dem Stammzertifizierungsserver oder -cluster oder auf einem Lizenzierungsserver oder -cluster ausgeführt wird.
2.  Der Server überprüft, ob die Clientregistrierung basierend auf den Einstellungen des Netzwerkadministrators zulässig ist und ob das Rechtekontozertifikat nicht auf einer in der Konfigurationsdatenbank gespeicherten Ausschlussliste verzeichnet ist. Weitere Informationen zum Erstellen von Ausschlusslisten finden Sie unter „Verwalten von Ausschlussrichtlinien“ im Abschnitt „Betreiben eines RMS-Servers“ in dieser Dokumentationssammlung.
3.  Der Veröffentlichungsdienst erstellt ein Schlüsselpaar für den Clientcomputer. Er erstellt ein Client-Lizenzgeberzertifikat und speichert den öffentlichen Schlüssel im Zertifikat. Er verschlüsselt den privaten Schlüssel mit dem öffentlichen Schlüssel des Rechtekontozertifikats und fügt ihn dann in das Zertifikat ein.
4.  Der Veröffentlichungsdienst stellt ein Client-Lizenzgeberzertifikat für den Clientcomputer aus.
