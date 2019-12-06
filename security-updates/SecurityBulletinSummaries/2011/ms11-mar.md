---
TOCTitle: 'MS11-MAR'
Title: Microsoft Security Bulletin Summary für März 2011
ms:assetid: 'ms11-mar'
ms:contentKeyID: 61225098
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-mar(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für März 2011
=================================================

Veröffentlicht: Dienstag, 8. März 2011 | Aktualisiert: Mittwoch, 16. März 2011

**Version:** 1.1

In diesem Bulletin Summary sind die im März 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für März 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 3. März 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 9. März 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im März](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032455049&eventcategory=4). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

Kurzzusammenfassungen
---------------------

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software und Downloadadressen**.

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel des Bulletins und Kurzzusammenfassung</th>
<th style="border:1px solid black;" >Bewertung des maximalen Schweregrads und Sicherheitsauswirkung</th>
<th style="border:1px solid black;" >Neustartanforderung</th>
<th style="border:1px solid black;" >Betroffene Software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207841">MS11-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Media Runtime können Remotecodeausführung ermöglichen (2510030)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in DirectShow und eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Player und Windows Media Center. Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete DVR-MS-Datei (Microsoft Digital Video Recording-Datei) öffnet. In allen Fällen kann ein Benutzer nicht gezwungen werden, die Datei zu öffnen. Damit ein Angriff erfolgreich ist, muss ein Benutzer dazu verleitet werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207892">MS11-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Remotedesktopclient kann Remotecodeausführung ermöglichen (2508062)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Windows Remotedesktopclient. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine gültige RDP-Konfigurationsdatei (Remotedesktop) öffnet, die sich im selben Netzwerkordner befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=209774">MS11-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Outlook kann Remotecodeausführung ermöglichen (2494047)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Groove, die Remotecodeausführung ermöglichen kann, wenn ein Benutzer eine gültige, Groove-bezogene Datei öffnet, die sich in dem gleichen Netzwerkverzeichnis befindet wie eine speziell gestaltete Bibliotheksdatei. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
| Kennung des Bulletins                                     | Titel der Sicherheitsanfälligkeit                                                               | CVE-ID                                                                           | Ausnutzbarkeitsindex - Bewertung                                                                      | Wichtige Hinweise                                                                             |  
|-----------------------------------------------------------|-------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------|  
| [MS11-016](https://go.microsoft.com/fwlink/?linkid=209774) | Sicherheitsanfälligkeit in Microsoft Groove aufgrund des nicht sicheren Ladens von Bibliotheken | [CVE-2010-3146](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3146) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet, und u. U. ist PoC-Code verfügbar** |  
| [MS11-017](https://go.microsoft.com/fwlink/?linkid=207892) | Sicherheitsanfälligkeit in Remotedesktop aufgrund des nicht sicheren Ladens von Bibliotheken    | [CVE-2011-0029](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0029) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.**                                  |  
| [MS11-015](https://go.microsoft.com/fwlink/?linkid=207841) | Sicherheitsanfälligkeit durch nicht sichereres Laden von Bibliotheken in DirectShow             | [CVE-2011-0032](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0032) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich | **Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet, und u. U. ist PoC-Code verfügbar** |  
| [MS11-015](https://go.microsoft.com/fwlink/?linkid=207841) | Sicherheitsanfälligkeit in DVR-MS                                                               | [CVE-2011-0042](https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0042) | [1](https://technet.microsoft.com/de-de/security/cc998259) - Konsistenter Angreifercode wahrscheinlich | (Keine)                                                                                       |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis**: Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
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
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d8284bfa-ed6c-4647-9fb0-588e53173775)  
(KB2479943)  
(Kritisch)  
[Windows XP Media Center Edition 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b1be30de-7e88-467d-aee2-68f88e6a7355)  
(KB2502898)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 5.2](https://www.microsoft.com/download/details.aspx?familyid=1aed6080-feab-4b5e-9d26-6a3f4b92434d)  
(KB2483618)  
(Hoch)  
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=d67e4d8c-aeb9-45e6-9555-7456c5540475)  
(KB2481109)  
(Hoch)  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=6a01992e-c9a1-4dc9-a3ef-7410b81f17e6)  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5270b5d3-3720-42a2-a8cf-67089c0cc658)  
(KB2479943)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.0](https://www.microsoft.com/download/details.aspx?familyid=6d4539ef-4a05-4c7d-9489-436f7b7a3ebe)<sup>[1]</sup>
(KB2481109)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.0](https://www.microsoft.com/download/details.aspx?familyid=641d5d12-0790-4551-831a-e78febad17a7)<sup>[1]</sup>
(KB2481109)  
(Hoch)  
[Mehrsprachige Benutzeroberfläche (MUI) des Remotedesktopverbindungs-Clients 6.0](https://www.microsoft.com/download/details.aspx?familyid=6fec0d06-042d-4e55-9843-009edd7d26ce)<sup>[2]</sup>
(KB2483619)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.0](https://www.microsoft.com/download/details.aspx?familyid=78dbb9cf-8a18-4f0a-8edf-f1ce0c993c63)<sup>[1]</sup>
(KB2481109)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f9f1dde2-2219-4bf1-a497-edd011577b96)<sup>[1]</sup>
(KB2479943)  
(Kritisch)  
[Windows Media Center TV Pack für Windows Vista (32-Bit-Editionen](https://www.microsoft.com/download/details.aspx?familyid=1bc240b3-1938-4350-b26f-67b81a79f8a0))<sup>[2]</sup>
(KB2494132)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=e3ea7690-386b-4cdf-889f-b3914921c56f)  
(KB2481109)  
(Hoch)  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=3c30f67e-7c31-4553-ba3e-e056df1bf8eb)  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e11d00df-d1cf-4a33-a1be-6721cdff5995)<sup>[1]</sup>
(KB2479943)  
(Kritisch)  
[Windows Media Center TV Pack für Windows Vista (64-Bit-Editionen](https://www.microsoft.com/download/details.aspx?familyid=cd4c5a80-db24-4696-a248-1286c3b9f550))<sup>[2]</sup>
(KB2494132)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=5735bed6-0e3d-46a4-85d0-14ec34a82edd)  
(KB2481109)  
(Hoch)  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=8025482b-f58f-4f5a-a133-5563c65b21f6)  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=31d790c9-92f9-4a2b-800b-8e8d2b570bb9)\*\*  
(KB2481109)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=5b0a8eb5-4bc2-4054-b952-58aa645afcf5)\*\*  
(KB2481109)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](https://www.microsoft.com/download/details.aspx?familyid=25da7e00-745d-4d98-9dd8-52a8a4340404)  
(KB2481109)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1be77daa-29b1-4dae-a87f-2cb8f7e6a305)  
(KB2479943)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme:  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=0768a5f4-da28-4b2e-8aff-d68f890df3e6)  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=56fb24ce-65c7-4573-b613-e424ccc1a3a6)  
(KB2479943)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für x64-basierte Systeme:  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=935adb10-1e7e-4501-b543-8247b88f6d18)  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-015**](https://go.microsoft.com/fwlink/?linkid=207841)
</td>
<td style="border:1px solid black;">
[**MS11-017**](https://go.microsoft.com/fwlink/?linkid=207892)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6f45658a-1db8-4ef5-b840-4d0180d4d90e)\*\*  
(KB2479943)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Remotedesktopverbindungs-Client 7.0](https://www.microsoft.com/download/details.aspx?familyid=3fcb2e11-591e-484a-a992-2f1d563e6d17)\*\*  
(KB2483614)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Clients 7.0](https://www.microsoft.com/download/details.aspx?familyid=c29b6487-78f0-421c-810c-c5e45d6a2352)  
(KB2483614)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für Windows Server 2008 und Windows Server 2008 R2**

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweise für MS11-015**

<sup>[1]</sup>Siehe Hinweis <sup>[2]</sup> unten bezüglich Windows Media Center TV Pack für Windows Vista.

<sup>[2]</sup>Windows Media Center TV Pack für Windows Vista ist nur auf OEM-Installationen (Originalgerätehersteller) der Home Premium- und Ultimate-Editionen von Windows Vista als optionale Komponente verfügbar. Benutzer, die diese optionale Komponente auf ihren Systemen installiert haben, sollten beide verfügbaren Updates installieren. Im Einklang mit den empfohlenen Vorgehensweisen empfiehlt Microsoft, das Update des Betriebssystems (KB2479943) zu installieren, bevor das Windows Media Center TV Pack-Update (KB2494132) installiert wird.

**Hinweise für MS11-017**

<sup>[1]</sup>Mit diesem Download wird der Remotedesktopverbindungs-Client 6.0 auf eine nicht betroffene Version von Remotedesktopverbindungs-Client 6.1 aktualisiert.

<sup>[2]</sup>Mit diesem Download wird die mehrsprachige Benutzeroberfläche (MUI) des Remotedesktopverbindungs-Clients 6.0 auf eine nicht betroffene Version der mehrsprachigen Benutzeroberfläche (MUI) des Remotedesktopverbindungs-Clients 6.1 aktualisiert.

#### Microsoft Office Suites und Software

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
Microsoft Office-Programme
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-016**](https://go.microsoft.com/fwlink/?linkid=209774)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Groove 2007
</td>
<td style="border:1px solid black;">
[Microsoft Groove 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3981ab53-1082-4155-9000-11d8a976ff33)  
(KB2494047)  
(Hoch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**System Center Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](https://www.microsoft.com/germany/systemcenter/sccm/evaluation/updatemgmt.mspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/common/international.aspx?rdpath=dm;de-de;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&amp;displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Security Guidance für Updateverwaltung](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Matthew Watchinski von [Sourcefire VRT](https://www.sourcefire.com/services/sf_vrt.html) für den Hinweis auf ein in MS11-015 beschriebenes Problem.
-   HD Moore von [Rapid 7](https://www.rapid7.com/) für den Hinweis auf ein in MS11-016 beschriebenes Problem
-   Eyal Gruner von [Versafe Anti Fraud](https://www.versafe-login.com/) für den Hinweis auf ein in MS11-017 beschriebenes Problem

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (8. März 2011): Bulletin Summary veröffentlicht.
-   V1.1 (16. März 2011): Aus dem Abschnitt **Betroffene Software und Downloadadressen** in den Hinweisen für MS11-015 wurde ein fehlerhafter Verweis auf Windows XP Home Edition Service Pack 3 und Windows XP Tablet PC Edition Service Pack 3 als nicht betroffen entfernt. Dies ist lediglich eine Informationsänderung. An den Dateien des Sicherheitsupdates oder der Erkennungslogik wurden keine Änderungen vorgenommen. Benutzern, die diese Editionen von Windows XP ausführen und dieses Update nicht bereits übernommen haben, empfiehlt Microsoft, das Update sofort zu installieren. Benutzer, die dieses Update bereits installiert haben, müssen keine Maßnahmen ergreifen.

*Built at 2014-04-18T01:50:00Z-07:00*