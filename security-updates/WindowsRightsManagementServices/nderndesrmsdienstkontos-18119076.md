---
TOCTitle: 'Ändern des RMS-Dienstkontos'
Title: 'Ändern des RMS-Dienstkontos'
ms:assetid: 'f257d66d-b823-41e4-bcb7-7c90eb295238'
ms:contentKeyID: 18119076
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747736(v=WS.10)'
---

Ändern des RMS-Dienstkontos
===========================

Während der Installation erstellt RMS (Rights Management Services oder Dienste für die Rechteverwaltung) die RMS Service Group (RMS-Dienstgruppe) auf dem lokalen Computer und erteilt ihr die entsprechenden Berechtigungen an allen Ressourcen, die zum Betrieb von RMS erforderlich sind. Wenn Sie RMS auf einem Server bereitstellen, definieren Sie das RMS-Dienstkonto mithilfe eines Domänenkontos. Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS verwendet wurde. Das Konto wird RMS Service Group als Mitglied hinzugefügt. Dabei werden ihm die Berechtigungen dieser Gruppe erteilt. Bei Standardoperationen wird RMS unter dem RMS-Dienstkonto ausgeführt.

Sie können das RMS-Dienstkonto jederzeit ändern. Dabei wird das zuvor angegebene Konto automatisch aus der RMS Service Group entfernt, und das neue Konto wird Mitglied bei dieser.

| ![](images/Cc747736.Important(WS.10).gif)Wichtig                                                                                                                                                   |
|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Aus Sicherheitsgründen sollten Sie unbedingt ein spezielles Benutzerkonto erstellen, das ausschließlich als Windows RMS-Dienstkonto verwendet wird. Diesem Konto sollten außerdem keine weiteren Berechtigungen erteilt werden. |

| ![](images/Cc747736.note(WS.10).gif)Hinweis                                                             |
|--------------------------------------------------------------------------------------------------------------------------------------|
| Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS mit Service Pack 1 verwendet wurde. |
