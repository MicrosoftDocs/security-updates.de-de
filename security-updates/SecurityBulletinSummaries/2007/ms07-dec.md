---
TOCTitle: 'MS07-DEZ'
Title: Microsoft Security Bulletin Summary für Dezember 2007
ms:assetid: 'ms07-dez'
ms:contentKeyID: 61225045
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms07-dez(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Dezember 2007
=====================================================

Veröffentlicht: Dienstag, 11. Dezember 2007 | Aktualisiert: Mittwoch, 16. Juli 2008

**Version:** 2.0

In diesem Bulletin Summary sind die im Dezember 2007 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Dezember 2007 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 6. Dezember 2007 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 12. Dezember 2007 um 20:00 Uhr (MEZ) führt Microsoft einen englischsprachigen Webcast durch, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Dezember.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032344696&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (3)
------------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-064                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeiten in DirectX können Remotecodeausführung ermöglichen (941568)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-064.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Kurzzusammenfassung**                     | Dieses kritische Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft DirectX. Diese Sicherheitsanfälligkeiten können Codeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Datei öffnet, die für Streaming Media in DirectX verwendet wird. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert keinen Neustart, mit Ausnahme von bestimmten Situationen.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Betroffene Software**                     | **Windows, DirectX, DirectShow.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-068                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Windows Mediendateiformat kann Remotecodeausführung ermöglichen (941569 und 944275)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-068.mspx)                                                                                                                                                                                                                                                                              |
| **Kurzzusammenfassung**                     | Dieses kritische Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows Media Format. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Datei in der Windows Media Format Runtime anzeigt. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                           |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert keinen Neustart, mit Ausnahme von bestimmten Situationen.                                                                                                                                                                                                                                                                                              |
| **Betroffene Software**                     | **Windows, Windows Media Format Runtime.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                          |

| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-069                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Kumulatives Sicherheitsupdate für Internet Explorer (942615)**](https://go.microsoft.com/fwlink/germany/technet/sicherheit/bulletins/ms07-069.mspx)                                                                                                                                                                                                                                                                                                                                      |
| **Kurzzusammenfassung**                     | Dieses kritische Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten. Die Sicherheitsanfälligkeit mit der schwerwiegendsten Sicherheitsauswirkung kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                                                                                                                                     |
| **Betroffene Software**                     | **Windows, Internet Explorer.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                  |

Hoch (4)
--------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-063                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in SMBv2 kann Remotecodeausführung ermöglichen (942624)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-063.mspx)                                                                                                                                                                                                         |
| **Kurzzusammenfassung**                     | Dieses wichtige Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Server Message Block Version 2 (SMBv2). Die Sicherheitsanfälligkeit kann einem Angreifer ermöglichen, Daten zu manipulieren, die mithilfe von SMBv2 übertragen werden. Dies kann in Domänenkonfigurationen, die mit SMBv2 kommunizieren, Remotecodeausführung ermöglichen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                           |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                      |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                    |
| **Betroffene Software**                     | **Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                   |

| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-065                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Message Queuing kann Remotecodeausführung ermöglichen (937894)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-065.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Kurzzusammenfassung**                     | Dieses wichtige Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Message Queuing-Dienst (MSMQ), die in Implementierungen unter Microsoft Windows 2000 Server Remotecodeausführung oder in Implementierungen unter Microsoft Windows 2000 Professional oder Windows XP Erhöhung von Berechtigungen ermöglichen kann. Ein Angreifer muss über gültige Anmeldeinformationen verfügen, um die Sicherheitsanfälligkeit bezüglich der Erhöhung von Berechtigungen unter Microsoft Windows 2000 Professional und Windows XP auszunutzen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Berechtigungen erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Betroffene Software**                     | **Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-066                                                                                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im Windows-Kernel kann Erhöhung von Berechtigungen ermöglichen (943078)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-066.mspx)                                                                                                                                                                                                                                         |
| **Kurzzusammenfassung**                     | Dieses wichtige Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows-Kernel. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                           |
| **Auswirkung der Sicherheitsanfälligkeit:** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                                               |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                                                                    |
| **Betroffene Software**                     | **Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                    |

| Kennung des Bulletins                       | Microsoft Security Bulletin MS07-067                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Macrovision-Treiber kann lokale Erhöhung von Berechtigungen ermöglichen (944653)**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-067.mspx)                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Kurzzusammenfassung**                     | Dieses wichtige Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit. Es liegt eine Sicherheitsanfälligkeit bezüglich der lokalen Erhöhung von Berechtigungen vor, die dadurch entsteht, dass der Macrovision-Treiber Konfigurationsparameter falsch verarbeitet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren; Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Auswirkung der Sicherheitsanfälligkeit:** | Lokale Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update erfordert einen Neustart.                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Betroffene Software**                     | **Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |

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
[**MS07-063**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-063.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-064**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-064.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-065**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-065.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-066**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-066.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-067**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-067.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-068**](https://go.microsoft.com/germany/technet/sicherheit/bulletins/ms07-068.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-069**](https://go.microsoft.com/fwlink/germany/technet/sicherheit/bulletins/ms07-069.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads:**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows-Betriebssystem:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Server Service Pack 4 und Microsoft Windows 2000 Professional Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bda9d0b4-f7cb-4d9d-b030-043d7437734b)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=09d4e6ae-5d19-4f11-bb7e-60cee8263bc8)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c7d368d0-f7bf-4946-a4a6-3e88315e5317)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=5f4fa8e9-fcf2-4daf-93c0-8bb267da69aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=5f4fa8e9-fcf2-4daf-93c0-8bb267da69aa)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0f84f5e2-1dd8-4882-b796-444ab70b6b02)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=0f84f5e2-1dd8-4882-b796-444ab70b6b02)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1f416b71-783f-4cbc-9b85-9a9be7daa0d7)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1f416b71-783f-4cbc-9b85-9a9be7daa0d7)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9d22a9ee-cc08-4b2d-af4e-55d326f82761)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9787619f-1297-411e-8b9c-3ad3e6a99797)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=05a9501c-4da3-4fa1-901e-99cb262e5e36)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5f382050-8df6-43aa-82e9-8fad5ff8ecec)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Betroffene Systemkomponenten des Windows-Betriebssystems:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 7.0 unter Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=06196774-5a11-4525-b53c-8cb000738949)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
DirectX 8.1 unter Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ccb872bd-fc06-4a3f-ac70-3c9a42d57b37)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 9.0\* unter Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=03b14ce0-5189-4803-8151-6ac5cb6a9179)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
DirectX 9.0\* unter Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=04a8f8d3-69f9-4445-baab-f45616a6b9b7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 9.0\* unter Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=f096c500-e765-4e75-8443-7ffec4ddf149)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
DirectX 9.0\* unter Windows Server 2003 Service Pack 1 oder unter Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d80a295a-baf9-4981-8a28-1b4207ecc5f7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 9.0\* unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=378086ea-60b8-409f-970a-fcfd62025150)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
DirectX 9.0\* unter Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2e6ea4bb-9f4f-46fb-9d51-e20b15e61a89)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
DirectX 10.0 unter Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bfa571bc-e43f-45e3-bc98-4086985c99aa)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
DirectX 10.0 unter Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3d8803da-108b-4b9d-a039-84932dce8e42)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 5.01 Service Pack 4 unter Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b3bd16ea-5d69-4ae3-84b3-ab773052ceeb)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 Service Pack 1 unter Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bc8edf05-262a-4d1d-b196-4fc1a844970c)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 für Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6e4ebafc-34c3-4dc7-b712-152c611d3f0a)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 für Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f5a5af23-30fb-4e47-94bd-3b05b55c92f2)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 für Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bf466060-a585-4c2e-a48d-70e080c3bbe7)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 6 für Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=074697f2-18c8-4521-bbf7-1d0e7395d27d)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 6 für Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b3f390a6-0361-4553-b627-5e7ad6bf5055)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 für Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b15a6506-02dd-43c2-aef4-e10c1c76ee97)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 für Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c092a6bb-8e62-4d90-bdb1-5f3a15968f75)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 für Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=34759c10-16a5-42a2-974d-9d532fb5a0a7)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 für Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7dccce5a-7562-448b-a345-cf1cc758e35c)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 für Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8414f3fb-216a-4d46-b590-4c1f304dff91)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Internet Explorer 7 in Windows Vista
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=26d303da-bb2e-4555-96f1-becb0e277341)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Internet Explorer 7 in Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c5e88e0b-a4c2-4690-91d9-326800030a16)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 7.1 unter Microsoft Windows 2000 Service Pack 4 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=eecdf2ce-9aa7-4f0c-b62b-2fa7a32f369e)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9 unter Microsoft Windows 2000 Service Pack 4 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=eecdf2ce-9aa7-4f0c-b62b-2fa7a32f369e)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9 unter Windows XP Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bece702a-6e61-433e-8275-20f4e84f2c92)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 unter Windows XP Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bece702a-6e61-433e-8275-20f4e84f2c92)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 unter Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=81f20b45-dfc7-4ddf-a4b4-6c0e9476ed51)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8fea7da8-a7f3-4786-97c2-fb5ea7018159)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ffc69c76-02f1-4b15-8ec1-dab8c7e33bd4)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 x64 Edition unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ffc69c76-02f1-4b15-8ec1-dab8c7e33bd4)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9.5 x64 Edition unter Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=72d2ca0e-da81-45ee-9321-4970b80f4a5a)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 11 unter Windows XP Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bece702a-6e61-433e-8275-20f4e84f2c92)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 11 unter Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2 (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=1037b224-ac89-4efd-b189-6f3da77a88e6)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 11 unter Windows Vista (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9a98ef96-bc2e-42b7-9a24-c82c8fb379db)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 11 unter Windows Vista x64 Edition (KB941569)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3ce02c95-d695-4f14-9fb3-30c83a9cfb9c)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Media Format Runtime 9.1 unter Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2 (KB944275)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=096711d4-ce01-45d0-9c2d-ebfa5c671b9f)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Media Format Runtime 9.1 x64 Edition unter Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2 (KB944275)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=23c23800-5aaa-455b-96bf-4ead4dfdd95d)
</td>
<td style="border:1px solid black;">
</td>
</tr>
</table>
 
**Hinweise**

**<sup>[1]</sup>** Für dieses Betriebssystem steht ein Sicherheitsupdate zur Verfügung. In der Tabelle finden Sie weitere Informationen zum entsprechenden Security Bulletin für die betroffene Software oder Komponente.

\* Umfasst DirectX 9.0a, DirectX 9.0b und DirectX 9.0c

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](https://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](https://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Hinweis:** Nach dem 9. Oktober 2007 wird die von MBSA 1.2.1 verwendete Datei MSSecure.XML nicht mehr aktualisiert. Nach diesem Datum werden keine neuen Sicherheitsupdates für die von MBSA 1.2.1 verwendete Datei MSSecure.XML erstellt und keine neuen Versionen des Enterprise Scan Tools veröffentlicht. Dies betrifft nicht das Sicherheitsupdate-Inventurprogramm (SUIT) oder das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT) für SMS 2.0 und SMS 2003. Weitere Informationen finden Sie unter [Microsoft Baseline Security Analyzer.](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx)

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie auf der Website [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection Tool, um eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates bereitzustellen. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Für diesen Monat:

-   Microsoft hat drei **nicht sicherheitsrelevante** Updates mit hoher Priorität und 2007 Microsoft Office Service Pack 1 auf Microsoft Update (MU) und Windows Server Update Services (WSUS) veröffentlicht.
-   Microsoft hat drei **nicht sicherheitsrelevante** Updates mit hoher Priorität für Windows und Windows SharePoint Services 3.0 Service Pack 1 auf Windows Update (WU) und Windows Server Update Services (WSUS) veröffentlicht.

Diese Informationen gelten **nur** für wichtige, **nicht sicherheitsrelevante** Updates auf Microsoft Update, Windows Update und Windows Server Update Services, die an demselben Tag wie das Security Bulletin Summary veröffentlicht wurden. Es werden **keine** Informationen zu **nicht sicherheitsrelevanten** Updates bereitgestellt, die an anderen Tagen veröffentlicht werden.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Nutzen Sie den [Microsoft-Leitfaden zur Sicherheitspatch-Verwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx). Er enthält Best Practices und von Microsoft empfohlene Vorgehensweisen für die Bereitstellung, Verteilung und Installation von Sicherheitsupdates in Ihrer IT-Umgebung.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Jun Mao von [VeriSign iDefense Labs](https://labs.idefense.com/) für die Zusammenarbeit mit uns an einem in MS07-064 beschriebenen Problem.
-   Peter Winter Smith von [NGSSoftware](https://www.ngssoftware.com/) für die Zusammenarbeit mit uns an einem in MS07-064 beschriebenen Problem.
-   Jung-hyung Lee von [AhnLab](https://global.ahnlab.com/) für die Zusammenarbeit mit uns an den in MS07-064 beschriebenen Tiefenverteidigungsänderungen in DirectX.
-   [Zero Day Initiative](https://www.zerodayinitiative.com/) für die Zusammenarbeit mit uns an einem in MS07- 065 beschriebenen Problem.
-   Venustech von [ADLABS](https://www.venustech.com.cn/) für die Zusammenarbeit mit uns an einem in MS07- 065 beschriebenen Problem.
-   Thomas Garnier von [SkyRecon](https://www.skyrecon.com/) für den Hinweis auf ein in MS07-066 beschriebenes Problem.
-   Ryan Smith von [ISS X-Force](https://xforce.iss.net/) für die Zusammenarbeit mit uns an einem in MS07-068 beschriebenen Problem.
-   Alex Wheeler von [ISS X-Force](https://xforce.iss.net/) für die Zusammenarbeit mit uns an einem in MS07-068 beschriebenen Problem.
-   Peter Vreugdenhil, der mit [iDefense VCP](https://idefense.com/) zusammenarbeitet, für den Hinweis auf ein in MS07-069 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS07-069 beschriebenes Problem.
-   Sam Thomas, der mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS07-069 beschriebenes Problem.
-   Peter Vreugdenhil, der mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS07-069 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (11. Dezember 2007): Bulletin Summary veröffentlicht.
-   V1.1 (12. Dezember 2007): Aktualisierung des Bulletins, um auf Änderungen an den Kurzzusammenfassungen von MS07-065 und MS-07-067 hinzuweisen.
-   V1.2 (23. Januar 2008): Aktualisierung des Bulletins, um auf Änderungen bezüglich der betroffenen Software im Bulletin MS07-064 hinzuweisen.
-   V2.0 (16. Juli 2008): Aktualisierung des Bulletins, um auf Änderungen bezüglich der betroffenen Software im Bulletin MS07-064 hinzuweisen.

*Built at 2014-04-18T01:50:00Z-07:00*
