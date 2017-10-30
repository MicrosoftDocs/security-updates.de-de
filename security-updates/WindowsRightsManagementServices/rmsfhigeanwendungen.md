---
TOCTitle: 'RMS-fähige Anwendungen'
Title: 'RMS-fähige Anwendungen'
ms:assetid: '30bb5565-81d3-43d9-a64d-cf0c5b990712'
ms:contentKeyID: 18118788
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720231(v=WS.10)'
---

RMS-fähige Anwendungen
======================

Wenn RMS-geschützte Inhalte erstellt oder eingesehen werden sollen, müssen die betreffenden Benutzer über eine RMS-fähige Anwendung verfügen, wie nachstehend beschrieben. Darüber hinaus müssen der RMS-Client installiert und die verwendeten Computer aktiviert sein. Weitere Informationen finden Sie nachstehend unter [RMS-Client](https://technet.microsoft.com/03294fa2-8350-430d-b4b0-03d5169937c2) und [RMS-Computeraktivierung](https://technet.microsoft.com/09a0d631-9860-477f-9d10-df61b3bfe125).

RMS-fähige Anwendungen ermöglichen den Autoren von Inhalten in Form von Veröffentlichungslizenzen das Zuweisen von Nutzungsrechten für von ihnen erstellte Dateien. Damit können die Autoren das Abrufen dieser Inhalte kontrollieren. RMS-fähige Anwendungen verarbeiten darüber hinaus auch verschlüsselte Daten und ermöglichen es Benutzern, solche Inhalte gemäß den in der Veröffentlichungslizenz festgelegten Berechtigungen abzurufen.

Entwickler können mit dem Software Development Kit (SDK) für RMS-Clients RMS-fähige Anwendungen erzeugen, die RMS-geschützte Inhalte lizenzieren, veröffentlichen und abrufen können. Es können RMS-fähige Anwendungen für Computer mit den Betriebssystemen Microsoft® Windows® 98 Second Edition oder später entwickelt werden.

Entwickler können mit dem Software Development Kit (SDK) für RMS-Clients auch RMS-fähige Serveranwendungen erstellen. Diese Anwendungen können Inhalte veröffentlichen, aber nicht abrufen.

Benutzer, die nicht über eine spezielle RMS-fähige Anwendung für das Abrufen RMS-geschützter Inhalte in E-Mail und auf Webseiten verfügen, können dies mit dem Add-On für die Rechteverwaltung für Microsoft® Internet Explorer tun. Beispielsweise können Kunden von Outlook Web Access (OWA) mit dem Add-On für die Rechteverwaltung für Internet Explorer RMS-geschützte E-Mail-Nachrichten abrufen.

Sie können das Add-On für die Rechteverwaltung für Internet Explorer von der [Microsoft-Website](http://go.microsoft.com/fwlink/?linkid=14450) (http://go.microsoft.com/fwlink/?LinkId=14450) herunterladen.

| ![](images/Cc720231.note(WS.10).gif)Hinweis                                                                                                                                       |
|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Wenn Sie das Add-On für die Rechteverwaltung für Internet Explorer mit Windows XP Service Pack 2 verwenden, kann die erweiterte Sicherheitskonfiguration zu Problemen bei der Anwendungskompatibilität führen. |

Wenn der URL für die Extranetverbindung aller Domänen innerhalb der Organisation in Internet Explorer nicht zu den lokalen Intranetsites hinzugefügt wird, erhalten Benutzer, die das Add-On für die Rechteverwaltung für Internet Explorer verwenden, wiederholt Meldungen, die sie auffordern, zu bestätigen, dass sie wirklich auf die Sites zugreifen möchten. Eine falsche Antwort auf diese Meldung kann dazu führen, dass der RMS-Client ein neues Rechtekontozertifikat für das Benutzerkonto ausstellt.

Um diese Sites innerhalb der gesamten Organisation korrekt einzurichten, müssen mit einem Skript die nötigen URLs in der Registrierung als Teil der lokalen Intranetzone eingetragen werden. Das lokale Intranet verfügt standardmäßig über eine so hohe Sicherheitsstufe, dass solche Meldungen blockiert werden.