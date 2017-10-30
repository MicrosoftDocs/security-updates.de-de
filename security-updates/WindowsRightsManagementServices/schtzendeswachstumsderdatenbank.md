---
TOCTitle: Schätzen des Wachstums der Datenbank
Title: Schätzen des Wachstums der Datenbank
ms:assetid: '87652cc2-b886-4797-8d40-356669768089'
ms:contentKeyID: 18118924
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747585(v=WS.10)'
---

Schätzen des Wachstums der Datenbank
====================================

Beim Ermitteln des erforderlichen Speicherplatzes für die RMS-Datenbanken sollte eine Mindestkapazität von 10 Megabyte (MB) eingeplant und pro 500 Benutzer jeweils ein weiteres MB bereitgestellt werden. Die Protokollierungsdatenbank kann auf einem anderen Datenbankserver als die Konfigurationsdatenbank gespeichert werden.

Wenn Sie die Protokollfunktion von RMS verwenden, muss für die Protokollierungsdatenbank ein Wachstum von je 1 MB pro Benutzer während der ersten Benutzerzertifizierungsphase möglich sein, wenn häufig protokolliert wird. Wenn beispielsweise RMS für 1.000 Benutzer bereitgestellt werden soll, dann wird die Protokollierungsdatenbank auf 1 Gigabyte (GB) anwachsen, wenn die Benutzer einzeln über den RMS-Zertifizierungsserver aktiviert und zertifiziert werden. Im Standardbetrieb wird die Protokollierungsdatenbank üblicherweise um etwa 200 Kilobyte (KB) pro Benutzer und Tag anwachsen. Sollte die Implementierung schrittweise erfolgen, müssen Sie für jeden Benutzer, der dem System hinzugefügt wird, ein weiteres MB einplanen.