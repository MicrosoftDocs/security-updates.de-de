---
TOCTitle: Verwalten von Ausschlussrichtlinien
Title: Verwalten von Ausschlussrichtlinien
ms:assetid: 'ee31e099-e095-4648-95da-0009fbeb48cb'
ms:contentKeyID: 18119074
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747730(v=WS.10)'
---

Verwalten von Ausschlussrichtlinien
===================================

Sie können serverseitige Ausschlussrichtlinien implementieren, um Zertifikat- und Lizenzanforderungen abzulehnen, die auf dem Rechte-Kontozertifikat oder der Lockbox-Version basieren. Ausschlussrichtlinien lehnen neue Zertifikat- und Lizenzanforderungen von unsicheren Prinzipalen ab. Im Gegensatz zur Sperrung werden die Prinzipale durch Ausschlussrichtlinien jedoch nicht annulliert. Administratoren können auch potenziell schädliche oder unsichere Anwendungen ausschließen, damit diese RMS-geschützte Inhalte nicht entschlüsseln können. Darüber hinaus können Administratoren bestimmte Versionen des Betriebssystems Windows ausschließen und so das Abrufen von RMS-geschützten Inhalten auf Clientcomputern unter diesen Versionen des Betriebssystems Windows verhindern.

Beim Ausschließen einer Entität wird diese in der Ausschlussliste der vom Server mit RMS (Rights Management Services oder Dienste für die Rechteverwaltung) erstellten Nutzungslizenzen angegeben. Wenn Sie nach einem gewissen Zeitraum eine zuvor in einer Ausschlussrichtlinie eingeschlossene Entität löschen möchten, können Sie sie auf der Seite Ausschlussrichtlinien der Verwaltungswebsite löschen. Damit wird die Entität aus der Ausschlussliste entfernt. Neue Zertifizierungs- oder Lizenzierungsanforderungen sehen diese Entität nicht als ausgeschlossen an.

Sofern Sie eine Entität nicht versehentlich ausgeschlossen haben, sollten Sie diese erst aus einer Ausschlussrichtlinie entfernen, wenn Sie sicher sind, dass alle vor Inkrafttreten der Ausschlussrichtlinie ausgestellten Zertifikate abgelaufen sind. Andernfalls ermöglichen sowohl die alten als auch die neuen Zertifikate gegen den Wunsch der Organisation das Entschlüsseln von Inhalten.

Dieses Thema enthält Informationen zum Verwalten von Ausschlussrichtlinien. Sie finden eine in logische Schritte unterteilte Anleitung zum Ausschließen von Entitäten nachstehend unter [Aktivieren von Ausschlussrichtlinien](https://technet.microsoft.com/bbb1ce50-bc11-41cf-b75b-a6756141908f).

Dieser Abschnitt behandelt die folgenden Themen:

-   [Ausschließen von Lockbox-Versionen](https://technet.microsoft.com/e287f026-aab2-43ab-93bc-48087da82f36)
-   [Ausschließen von Rechtekontozertifikaten](https://technet.microsoft.com/cba5e901-942c-4d06-9865-e6c4648c95e6)
-   [Ausschließen von Windows-Versionen](https://technet.microsoft.com/8b8a184d-ac0e-4a43-822c-d2fae2faf484)
-   [Ausschließen von Anwendungen](https://technet.microsoft.com/b68ae4b2-b9ba-44ae-90cb-c88df600ec86)