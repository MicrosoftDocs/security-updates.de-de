---
TOCTitle: 'RMS-Vertrauenshierarchie'
Title: 'RMS-Vertrauenshierarchie'
ms:assetid: '2d44182f-a653-4383-aba1-dade53f7cf9a'
ms:contentKeyID: 18118783
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720232(v=WS.10)'
---

RMS-Vertrauenshierarchie
========================

Die mit dem RMS-System interagierenden Einheiten sind u. a. der Microsoft-Registrierungsdienst, die RMS-Server und Client-Computer in der Organisation sowie die Systembenutzer. Für jede Komponente wird ein Zertifikat ausgestellt, das deren Identität im System einrichtet. Eine Vertrauenshierarchie definiert die Vertrauensstellung zwischen diesen Zertifikaten und somit die Entitäten, die sie besitzen. Darüber hinaus definiert sie die Vertrauensstellung zwischen vertrauenswürdigen Entitäten und den Lizenzen, die diese für andere vertrauenswürdige Entitäten ausstellen.

Die Vertrauenshierarchie stellt eine Art Kette zwischen Zertifikaten und Lizenzen dar. RMS kann diese Verkettung von einem bestimmten Zertifikat oder einer bestimmten Lizenz aus bis zu einem vertrauenswürdigen Schlüsselpaar zurückverfolgen. Die Vertrauenskette umfasst das aktuelle Zertifikat; das Zertifikat der Entität, die das aktuelle Zertifikat ausgestellt hat; das Zertifikat der Entität, die das Zertifikat der ausstellenden Entität ausgestellt hat, usw., also die ganze Kette aufwärts bis zum Vertrauensstamm.

Im Fall von RMS ist die „Wurzel allen Vertrauens“ ein Schlüsselpaar von Microsoft. Dieser gemeinsame Vertrauensstamm ermöglicht einer Organisation das Erstellen eines Vertrauenssystems aus vertrauenswürdigen Entitäten, wie Benutzern und Partnern, sowohl innerhalb als auch außerhalb der Organisation.

Im folgenden Schema wird die Vertrauenshierarchie in einer Organisation dargestellt. Die Vertrauenskette verläuft zurück bis zu den Microsoft-Diensten, die die Basiszertifikate ausstellen.

![](images/Cc720232.6c169175-94fb-4ec0-93bc-12748aae3ac4(WS.10).gif)
1.  Jeder Clientcomputer erhält eine individuelle Lockbox, die den öffentlichen Stammschlüssel von Microsoft enthält.
2.  RMS überprüft bei jeder Lizenzanforderung die Prinzipale, indem es den Pfad in der Vertrauenshierarchie zum Vertrauensstamm zurückverfolgt.
3.  RMS überprüft die Authentizität der vertrauenswürdigen Entität, die in der Lizenz angegeben wird.
4.  RMS überprüft, ob das Zertifikat der vertrauenswürdigen Entität von einem Server ausgestellt wurde, der Teil der Vertrauenshierarchie ist.

Auf jeder Stufe der Zertifikatskette überprüft RMS Lizenzen und Zertifikate und ihre Verbindung mit einem bekannten Vertrauensstamm über eine Vertrauenskette. Alle Lizenzen und Zertifikate, die Teil der Kette sind, werden von RMS auf folgende Aspekte hin überprüft:

-   Die XrML ist gültig.
-   Die Signatur des Ausstellers ist gültig.
-   Die Semantik der Lizenz ist für den vorgesehenen Verwendungszweck geeignet.
-   Die Bedingungen (z. B. Gültigkeitsdaten) sind erfüllt.
-   Die Lizenz wurde nicht gesperrt.
-   Der Lizenzsignaturschlüssel und der zertifizierte Ausstellerschlüssel stimmen überein.
