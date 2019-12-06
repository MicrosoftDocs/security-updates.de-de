---
TOCTitle: 'MS08-APR'
Title: Microsoft Security Bulletin Summary für April 2008
ms:assetid: 'ms08-apr'
ms:contentKeyID: 61225055
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms08-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2008
==================================================

Veröffentlicht: Dienstag, 8. April 2008 | Aktualisiert: Mittwoch, 18. Februar 2009

**Version:** 1.3

In diesem Bulletin Summary sind die im April 2008 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für April 2008 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 3. April 2008 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 9. April 2008 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032357219&eventcategory=4&culture=en-us&countrycode=us). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

Die Security Bulletins für diesen Monat, nach Schweregrad geordnet:

Kritisch (5)
------------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-018                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in Microsoft Project kann Remotecodeausführung ermöglichen (950183)**](http://go.microsoft.com/fwlink/?linkid=115454)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Project, die Remotecodeausführung ermöglichen kann, wenn ein Benutzer eine speziell gestaltete Project-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Betroffene Software**                     | **Microsoft Office.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-021                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in GDI kann Remotecodeausführung ermöglichen (948590)**](http://go.microsoft.com/fwlink/?linkid=111955)                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in GDI. Die Ausnutzung einer dieser beiden Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete EMF- oder WMF-Bilddatei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-022                                                                                                                                                                                                                                                                                                                                                                                                |
|---------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in den Skriptmodulen VBScript und JScript kann Remotecodeausführung ermöglichen (944338)**](http://go.microsoft.com/fwlink/?linkid=108169)                                                                                                                                                                                                                                                               |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den Skriptmodulen VBScript und JScript in Windows. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                 |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                                  |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                    |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-023                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
|---------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsupdate von ActiveX-Kill Bits (948881)**](http://go.microsoft.com/fwlink/?linkid=112366)                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit für ein Microsoft-Produkt. Dieses Update enthält auch ein Kill Bit für das Yahoo! Music Jukebox-Produkt. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Das Update kann einen Neustart erfordern.                                                                                                                                                                                                                                                                                                                                                                                              |
| **Betroffene Software**                     | **Microsoft Windows, Internet Explorer.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                      |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-024                                                                                                                                                                                                                                                                                                                                                                                             |
|---------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Kumulatives Sicherheitsupdate für Internet Explorer (947864)**](http://go.microsoft.com/fwlink/?linkid=110557)                                                                                                                                                                                                                                                                                                                |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Kritisch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                              |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                             |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                                               |
| **Betroffene Software**                     | **Microsoft Windows, Internet Explorer.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                              |

Hoch (3)
--------


| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-020                                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit in DNS-Client kann Spoofing ermöglichen (945553)**](http://go.microsoft.com/fwlink/?linkid=108231)                                                                                                                                                                                                                             |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit. Diese Sicherheitsanfälligkeit bezüglich Spoofing liegt auf Windows DNS-Clients vor und kann einem Angreifer ermöglichen, speziell gestaltete Antworten auf DNS-Anforderungen zu senden und dadurch Internetverkehr von legitimen Orten vorzutäuschen oder umzuleiten. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                           |
| **Auswirkung der Sicherheitsanfälligkeit:** | Spoofing                                                                                                                                                                                                                                                                                                                                                  |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                        |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                          |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-025                                                                                                                                                                                                                                                                                                                                                                    |
|---------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeit im Windows-Kernel kann Erhöhung von Berechtigungen ermöglichen (941693)**](http://go.microsoft.com/fwlink/?linkid=111956)                                                                                                                                                                                                                                                    |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows-Kernel. Nutzt ein lokaler Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Berechtigungen erstellen. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                         |
| **Auswirkung der Sicherheitsanfälligkeit:** | Erhöhung von Berechtigungen                                                                                                                                                                                                                                                                                                                                                                             |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist ein Neustart erforderlich.                                                                                                                                                                                                                                                      |
| **Betroffene Software**                     | **Microsoft Windows.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                        |

<p></br></p>

| Kennung des Bulletins                       | Microsoft Security Bulletin MS08-019                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|---------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Titel des Bulletins**                     | [**Sicherheitsanfälligkeiten in Microsoft Visio können Remotecodeausführung ermöglichen (949032)**](http://go.microsoft.com/fwlink/?linkid=115455)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| **Kurzzusammenfassung**                     | Dieses Sicherheitsupdate behebt vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Visio, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. |
| **Bewertung des maximalen Schweregrads:**   | [Hoch](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| **Auswirkung der Sicherheitsanfälligkeit:** | Remotecodeausführung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Erkennung**                               | Microsoft Baseline Security Analyzer kann erkennen, ob Ihr Computersystem dieses Update benötigt. Für dieses Update ist kein Neustart des Computers erforderlich.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Betroffene Software**                     | **Microsoft Office.** Weitere Informationen finden Sie im Abschnitt „Betroffene Software und Downloadadressen“.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |

Betroffene Software und Downloadadressen
----------------------------------------

**Wie verwende ich diese Tabelle?**  

In dieser Tabelle finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Sie sollten jedes aufgeführte Softwareprogramm und jede Komponente überprüfen, um zu sehen, ob Sicherheitsupdates erforderlich sind. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.

**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.

#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft Windows 2000</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Windows 2000 Service Pack 4</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=caac000a-22b6-48cb-aa00-1a0bfe886de2">Microsoft Windows 2000 Service Pack 4</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.1 und JScript 5.1</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8e3ff44f-145b-4a68-9ad4-4a55d74b216e">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=0395451f-b719-4f71-a7b4-403d0c7e8fcc">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=ba6d3aeb-e35a-47cc-bace-7bd9d58a9d3f">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=b051ae04-fe81-440d-9136-d6b239ca954e">Microsoft Internet Explorer 5.01 Service Pack 4</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=75d2dc78-e3a4-4ff6-9e2d-bf1935003e8e">Microsoft Internet Explorer 6 Service Pack 1</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=41326ade-96b6-47ce-9291-d4e3039471c4">Microsoft Windows 2000 Service Pack 4</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8db9f328-da0e-4fb8-96c4-6d368b47c224">Microsoft Windows 2000 Service Pack 4</a><br />
(Hoch)</td>
</tr>
</tbody>
</table>
 

<p> </p>
<table style="border:1px solid black;">
<caption>Windows XP</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows XP Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=c2763dd8-a03e-4a48-aa86-a7ec00250a7a">Windows XP Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=c0124698-3b94-4474-9473-22a2f39a4a56">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=9dbf002f-fe53-4cc7-a430-35f45c520d10">Windows XP Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=36c641ad-953f-4b09-ba1c-9c383295e180">Microsoft Internet Explorer 6</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=e771efe8-8881-4f23-b5b0-15651a390ba9">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=893f4cef-0395-4c44-ba28-7a10b6e7dd48">Windows XP Service Pack 2</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=0e937f65-abd0-46dd-8883-5bfd70ea1178">Windows XP Service Pack 2</a><br />
(Hoch)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=166f2ab5-913c-47a9-86fe-b814797b751e">Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=87b80ae3-e299-4d15-a135-3b1bcf943652">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=01400970-df68-4daf-aa39-2fc4f969974c">Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=85beacc0-8ca2-4ded-9c24-23348d05c735">Microsoft Internet Explorer 6</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=9364bf81-6505-4788-958d-a4bd29dc98ad">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=8fdd1207-6e93-4c43-bacc-fe3623a6ebe7">Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=a29bbd13-761f-44fa-8948-e1a8c244bd7a">Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2</a><br />
(Hoch)</td>
</tr>
</tbody>
</table>
 

<p> </p>
<table style="border:1px solid black;">
<caption>Windows Server 2003</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=bee91d80-d49a-4d3d-82d6-d5aa63f54979">Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=88518aa6-e334-4529-aa63-0bf2ef417ce3">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=ad384fea-53be-4be3-8acb-1cd23a7f5405">Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2</a><br />
(Mittel)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=0444b76e-93fa-43c2-b1bc-a5c054529eb5">Microsoft Internet Explorer 6</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=9acd2a03-5530-49c8-9ea1-0bfaf259700d">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=214bd8f5-6eb2-414c-b013-c516a306d692">Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d3b855a6-4648-4771-826d-11a151828eac">Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2</a><br />
(Hoch)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=e3dde449-e062-4ce0-a9f4-433bff23e224">Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=12cefefc-8553-4dca-9850-c653371de61e">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=ffc5c893-cb24-4875-b0a7-6d5c7aa4d642">Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Mittel)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=5ebb5ef9-615f-4cab-bac5-6f45f1b94952">Microsoft Internet Explorer 6</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=a9e406aa-33e2-49b8-ab54-4a7328e46147">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=fd123394-a5d6-4b55-be74-2938f52ce922">Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=320fd100-35e1-4345-9399-796393235cbc">Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2</a><br />
(Hoch)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=7886a802-f2b5-489c-b14b-631f4c4c0742">Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=fe22a828-cca4-4b51-bbd5-995c65fead21">VBScript 5.6 und JScript 5.6</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=94cf78d3-b6c3-41bc-993e-3af3be0d70f1">Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme</a><br />
(Mittel)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=63da8040-fda2-42c7-8543-26ad6f9811f2">Microsoft Internet Explorer 6</a><br />
(Kritisch)<br />
<br />
<a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=75a05d3a-92a0-4a00-95d4-e2b2f6755180">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=e0e63f03-904d-47ee-94fc-51a8dea668eb">Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=126426a7-be38-4327-89db-02d99d76589d">Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme</a><br />
(Hoch)</td>
</tr>
</tbody>
</table>
 

<p> </p>
<table style="border:1px solid black;">
<caption>Windows Vista</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Vista und Windows Vista Service Pack 1</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=9b51deb8-3873-4146-977f-7e3d0840a4c5">Windows Vista und Windows Vista Service Pack 1</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d7f14001-7f42-4ca0-9193-cdf061179b59">Windows Vista und Windows Vista Service Pack 1</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d4e24966-6530-463a-9ee2-f6a9d000f998">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8203d303-c855-4579-9bbf-b06ddf5c1b87">Windows Vista</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=9640cd8b-d749-4ddd-8af9-b298cebed969">Windows Vista und Windows Vista Service Pack 1</a><br />
(Hoch)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=4ad6dcd1-6ea5-43bf-8bee-a5f507beadc6">Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d33462b6-7391-482d-babe-fb4cd0beaa21">Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=295cf8f2-265e-4570-b708-21033337fe05">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=73f3a234-3973-4467-be7e-69efa7ee978c">Windows Vista x64 Edition</a><br />
(Hoch)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=d56bb4fe-304e-45e0-95f2-fde2f47b2a04">Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1</a><br />
(Hoch)</td>
</tr>
</tbody>
</table>
 

<p> </p>
<table style="border:1px solid black;">
<caption>Windows Server 2008</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111955"><strong>MS08-021</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108169"><strong>MS08-022</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=112366"><strong>MS08-023</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=110557"><strong>MS08-024</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=108231"><strong>MS08-020</strong></a></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=111956"><strong>MS08-025</strong></a></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 für 32-Bit-Systeme</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=006d5c47-53e6-4ee1-932c-497611804938">Windows Server 2008 für 32-Bit-Systeme</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=95691924-2813-4a86-9e11-99d853f8e606">Windows Server 2008 für 32-Bit-Systeme</a><br />
(Niedrig)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=e57b4d94-19ad-4818-8311-a3f94be01a4b">Windows Internet Explorer 7</a>*<br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=4497333c-9418-4b91-83dc-0155735421c0">Windows Server 2008 für 32-Bit-Systeme</a><br />
(Hoch)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Windows Server 2008 für x64-basierte Systeme</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=8909f144-655b-4f07-916f-fd967f1efb2b">Windows Server 2008 für x64-basierte Systeme</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=920ae29b-19d0-4089-ac79-f2da824a2256">Windows Server 2008 für x64-basierte Systeme</a><br />
(Niedrig)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=93e9f52a-c7d0-4033-9c12-740665a219af">Windows Internet Explorer 7</a>*<br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=5aefc7a6-79a4-45a2-b534-35d0ec400dda">Windows Server 2008 für x64-basierte Systeme</a><br />
(Hoch)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Windows Server 2008 für Itanium-basierte Systeme</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=b7771a4a-4e4f-48d1-8551-bb8b778ca5a7">Windows Server 2008 für Itanium-basierte Systeme</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=66df79ac-8364-4922-9688-ebc7ec76d89f">Windows Server 2008 für Itanium-basierte Systeme</a><br />
(Niedrig)</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=acf948e8-c4a9-40da-b282-f5e584e77b05">Windows Internet Explorer 7</a><br />
(Kritisch)</td>
<td style="border:1px solid black;">Keine</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=3080c26b-7456-41ef-8668-28f15bc7b8ce">Windows Server 2008 für Itanium-basierte Systeme</a><br />
(Hoch)</td>
</tr>
</tbody>
</table>
 

**\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch diese Updates behobenen Sicherheitsanfälligkeiten wirken sich nicht auf unterstützte Editionen von Windows Server 2008 aus, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Dennoch können die von diesen Sicherheitsanfälligkeiten betroffenen Dateien auf dem System vorhanden sein. Benutzern mit den betroffenen Dateien wird dieses Update jedoch immer noch angeboten, da die Updatedateien neuer sind (höhere Versionsnummern haben) als die Dateien, die derzeit auf Ihrem System vorhanden sind. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft Project</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=115454"><strong>MS08-018</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Kritisch</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2000 Service Release 1</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=fbe46241-b9da-40c6-803d-42eb6234be77">Project 2000 Service Release 1</a><br />
(KB949043)<br />
(Kritisch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Project 2002 Service Pack 1</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=07a90718-6597-426d-9dca-a336d60c01b8">Project 2002 Service Pack 1</a><br />
(KB949005)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Project 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=aaba07d6-e972-4e85-bccd-406aa2c4a4f4">Project 2003 Service Pack 2</a><br />
(KB948962)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
</table>

<p> </p>
<table style="border:1px solid black;">
<caption>Microsoft Visio</caption>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><strong>Kennung des Bulletins</strong></td>
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=115455"><strong>MS08-019</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><strong>Bewertung des maximalen Schweregrads:</strong></td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx"><strong>Hoch</strong></a></td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2002 Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?familyid=0056a936-def5-40fa-bcfc-0ab0dd5c3964">Visio 2002 Service Pack 2</a><br />
(KB947896)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2003 Service Pack 2</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 Service Pack 2</a><br />
(KB947650)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2003 Service Pack 3</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=18af0ce6-99a0-4471-8d26-9700a8a8e631">Visio 2003 Service Pack 3</a><br />
(KB947650)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="even">
<td style="border:1px solid black;">Microsoft Visio 2007</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007</a><br />
(KB947590)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;">Microsoft Visio 2007 Service Pack 1</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/download/details.aspx?displaylang=de&amp;familyid=0510a1bb-b464-452c-900f-7f4e58ed9c7e">Visio 2007 Service Pack 1</a><br />
(KB947590)<br />
(Hoch)</td>
<td style="border:1px solid black;"></td>
</tr>
</tbody>
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
  
-   [National Cyber Security Center](http://www.ncsc.go.kr/eng/), Republik Korea, für den Hinweis auf ein in MS08-018 beschriebenes Problem.  
-   Einer Person, die anonym bleiben möchte, für den Hinweis auf ein in MS08-019 beschriebenes Problem.  
-   Einer Person, die anonym bleiben möchte, für den Hinweis auf ein weiteres, in MS08-019 beschriebenes Problem.  
-   Amit Klein von [Trusteer](http://www.trusteer.com/) für den Hinweis auf ein in MS08-020 beschriebenes Problem.  
-   Alla Berzroutchko von [Scanit](http://www.scanit.be/) für den Hinweis auf ein in MS08-020 beschriebenes Problem.  
-   Roy Arends von [Nominet UK](http://www.nominet.org.uk/) für den Hinweis auf ein in MS08-020 beschriebenes Problem.  
-   Jun Mao von [iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS08-021 beschriebenes Problem.  
-   Sebastian Apelt von [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-021 beschriebenes Problem.  
-   Thomas Garnier von [SkyRecon](http://www.skyrecon.com/) für den Hinweis auf ein in MS08-021 beschriebenes Problem.  
-   Yamata Li von [Palo Alto Networks](http://www.paloaltonetworks.com/) für den Hinweis auf ein in MS08-021 beschriebenes Problem.  
-   Peter Ferrie von [Symantec](http://www.symantec.com/) für den Hinweis auf ein in MS08-022 beschriebenes Problem.  
-   Einer Person, die mit [iDefense VCP](http://labs.idefense.com/vcp/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS08-023 beschriebenes Problem.  
-   Carsten Eiram von [Secunia](http://secunia.com/) für den Hinweis auf ein in MS08-024 beschriebenes Problem.  
-   Thomas Garnier von [SkyRecon](http://www.skyrecon.com/) für den Hinweis auf ein in MS08-025 beschriebenes Problem.
  
#### Support
  
-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.  
-   Technischer Support ist über die [Microsoft Support Services](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.  
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).
  
#### Haftungsausschluss
  
Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.
  
#### Revisionen
  
-   V1.0 (8. April 2008): Bulletin Summary veröffentlicht.  
-   V1.1 (9. April 2008): Aktualisierung der Kurzzusammenfassung für das Microsoft Security Bulletin MS08-018.  
-   V1.2 (16. April 2008): Aktualisierung der Finderinformationen für MS08-021 und Verdeutlichung der „Betroffenen Software“ für Microsoft Office Suites und Software.  
-   V1.3 (18. Februar 2009): Es wurde ein Hinweis in MS08-024 hinzugefügt, dass Server Core-Installationen von Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für x64-basierte Systeme nicht betroffen sind.
  
*Built at 2014-04-18T01:50:00Z-07:00*
