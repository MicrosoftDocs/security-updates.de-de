---
TOCTitle: Definieren von Vertrauensrichtlinien
Title: Definieren von Vertrauensrichtlinien
ms:assetid: 'e8d78300-4b26-4f15-9e4f-5ae9eb827ef9'
ms:contentKeyID: 18119067
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747711(v=WS.10)'
---

Definieren von Vertrauensrichtlinien
====================================

Sie können vertrauenswürdige Benutzer- und Veröffentlichungsdomänen folgendermaßen definieren:

-   **Vertrauenswürdige Benutzerdomänen**. Wenn Sie eine Benutzerdomäne hinzufügen, kann RMS (Rights Management Services oder Dienste für die Rechteverwaltung) Anforderungen für Nutzungslizenzen von Benutzern verarbeiten, deren Rechtekontozertifikate von einer RMS-Installation in einer anderen Active Directory-Gesamtstruktur, d. h. in einem anderen Stammzertifizierungscluster, ausgestellt wurden. Sie können eine vertrauenswürdige Benutzerdomäne durch Importieren des Server-Lizenzgeberzertifikats der vertrauenswürdigen Installation hinzufügen.
-   **Vertrauenswürdige Veröffentlichungsdomänen**. Durch Hinzufügen einer Veröffentlichungsdomäne wird einem Server mit RMS das Ausstellen von Nutzungslizenzen für Veröffentlichungslizenzen ermöglicht, die von einem anderen Server mit RMS ausgestellt wurden. Sie können eine vertrauenswürdige Veröffentlichungsdomäne durch Importieren des Server-Lizenzgeberzertifikats und des privaten Schlüssels des Servers hinzufügen, dem vertraut werden soll.

Weitere Informationen hierzu finden Sie nachstehend unter [Hinzufügen und Entfernen von vertrauenswürdigen Benutzerdomänen](https://technet.microsoft.com/7c440b15-01c4-49f1-b43c-00f67f3388c1) und [Hinzufügen und Entfernen von vertrauenswürdigen Veröffentlichungsdomänen](https://technet.microsoft.com/d87b502d-5497-4ccd-badf-f6807d587cee). Eine in logische Schritte unterteilte Anleitung hierzu finden Sie nachstehend unter [Einrichten von Vertrauensrichtlinien](https://technet.microsoft.com/6c2be3c2-1837-4de4-a72e-3ba3eec3321d).