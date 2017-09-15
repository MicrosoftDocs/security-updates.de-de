---
TOCTitle: Aktivieren und Deaktivieren der Protokollierung
Title: Aktivieren und Deaktivieren der Protokollierung
ms:assetid: '50ccd827-2d39-41e7-a395-3d5f5836869b'
ms:contentKeyID: 18118836
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747565(v=WS.10)'
---

Aktivieren und Deaktivieren der Protokollierung
===============================================

Sie können die Protokollierung für den aktuellen Cluster oder Server auf der Seite **Protokollierungseinstellungen** aktivieren oder deaktivieren. Das Deaktivieren der Protokollierung verhindert, dass die RMS-Webdienste (Rights Management Services oder Dienste für die Rechteverwaltung) protokollierte Daten an die Warteschlange für Protokollierungsnachrichten senden. Außerdem wird auch der Protokollierungslistenerdienst beendet. Das Deaktivieren der Protokollierung mithilfe des Verwaltungsprogramms für die Dienste von Windows Server 2003 wird nicht unterstützt.

RMS-Protokolle werden mit Message Queuing an den Datenbankserver gesendet. Bei einer Unterbrechung der Verbindung zum Datenbankserver werden die Protokolle bis zur Wiederherstellung der Konnektivität von Message Queuing in einem lokalen Cache zwischengespeichert. Wenn Sie die Protokollierung zum ersten Mal aktivieren, sollten Sie sicherstellen, dass der Server mit RMS eine Verbindung zum Datenbankserver hat und der Datenbankdienst gestartet wurde. Wenn Sie SQL Server als Datenbankserver verwenden, können Sie überprüfen, ob die Protokolle in die Datenbank geschrieben werden, indem Sie folgende Schritte ausführen:

-   Wechseln Sie in SQL Server Enterprise Manager zur Protokollierungsdatenbank, erweitern Sie **Datenbanken**, und erweitern Sie dann die Datenbank, die die RMS-Protokollierungsdatenbank enthält.
-   Klicken Sie auf die Protokollierungsdatenbank, klicken Sie auf **Tabellen**, klicken Sie mit der rechten Maustaste auf **DRMS\_log\_master**, und klicken Sie dann auf **Tabelle öffnen – Alle Zeilen zurückgeben**. Wenn Protokolldateien erstellt werden, werden eine oder mehrere Protokolldateien angezeigt.
