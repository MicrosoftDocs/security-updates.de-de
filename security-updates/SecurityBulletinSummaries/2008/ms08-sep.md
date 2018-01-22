---
TOCTitle: 'MS08-SEP'
Title: Microsoft Security Bulletin Summary für September 2008
ms:assetid: 'ms08-sep'
ms:contentKeyID: 61225066
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms08-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für September 2008
======================================================

Veröffentlicht: Dienstag, 9. September 2008 | Aktualisiert: Dienstag, 9. Dezember 2008

**Version:** 3.0

In diesem Bulletin Summary sind die im September 2008 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für September 2008 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 4. September 2008 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 10. September 2008 um 20:00 Uhr (MEZ) führt Microsoft einen englischsprachigen Webcast durch, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im September.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374633&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (4)
------------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-054                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Windows Media Player kann Remotecodeausführung ermöglichen (954154)**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Player, die Remotecodeausführung ermöglichen kann, wenn eine speziell gestaltete Audiodatei von einem Windows Media Server gestreamt wird. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-052                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeiten in GDI+ können Remotecodeausführung ermöglichen (954593)**](http://go.microsoft.com/fwlink/?linkid=125468)                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows GDI+. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Bilddatei mithilfe betroffener Software anzeigt oder eine Website durchsucht, die speziell gestaltete Inhalte enthält. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Betroffene Software**                     | **Microsoft Windows, Internet Explorer, .NET Framework, Office, SQL Server, Visual Studio.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                             |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-053                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Windows Media Encoder 9 kann Remotecodeausführung ermöglichen (954156)**](http://go.microsoft.com/fwlink/?linkid=123091)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Encoder 9. Wenn ein Benutzer eine speziell gestaltete Webseite anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-055                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Microsoft Office kann Remotecodeausführung ermöglichen (955047)**](http://go.microsoft.com/fwlink/?linkid=125229)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer auf eine speziell gestaltete OneNote-URL klickt. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist meist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Betroffene Software**                     | **Microsoft Office.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |

Betroffene Software und Downloadadressen
----------------------------------------

**Wie verwende ich diese Tabelle?**  

In dieser Tabelle finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Sie sollten jedes aufgeführte Softwareprogramm und jede Komponente überprüfen, um zu sehen, ob Sicherheitsupdates erforderlich sind. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.

**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.

#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Microsoft Windows 2000
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a860d2d9-653d-4ddb-bbff-323d3ccdb866)  
(KB938464)  
(Kritisch)  
[Microsoft .NET Framework 1.0 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c7cbcd19-acc1-4a89-adfa-99b2f431510d)  
(KB947739)  
(Keine Bewertung des Schweregrads)  
[Microsoft .NET Framework 1.1 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6013f866-3ea1-4672-b1bf-e516204c3a7a)  
(KB947742)  
(Keine Bewertung des Schweregrads)  
[Microsoft .NET Framework 2.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7f1cd013-2c4b-4582-9114-cb840a96124a)  
(KB947746)  
(Keine Bewertung des Schweregrads)  
[Microsoft .NET Framework 2.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=215b73a3-46ab-44a8-a0fb-6d37bd1c39b8)  
(KB947748)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0cabfbc0-db5d-4a6a-a4cd-e6df89ac2b25)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d5891180-5dd1-49ec-bcc6-3030a544202c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e0bd6fbe-f46e-4961-9a79-49ec77d39439)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=57bcb3c2-49d3-4f18-8d03-36abd03d7403)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?familyid=caf8a45e-a9f8-4e91-98fd-87eddbeae64c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c5d26771-1f49-4bbf-902c-bf92e527cadb)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?familyid=18efea9e-b103-46de-90d9-5e295854cec3)  
(Kritisch)  
[Windows Media Encoder 9 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ebc1737c-6e78-4244-a1b2-a56d031f16e9)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ac03f138-eca4-46e1-9782-e811820e547f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=54ce1080-94cf-4e4f-8e09-a7dbab2757c5)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=93f1451b-5b62-47e5-8f0c-b720b957999a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c83011cd-90b8-494c-9cad-fa055e101992)  
(Mittel)  
[Windows Media Encoder 9 x64 Edition](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d8f1b782-136b-443f-b5f2-63aa4d1fd94a)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=14e99f8a-cdd4-40d7-8cfc-73ae6bd6dfad)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2f4118fd-1ffb-46da-b922-cd4ca4f9d84e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=16f3ad21-ed77-4c32-93df-3b650b2b32a5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=334352e7-d41f-494f-866d-f1f1745ffd17)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa47d016-f5c9-4586-8876-f1f4f255f54d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99beebc4-553a-46f8-8245-e3d932306c93)  
(Kritisch)  
[Windows Media Encoder 9 x64 Edition](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=54d1279a-7f26-4727-a39d-5505bcd4fc53)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-054**](http://www.microsoft.com/germany/technet/sicherheit/bulletins/ms08-054.mspx)
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-053**](http://go.microsoft.com/fwlink/?linkid=123091)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=72fc6028-6af4-44ec-8d2a-28c53807d6bc)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&amp;familyid=23bd3be5-cc66-46f8-9420-49d65d8afe1d)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Media Player 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3906512b-26db-473e-b522-3883ff34a21c)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7f1e0f05-6c9d-4ad1-9b19-50ee4fa7bd7e)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Encoder 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5434ca66-5a6b-4517-92fb-72dea0a172ec)\*  
(Mittel)  
[Windows Media Encoder 9 x64 Edition](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e30f9427-26d0-4e86-b9b8-bc637c3b5734)\*  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5159bdba-3825-4816-a2be-ab035332b9e2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch diese Updates behobenen Sicherheitsanfälligkeiten wirken sich nicht auf unterstützte Editionen von Windows Server 2008 aus, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Dennoch können die von diesen Sicherheitsanfälligkeiten betroffenen Dateien auf dem System vorhanden sein. Benutzern mit den betroffenen Dateien wird dieses Update jedoch immer noch angeboten, da die Updatedateien neuer sind (höhere Versionsnummern haben) als die Dateien, die derzeit auf Ihrem System vorhanden sind. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 2 und Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Hoch)  
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Hoch)  
[Microsoft Office 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e670ad22-d3c1-41f7-ba30-6a67139feaa3)  
(KB953404)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 und Microsoft Office System 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office System 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Hoch)  
[Microsoft Office System 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office System 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Hoch)  
[Microsoft Office System 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=fb457536-26c5-428b-97e4-1fc13718266e)  
(KB951944)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
<td style="border:1px solid black;">
[**MS08-055**](http://go.microsoft.com/fwlink/?linkid=125229)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Project 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ef3de64c-fc17-4500-9da4-a3bba97fda6d)  
(KB953405)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a6d9d3ef-f087-4f61-9ec1-522b7d4b9c48)  
(KB954479)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Word Viewer, Microsoft Word Viewer 2003, Microsoft Word Viewer 2003 Service Pack 3, Microsoft Office Excel Viewer 2003, Microsoft Office Excel Viewer 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer, Microsoft Word Viewer 2003, Microsoft Word Viewer 2003 Service Pack 3, Microsoft Office Excel Viewer 2003, Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e9f8e309-d721-4bab-b485-5eede8d49eb8)  
(KB954478)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office PowerPoint Viewer 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint Viewer 2003](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=cd503f08-1831-45ff-bdf4-dd918ca40505)  
(KB956500)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer, Microsoft Office PowerPoint Viewer 2007, Microsoft Office PowerPoint Viewer 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer, Microsoft Office PowerPoint Viewer 2007, Microsoft Office PowerPoint Viewer 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Expression Web und Microsoft Expression Web 2
</td>
<td style="border:1px solid black;">
[Microsoft Expression Web und Microsoft Expression Web 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Groove 2007 und Microsoft Office Groove 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Groove 2007 und Microsoft Office Groove 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b656fe8-6253-490c-a81a-e4e8f0bb58d2)  
(KB954326)\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eb0d224e-a517-40d9-9fc6-2345fa12a841)  
(KB956483)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Digital Image Suite 2006
</td>
<td style="border:1px solid black;">
[Microsoft Digital Image Suite 2006](http://www.microsoft.com/downloads/details.aspx?familyid=04afd760-8173-4069-9e82-d3bf053d9eae)  
(KB955992)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office OneNote 2007
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office OneNote 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Kritisch)  
[Microsoft Office OneNote 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8ac3576c-7873-4ac6-8bbc-033f6a7bb395)  
(KB950130)  
(Kritisch)
</td>
</tr>
</table>
 
\*Das Update für diese betroffene Software ist identisch mit dem Update für Microsoft Office XP Service Pack 3.

\*\*Das Update für diese betroffene Software ist identisch mit dem Update für Microsoft Office 2003 Service Pack 2 und Microsoft Office 2003 Service Pack 3.

\*\*\*Das Update für diese betroffene Software ist identisch mit dem Update für Microsoft Office System 2007 und Microsoft Office System 2007 Service Pack 1.

#### Microsoft Server Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2000 Reporting Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
Nicht anwendbar  
QFE-Update:  
[SQL Server 2000 Reporting Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5f9e7f78-7439-414b-a9dc-a779b89427db)  
(KB954609)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4603c722-2468-4adb-b945-2ed0458b8f47)  
(KB954606)  
(Kritisch)  
QFE-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5148b887-f323-4adb-9721-61e1c0cfd213)  
(KB954607)  
(Kritisch)
</td>
</tr>
</table>
 

#### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2002 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7848a652-4025-44bb-9c98-37a078b56d01)  
(KB947736)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9bc1e8f8-6c30-4aa0-90f5-fbb0ad5fd90e)  
(KB947737)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7bf790b-3249-4ee8-9440-fa911ebbc08a)  
(KB947738)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2008
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a8c80b29-6d00-4949-a005-5d706122919a)  
(KB952241)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2005 Service Pack 1 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=82833f27-081d-4b72-83ef-2836360a904d)  
(KB954765)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Report Viewer 2008 Redistributable Package
</td>
<td style="border:1px solid black;">
[Microsoft Report Viewer 2008 Redistributable Package](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6ae0aa19-3e6c-474c-9d57-05b2347456b1)  
(KB954766)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 8.0 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1f4371b9-b8be-4455-94d2-2304ee340543) unter Microsoft Windows 2000 Service Pack 4  
(KB955368)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=49b21e30-722d-446e-9020-aceb3870db69) unter Microsoft Windows 2000 Service Pack 4  
(KB955369)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro 9.0 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=36957f47-9d8b-477d-bd60-5959e5a2eafa) unter Microsoft Windows 2000 Service Pack 4  
(KB955370)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Platform SDK Redistributable: GDI+
</td>
<td style="border:1px solid black;">
[Microsoft Platform SDK Redistributable: GDI+](http://www.microsoft.com/downloads/details.aspx?familyid=6a63ab9c-df12-4d41-933c-be590feaa05a)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
</table>
 

#### Microsoft Sicherheitssoftware

<p> </p>
<table style="border:1px solid black;">
<tr class="thead">
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Forefront Security
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-052**](http://go.microsoft.com/fwlink/?linkid=125468)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads des Bulletins**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Forefront Client Security 1.0
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Client Security 1.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1eb1a79f-44ca-499e-90bb-ac51894e9d1e) unter Microsoft Windows 2000 Service Pack 4  
(KB957177)  
(Hoch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Security Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](http://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](http://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](http://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](http://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](http://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](http://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](http://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet2.microsoft.com/windowsvista/en/library/4279e239-37a4-44aa-aec5-4e70fe39f9de1033.mspx?mfr=true), die im [Anwendungskompatibilitäts-Toolkit 5.0](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Anwendungskompatibilitäts-Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services für 2008. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Greg MacManus von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS08-052 beschriebenes Problem.
-   Bing Liu vom [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) für den Hinweis auf ein in MS08-052 beschriebenes Problem.
-   Peter Winter-Smith von [NGSSoftware](http://www.ngssoftware.com/) und Ivan Fratric in Zusammenarbeit mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-052 beschriebenes Problem.
-   [Vulnerability Research Team, Assurent Secure Technologies](http://www.assurent.com/) für den Hinweis auf ein in MS08-052 beschriebenes Problem.
-   Einer Person, die mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS08-052 beschriebenes Problem.
-   Nguyen Minh Duc und Le Manh Tung in Zusammenarbeit mit dem [Bach Khoa Internetwork Security Center (BKIS) Hanoi University of Technology (Vietnam)](http://security.bkis.vn/) für den Hinweis auf ein in MS08-053 beschriebenes Problem.
-   Brett Moore von [Insomnia Security](http://www.insomniasec.com/) für den Hinweis auf ein in MS08- 055 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (9. September 2008): Bulletin Summary veröffentlicht.
-   V2.0 (9. September 2008): Aktualisierung des Bulletin Summary, um Microsoft Office Project 2002 Service Pack 2, die gesamte Office Viewer-Software für Microsoft Office 2003 und die gesamte Office Viewer-Software für Microsoft Office System 2007 als betroffene Software für MS08-052 hinzuzufügen.
-   V2.1 (17. September 2008): Aktualisierung des Bulletin Summary, um Microsoft Office Project 2002 Service Pack 2 in der Tabelle „Betroffene Software“ in Microsoft Office Project 2002 Service Pack 1 zu ändern. Dies ist lediglich eine Namenänderung. Die Binärdateien oder die Erkennung wurden nicht verändert.
-   V2.2 (29. Oktober 2008): Aktualisierung des Bulletin Summary, um Microsoft Visio Viewer 2003, Microsoft Visio Viewer 2007 und Microsoft Visio Viewer 2007 Service Pack 1 als betroffene Software für MS08-052 zu entfernen.
-   V3.0 (9. Dezember 2008): Aktualisierung des Bulletin Summary, um Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1, Microsoft Expression Web, Microsoft Expression Web 2, Microsoft Office Groove 2007 und Microsoft Office Groove 2007 Service Pack 1 als betroffene Software für MS08-052 hinzuzufügen.

*Built at 2014-04-18T01:50:00Z-07:00*
