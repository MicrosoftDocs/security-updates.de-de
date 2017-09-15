---
TOCTitle: Veröffentlichungslizenzen
Title: Veröffentlichungslizenzen
ms:assetid: '187228fc-370b-4e23-a53a-21bb296b84a1'
ms:contentKeyID: 18118762
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720211(v=WS.10)'
---

Veröffentlichungslizenzen
=========================

Benutzer RMS-fähiger Anwendungen können zur Einhaltung unternehmensweit geltender Richtlinien digitale Dateien und Informationen mit bestimmten Nutzungsrechten versehen. Diese Nutzungsrechte werden in Veröffentlichungslizenzen gespeichert, die spezifizieren, welche Benutzer die Inhalte einsehen dürfen, und in welchem Maße diese Benutzer den Inhalt bearbeiten bzw. weiterleiten dürfen.

Eine Veröffentlichungslizenz kann von einer RMS-fähigen Clientanwendung, dem Stammzertifizierungsserver oder einem RMS-Lizenzierungsserver ausgestellt werden. Wenn eine Veröffentlichungslizenz von einer RMS-fähigen Clientanwendung ausgestellt wird, wird dieser Anwendung vom RMS-Server ein Client-Lizenzgeberzertifikat ausgestellt. Dies wird als Offlinepublishing bezeichnet. Dabei handelt es sich um eine häufige Veröffentlichungsmethode, da sie Benutzern RMS-fähiger Anwendungen das Erstellen geschützter Inhalte ermöglicht, ohne dass eine Verbindung mit dem RMS-Server bestehen muss. Wenn die RMS-fähige Clientanwendung keine Client-Lizenzgeberzertifikate nutzt, muss der Benutzer über eine Verbindung zu einem RMS-Server verfügen, von dem er eine Veröffentlichungslizenz für die geschützten Inhalte erhalten kann.

Eine Veröffentlichungslizenz enthält den symmetrischen Schlüssel für Inhalte zum Verschlüsseln derselben. Die Verschlüsselung nutzt den öffentlichen Schlüssel des RMS-Servers. Damit wird sichergestellt, dass nur der Server die Inhalte entschlüsseln und Nutzungslizenzen ausstellen kann.

Eine Veröffentlichungslizenz wird mit dem privaten Schlüssel des ausstellenden Servers oder dem privaten Schlüssel des Client-Lizenzgeberzertifikats signiert.
