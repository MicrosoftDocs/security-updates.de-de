---
TOCTitle: 'RMS-Protokollierungsdatenbank'
Title: 'RMS-Protokollierungsdatenbank'
ms:assetid: '8ba147f3-16e4-4d9a-ac8f-f05ba2ba11bb'
ms:contentKeyID: 18118929
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747669(v=WS.10)'
---

RMS-Protokollierungsdatenbank
=============================

Für jeden Stammzertifizierungs- oder Lizenzierungscluster installiert RMS-Setup eine Protokollierungsdatenbank in derselben Datenbankserverinstanz, die auch die Konfigurationsdatenbank hostet. Darüber hinaus erstellt Setup eine private Nachrichtenwarteschlange zur Protokollierung in Message Queuing. Der Protokollierungslistenerdienst überträgt die Daten aus dieser Warteschlange in die Protokollierungsdatenbank.

Die RMS Service Group (RMS-Dienstgruppe) hat Berechtigungen vom Typ „Ausführen“ für die gespeicherten Verfahren, die sich in der Protokollierungsdatenbank befinden.

Da der Protokollierungslistenerdienst große Datenmengen zur Protokollierungsdatenbank sendet, können Administratoren Filter erstellen, damit in der Datenbank nur die für die jeweiligen Organisationen erforderlichen Informationen gespeichert werden.
