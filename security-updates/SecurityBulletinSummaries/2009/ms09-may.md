---
TOCTitle: 'MS09-MAY'
Title: Microsoft Security Bulletin Summary für Mai 2009
ms:assetid: 'ms09-may'
ms:contentKeyID: 61225075
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-may(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Mai 2009
================================================

Veröffentlicht: Dienstag, 12. Mai 2009 | Aktualisiert: Dienstag, 9. Juni 2009

**Version:** 2.0

In diesem Bulletin Summary sind die im Mai 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Mai 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 7. Mai 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 13. Mai 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Mai](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395223). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und mehrere vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office PowerPoint, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete PowerPoint-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
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

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel des Bulletins</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Ausnutzbarkeitsindex – Bewertung</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0220">CVE-2009-0220</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0221">CVE-2009-0221</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0222">CVE-2009-0222</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0223">CVE-2009-0223</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0224">CVE-2009-0224</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0225">CVE-2009-0225</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0226">CVE-2009-0226</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0227">CVE-2009-0227</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0556">CVE-2009-0556</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wird derzeit in der Internetumgebung ausgenutzt.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1128">CVE-2009-1128</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1129">CVE-2009-1129</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1130">CVE-2009-1130</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1131">CVE-2009-1131</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=141704">MS09-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office PowerPoint können Remotecodeausführung ermöglichen (967340)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1137">CVE-2009-1137</a></td>
<td style="border:1px solid black;">Für Office-Versionen, die ohne /GS kompiliert wurden:<br />
<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Der /GS-Schutz, der beim Kompilieren von Office 2003 Service Pack 3 und höheren Office-Versionen erstellt wurde, ist ein schadensbegrenzender Faktor für diese Sicherheitsanfälligkeit. Dadurch wird das Risiko für solche Systeme deutlich auf „<a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich“ reduziert.</td>
</tr>
</tbody>
</table>
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Prüfen Sie für jede aufgeführte Kennung der Bulletins die gesamte Spalte, um basierend auf den in Ihrem System installierten Programmen und Komponenten alle Updates zu finden, die Sie installieren müssen.
  
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
Microsoft Office Suites, Systeme und Komponenten  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-017**](http://go.microsoft.com/fwlink/?linkid=141704)
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
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f443312a-ac74-4ebc-a4ac-7a756aa67894)  
(KB957790)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=a24ec7ab-c1c7-4ddb-8b6e-107f1af67f49)  
(KB957781)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=ccfa978b-3340-40db-a45d-c880ba36b106)  
(KB957784)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1 und Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint 2007 Service Pack 1 und Microsoft Office PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=11f8380f-ffb6-4c22-a89c-3dc55d0f9834)  
(KB957789)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-017**](http://go.microsoft.com/fwlink/?linkid=141704)
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
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-017**](http://go.microsoft.com/fwlink/?linkid=141704)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
PowerPoint Viewer
</td>
<td style="border:1px solid black;">
[PowerPoint Viewer 2003](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=6a57e6ed-bd24-406f-87bb-117391e083e0)  
(KB969615)  
(Hoch)  
[PowerPoint Viewer 2007 Service Pack 1 und PowerPoint Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=141b8338-5c52-4326-a9e4-d2f2d8940d9c)  
(KB970059)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=e1d3a4c3-538a-4f98-8d60-250803a80e2a)  
(KB969618)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS09-017**

Microsoft hat MS09-017 erneut veröffentlicht, um Sicherheitsupdatepakete für Microsoft Office 2004 für Mac, Microsoft Office 2008 für Mac, Open XML-Dateiformatkonverter für Mac, Microsoft Works 8.5 und Microsoft Works 9 bereitzustellen. Benutzer, die diese Software besitzen, sollten dieses Update sofort installieren.

Als MS09-017 zuerst veröffentlicht wurde, befanden sich diese Sicherheitsupdatepakete noch in der Entwicklung. Microsoft hat MS09-017 zu jener Zeit veröffentlicht, weil Updatepakete im regulären Veröffentlichungszeitraum der Bulletins für eine gesamte Produktreihe bereitstanden, um die überwiegende Mehrheit der gefährdeten Benutzer zu schützen. Diese aktuelle Veröffentlichung von MS09-017 vervollständigt nun die Reihe der Updates für Software, die von den in diesem Bulletin erörterten Sicherheitsanfälligkeiten betroffen ist.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

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

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc766043.aspx), die im [Microsoft Application Compatibility Toolkit 5.0](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](http://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf zwei in MS09-017 beschriebene Probleme.
-   Sean Larsson von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf zwei in MS09-017 beschriebene Probleme.
-   Nicolas Joly von [VUPEN Security](http://www.vupen.com/) für den Hinweis auf ein in MS09-017 beschriebenes Problem.
-   Marsu Pilami von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf mehrere in MS09-017 beschriebene Probleme.
-   Nicolas Joly von [VUPEN Security](http://www.vupen.com/) für den Hinweis auf ein in MS09-017 beschriebenes Problem.
-   Marsu Pilami in Zusammenarbeit mit [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-017 beschriebenes Problem.
-   Ling und Wushi von [team509](http://www.team509.com/) in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und [Zero Day Initiative](http://www.zerodayinitiative.com/) und Sean Larsson von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS09-017 beschriebenes Problem.
-   Carsten H. Eiram von [Secunia Research](http://secunia.com/) für den Hinweis auf ein in MS09-017 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (12. Mai 2009): Bulletin Summary veröffentlicht.
-   V1.1 (13. Mai 2009): Es wurde ein fehlerhafter Hinweis für MS09-017 entfernt, der die Sicherheitsupdates KB969618 und KB957789 für unterstützte Versionen von Microsoft Office PowerPoint 2007 betrifft.
-   V2.0 (9. Juni 2009): Das Bulletin Summary wurde überarbeitet, um die erneute Veröffentlichung von MS09-017 anzukündigen. MS09-017 wird erneut veröffentlicht, um Sicherheitsupdatepakete für Microsoft Office 2004 für Mac, Microsoft Office 2008 für Mac, Open XML-Dateiformatkonverter für Mac, Microsoft Works 8.5 und Microsoft Works 9 bereitzustellen. Benutzer, die diese Software besitzen, sollten dieses Update sofort installieren.

*Built at 2014-04-18T01:50:00Z-07:00*
