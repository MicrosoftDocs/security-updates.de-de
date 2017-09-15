---
TOCTitle: 'Erstellen des RMS-Dienstkontos'
Title: 'Erstellen des RMS-Dienstkontos'
ms:assetid: '6eb38729-f0f0-431a-bc8c-17102cf175d8'
ms:contentKeyID: 18118894
ms:mtpsurl: 'https://technet.microsoft.com/de-de/library/Cc747546(v=WS.10)'
---

Erstellen des RMS-Dienstkontos
==============================

Während der Installation erstellt RMS die Sicherheitsgruppe **RMS Service Group (RMS-Dienstgruppe)** auf dem lokalen Computer und gewährt dieser die entsprechenden Berechtigungen für alle Ressourcen, die zur Ausführung von RMS erforderlich sind.

Wenn Sie RMS auf einem Server bereitstellen, legen Sie ein Benutzerkonto als RMS-Dienstkonto fest. Das von Ihnen festgelegte Konto wird der RMS-Dienstgruppe hinzugefügt. Dabei werden ihm die Berechtigungen dieser Gruppe erteilt. Bei Standardoperationen wird RMS für die meisten Zwecke unter dem RMS-Dienstkonto ausgeführt.

| ![](images/Cc747546.note(WS.10).gif)Hinweis                                          |
|-------------------------------------------------------------------------------------------------------------------|
| Das RMS-Dienstkonto darf nicht mit dem Domänenkonto identisch sein, das zum Installieren von RMS verwendet wurde. |

Aus Sicherheitsgründen wird dringend empfohlen, ein spezielles Benutzerkonto zu erstellen, das ausschließlich als Windows RMS-Dienstkonto verwendet wird. Diesem Konto sollten außerdem keine weiteren Berechtigungen erteilt werden.

| ![](images/Cc747546.Important(WS.10).gif)Wichtig                      |
|----------------------------------------------------------------------------------------------------|
| Sie sollten das spezielle Benutzerkonto vor der Installation und Bereitstellung von RMS erstellen. |

Weitere Informationen über die der RMS-Dienstgruppe erteilten Berechtigungen und die Konten, über die RMS ausgeführt wird, finden Sie unter „RMS-Sicherheitsmodell“ im Teil „Technische Referenz für RMS“ dieser Dokumentationssammlung.
