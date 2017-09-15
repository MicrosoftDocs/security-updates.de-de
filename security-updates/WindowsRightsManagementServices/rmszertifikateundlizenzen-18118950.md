---
TOCTitle: 'RMS-Zertifikate und -Lizenzen'
Title: 'RMS-Zertifikate und -Lizenzen'
ms:assetid: '91916ecb-9e5d-49e8-ab65-ef2c56339b83'
ms:contentKeyID: 18118950
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747600(v=WS.10)'
---

RMS-Zertifikate und -Lizenzen
=============================

Die verschiedenen Komponenten einer RMS-Installation (Rights Management Services oder Dienste für die Rechteverwaltung) haben vertrauenswürdige Verbindungen, die durch eine Gruppe von Zertifikaten implementiert werden. Es gehört zu den Kernfunktionen der RMS-Technologie, die Gültigkeit dieser Zertifikate zu erzwingen. Jeder einzelne RMS-geschützte Inhalt wird mit einer Lizenz veröffentlicht, die seine Nutzungsrichtlinien festlegt, und jeder Benutzer, der diesen Inhalt abruft, erhält eine eindeutige Lizenz, mit der diese Nutzungsrichtlinien gelesen, interpretiert und erzwungen werden. In diesem Zusammenhang steht „Lizenz“ für einen bestimmten Zertifikattyp.

Um die Nutzungsrechte für RMS-geschützten Inhalt festzulegen, bedient sich RMS des XML-Vokabulars in Form der XrML-Sprache (eXtensible Rights Markup Language) Version 1.2.1. Weitere Informationen hierzu finden Sie unter „XrML“ weiter unten in diesem Thema.

Die in RMS verwendeten Zertifikate und Lizenzen sind untereinander hierarchisch verbunden, so dass RMS von einem bestimmten Zertifikat oder einer Lizenz aus über vertrauenswürdige Zertifikate bis zu einem vertrauenswürdigen Schlüsselpaar hin immer einer Kette folgen kann. Weitere Informationen hierzu finden Sie unter „[RMS-Vertrauenshierarchie](https://technet.microsoft.com/2d44182f-a653-4383-aba1-dade53f7cf9a)“ weiter unten in diesem Thema.

Dieser Abschnitt behandelt die folgenden Themen:

-   [RMS-Zertifikate und -Lizenzen – Zusammenfassung](https://technet.microsoft.com/637ccfca-318e-4346-85b5-0945b058fb9c)
-   [Server-Lizenzgeberzertifikate](https://technet.microsoft.com/0b35fbcd-25a9-4587-898d-9a30fd1d3c5b)
-   [Client-Lizenzgeberzertifikate](https://technet.microsoft.com/bfb36387-3e15-4cde-8b8f-482219569a64)
-   [RMS-Computerzertifikate](https://technet.microsoft.com/1841d53e-d01b-47c3-9d43-3805ceefed5a)
-   [Rechtekontozertifikate](https://technet.microsoft.com/2ff315cc-211d-4e6e-85e8-56867c2abd94)
-   [Veröffentlichungslizenzen](https://technet.microsoft.com/187228fc-370b-4e23-a53a-21bb296b84a1)
-   [Nutzungslizenzen](https://technet.microsoft.com/6e609db3-49b3-4cac-a34c-8a96da627067)
