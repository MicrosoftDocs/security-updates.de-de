---
TOCTitle: Suche nach dem Kontozertifizierungsdienst
Title: Suche nach dem Kontozertifizierungsdienst
ms:assetid: '293a2f91-4712-45ec-8b74-7533f4144cbd'
ms:contentKeyID: 18118779
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720224(v=WS.10)'
---

Suche nach dem Kontozertifizierungsdienst
=========================================

Der Kontozertifizierungsdienst von RMS stellt Benutzern Rechtekontozertifikate aus. Jedes dieser Zertifikate gilt nur für einen bestimmten Computer bzw. ein bestimmtes Gerät und erfordert, dass der anfordernde Benutzer über ein gültiges Computerzertifikat verfügt.

Der Kontozertifizierungsdienst wird nur auf dem Stammzertifizierungsserver oder -cluster ausgeführt. Für das Anfordern einer Kontozertifizierung ermittelt der Client zunächst über Active Directory den URL des virtuellen Verzeichnisses für die Zertifizierung auf dem Stammzertifizierungsserver. Dort befindet sich der Kontozertifizierungsdienst. Anschließend fügt er den Pfad an den Kontozertifizierungsdienst an.

Zum Beispiel wird der Zertifizierungs-URL des Stammzertifizierungsservers in der folgenden Form bei Active Directory gespeichert:

http://*Servername*/\_wmcs/Certification

Wenn ein Client ein Rechtekontozertifikat anfordert, wird der Dateiname des Kontozertifizierungsdienstes an den URL angehängt:

http://*Servername*/\_wmcs/Certification/Certification.asmx

> [!NOTE]
> Wenn SSL auf dem RMS-Server aktiviert wurde, wird für diese URL das HTTPS-Verbindungsprotokoll verwendet. 