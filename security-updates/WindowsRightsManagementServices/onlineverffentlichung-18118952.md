---
TOCTitle: Onlineveröffentlichung
Title: Onlineveröffentlichung
ms:assetid: '962c4e83-cf34-4c61-9589-31d24b0299fb'
ms:contentKeyID: 18118952
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747694(v=WS.10)'
---

Onlineveröffentlichung
======================

Im folgenden Schema wird der Onlineveröffentlichungsprozess dargestellt.

![](images/Cc747694.897e47b6-fffe-4b11-bc9f-be58539b9f19(WS.10).gif)

Der Onlineveröffentlichungsprozess besteht aus folgenden Schritten:

1.  Der Autor von Inhalt erstellt ein Dokument und verwendet die RMS-fähigen Anwendung, um Benutzer festzulegen und dem Inhalt Rechte und Bedingungen zuzuweisen.
2.  Die RMS-fähige Anwendung erstellt einen symmetrischen Inhaltsschlüssel und sendet eine Anforderung für eine Veröffentlichungslizenz an den Zertifikatsserver oder den Lizenzierungsserver. Die Anforderung schließt den Inhaltsschlüssel und die Nutzungseinstellungen ein.
3.  Der Lizenzierungsserver erstellt die Veröffentlichungslizenz, verschlüsselt den Inhaltsschlüssel mit dem öffentlichen Serverschlüssel und gibt anschließend die Veröffentlichungslizenz an die RMS-fähige Anwendung zurück.
4.  Die Anwendung verschlüsselt die Datei mit dem Inhaltsschlüssel und bindet die Veröffentlichungslizenz an die Datei.
5.  Die RMS-fähige Anwendung auf dem Computer des Benutzers, der den Inhalt abruft, sendet eine Anforderung, die das Rechtekontozertifikat des abrufenden Benutzers enthält, an den RMS-Server (der die Veröffentlichungslizenz ausgestellt hat), um eine Nutzungslizenz für das Dokument anzufordern.
6.  Der RMS-Server überprüft die Anmeldeinformationen des Benutzers. Wenn die Überprüfung erfolgreich ist, wird eine Nutzungslizenz erstellt und an die RMS-fähige Anwendung auf dem Computer des Benutzers, der den Inhalt abruft, zurückgegeben.
7.  Die RMS-fähige Anwendung öffnet das Dokument und erteilt die Benutzerrechte gemäß den in der Nutzungslizenz definierten Parametern.