---
TOCTitle: 'MS07-JUN'
Title: Microsoft Security Bulletin Summary für Juni 2007
ms:assetid: 'ms07-jun'
ms:contentKeyID: 61225049
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms07-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Juni 2007
=================================================

Veröffentlicht: Dienstag, 12. Juni 2007

**Version:** 1.0

In diesem Bulletin Summary sind die im Juni 2007 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Juni 2007 ersetzt dieses Bulletin Summary die Bulletin-Vorankündigung, die erstmalig am 7. Juni 2007 veröffentlicht wurde. Weitere Informationen zum Bulletin-Vorankündigungsdienst finden Sie unter [Microsoft Security Bulletin-Vorankündigung.](https://technet.microsoft.com/security/bulletin/advance)

Abonnieren Sie die [Microsoft-Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx), um automatisch eine Benachrichtigung zu erhalten, sobald ein Microsoft Security Bulletin veröffentlicht wird.

Am Mittwoch, den 13. Juni 2007 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Juni.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032327013&eventcategory=4&culture=en-us&countrycode=us) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (4)
------------


| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-031                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit im Windows SChannel-Sicherheitspaket kann Remotecodeausführung ermöglichen (935840)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-031.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Kurzzusammenfassung**                    | Dieses kritische Sicherheitsupdate behebt eine von Privatanwendern gemeldete Sicherheitsanfälligkeit im SChannel-Sicherheitspaket (Security Channel) in Windows. Das SChannel-Sicherheitspaket implementiert die standardmäßigen Internetauthentifizierungsprotokolle Secure Sockets Layer (SSL) und Transport Layer Security (TLS). Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mithilfe eines Internetwebbrowsers anzeigt oder eine Anwendung verwendet, die SSL/TLS nutzt. Das Ausnutzen dieser Sicherheitsanfälligkeit würde jedoch höchstwahrscheinlich zum Beenden des Internetwebbrowsers oder der Anwendung führen. Das System kann keinesfalls Websites oder Ressourcen mit SSL oder TLS aufrufen, bis das System neu gestartet wurde. |
| **Bewertung des maximalen Schweregrads**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Betroffene Software**                    | **Windows:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

<p></br></p>

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-033                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|--------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Kumulatives Sicherheitsupdate für Internet Explorer (933566)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Kurzzusammenfassung**                    | Dieses kritische Sicherheitsupdate behebt fünf von Privatanwendern gemeldete Sicherheiitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit. Bis auf eine Ausnahme können alle dieser Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen, wenn ein Benutzer in Internet Explorer eine speziell gestaltete E-Mail anzeigt. Eine Sicherheitsanfälligkeit könnte Spoofing-Angriffe ermöglichen und erfolgt auch über eine speziell gestaltete Webseite. Bei allen Fällen der Remotecodeausführung könnten Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, weniger stark betroffen sein als Benutzer, die mit administrativen Benutzerrechten arbeiten. Damit der Spoofing-Angriff ausgenutzt werden kann, sind Benutzereingriffe erforderlich. |
| **Bewertung des maximalen Schweregrads**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Betroffene Software**                    | **Windows, Internet Explorer:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |

<p></br></p>

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-034                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Kumulatives Sicherheitsupdate für Outlook Express und Windows Mail (929123)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-034.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Kurzzusammenfassung**                    | Mit diesem kritischen Sicherheitsupdate werden zwei Sicherheitsanfälligkeiten behoben, die privat gemeldet wurden, sowie zwei öffentlich gemachte Anfälligkeit. Eine dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer in Windows Mail in Windows Vista eine speziell gestaltete E-Mail anzeigt. Die anderen Sicherheitsanfälligkeiten könnten die Offenlegung von Information ermöglichen, wenn ein Benutzer mit Internet Explorer eine speziell gestaltete Web-Seite besucht; diese Sicherheitsanfälligkeiten können nicht direkt in Outlook Express ausgenutzt werden. Bei den Sicherheitsanfälligkeiten durch die Offenlegung von Informationen sind Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, u. U. weniger stark gefährdet als Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Erkennung**                              | Microsoft Baseline Security Analyzer und das Enterprise Scan Tool können erkennen, ob Ihr Computersystem dieses Update erfordert. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Betroffene Software**                    | **Windows, Outlook Express, Windows Mail:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |

<p></br></p>

| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-035                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|--------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in Win32 API kann Remotecodeausführung ermöglichen (935839)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-035.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Kurzzusammenfassung**                    | Dieses kritische Sicherheitsupdate behebt eine von Privatanwendern gemeldete Sicherheitsanfälligkeit in einer Win32 API. Diese Sicherheitsanfälligkeit kann Remotecodeausführung oder nicht autorisiertes Erteilen von Benutzerrechten (Elevation of Privilege) ermöglichen, wenn die betroffene API lokal von einer speziell gestalteten Anwendung verwendet wird. Daher könnten Anwendungen, die diese Komponente der Win32 API verwenden, als ein Vektor für diese Sicherheitsanfälligkeit verwendet werden. Internet Explorer z. B. verwendet diese Win32 API-Funktion beim Analysieren speziell gestalteter Web-Seiten. |
| **Bewertung des maximalen Schweregrads**   | [Kritisch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Betroffene Software**                    | **Windows:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |

Hoch (1)
--------


| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-030                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|--------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeiten in Microsoft Visio können Remotecodeausführung ermöglichen (927051)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-030.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Kurzzusammenfassung**                    | Mit diesem wichtigen Sicherheitsupdate werden zwei Sicherheitsanfälligkeiten, die privat und verantwortungsbewusst gemeldet wurden, zusammen mit anderen Problemen behoben, die im Laufe der Untersuchungen identifiziert wurden. Die von Privatanwendern gemeldeten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Zum Ausnutzen dieser Sicherheitsanfälligkeiten sind jedoch Benutzereingriffe erforderlich. |
| **Bewertung des maximalen Schweregrads**   | [Hoch](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Auswirkung der Sicherheitsanfälligkeit** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Betroffene Software**                    | **Office, Visio:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |

Mittel (1)
----------


| Kennung des Bulletins                      | Microsoft Security Bulletin MS07-032                                                                                                                                                                                                                                                                                                                                  |
|--------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                    | [**Sicherheitsanfälligkeit in Windows Vista kann Offenlegung von Informationen ermöglichen (931213)**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-032.mspx)                                                                                                                                                                                   |
| **Kurzzusammenfassung**                    | Dieses mittlere Sicherheitsupdate behebt eine von einem Privatanwender gemeldete Sicherheitsanfälligkeit. Diese Sicherheitsanfälligkeit könnte nicht berechtigten Benutzern den Zugriff auf lokale Datenspeicher für Benutzerinformationen einschließlich administrativer Kennwörter ermöglichen, die in der Registrierung und im lokalen Dateisystem enthalten sind. |
| **Bewertung des maximalen Schweregrads**   | [Mittel](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                     |
| **Auswirkung der Sicherheitsanfälligkeit** | Offenlegung von Informationen                                                                                                                                                                                                                                                                                                                                         |
| **Erkennung**                              | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                           |
| **Betroffene Software**                    | **Windows:** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                |

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
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS07-030**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-030.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-031**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-031.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-032**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-032.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-033**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-034**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-034.mspx)
</td>
<td style="border:1px solid black;">
[**MS07-035**](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-035.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des maximalen Schweregrads**
</td>
<td style="border:1px solid black;">
[**Wichtig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Betroffene Windows-Software:
</th>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5b8e728c-cb9f-4176-93a0-bf42d6387f93)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3918ac76-ebb6-4886-9a9e-808eafb96b1b)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=8615e6f3-415b-4c23-ba52-7eef70a11d77)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=27c7f1b9-2d1d-40cb-ad7e-bfedb6156a9c)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=7e994340-c616-4f66-845b-7eaf095e968a&displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=0ba12191-1e6f-443b-9150-7ab8b2deb7c2&displaylang=en)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=7e994340-c616-4f66-845b-7eaf095e968a&displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?familyid=0ba12191-1e6f-443b-9150-7ab8b2deb7c2&displaylang=en)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=39e6c6d2-7e6f-4992-a731-36f44fe2d87f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d554dff4-bcfb-4bbc-8fa0-af2f939d2610)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=39e6c6d2-7e6f-4992-a731-36f44fe2d87f)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=d554dff4-bcfb-4bbc-8fa0-af2f939d2610)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=da424772-079c-4351-9759-8886e0f1ba79)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=170473d8-6bb1-4fbd-8494-a059dbfdf182)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=da424772-079c-4351-9759-8886e0f1ba79)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=170473d8-6bb1-4fbd-8494-a059dbfdf182)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=028592ff-2b69-472e-b186-bd2cc76bdfa4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f5e45e3c-4cac-41a5-99f7-42c2c2c73e99)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=028592ff-2b69-472e-b186-bd2cc76bdfa4)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f5e45e3c-4cac-41a5-99f7-42c2c2c73e99)
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=cdf79d00-6f34-404b-8ad5-a2801ff35443)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=89dde3f4-4123-4c97-86d8-00a83462c34b)
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
**<sup>[1]</sup>**
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Betroffene Systemkomponenten des Windows-Betriebssystems:
</th>
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=3b49f1ed-abe3-4dbd-a91d-973415658f6b)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5c958650-28d2-4dd0-96a8-dbfe79ce3f68)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=60fb294e-a8e1-405e-a289-2d2723edf7ee)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=086d6d6e-4703-4c6c-a7af-b6dafeeede5d)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=7ed19127-5c2d-48e4-a8d1-090dc69fd68b)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=1449eb5d-6e4c-4332-8cb6-ab9ee59c9a95)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=b628a3cc-a70c-478a-a10c-eee254ee34ab)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c2191703-8cbd-4959-9f84-e13f21173926)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=69c526b8-8b07-42bc-9bed-e18deae21c8e)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a074d9c0-1fed-4753-845e-073cfce99f45)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=744acb43-64da-48cc-ae69-9386b597eabc)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=069c1560-b5e5-4dfe-a18d-e0507d406028)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=77287386-48eb-4aa9-9537-626a3093aaf7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=77287386-48eb-4aa9-9537-626a3093aaf7)
</td>
<td style="border:1px solid black;">
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Outlook Express 6 für Windows XP Service Pack 2
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
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=27cca556-0872-4803-b610-4c895ceb99aa)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Outlook Express 6 unter Windows XP Professional x64 Edition
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
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=1ea813bf-bddb-40f0-8960-b9debc8413e7&displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Outlook Express 6 für Windows XP Professional x64 Edition Service Pack 2
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
[Hoch](https://www.microsoft.com/download/details.aspx?familyid=1ea813bf-bddb-40f0-8960-b9debc8413e7&displaylang=en)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Outlook Express 6 unter Microsoft Windows Server 2003 Service Pack 1
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
[Niedrig](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=93808a74-035c-4ab7-9283-c693d7bd82be)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Outlook Express 6 für Windows Server 2003 Service Pack 2
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
[Niedrig](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=93808a74-035c-4ab7-9283-c693d7bd82be)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Outlook Express 6 unter Windows Server 2003 x64 Edition
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f63323a9-e285-45e5-84bd-71ae9da126e3)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Outlook Express 6 für Windows Server 2003 x64 Edition Service Pack 2
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
[Mittel](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f63323a9-e285-45e5-84bd-71ae9da126e3)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Outlook Express 6 für Windows Server 2003 mit SP1 für Itanium-basierte Systeme
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
[Niedrig](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2e62e96e-6571-437d-a612-99175ac39025)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Outlook Express 6 für Windows Server 2003 mit SP2 für Itanium-basierte Systeme
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
[Niedrig](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=2e62e96e-6571-437d-a612-99175ac39025)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Mail in Windows Vista
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ee57de19-44ea-48f2-ae28-e76fd2018633)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Mail in Windows Vista x64 Edition
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
[Kritisch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=343db20f-7794-4423-b11d-885329fbdf78)
</td>
<td style="border:1px solid black;">
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Betroffene Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=fc1d0483-27e8-4541-b81d-4a47973bea30)
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
Visio 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Hoch](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=c47f432e-8538-42fd-92c9-7e0f1d643e8e)
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
</table>
 
**Hinweise**

**<sup>[1]</sup>** Für dieses Betriebssystem steht ein Sicherheitsupdate zur Verfügung. In der Tabelle finden Sie weitere Informationen zum entsprechenden Security Bulletin für die betroffene Software oder Komponente.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://www.microsoft.com/germany/technet/updatemanagement/default.mspx). Im [TechNet Security Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch im [Microsoft Download Center](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar und können am einfachsten durch eine Suche nach dem Begriff „security\_patch“ oder „security\_update“ ermittelt werden, oder über [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](https://office.microsoft.com/de-de/officeupdate/default.aspx). Außerdem können Sicherheitsupdates vom Windows Update-Katalog heruntergeladen werden. Weitere Informationen zum Windows Update-Katalog finden Sie im [Microsoft Knowledge Base-Artikel 323166](https://support.microsoft.com/kb/323166).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS), Extended Security Update Inventory Tool und Enterprise Update Scan Tool (EST). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](https://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer und** **Enterprise** **Update Scan Tool**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

Wenn MBSA 1.2.1 die Erkennung für ein bestimmtes Sicherheitsupdate nicht unterstützen kann, veröffentlicht Microsoft für dieses bestimmte Sicherheitsupdate eine Version des Enterprise Update Scan Tools (EST). Weitere Informationen zu EST finden Sie auf der Website [Enterprise Update Scan Tool](https://support.microsoft.com/default.aspx?id=894193).

**Hinweis:** Nach dem 9. Oktober 2007 wird die von MBSA 1.2.1 verwendete Datei MSSecure.XML nicht mehr aktualisiert. Nach diesem Datum werden keine neuen Sicherheitsupdates für die von MBSA 1.2.1 verwendete Datei MSSecure.XML erstellt und keine neuen Versionen des Enterprise Scan Tools veröffentlicht. Weitere Informationen dazu finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Software Update Services**

Mit den Microsoft Software Update Services (SUS) können Sie als IT-Administrator neue wichtige Updates, Hotfixes oder Patches schnell und zuverlässig auf den Servern und Desktop-Computern in Ihrem Netzwerk bereitstellen. Die SUS unterstützen die Produkte der Windows 2000 Server- und Windows Server 2003-Familie sowie Windows 2000 Professional und Windows XP Professional.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mit Software Update Services finden Sie auf der Website zu [Software Update Services](https://go.microsoft.com/fwlink/?linkid=21133).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/windowsserver2003/technologien/updateservices/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie auf der Website [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection Tool, um eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates bereitzustellen. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

Beachten Sie, dass dieses Tool **nicht** mit Software Update Services (SUS) verteilt wird.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU, WSUS und SUS

Für diesen Monat:

-   Microsoft hat sieben **nicht sicherheitsrelevante** Updates mit hoher Priorität auf Microsoft Update (MU) und Windows Server Update Services (WSUS) veröffentlicht.
-   Microsoft hat keine **nicht sicherheitsrelevanten** Updates mit hoher Priorität für Windows auf Windows-Update (WU) und Software Update Services (SUS) veröffentlicht.

Diese Informationen gelten **nur** für wichtige, **nicht sicherheitsrelevante** Updates auf Microsoft Update, Windows Update, Windows Server Update Services und Software Update Services, die an demselben Tag wie das Security Bulletin Summary veröffentlicht wurden. Es werden **keine** Informationen zu **nicht sicherheitsrelevanten** Updates bereitgestellt, die an anderen Tagen veröffentlicht werden.

#### Sicherheitsstrategien und Communiy

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der [TechNet Webseite zum Thema Patchverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar und können am einfachsten durch eine Schlüsselwortsuche nach dem Begriff „security\_patch“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Zone Community:**

Auf der Website [IT Pro Security Community](https://go.microsoft.com/fwlink/?linkid=21164) erfahren Sie, wie Sie die Sicherheit erhöhen und die IT-Infrastruktur optimieren können. Sie haben zudem die Möglichkeit sich mit anderen IT-Fachleuten über Sicherheitsthemen auszutauschen.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Einem anonymen Forscher, der mit [iDefense VCP](https://idefense.com/) zusammenarbeitet, für den Hinweis auf ein in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenes Problem.
-   Tom Cross von [ISS](https://www.iss.net/) für die Zusammenarbeit mit Microsoft an einem in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenen Problem.
-   Einem anonymen Forscher, der mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenes Problem.
-   Sam Thomas, der mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenes Problem.
-   Will Dormann von [CERT/CC](https://www.cert.org/certcc.html) für den Hinweis auf ein in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenes Problem.
-   Cocoruder von [Fortinet Security Research](https://www.fortinet.com/) für die Zusammenarbeit mit Microsoft an einem in [MS07-033](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-033.mspx) beschriebenen Problem.
-   Billy Rios für den Hinweis auf ein in [MS07-035](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-035.mspx) beschriebenes Problem.
-   Thomas Lim von [COSEINC](https://www.coseinc.com/) für den Hinweis auf ein in [MS07-031](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-031.mspx) beschriebenes Problem.
-   [SANS ISC](https://isc.sans.org/) für die Zusammenarbeit mit uns an einem in [MS07-034](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-034.mspx) beschriebenen Problem.
-   Yosuke Hasegawa von [WebAppSec.JP](https://www.webappsec.jp/) für den Hinweis auf ein in [MS07-034](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-034.mspx) beschriebenes Problem.
-   Robbie Sohlman für den Hinweis auf ein in [MS07-032](https://www.microsoft.com/germany/technet/sicherheit/bulletins/ms07-032.mspx) beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (12. Juni 2007): Bulletin Summary veröffentlicht.

*Built at 2014-04-18T01:50:00Z-07:00*
