---
TOCTitle: Offlineveröffentlichung
Title: Offlineveröffentlichung
ms:assetid: 'f6384ed2-f917-442e-aa63-c1394a1c4d06'
ms:contentKeyID: 18119078
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747741(v=WS.10)'
---

Offlineveröffentlichung
=======================

Die Offlineveröffentlichung unterscheidet sich von der Onlineveröffentlichung durch die Art, in der die RMS-fähige Anwendung die Veröffentlichungslizenz erwirbt.

Bevor ein Autor Inhalte offline veröffentlichen kann, muss er ein Client-Lizenzgeberzertifikat erwerben, während er Netzwerkzugriff auf den Stammzertifizierungsserver hat.

Der Offlineveröffentlichungsprozess besteht aus folgenden Schritten:

1.  Der Autor erstellt das Dokument mit einer RMS-fähigen Anwendung und gibt anschließend die Rechte und Bedingungen für den Inhalt an.
2.  Wenn der Autor die Datei speichert, ermöglicht das Client-Lizenzgeberzertifikat dem lokalen Computer oder Gerät das Ausstellen und Signieren einer Veröffentlichungslizenz für die Datei.
    Die Veröffentlichungslizenz enthält zwei Kopien des Inhaltsschlüssels. Eine Kopie wird mit dem öffentlichen Schlüssel des Client-Lizenzgeberzertifikats verschlüsselt, und eine Kopie wird mit dem öffentlichen Schlüssel des Servers verschlüsselt, der das Client-Lizenzgeberzertifikat ausgestellt hat. Außerdem enthält sie den URL des Servers. Die beiden öffentlichen Schlüssel und der URL werden aus dem Client-Lizenzgeberzertifikat übernommen.
3.  Der Computer verwendet das Client-Lizenzgeberzertifikat zum Erstellen einer Besitzerlizenz. Dies ist eine besondere Nutzungslizenz, die dem Autor das Recht erteilt, den RMS-geschützten Inhalt abzurufen, obwohl er nicht mit dem Netzwerk verbunden ist (offline). Das Client-Lizenzgeberzertifikat entschlüsselt den symmetrischen Inhaltsschlüssel aus der Veröffentlichungslizenz mithilfe seines privaten Schlüssels und verschlüsselt ihn anschließend erneut für die Besitzerlizenz.
4.  Die Anwendung verschlüsselt die Datei mit dem Inhaltsschlüssel und bindet die Veröffentlichungslizenz an die Datei. Nur der RMS-Server, der die Veröffentlichungslizenz ausgestellt hat, oder ein Mitglied einer vertrauenswürdigen Veröffentlichungsdomäne kann Lizenzen zum Entschlüsseln dieser Datei ausstellen.
