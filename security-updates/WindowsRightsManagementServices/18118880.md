---
TOCTitle: 'RMS-Sperrung'
Title: 'RMS-Sperrung'
ms:assetid: '72689f90-f3c5-4b61-94ea-d825f3199b3b'
ms:contentKeyID: 18118880
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747622(v=WS.10)'
---

RMS-Sperrung
============

Eine Sperrung ist ein Mechanismus, mit dem Anmeldeinformationen, die bereits erteilt wurden, wie z. B. in einem Zertifikat oder einer Lizenz, gesperrt werden. Der Hauptzweck einer Sperrung ist es, Entitäten, die nicht mehr vertrauenswürdig sind, von der Teilnahme an einem RMS-System auszuschließen. Eine Sperrung kann beispielsweise in folgenden Szenarien angewendet werden:

-   Um zu verhindern, dass Inhalt abgerufen wird, wenn ein Prinzipal oder eine Identität, der oder die sich in der Vertrauenskette befindet, gefährdet ist, wie es z. B. der Fall ist, wenn eine Person eine Organisation verlässt und danach nicht länger dazu berechtigt sein soll, RMS-geschützten Inhalt abzurufen.
-   Um zu verhindern, dass eine bestimmte RMS-fähige Anwendung einen bestimmten Inhalt öffnet, wenn diese Anwendung nicht mehr vertrauenswürdig ist.
-   Um zu verhindern, dass bestimmter Inhalt, der fälschlicherweise bereits verteilt und zum Abrufen lizenziert wurde, weiterhin abgerufen werden kann.

Die Sperrung ist auf dem Client funktionsfähig und hindert Benutzer am Abrufen bestimmter Inhalte, auch wenn dafür bereits eine Nutzungslizenz ausgestellt wurde. Wenn die Sperrung aktiviert ist, wird sie jedes Mal wirksam, wenn ein Benutzer versucht, geschützten Inhalt abzurufen, und zwar unabhängig davon, ob der Benutzer eine lokal gespeicherte Kopie der Nutzungslizenz hat oder zum Zeitpunkt des Abrufens eine neue Nutzungslizenz vom RMS-Server anfordert.

Dieser Abschnitt stellt einen Überblick über die Sperrung bereit. Weitere Informationen zum Verwenden der RMS-Sperrung finden Sie unter „Verwalten der Sperrung“ im Abschnitt "Betreiben eines RMS-Servers" in dieser Dokumentationssammlung.

Dieser Abschnitt behandelt die folgenden Themen:

-   [Funktionsweise der RMS-Sperrung](https://technet.microsoft.com/469e3938-a59b-4c92-9779-ead64e724d00)
-   [RMS-Sperrlisten](https://technet.microsoft.com/688d4dfa-c928-4b2f-8116-2f9e87d2b6f7)
-   [Sperrung in Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/287c5b92-fcb5-4295-9c2b-4e37e643beb2)
-   [Sperrung und nicht verbundene Autoren](https://technet.microsoft.com/a9cf0541-9101-4e90-9c56-7c1b9a8deca6)