---
TOCTitle: 'MS09-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2009
ms:assetid: 'ms09-feb'
ms:contentKeyID: 61225070
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-feb(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Februar 2009
====================================================

Veröffentlicht: Dienstag, 10. Februar 2009 | Aktualisiert: Mittwoch, 25. Februar 2009

**Version:** 2.1

In diesem Bulletin Summary sind die im Februar 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Februar 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 5. Februar 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 11. Februar 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Februar](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032395122). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten wichtigen Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

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
<th style="border:1px solid black;" >Neustartanforderung:</th>
<th style="border:1px solid black;" >Betroffene Software</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139814">MS09-002</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (961260)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=136636">MS09-003</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen (959239)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Exchange Server. Die erste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn eine speziell gestaltete TNEF-Nachricht an einen Microsoft Exchange Server gesendet wird. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann vollständige Kontrolle über das betroffene System mit Exchange Server-Dienstkontoberechtigungen erlangen. Die zweite Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein speziell gestalteter MAPI-Befehl an einen Microsoft Exchange Server gesendet wird. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann bewirken, dass der Microsoft Exchange-Systemaufsichtsdienst oder andere Dienste, die den EMSMDB32-Provider verwenden, nicht mehr reagieren.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Exchange Server</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=139513">MS09-004</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft SQL Server kann Remotecodeausführung ermöglichen (959420)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft SQL Server. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn nicht vertrauenswürdige Benutzer auf ein betroffenes System zugreifen, oder wenn ein Angriff durch Einschleusung von SQL-Befehlen auf ein betroffenes System ausgeführt wird. Systeme mit SQL Server 7.0 Service Pack 4, SQL Server 2005 Service Pack 3 und SQL Server 2008 sind von diesem Problem nicht betroffen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft SQL Server</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=128107">MS09-005</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Visio können Remotecodeausführung ermöglichen (957634)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Visio, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/en-us/security/cc998259.aspx).
  
| Kennung des Bulletins                                     | Titel des Bulletins                                                                                  | CVE-ID                                                                           | Ausnutzbarkeitsindex – Bewertung                                                                                 | Wichtige Hinweise                                                                                                                                                                                                                     |  
|-----------------------------------------------------------|------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|  
| [MS09-002](http://go.microsoft.com/fwlink/?linkid=139814) | Kumulatives Sicherheitsupdate für Internet Explorer (961260)                                         | [CVE-2009-0075](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0075) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich   | Konsistenter Angreifercode kann problemlos gestaltet werden.                                                                                                                                                                          |  
| [MS09-002](http://go.microsoft.com/fwlink/?linkid=139814) | Kumulatives Sicherheitsupdate für Internet Explorer (961260)                                         | [CVE-2009-0076](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0076) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich   | Konsistenter Angreifercode kann problemlos gestaltet werden.                                                                                                                                                                          |  
| [MS09-003](http://go.microsoft.com/fwlink/?linkid=136636) | Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen (959239)     | [CVE-2009-0098](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0098) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | (Keine)                                                                                                                                                                                                                               |  
| [MS09-003](http://go.microsoft.com/fwlink/?linkid=136636) | Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen (959239)     | [CVE-2009-0099](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0099) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | Es handelt sich um eine Sicherheitsanfälligkeit bezüglich Denial-of-Service. Angriffe, bei denen diese Sicherheitsanfälligkeit ausgenutzt wird, führen wahrscheinlich nur zu einem Denial-of-Service, nicht zu Remotecodeausführung.  |  
| [MS09-004](http://go.microsoft.com/fwlink/?linkid=139513) | Sicherheitsanfälligkeit in Microsoft SQL Server kann Remotecodeausführung ermöglichen (959420)       | [CVE-2008-5416](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-5416) | [**1**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Konsistenter Angreifercode wahrscheinlich   | Nach Authentifizierung wurde funktionaler Angreifercode veröffentlicht.                                                                                                                                                               |  
| [MS09-005](http://go.microsoft.com/fwlink/?linkid=128107) | Sicherheitsanfälligkeiten in Microsoft Office Visio können Remotecodeausführung ermöglichen (957634) | [CVE-2009-0095](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0095) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | (Keine)                                                                                                                                                                                                                               |  
| [MS09-005](http://go.microsoft.com/fwlink/?linkid=128107) | Sicherheitsanfälligkeiten in Microsoft Office Visio können Remotecodeausführung ermöglichen (957634) | [CVE-2009-0096](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0096) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | (Keine)                                                                                                                                                                                                                               |  
| [MS09-005](http://go.microsoft.com/fwlink/?linkid=128107) | Sicherheitsanfälligkeiten in Microsoft Office Visio können Remotecodeausführung ermöglichen (957634) | [CVE-2009-0097](http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0097) | [**2**](http://technet.microsoft.com/en-us/security/cc998259.aspx) – Inkonsistenter Angreifercode wahrscheinlich | (Keine)                                                                                                                                                                                                                               |
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
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
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-002**](http://go.microsoft.com/fwlink/?linkid=139814)
</td>
<td style="border:1px solid black;">
[**MS09-004**](http://go.microsoft.com/fwlink/?linkid=139513)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8cd902ec-e018-4b61-80f9-825d973f998e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=dd3e2236-9cc0-478e-a46c-981ef685c0e3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-002**](http://go.microsoft.com/fwlink/?linkid=139814)
</td>
<td style="border:1px solid black;">
[**MS09-004**](http://go.microsoft.com/fwlink/?linkid=139513)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e52aa1fd-e694-4322-b3ff-6abc1b4a16fe)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=218809d6-a9fb-408b-a34d-ab2ac786994c)  
(KB960082)  
(Hoch)  
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=16925be5-98d0-446b-9bbc-d9a2d335c69e)  
(KB960089)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=edbf1566-b96b-4c7d-98fe-b15f8e766792)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft SQL Server 2000 Desktop Engine (WMSDE)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=87183155-6770-4ea2-acca-191de4d40d27)  
(KB960082)  
(Hoch)  
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=05c5c265-cfd7-4364-b323-77650b7f1e67)  
(KB960089)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5ce78797-d1c0-40d4-84e1-1004389833be)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-002**](http://go.microsoft.com/fwlink/?linkid=139814)
</td>
<td style="border:1px solid black;">
[**MS09-004**](http://go.microsoft.com/fwlink/?linkid=139513)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5f9fa4b6-85a4-43bc-b84f-6bd847799650)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e9a8c94b-b9d2-4d64-855f-b5f02ce3dfb5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-002**](http://go.microsoft.com/fwlink/?linkid=139814)
</td>
<td style="border:1px solid black;">
[**MS09-004**](http://go.microsoft.com/fwlink/?linkid=139513)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2491dbf2-7cd3-44f1-bfad-77e6f760a25c)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Internal Database (WYukon) Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=16925be5-98d0-446b-9bbc-d9a2d335c69e)\*  
(KB960089)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=794373cc-2dce-4ef5-af50-7804c622c230)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Internal Database (WYukon) x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=05c5c265-cfd7-4364-b323-77650b7f1e67)\*  
(KB960089)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=11985325-4b33-4077-82cf-6afc7a71c510)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**Hinweis für MS09-004**

Im Abschnitt **Microsoft Server Software** finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Windows-Betriebssystem als auch Komponenten und Microsoft Server-Software.

#### Microsoft Server-Software

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
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-003**](http://go.microsoft.com/fwlink/?linkid=136636)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange 2000 Server
</td>
<td style="border:1px solid black;">
[Microsoft Exchange 2000 Server Service Pack 3 mit dem Update-Rollup von August 2004](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=805dc856-ea60-477d-be40-6ac535a7e7e5)  
(KB959897)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2003
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1d9f0956-88bd-4e13-a86b-b1c8d4782f71)\*  
(KB959897)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=93cb3f66-ae72-4356-bdbf-35029cff6df1)\*\*  
(KB959241)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server MAPI-Client und Datenobjekte für die Zusammenarbeit 1.2.1
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server MAPI-Client und Datenobjekte für die Zusammenarbeit 1.2.1](http://www.microsoft.com/downloads/details.aspx?familyid=e17e7f31-079a-43a9-bff2-0a110307611e)\*\*\*  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise für MS09-003**

\*Umfasst das Exchange-Systemverwaltungstool für Exchange Server 2003, wenn auf dem Server ebenfalls eine aktive Instanz des Exchange-Diensts ausgeführt wird.

\*\*Umfasst 32-Bit und x64-basierte Editionen

\*\*\*Der Microsoft Exchange Server MAPI-Client enthält den anfälligen Code. Zum Schutz vor den in MS09-003 beschriebenen Sicherheitsanfälligkeiten müssen Benutzer, die den Microsoft Exchange Server MAPI-Client ausführen, auf Version 6.5.8069 des MAPI-Clients aktualisieren. 

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
[**MS09-004**](http://go.microsoft.com/fwlink/?linkid=139513)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d5bb816a-6e1a-47cb-92be-51c565ee184c)  
(KB960082)  
(Hoch)  
QFE-Update:  
[SQL Server 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a93f3cfe-18c9-4218-a551-13bf415e418a)  
(KB960083)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2000 Itanium-basierte Edition Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2000 Itanium-basierte Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d5bb816a-6e1a-47cb-92be-51c565ee184c)  
(KB960082)  
(Hoch)  
QFE-Update:  
[SQL Server 2000 Itanium-basierte Edition Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a93f3cfe-18c9-4218-a551-13bf415e418a)  
(KB960083)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5dfb7998-0316-40e5-9fc5-7a1afc18e15e)  
(KB960089)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa2b82ca-e94e-4491-8639-f0749b1a0f3a)  
(KB960090)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5dfb7998-0316-40e5-9fc5-7a1afc18e15e)  
(KB960089)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa2b82ca-e94e-4491-8639-f0749b1a0f3a)  
(KB960090)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5dfb7998-0316-40e5-9fc5-7a1afc18e15e)  
(KB960089)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa2b82ca-e94e-4491-8639-f0749b1a0f3a)  
(KB960090)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d5bb816a-6e1a-47cb-92be-51c565ee184c)  
(KB960082)  
(Hoch)  
QFE-Update:  
[Microsoft SQL Server 2000 Desktop Engine (MSDE 2000) Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a93f3cfe-18c9-4218-a551-13bf415e418a)  
(KB960083)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Express Edition Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5dfb7998-0316-40e5-9fc5-7a1afc18e15e)  
(KB960089)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa2b82ca-e94e-4491-8639-f0749b1a0f3a)  
(KB960090)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Express Edition mit Advanced Services Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5dfb7998-0316-40e5-9fc5-7a1afc18e15e)  
(KB960089)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=aa2b82ca-e94e-4491-8639-f0749b1a0f3a)  
(KB960090)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS09-004**

Weitere Updatedateien finden Sie auch in dem Abschnitt **Windows-Betriebssystem und Komponenten**. Dieses Bulletin umfasst sowohl Windows-Betriebssystem als auch Komponenten und Microsoft Server-Software.

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
Microsoft Office Visio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-005**](http://go.microsoft.com/fwlink/?linkid=128107)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio 2002
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2002 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a30cef3f-9eaf-45bd-9a25-4b65302362cb)  
(KB955654)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Visio 2003
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c9cb589e-1a37-485d-8402-7f42bcd7a1a9)  
(KB955655)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Visio 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b711e89-8de2-4f17-8afc-691e0604ff82)  
(KB957831)  
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

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/bb466214.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

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

-   [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-002 beschriebenes Problem.
-   Sam Thomas (<http://eshu.co.uk/>), der mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS09-002 beschriebenes Problem.
-   Bogdan Materna von [VoIPshield Systems](http://www.voipshield.com) für den Hinweis auf ein in MS09-003 beschriebenes Problem.
-   Bernhard Mueller von [SEC Consult Vulnerability Lab](http://www.sec-consult.com/) für den Hinweis auf ein in MS09-004 beschriebenes Problem.
-   Bing Liu von Fortinets [FortiGuard Global Security Research Team](http://www.fortiguardcenter.com/) für den Hinweis auf mehrere in MS09-005 beschriebene Probleme.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (10. Februar 2009): Bulletin Summary veröffentlicht.
-   V2.0 (16. Februar 2009): Microsoft Exchange Server MAPI-Client wurde als betroffene Software für MS09-003 hinzugefügt.
-   V2.1 (25. Februar 2009): Es wurde ein Hinweis bezüglich der Exchange-Systemverwaltungstools für Exchange Server 2003 für MS09-003 hinzugefügt.

*Built at 2014-04-18T01:50:00Z-07:00*
