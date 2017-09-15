---
TOCTitle: Planen der Wiederherstellung des Systems
Title: Planen der Wiederherstellung des Systems
ms:assetid: 'a7779ffd-7a94-4e13-b846-0ffd00608e02'
ms:contentKeyID: 18118982
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747718(v=WS.10)'
---

Planen der Wiederherstellung des Systems
========================================

Ein System kann aus vielerlei unvorhersehbaren Gründen versagen: Hardwarefehler, höhere Gewalt, Überspannung, Softwarefehler, usw. Eine erfolgreiche Bereitstellung muss einen Plan für das schnelle Wiederherstellen des Systems im Falle eines Versagens umfassen. Bei einem RMS-System ist die wichtigste Vorbedingung zur Wahrung der RMS-Funktionalität eine regelmäßige Sicherung des privaten Serverschlüssels und der RMS-Datenbanken, insbesondere der Konfigurationsdatenbank. Damit werden die Vorlagen für Benutzerrechterichtlinien, die Schlüssel und andere Daten erhalten, die für den Zugriff auf frühere Lizenzen und veröffentlichte Inhalte erforderlich sind. Wenn die bestehende RMS-Instanz versagt, kann RMS auf anderen Servern installiert und anschließend durch Angabe der Konfigurationsdatenbank der Sicherung als zu verwendende Datenbank neu bereitgestellt werden. Die neue Sicherungsinstallation ist mit der Version der vorherigen Installation zum Zeitpunkt der letzten Sicherung identisch.

Dieser Abschnitt behandelt die folgenden Themen:

-   [Vorbereitungen zur Systemwiederherstellung](https://technet.microsoft.com/885c047f-1e3b-4bf5-8248-3a4505759cbb)
-   [Systemsicherungen für RMS](https://technet.microsoft.com/c29894da-ee00-428c-8d48-80d8e5a83678)
-   [Sichern und Wiederherstellen des Systems](https://technet.microsoft.com/c11f3ac1-e512-402b-bf13-9ff21f5fe745)
-   [Sichern und Wiederherstellen der Vorlagen für Benutzerrechterichtlinien](https://technet.microsoft.com/a6ed3328-4128-45e8-9236-3de484b460de)
