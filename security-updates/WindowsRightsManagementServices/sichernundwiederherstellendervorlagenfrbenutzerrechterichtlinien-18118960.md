---
TOCTitle: Sichern und Wiederherstellen der Vorlagen für Benutzerrechterichtlinien
Title: Sichern und Wiederherstellen der Vorlagen für Benutzerrechterichtlinien
ms:assetid: 'a6ed3328-4128-45e8-9236-3de484b460de'
ms:contentKeyID: 18118960
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747625(v=WS.10)'
---

Sichern und Wiederherstellen der Vorlagen für Benutzerrechterichtlinien
=======================================================================

Sie können wichtige Vorlagen für Benutzerrechterichtlinien schützen, indem Sie die Vorlagendaten in der Konfigurationsdatei in regelmäßigen Abständen auf Medien sichern und die Medien an einem sicheren Ort aufbewahren. Im Falle eines Systemausfalls können Sie die Vorlagen von der Sicherungskopie wiederherstellen.

Führen Sie eine der folgenden Aktionen aus:

-   Sichern Sie die gesamte Konfigurationsdatenbank, einschließlich der Vorlagendaten für Benutzerrechterichtlinien. Weitere Informationen zum Sichern einer SQL Server-Datenbank finden Sie in der SQL Server-Dokumentation.
    – Oder –
-   Sichern Sie nur die in der Konfigurationsdatenbank enthaltenen Vorlagendaten. Dazu können Sie die GUID- und TemplateData-Informationen aus der Tabelle namens DRMS\_RightsTemplate in eine neue Textdatei exportieren. Weitere Informationen zum Exportieren von Daten aus einer SQL Server-Datenbank finden Sie in der SQL Server-Dokumentation.

Wenn Sie die in der Konfigurationsdatei enthaltenen Vorlagendaten für Benutzerrechterichtlinien wiederherstellen müssen, können Sie die GUID- und TemplateData-Informationen aus der Tabelle namens DRMS\_RightsTemplate in der Sicherungskopie der Konfigurationsdatenbank extrahieren oder die Daten einfach aus der Textdatei importieren. Weitere Informationen zum Durchführen dieser Aufgaben finden Sie in der SQL Server-Dokumentation.

| ![](images/Cc747625.note(WS.10).gif)Hinweis                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------|
| Wenden Sie sich an den SQL Server-Administrator, um einen Plan zum Sichern der Vorlagen für Benutzerrechterichtlinien zu entwickeln. |
