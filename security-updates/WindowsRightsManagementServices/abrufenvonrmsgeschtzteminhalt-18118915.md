---
TOCTitle: 'Abrufen von RMS-geschütztem Inhalt'
Title: 'Abrufen von RMS-geschütztem Inhalt'
ms:assetid: '3cf6d64b-1187-433c-bbb2-c68069bc3c30'
ms:contentKeyID: 18118915
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc720251(v=WS.10)'
---

Abrufen von RMS-geschütztem Inhalt
==================================

Wenn Benutzer geschützte Inhalte abrufen, finden zwei für sie transparente Prozesse statt. Wenn der Benutzer das Dokument öffnet, ruft die RMS-fähige Anwendung zunächst eine Nutzungslizenz ab. Danach überprüft die RMS-fähige Anwendung die Nutzungslizenz, um festzustellen, ob dafür eine Sperrliste erforderlich ist und ob ein Zertifikat, das sich in der Vertrauenskette der Nutzungslizenz oder des Rechtekontozertifikats befindet, gesperrt wurde. Nachdem beide Prozesse abgeschlossen sind, gibt die RMS-fähige Anwendung den RMS-geschützten Inhalt wieder, sofern alle Rechte und Sperrungen dies zulassen.

Falls eine Sperrliste erforderlich ist, sucht die Anwendung nach einer lokalen, nicht abgelaufenen Kopie der Liste. Bei Bedarf ruft sie eine aktuelle Kopie der Sperrliste ab. Die Anwendung wendet dann alle im aktuellen Kontext relevanten Sperrbedingungen an.

Wenn keine Sperrbedingung den Zugriff auf die Inhalte blockiert, gibt die Anwendung die Inhalte wieder, und der Benutzer kann die ihm erteilten Rechte ausüben.

Sie können RMS für die Verarbeitung von Nutzungslizenzanforderungen von autorisierten externen Benutzern konfigurieren. Damit wird Benutzern die gemeinsame Verwendung geschützter Inhalte über das Internet ermöglicht.

Dieser Abschnitt enthält folgende Themen:

-   [Erwerb von Nutzungslizenzen](https://technet.microsoft.com/0b6cde34-418a-4dee-9d27-b65b93b535ac)
-   [Nutzungslizenzen und externe Benutzer](https://technet.microsoft.com/02db9bda-180e-438f-863d-26252083a471)
