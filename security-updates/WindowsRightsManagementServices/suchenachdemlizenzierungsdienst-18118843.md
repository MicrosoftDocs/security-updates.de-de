---
TOCTitle: Suche nach dem Lizenzierungsdienst
Title: Suche nach dem Lizenzierungsdienst
ms:assetid: '4eabbb76-b359-443a-b737-098c5659e9c6'
ms:contentKeyID: 18118843
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720269(v=WS.10)'
---

Suche nach dem Lizenzierungsdienst
==================================

Der RMS-Lizenzierungsdienst gibt Nutzungslizenzen aus, mit denen authentifizierte Benutzer geschützten Inhalt abrufen können.

Dieser Dienst wird auf dem Stammzertifizierungsserver und Lizenzierungsservern oder auf Clustern ausgeführt. Zum Generieren einer Nutzungslizenzanforderung ruft ein Client zunächst den URL (Uniform Resource Locator) zum virtuellen Verzeichnis Licensing des Stammzertifizierungsclusters, auf dem sich der Lizenzierungsdienst befindet, von Active Directory ab. Anschließend fügt er den Pfad an den Lizenzierungsdienst an.

Beispiel: Der URL zum virtuellen Verzeichnis Licensing des Stammzertifizierungsclusters wird in Active Directory in folgender Form gespeichert:

http://*Servername*/\_wmcs/Licensing

Wenn ein Server eine Nutzungslizenz anfordert, fügt er den Dateinamen des Lizenzierungsdienstes folgendermaßen an den URL an:

http://*Servername*/\_wmcs/Licensing/License.asmx

Die Dienstpfad ist entweder der RMS-Server oder das .NET Passport-Konto, das die Veröffentlichungslizenz ausgegeben hat. Der URL ist in der Veröffentlichungslizenz enthalten.

| ![](images/Cc720269.note(WS.10).gif)Hinweis                              |
|-------------------------------------------------------------------------------------------------------|
| Wenn Sie SSL auf dem RMS-Server aktiviert haben, verwenden diese URLs das HTTPS-Verbindungsprotokoll. |
