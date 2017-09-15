---
TOCTitle: Überwachen von Message Queuing
Title: Überwachen von Message Queuing
ms:assetid: 'a7109399-3a84-4681-874b-f6ea1646b0a0'
ms:contentKeyID: 18118986
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747716(v=WS.10)'
---

Überwachen von Message Queuing
==============================

Die RMS-Protokollierung sendet Ereignisse mithilfe von Message Queuing (MSMQ) an die Protokollierungsdatenbank. Jeder RMS-Frontendserver sendet Nachrichten an den Message Queuing-Dienst. Der Protokollierungslistenerdienst auf jedem Frontendserver ruft die Protokollierungsnachrichten aus der Message Queuing-Warteschlange ab und schreibt sie in die Protokollierungsdatenbank. Ist die Protokollierungsdatenbank oder der Datenbankserver nicht verfügbar oder wird der Protokollierungslistenerdienst beendet, speichert Message Queuing die Nachrichten in der Warteschlange. Wenn die Protokollierungsdatenbank oder der Datenbankserver heruntergefahren werden soll, sollten Sie zuerst den Protokollierungslistenerdienst auf jedem Frontendserver herunterfahren. Nach dem Neustarten der Datenbank oder des Datenbankservers sollten Sie ihn auf jedem Frontendserver neu starten.

Wenn die Datenbank nicht mehr verfügbar ist, der Protokollierungslistenerdienst aber weiterhin ausgeführt wird, kann der Protokollierungslistenerdienst keine Protokollierungsnachrichten in die Datenbank schreiben. Der Protokollierungslistenerdienst verschiebt die Nachrichten zunächst in eine Message Queuing-Warteschlange für unzustellbare Nachrichten, bis die Datenbank wieder verfügbar ist. Zu diesem Zeitpunkt werden neue Protokollierungsnachrichten in die Datenbank geschrieben. Die Nachrichten in der Warteschlange für unzustellbare Nachrichten werden nicht automatisch in die Protokollierungsdatenbank geschrieben. Führen Sie die folgenden Schritte aus, um die Nachrichten in der Warteschlange für unzustellbare Nachrichten anzuzeigen und zu löschen:

1.  Öffnen Sie das Snap-In **Computerverwaltung** von Microsoft Management Console (MMC). Klicken Sie dazu auf **Start**, zeigen Sie dann auf **Alle Programme** und **Verwaltung**, und klicken Sie dann auf Computerverwaltung.
2.  Klicken Sie in der Konsolenstruktur auf Dienste und Anwendungen, klicken Sie dann auf Message Queuing und anschließend auf Private Warteschlangen.
3.  Jetzt werden zwei Warteschlangen angezeigt. Ihre Namen beginnen beide mit „**drms\_logging**“, gefolgt vom Namen des Clusters. Eine der Warteschlangen heißt „**drms\_logging\_***&lt;Ihr Clustername&gt;*\_**deadletter**“. Dabei handelt es sich um die Warteschlange für unzustellbare Nachrichten. Klicken Sie auf den Warteschlangennamen und dann auf die Warteschlange Warteschlangennachrichten.
4.  Doppelkicken Sie auf jede Nachricht, um ihre Eigenschaften anzuzeigen.
5.  Zum Löschen der Warteschlange klicken Sie mit der rechten Maustaste auf die Warteschlange **Warteschlangennachrichten**, wählen Sie **Alle Aufgaben** aus, und klicken Sie auf **Leeren**.

In der Standardkonfiguration speichert Message Queuing alle Nachrichten in der Warteschlange, bis der maximal auf dem Server verfügbare freie Speicherplatz ausgefüllt ist. Wenn Message Queuing den gesamten verfügbaren Festplattenspeicherplatz verwendet, kann der RMS-Server keine Dienstanforderungen von Clients mehr erfüllen. Führen Sie die folgenden Schritte aus, um dies zu verhindern und den verfügbaren Speicherplatz einzuschränken, den Message Queuing zum Aufnehmen von Nachrichten in der Warteschlange verwenden kann:

1.  Öffnen Sie das Snap-In Computerverwaltung von Microsoft Management Console (MMC). Klicken Sie dazu auf Start, zeigen Sie dann auf Alle Programme und Verwaltung, und klicken Sie dann auf Computerverwaltung.
2.  Klicken Sie in der Konsolenstruktur auf Dienste und Anwendungen, klicken Sie dann auf Message Queuing und anschließend auf Private Warteschlangen.
3.  Jetzt werden zwei Warteschlangen angezeigt. Der Name beider Warteschlangen beginnt mit „drms\_logging“. Führen Sie für jede Warteschlange die folgenden Schritte aus:
    -   Klicken Sie auf Eigenschaften.
    -   Aktivieren Sie das Kontrollkästchen Nachrichtenspeicher beschränken auf (in KB), und geben Sie dann die Gesamtgröße aller Warteschlangennachrichten, die in der Warteschlange gespeichert werden können, in Kilobyte ein.

Wenn eine Warteschlange voll ist, werden die von RMS eingehenden Nachrichten bei ihrer Ankunft gelöscht, und die folgende Ereignisnachricht mit der Ereignis-ID 48 wird an das Systemereignisprotokoll gesendet:

„Fehler beim Senden des Eigenschaftenbehälters an Message Queuing.“

Die Systemüberwachungstools sollten so konfiguriert werden, dass Sie beim Auftreten dieses Ereignisses benachrichtigt werden. Das Ereignis weist auf ein Problem in der Protokollierungsdatenbank hin.
