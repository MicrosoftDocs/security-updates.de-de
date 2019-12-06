---
TOCTitle: 'MS07-SEP'
Title: Microsoft Security Bulletin Summary für September 2007
ms:assetid: 'ms07-sep'
ms:contentKeyID: 61225054
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms07-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für September 2007
======================================================

Veröffentlicht: Dienstag, 11. September 2007 | Aktualisiert: Mittwoch, 12. September 2007

**Version:** 1.1

In diesem Bulletin Summary sind die im September 2007 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für September 2007 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 6. September 2007 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification.](https://technet.microsoft.com/security/bulletin/advance)

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 12. September 2007 um 20:00 Uhr (MEZ) führt Microsoft einen englischsprachigen Webcast durch, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im September.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344690&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (1)
------------

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-051                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in Microsoft Agent kann Remotecodeausführung ermöglichen (938827)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-051.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Kurzzusammenfassung**                    | Dieses kritische Sicherheitsupdate behebt eine von einem Privatanwender gemeldete Sicherheitsanfälligkeit. In Microsoft Agent liegt eine Sicherheitsanfälligkeit vor, die aufgrund der Art der Handhabung speziell gestalteter URLs eine Remotecodeausführung ermöglichen kann. Die Sicherheitsanfälligkeit kann einem Angreifer ermöglichen, Code von einem Remotestandort aus auf dem betroffenen System auszuführen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Betroffene Software**                    | **Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

Hoch (3)
--------

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-052                                                                                                                                                                                                                                                                                                                                                                               |
|--------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in Crystal Reports für Visual Studio kann Remotecodeausführung ermöglichen (941522)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-052.mspx)                                                                                                                                                                                                                     |
| **Kurzzusammenfassung**                    | Dieses wichtige Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete RPT-Datei öffnet. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                    |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                               |
| **Erkennung**                              | Microsoft Baseline Security Analyzer und das Enterprise Scan Tool können erkennen, ob Ihr Computersystem dieses Update erfordert. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                        |
| **Betroffene Software**                    | **Visual Studio.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                       |
<p></br></p>

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-053                                                                                                                                                                                                                                                                                                                                                           |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in Windows Services for UNIX kann Erhöhung von Berechtigungen ermöglichen (939778)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-053.mspx)                                                                                                                                                                                                  |
| **Kurzzusammenfassung**                    | Dieses wichtige Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit. Es besteht eine Sicherheitsanfälligkeit in Windows Services for UNIX 3.0, Windows Services for UNIX 3.5 und im Subsystem für UNIX-basierte Anwendungen, in denen die Ausführung bestimmter binärer setuid-Dateien einem Angreifer ermöglichen kann, eine Erhöhung von Berechtigungen zu erreichen. |
| **Bewertung des maximalen Schweregrads**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                |
| **Auswirkung der Sicherheitsanfälligkeit** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                    |
| **Erkennung**                              | Microsoft Baseline Security Analyzer und das Enterprise Scan Tool können erkennen, ob Ihr Computersystem dieses Update erfordert. Das Update erfordert einen Neustart.                                                                                                                                                                                                                         |
| **Betroffene Software**                    | **Windows Services for UNIX, Subsystem für UNIX-basierte Anwendungen.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                              |
<p></br></p>

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|--------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in MSN Messenger und Windows Live Messenger kann Remotecodeausführung ermöglichen (942099)**](https://go.microsoft.com/fwlink/?linkid=100148)                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Kurzzusammenfassung**                    | Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in MSN Messenger und Windows Live Messenger. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Einladung zu einem Webcam- oder Video-Chat von einem Angreifer akzeptiert. Wenn ein Angreifer diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann er vollständige Kontrolle über das betroffene System erlangen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Erkennung**                              | Diese Produkte stellen integrierte Mechanismen zur automatischen Erkennung und Bereitstellung der Updates bereit. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Betroffene Software**                    | **MSN Messenger, Windows Live Messenger.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

Betroffene Software und Downloadadressen
----------------------------------------

**Wie verwende ich diese Tabelle?**  

In dieser Tabelle finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Sie sollten jedes aufgeführte Softwareprogramm und jede Komponente überprüfen, um zu sehen, ob Sicherheitsupdates erforderlich sind. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Auswirkung der Sicherheitsanfälligkeit aufgelistet und mit einem Softwareupdate verlinkt.

**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.

**Betroffene Software und Downloadadressen**

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
<th style="border:1px solid black;" >
Details
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS07-051**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-051.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-052**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-052.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-053**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-053.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-054**](https://go.microsoft.com/fwlink/?linkid=100148)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Windows-Betriebssystem:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=7cd248ed-d154-4dce-89ef-ceefd2700965)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Betroffene Systemkomponenten des Windows-Betriebssystems:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Services for UNIX 3.0 unter Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277&amp;displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Services for UNIX 3.5 unter Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663&amp;displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Services for UNIX 3.0 unter Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277&amp;displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Services for UNIX 3.5 unter Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663&amp;displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Services for UNIX 3.0 unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=557f89fc-c5d9-4405-9007-1654abf92277)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Services for UNIX 3.5 unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=70ae23c2-3ae8-4ea6-ba8d-8ac7e4f82663)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Subsystem für UNIX-basierte Anwendungen unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8ab5cc43-0b9c-45eb-aa51-47568ab6ce3f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Subsystem für UNIX-basierte Anwendungen unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=1d21e3e8-b5f6-4044-9db6-054af836492b)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Subsystem für UNIX-basierte Anwendungen unter Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=4d52e4f4-2888-42df-8163-85c648e65b29)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Subsystem für UNIX-basierte Anwendungen unter Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=4be667cc-c239-480b-a9a0-939bcd27f0de)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Entwicklungstools und Plattformen
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2002 Service Pack 1  
(KB937057)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c41d8159-b42f-4d06-a797-e510494976ee) **<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio .NET 2003  
(KB937058)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d612ad41-5a0d-4e13-99ea-d6a5589786d6) **<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio .NET 2003 Service Pack 1  
(KB937059)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=69d2219f-ce82-46a5-8aec-072bd4bb955e&displaylang=de) **<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visual Studio 2005  
(KB937060)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=21073cc2-919c-40df-8ebb-aa3db06050d2) **<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Visual Studio 2005 Service Pack 1  
(KB937061)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=967d43c8-efba-4221-beb0-981e7deef33a) **<sup>[2]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Weitere betroffene Software:
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 unter Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45) **<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 unter Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cf49c56c-8b3e-4eae-9904-9505f47bed45) **<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 6.2 unter Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista und Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc) **<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 7.0 unter Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista und Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc) **<sup>[3]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
MSN Messenger 7.5 unter Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista und Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc) **<sup>[3]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
MSN Messenger 8.0 unter Windows XP Service Pack 2, Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 Service Pack 1, Windows Server 2003 Service Pack 2, Windows Server 2003 x64 Edition, Windows Server 2003 x64 Edition Service Pack 2, Windows Vista und Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d78f2ff1-79ea-4066-8ba0-ddbed94864fc) **<sup>[3]</sup>**
</td>
</tr>
</table>
 
**Hinweise**

**[1]** Für dieses Betriebssystem steht ein Sicherheitsupdate zur Verfügung. In der Tabelle finden Sie weitere Informationen zum entsprechenden Security Bulletin für die betroffene Software oder Komponente.

**[2]** Nicht alle Editionen dieser Version von Visual Studio sind betroffen. In dem entsprechenden Security Bulletin finden Sie eine Liste betroffener Editionen.

**[3]** Für diese Software steht auch eine Option zur Verfügung, ein Online-Upgrade des MSN Messenger- bzw. Windows Live Messenger Service durchzuführen. Weitere Informationen finden Sie im entsprechenden Security Bulletin.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch im [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](https://office.microsoft.com/de-de/officeupdate/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. und können am einfachsten durch eine Suche nach dem Begriff „security\_patch“ oder „security\_update“ ermittelt werden. Außerdem können Sicherheitsupdates vom Windows Update-Katalog heruntergeladen werden. Weitere Informationen zum Windows Update-Katalog finden Sie im [Microsoft Knowledge Base-Artikel 323166](https://support.microsoft.com/kb/323166).

**Anleitungen zur Erkennung und Bereitstellung:**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool und Enterprise Update Scan Tool (EST). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](https://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer und** **Enterprise** **Update Scan Tool**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

Wenn MBSA 1.2.1 die Erkennung für ein bestimmtes Sicherheitsupdate nicht unterstützen kann, veröffentlicht Microsoft für dieses bestimmte Sicherheitsupdate eine Version des Enterprise Update Scan Tools (EST). Weitere Informationen zu EST finden Sie auf der Website [Enterprise Update Scan Tool](https://support.microsoft.com/default.aspx?id=894193).

**Hinweis:** Nach dem 9. Oktober 2007 wird die von MBSA 1.2.1 verwendete Datei MSSecure.XML nicht mehr aktualisiert. Nach diesem Datum werden keine neuen Sicherheitsupdates für die von MBSA 1.2.1 verwendete Datei MSSecure.XML erstellt und keine neuen Versionen des Enterprise Scan Tools veröffentlicht. Weitere Informationen dazu finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie auf der Website [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection Tool, um eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates bereitzustellen. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Für diesen Monat:

-   Microsoft hat keine **nicht sicherheitsrelevanten** Updates mit hoher Priorität auf Microsoft Update (MU) und Windows Server Update Services (WSUS) veröffentlicht.
-   Microsoft hat keine **nicht sicherheitsrelevanten** Updates mit hoher Priorität für Windows auf Windows-Update (WU) veröffentlicht.

Diese Informationen gelten **nur** für wichtige, **nicht sicherheitsrelevante** Updates auf Microsoft Update, Windows Update und Windows Server Update Services, die an demselben Tag wie das Security Bulletin Summary veröffentlicht wurden. Es werden **keine** Informationen zu **nicht sicherheitsrelevanten** Updates bereitgestellt, die an anderen Tagen veröffentlicht werden.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Patchverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar und können am einfachsten durch eine Schlüsselwortsuche nach dem Begriff „security\_patch“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Auf der Website [IT Pro Security Community](https://go.microsoft.com/fwlink/?linkid=21164) erfahren Sie, wie Sie die Sicherheit erhöhen und die IT-Infrastruktur optimieren können. Sie haben zudem die Möglichkeit sich mit anderen IT-Fachleuten über Sicherheitsthemen auszutauschen.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Dem Vulnerability Research-Team von [Assurent Secure Technologies](https://www.assurent.com/) für den Hinweis auf ein in [MS07-051](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-051.mspx) beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in [MS07-051](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-051.mspx) beschriebenes Problem.
-   Einem anonymen Forscher, der mit [iDefense VCP](https://labs.idefense.com/) zusammenarbeitet, für den Hinweis auf ein in [MS07-051](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-051.mspx) beschriebenes Problem.
-   Brian A. Reiter von WolfeReiter für die Zusammenarbeit mit uns an einem in [MS07-053](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-053.mspx) beschriebenen Problem.
-   Woo Shi von [team 509](https://www.team509.com/) für den Hinweis auf ein in [MS07-054](https://go.microsoft.com/fwlink/?linkid=100148) beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (11. September 2007): Bulletin Summary veröffentlicht.
-   V1.1 (12. September 2007): Die Neustartanforderung wurde umformuliert und für MS07-054 wurden Downloadlinks hinzugefügt.

*Built at 2014-04-18T01:50:00Z-07:00*
