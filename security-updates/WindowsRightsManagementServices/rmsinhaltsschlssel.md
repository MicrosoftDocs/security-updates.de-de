---
TOCTitle: 'RMS-Inhaltsschlüssel'
Title: 'RMS-Inhaltsschlüssel'
ms:assetid: '63c814bf-2809-477e-a2db-d90370442075'
ms:contentKeyID: 18118876
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720284(v=WS.10)'
---

RMS-Inhaltsschlüssel
====================

Wenn ein Autor RMS-geschützten Inhalt veröffentlicht, erstellt eine RMS-fähige Anwendung einen symmetrischen Inhaltsschlüssel, mit dem sie den Inhalt verschlüsselt. RMS (Rights Management Services oder Dienste für die Rechteverwaltung) verwendet AES (Advanced Encryption Standard oder Erweiterter Verschlüsselungsstandard) zum Erstellen des Inhaltsschlüssels.

Der Inhaltsschlüssel ist in der Veröffentlichungslizenz enthalten und wird mit dem öffentlichen Schlüssel des RMS-Servers, der die Lizenz ausgegeben hat, verschlüsselt.

Wenn dieser Server eine Anforderung für eine Nutzungslizenz empfängt, verschlüsselt er den Inhaltsschlüssel mit dem privaten Serverschlüssel. Dann verschlüsselt er ihn erneut mit dem öffentlichen Benutzerschlüssel (den er als Bestandteil der Anforderung empfangen hat). Danach ist der Inhaltsschlüssel in der Nutzungslizenz enthalten.