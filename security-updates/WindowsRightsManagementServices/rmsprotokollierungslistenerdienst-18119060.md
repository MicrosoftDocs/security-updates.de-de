---
TOCTitle: 'RMS-Protokollierungslistenerdienst'
Title: 'RMS-Protokollierungslistenerdienst'
ms:assetid: 'e81ea57d-1a7d-4c02-abfc-dbc1597e176b'
ms:contentKeyID: 18119060
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747709(v=WS.10)'
---

RMS-Protokollierungslistenerdienst
==================================

Der Protokollierungslistenerdienst wird von RMS-Setup installiert. Er wird sowohl auf den Stammzertifizierungs- als auch den Stammlizenzierungsservern ausgeführt. Jeder RMS-Webdienst protokolliert alle Anforderungen und Antworten, die er sendet und empfängt, und überträgt die Daten anschließend mit Message Queuing an die Warteschlange für Protokollierungsnachrichten. Anschließend überträgt der Protokollierungslistenerdienst diese Daten aus der Nachrichtenwarteschlange in die Protokollierungsdatenbank für den Cluster.

Sie können die Protokollierung über die Verwaltungswebsite aktivieren und deaktivieren. Damit beenden die Webdienste den Protokollierungsvorgang, und der Protokollierungslistenerdienst wird deaktiviert.
