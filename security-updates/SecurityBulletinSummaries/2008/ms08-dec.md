---
TOCTitle: 'MS08-DEC'
Title: Microsoft Security Bulletin Summary für Dezember 2008
ms:assetid: 'ms08-dec'
ms:contentKeyID: 61225057
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms08-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Dezember 2008
=====================================================

Veröffentlicht: Dienstag, 9. Dezember 2008 | Aktualisiert: Mittwoch, 29. April 2009

**Version:** 6.0

In diesem Bulletin Summary sind die im Dezember 2008 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Dezember 2008 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 4. Dezember 2008 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification.](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 10. Dezember 2008 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Dezember.](http://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032374647) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

Für das außerplanmäßige Security Bulletin MS08-078, das Version 3.0 dieses Bulletin Summary hinzugefügt wurde, stellt Microsoft zwei Webcasts bereit, um Kundenfragen zu diesen Bulletins zu beantworten: am 17. Dezember 2008 um 13:00 Uhr pazifischer Zeit (USA & Kanada) und am 18. Dezember 2008 um 11:00 Uhr pazifischer Zeit. Registrieren Sie sich jetzt für den [Webcast am 17. Dezember](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032399448&culture=en-us) und den [Webcast am 18. Dezember](http://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032399449&culture=en-us). Später sind diese Webcasts auf Anfrage verfügbar. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in GDI können Remotecodeausführung ermöglichen (956802)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in GDI. Die Ausnutzung einer dieser beiden Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete WMF-Bilddatei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in der Windows-Suche können Remotecodeausführung ermöglichen (959349)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in der Windows-Suche. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer in Windows Explorer eine speziell gestaltete gespeicherte Suchdatei öffnet und speichert oder wenn ein Benutzer auf eine speziell gestaltete Such-URL klickt. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (958215)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=137335">MS08-078</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsupdate für Internet Explorer (960714)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in den ActiveX-Steuerelementen für die Microsoft Visual Basic 6.0 Runtime Extended Files. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine Website durchsucht, die speziell gestaltete Inhalte enthält. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Entwicklertools und -software, Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</strong><br />
<br />
Dieses Sicherheitsupdate behebt acht vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Word und Microsoft Office Outlook, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Word- oder RTF-Datei (Rich Text-Format) öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (959070)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Excel, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Nutzt ein Angreifer diese Sicherheitsanfälligkeiten erfolgreich aus, kann er vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126307">MS08-077</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office SharePoint Server kann Erhöhung von Berechtigungen verursachen (957175)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer die Authentifizierung umgeht, indem er auf einer SharePoint-Website zu einer administrativen URL navigiert. Ein erfolgreicher Angriff, der zur Erhöhung von Berechtigungen führt, kann zu Denial-of-Service oder Offenlegung von Information führen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office, Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows Media-Komponenten können Remotecodeausführung ermöglichen (959807)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in den folgenden Windows Media-Komponenten: Windows Media Player, Windows Media Format Runtime und Windows Media-Dienste. Die schwerste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen. Wenn ein Benutzer mit administrativen Benutzerrechten angemeldet ist, kann ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, vollständige Kontrolle über ein betroffenes System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3704">CVE-2008-3704</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Konsistenter Angreifercode ist öffentlich verfügbar</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4252">CVE-2008-4252</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4256">CVE-2008-4256</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4253">CVE-2008-4253</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4254">CVE-2008-4254</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=130478">MS08-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Visual Basic 6.0 Runtime Extended Files (ActiveX-Steuerelemente) können Remotecodeausführung ermöglichen (932349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4255">CVE-2008-4255</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Systeme mit Windows 2000 sind am stärksten gefährdet. Es ist unwahrscheinlich, dass Windows XP SP2, Windows Server 2003 SP1 und höhere Betriebssysteme aufgrund ihres stärkeren Heapschutzes durch funktionalen Angreifercode betroffen sind</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in GDI können Remotecodeausführung ermöglichen (956802)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3465">CVE-2008-3465</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125440">MS08-071</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in GDI können Remotecodeausführung ermöglichen (956802)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-2249">CVE-2008-2249</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4024">CVE-2008-4024</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4025">CVE-2008-4025</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4026">CVE-2008-4026</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4027">CVE-2008-4027</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4028">CVE-2008-4028</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4030">CVE-2008-4030</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4837">CVE-2008-4837</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126306">MS08-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (957173)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4031">CVE-2008-4031</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4258">CVE-2008-4258</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4259">CVE-2008-4259</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4261">CVE-2008-4261</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=133437">MS08-073</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (958215)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4260">CVE-2008-4260</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4265">CVE-2008-4265</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4266">CVE-2008-4266</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=131481">MS08-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (959070)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4264">CVE-2008-4264</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in der Windows-Suche können Remotecodeausführung ermöglichen (959349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4269">CVE-2008-4269</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=132148">MS08-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in der Windows-Suche können Remotecodeausführung ermöglichen (959349)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4268">CVE-2008-4268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Windows Media-Komponenten können Remotecodeausführung ermöglichen (959807)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3009">CVE-2008-3009</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Für dieses Problem kann konsistenter Angreifercode erstellt werden. Die Begrenztheit der Angriffsszenarios bedeutet jedoch, dass tatsächliche Angriffe unwahrscheinlich sind.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=125419">MS08-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Windows Media-Komponenten können Remotecodeausführung ermöglichen (959807)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-3010">CVE-2008-3010</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Für dieses Problem kann konsistenter Angreifercode erstellt werden. Die Begrenztheit der Angriffsszenarios bedeutet jedoch, dass tatsächliche Angriffe unwahrscheinlich sind.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=126307">MS08-077</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office SharePoint Server kann Erhöhung von Berechtigungen verursachen (957175)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4032">CVE-2008-4032</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Für dieses Problem kann konsistenter Angreifercode erstellt werden. Angriffe, durch die diese Sicherheitsanfälligkeit ausgenutzt wird, führen jedoch wahrscheinlich nur zur Offenlegung von Information, nicht zu Remotecodeausführung.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=137335">MS08-078</a></td>
<td style="border:1px solid black;">Sicherheitsupdate für Internet Explorer (960714)</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2008-4844">CVE-2008-4844</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich<br />
(Öffentlich bei Veröffentlichung des Bulletins)</td>
<td style="border:1px solid black;">Konsistenter Angreifercode wurde in aktiven Angriffen entdeckt. Internet Explorer wird jedoch bei Standardinstallationen von Windows Vista und Windows Server 2008 im geschützten Modus ausgeführt und behindert dadurch die Ausnutzung.</td>
</tr>
</tbody>
</table>
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=3b775fb1-1077-455d-af4a-4ccb5237974f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c242ba42-556b-4c87-bf33-9d99166ff096)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c0583745-7e57-4265-9429-c3415cb8465f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](http://www.microsoft.com/downloads/details.aspx?familyid=d3e18732-47f1-40ce-999c-d1fd283bf138)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=124c14b6-9323-4f6f-902b-727aa56444bc)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=c33d558e-45f9-4e85-b48c-03bd0e8cb4bc)  
(KB954600)  
(Hoch)  
[Windows Media Format Runtime 7.1 und Windows Media Format Runtime 9.0](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6a459497-0ab8-41cb-87d0-b551631d8d8a)  
(KB952069)  
(Hoch)  
[Windows Media-Dienste 4.1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=58b7d241-cef6-48fa-aa52-017695f71db1)  
(KB952068)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=2151fbba-c464-4d1e-82d4-5b096e82bed0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=af9a6cb0-725d-490c-9858-16ec40e98560)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1b582695-b3cc-4c65-bc4b-d673c9a6d82a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=1d83e0af-46fa-4bfc-ba57-635435a7ef2d)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=0190a289-164e-41a7-8c01-fa1aaed3f531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99241309-e644-4088-a8f3-38837fab4037)  
(KB954600)  
(Hoch)  
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 und Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=504f816c-f554-4b93-ac28-b085574d9bac)  
(Nur Windows XP Service Pack 2)  
(KB952069)  
(Hoch)  
[Windows Media Format Runtime 9.0, Windows Media Format Runtime 9.5 und Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ad76fcf3-a2f9-4e36-bd1b-c1536749173c)  
(Nur Windows XP Service Pack 3)  
(KB952069)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2247f6a5-aa33-4c68-9ea8-a63488d126d3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=60bf9851-24fe-4658-8333-d353e82063c7)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=107cf54b-29d4-4c54-b091-2b5b3ffbf49d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=a585cb73-2c1a-4fa8-862a-ad6aeaeaf2f8)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9ba71e23-8cef-4399-b215-983b0dcf5cb5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?familyid=946d47c9-b208-4fab-8ef6-774413d61bc8)  
(KB954600)  
(Hoch)  
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?familyid=644ef023-ee40-45b0-9c9d-c76d9fab0005)  
(KB952069)  
(Hoch)  
[Windows Media Format Runtime 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ae9e8b07-5354-42f3-a226-ba2193244524)  
(KB952069)  
(Hoch)  
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?familyid=2dadc017-2be5-4240-ab8f-0291756dca6b)  
(KB952069)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 1 und Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0c396796-0929-4cd2-99e8-3c0f7075a89e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d53adf6f-9501-4862-a1ca-57eb4d40cd75)  
(Mittel)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9cdd4f9e-c578-405c-af9e-628f2d77fdf4)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=d81e9cf9-ce0c-463a-a359-49a348cb89ae)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=388847ec-817e-45cf-8fa7-32c7e1f57f80)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2315ce20-2f46-42c2-bb40-045f003409d7)  
(KB954600)  
(Hoch)  
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d8958248-c889-499e-a6a9-3b394cdb27ea)  
(KB952069)  
(Hoch)  
[Windows Media-Dienste 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e71abc2d-d60e-444a-9b7b-062c5805fe9e)  
(KB952068)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6d5c7d2f-1a82-4cdf-b3f2-b2c2390c6a64)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5e37cb34-32be-4bbe-87f3-c4e1974e4d00)  
(Mittel)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=7c36f92c-d8a0-4b70-b85f-83588a0299a0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=015df302-d79f-43a1-b5c5-32ac04de0510)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=2ae17caf-6204-470e-8480-380d3d505657)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Player 6.4](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4c29bed9-1b88-4d2f-80a5-305c2bedd89f)  
(KB954600)  
(Hoch)  
[Windows Media Format Runtime 9.5](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2278022e-a716-46c0-bedf-d626933bd815)  
(KB952069)  
(Hoch)  
[Windows Media Format Runtime 9.5 x64 Edition](http://www.microsoft.com/downloads/details.aspx?familyid=ae9e8b07-5354-42f3-a226-ba2193244524)  
(KB952069)  
(Hoch)  
[Windows Media-Dienste 9](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e0030155-1a9a-46cc-bbc8-6d0d1ed65c1f)  
(KB952068)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP1 für Itanium-basierte Systeme und Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=1edb62b4-3d0f-4891-b4b3-8f8bc4e7bdfe)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0da4e424-4682-4401-a226-7d8f1be19d44)  
(Mittel)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3811030d-5958-4b91-b5b8-20587dc7c4d6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=18016305-7f72-47f6-ab4c-94282289bf5f)  
(Kritisch)  
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=97d6c093-f68d-4ddf-8e3c-f29662a1940f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista und Windows Vista Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cddf9cf6-bdeb-4429-823a-879387a428d7)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0dcc5373-0435-42d5-864d-298e5bb122d9)  
(KB958623)  
(Hoch)  
[Windows Vista und Windows Vista Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5b1b65f0-6848-47c6-bdd5-be3c0621b323)  
(KB958624)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3f62030a-9ce2-4c92-b948-143a6881921e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=7887111d-4fac-4823-bdd2-a18d9468fdf0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1fcdc8dd-26d9-4d1a-8b3f-7b6a21a95999)  
(KB952069)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=73dc3775-b6f0-40f1-bd36-6b5fb80eb2fa)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2112c5c8-7c9f-4491-b127-b1093085e105)  
(KB958623)  
(Hoch)  
[Windows Vista x64 Edition und Windows Vista x64 Edition Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eb1d0ffe-1644-457b-9e82-768bd4c7f7ab)  
(KB958624)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=d8800493-fba4-41f8-bde5-a53eeaf89d54)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=69979d92-8d45-47fe-ac4c-c2f1f23cf1fb)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8839f6cd-dfbf-448c-bf1e-1da9bb5f3f25)  
(KB952069)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-071**](http://go.microsoft.com/fwlink/?linkid=125440)
</td>
<td style="border:1px solid black;">
[**MS08-075**](http://go.microsoft.com/fwlink/?linkid=132148)
</td>
<td style="border:1px solid black;">
[**MS08-073**](http://go.microsoft.com/fwlink/?linkid=133437)
</td>
<td style="border:1px solid black;">
[**MS08-078**](http://go.microsoft.com/fwlink/?linkid=137335)
</td>
<td style="border:1px solid black;">
[**MS08-076**](http://go.microsoft.com/fwlink/?linkid=125419)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=bbed9e8b-e75e-44ef-ba1d-fd6f852c1f67)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=90ab7e6f-5ae7-4f55-8838-868fc98d8a16)\*\*\*  
(KB958623)  
(Hoch)  
[Windows Server 2008 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=470d506f-77ae-4a44-8598-df645f484295)\*\*\*  
(KB958624)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=45a0de3c-c7d1-4314-a456-1f7428b7c90a)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5552e564-dd1c-4e2a-9a42-6317522c884d)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=91ec4195-bc1c-444e-a7b0-ebde46c088fa)  
(KB952069)  
(Hoch)  
[Windows Media-Dienste 2008](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ffb5d945-7f98-4849-b020-ed4873fa42df)\*  
(KB952068)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media-Dienste 2008](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ffb5d945-7f98-4849-b020-ed4873fa42df)\*  
(KB952068)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=48aecf4c-1296-490d-ba37-a28e3ec19bd6)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e1deab57-ada2-4b12-9157-5615e7b0071d)\*\*\*  
(KB958623)  
(Hoch)  
[Windows Server 2008 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e41f23e4-6a2f-4ebb-b425-d241a08da316)\*\*\*  
(KB958624)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=405b28db-47d7-4d6b-90e6-834c0a409323)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=889c6eb1-7d1f-4e60-b637-535cb6e4e443)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Media Format Runtime 11](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=8cab6fe8-161d-4d8c-9772-eb3174a2c3c3)  
(KB952069)  
(Hoch)  
[Windows Media-Dienste 2008](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0204a366-5641-4036-9cb0-a46d04af9d72)\*  
(KB952068)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Media-Dienste 2008](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0204a366-5641-4036-9cb0-a46d04af9d72)\*  
(KB952068)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9bfe15cd-02ff-45cf-85c8-5ff1e6c1a871)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=48bed90d-c243-4969-8e54-326d9a7af343)  
(KB958623)  
(Hoch)  
[Windows Server 2008 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=83de2263-de2a-4c13-96ba-ecfebdaf0bb9)  
(KB958624)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f0d4f321-941e-4da7-958f-582c75542ee8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=06cb502a-6818-4599-aa24-6eddb83e4b84)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS08-078**

Die von MS08-078 behandelte Sicherheitsanfälligkeit wurde nach der Veröffentlichung von Windows Internet Explorer 8 Beta 2 gemeldet. Benutzern, die Windows Internet Explorer 8 Beta 2 ausführen, wird empfohlen, das Update herunterzuladen und auf ihren Systemen zu installieren.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747) und [Windows-Update](http://go.microsoft.com/fwlink/?linkid=21130) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar und können am einfachsten durch eine Suche nach dem Begriff „Sicherheitsupdate“ ermittelt werden.

**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch diese Updates behobenen Sicherheitsanfälligkeiten wirken sich nicht auf unterstützte Editionen von Windows Server 2008 aus, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Dennoch können die von diesen Sicherheitsanfälligkeiten betroffenen Dateien auf dem System vorhanden sein. Benutzern mit den betroffenen Dateien wird dieses Update jedoch immer noch angeboten, da die Updatedateien neuer sind (höhere Versionsnummern haben) als die Dateien, die derzeit auf Ihrem System vorhanden sind. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](http://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=43e8c4d8-307b-48f6-ac99-a9617421d40a)  
(KB956328)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f39d2a49-f861-4f2d-bf91-94a8a85af40c)  
(KB958435)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=3ef41412-50b3-4077-b0e3-9a3704d2f876)  
(KB956329)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=72076e21-2aa3-48e8-883a-c3cb756fc72a)  
(KB958372)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=45c81c60-4b1b-4246-839b-198ebc4eeae2)  
(KB956357)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6c0771e5-fcd4-4365-b903-1a3bd95d9e66)  
(KB958436)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Hoch)  
[Microsoft Office Outlook 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=68bb8d99-f28b-4efd-9314-3eee0bb00ccf)  
(KB958437)\*\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Hoch)  
[Microsoft Office Outlook 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=5b51cb5e-3899-4257-82cf-7e92fa619c37)  
(KB956358)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=68bb8d99-f28b-4efd-9314-3eee0bb00ccf)  
(KB958437)\*\*\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office FrontPage
</td>
<td style="border:1px solid black;">
[Microsoft Office Frontpage 2002 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=0a6130ae-c5b4-43cb-afe3-ab6a55b9d9ea)\*  
(KB957797)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Project
</td>
<td style="border:1px solid black;">
[Microsoft Office Project 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=89a44042-a629-40f3-800a-0bb45fc36591)  
(KB949045)  
(Kritisch)  
[Microsoft Office Project 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2fbf6a5b-ff35-4a2d-9fa0-4e62b6486fe6)  
(KB949046)  
(Kritisch)  
[Microsoft Office Project 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=2fbf6a5b-ff35-4a2d-9fa0-4e62b6486fe6)  
(KB949046)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eca13ad8-62ae-41a8-b308-41e2d1773820)\*\*  
(KB960402)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=eca13ad8-62ae-41a8-b308-41e2d1773820)\*\*  
(KB960402)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ab31a564-43d2-45bd-98bf-19e9ca477b62)\*\*  
(KB960401)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=ab31a564-43d2-45bd-98bf-19e9ca477b62)\*\*  
(KB960401)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=edb6cd8f-832c-4123-8982-ac0c601ea0a7)\*\*  
(KB960403)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=edb6cd8f-832c-4123-8982-ac0c601ea0a7)\*\*  
(KB960403)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
</td>
<td style="border:1px solid black;">
[**MS08-072**](http://go.microsoft.com/fwlink/?linkid=126306)
</td>
<td style="border:1px solid black;">
[**MS08-074**](http://go.microsoft.com/fwlink/?linkid=131481)
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 8](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=1537d181-90d9-4bb5-b5ae-8d9990a349af)\*\*\*  
(KB959487)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b3989ef-02b8-4bd2-b2ab-c3716079936e)  
(KB958434)  
(Hoch)  
[Microsoft Office Excel Viewer 2003 Service Pack 3](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=4b3989ef-02b8-4bd2-b2ab-c3716079936e)  
(KB958434)  
(Hoch)  
[Microsoft Office Excel Viewer](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=9dbb35c1-aa7a-481b-a330-8ba916ddd443)  
(KB958442)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Word Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Word Viewer 2003 Service Pack 3 und Microsoft Office Word Viewer](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=70de7c3c-519f-4f4a-a03f-027f80b5415c)  
(KB956366)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=55430121-4476-48b8-9f6f-4a60fa0b2970)  
(KB956828)  
(Hoch)  
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=55430121-4476-48b8-9f6f-4a60fa0b2970)  
(KB956828)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f)  
(KB958439)  
(Hoch)  
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f)  
(KB958439)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server 2007
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 (32-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)  
(KB956716)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 (32-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)  
(KB956716)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 (64-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7fda284-273c-42ab-8188-433beaacca86)  
(KB956716)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 (64-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7fda284-273c-42ab-8188-433beaacca86)  
(KB956716)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS08-070**  
Im nächsten Abschnitt, **Microsoft-Entwicklertools und -software**, finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Microsoft Office als auch Microsoft-Entwicklertools und -software.

**Hinweis für MS08-077**  
Im Abschnitt **Microsoft Server Software** finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Microsoft Office Suites als auch Software und Microsoft Server Software.

**Hinweis für Microsoft Office FrontPage in MS08-070**  
\*Dieses Update gilt nur für Frontpage 2002 Service Pack 3-Versionen auf Chinesisch (vereinfacht) (China), Pan-Chinesisch (Hong Kong), Chinesisch (traditionell) (Taiwan) und Koreanisch.

**Hinweis für Microsoft Office für Mac in MS08-072 und MS08-074**  
\*\*Die entsprechenden Updates von MS08-072 und MS08-074 sind identisch. Da die Sicherheitsanfälligkeiten in den gleichen Dateien vorliegen, sind diese Updates für beide Bulletins gleich.

**Hinweise für Works 8 in MS08-072**  
\*\*\*Um dieses Sicherheitsupdate zu erhalten, müssen Benutzer, die Microsoft Works 8.0 ausführen, zuerst auf Works 8.5 aktualisieren, wie in [Microsoft Works Update](http://www.microsoft.com/products/works/international/update_1001.mspx) beschrieben. Dazu gehören alle Benutzer, die Microsoft Works 8.0, Works Suite 2004 und Works Suite 2005 verwenden. Für Benutzer, die Works Suite 2006 ausführen, ist Works 8.5 bereits enthalten.

**Hinweis für Microsoft Office Excel 2007 und Microsoft Office Excel 2007 Service Pack 1 in MS08-074**  
\*\*\*\*Für Microsoft Office Excel 2007 und Microsoft Office Excel 2007 Service Pack 1 müssen Benutzer zusätzlich zum Sicherheitsupdatepaket KB958437 auch das Sicherheitsupdate für [Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=99cca4ed-f1f9-4cfd-a986-edbec82ced4f) (KB958439) installieren, um vor den im Bulletin MS08-074 beschriebenen Sicherheitsanfälligkeiten geschützt zu sein. Benutzer, die sowohl das Updatepaket KB958437 als auch das Updatepaket KB958439 bereits erfolgreich installiert haben, müssen diese nicht erneut installieren.

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
Visual Studio
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-070**](http://go.microsoft.com/fwlink/?linkid=130478)
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
Microsoft Visual Basic
</td>
<td style="border:1px solid black;">
[Microsoft Visual Basic 6.0 Runtime Extended Files](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=e27eebcb-095d-43ec-a19e-4a46e591715c)  
(KB926857)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio .NET
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2002 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=afad980d-7f27-49d9-aa23-b762c7b94cd6)  
(KB958392)  
(Kritisch)  
[Microsoft Visual Studio .NET 2003 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=6ac7cf8f-d046-43a8-b4ef-253153d65aed)  
(KB958393)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual FoxPro
</td>
<td style="border:1px solid black;">
[Microsoft Visual FoxPro 8.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=a6977f81-f7f6-486b-96ad-8d296d79f205)  
(KB958369)  
(Kritisch)  
[Microsoft Visual FoxPro 9.0 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=386d27a6-b2c7-4acc-bf3e-edcbc7358172)  
(KB958370)  
(Kritisch)  
[Microsoft Visual FoxPro 9.0 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=5b1f28a9-da8d-463a-8ae4-dfc8fcc6c41a)  
(KB958371)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweis für MS08-070**  
Im vorherigen Abschnitt, **Microsoft-Entwicklertools und -software**, finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Microsoft Office Suites als auch Software und Microsoft-Entwicklertools und -software.

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
Suchserver
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS08-077**](http://go.microsoft.com/fwlink/?linkid=126307)
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
Microsoft Search Server
</td>
<td style="border:1px solid black;">
[Microsoft Search Server 2008 (32-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=f8f73997-6f4c-4b43-aa50-5c8276e83d3e)\*  
(KB956716)  
(Hoch)  
[Microsoft Search Server 2008 (64-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?displaylang=de&familyid=a7fda284-273c-42ab-8188-433beaacca86)\*\*  
(KB956716)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für MS08-077**

\*Umfasst Microsoft Search Server 2008 Express (32-Bit)

\*\*Umfasst Microsoft Search Server 2008 Express (64-Bit)

Im Abschnitt **Microsoft Office Suites und Software** finden Sie weitere Aktualisierungsdateien. Dieses Bulletin umfasst sowohl Microsoft Office Suites als auch Software und Microsoft Server Software.

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

-   ADLab von [VenusTech](http://www.venustech.com.cn/) für den Hinweis auf mehrere in MS08-070 beschriebene Probleme.
-   Jason Medeiros von [Affiliated Computer Services](http://www.acs-inc.com/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   Carsten Eiram von [Secunia Research](http://secunia.com/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   Mark Dowd in Zusammenarbeit mit [McAfee Avert Labs](http://www.avertlabs.com/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   Brett Moore von [Insomnia Security](http://www.insomniasec.com/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   CHkr\_D591 in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   Michal Bucko in Zusammenarbeit mit [CERT/CC](http://www.cert.org/) für den Hinweis auf ein in MS08-070 beschriebenes Problem.
-   Dem [Security Intelligence Analysis Team](http://www.symantec.com/) von Symantec für die Zusammenarbeit mit uns an einem in MS08-070 beschriebenen Problem.
-   Jun Mao von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS08-071 beschriebenes Problem.
-   Juan Caballero in Zusammenarbeit mit von der [Bitblaze Group an der Carnegie Mellon University und UC Berkeley](http://bitblaze.cs.berkeley.edu/) für den Hinweis auf ein in MS08-071 beschriebenes Problem.
-   Ricardo Narvaja von [Core Security Technologies](http://www.coresecurity.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Carsten Eiram von [Secunia Research](http://secunia.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](http://www.paloaltonetworks.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Wushi in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Aaron Portnoy von [TippingPoint DVLabs](http://dvlabs.tippingpoint.com/) für den Hinweis auf in MS08-072 beschriebene Probleme.
-   Wushi von [team509](http://www.team509.com/) in Zusammenarbeit mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Wushi und Ling in Zusammenarbeit mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS08-072 beschriebenes Problem.
-   Carlo Di Dato (alias shinnai) für den Hinweis auf ein in MS08-073 beschriebenes Problem.
-   Brett Moore, der mit [TippingPoint](http://www.tippingpoint.com/) und der [Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, für den Hinweis auf ein in MS08-073 beschriebenes Problem.
-   Chris Weber von [Casaba Security](http://www.casabasecurity.com/) für den Hinweis auf ein in MS08-073 beschriebenes Problem.
-   Jun Mao von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS08-073 beschriebenes Problem.
-   Joshua J. Drake von [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS08-074 beschriebenes Problem.
-   Claes M Nyberg von [signedness.org](http://www.signedness.org/) für den Hinweis auf ein in MS08-074 beschriebenes Problem.
-   Dyon Balding von [Secunia](http://secunia.com/) für den Hinweis auf ein in MS08-074 beschriebenes Problem.
-   Andre Protas von [eEye Digital Security](http://www.eeye.com/) für den Hinweis auf ein in MS08- 075 beschriebenes Problem.
-   Nate McFeters für den Hinweis auf ein in MS08- 075 beschriebenes Problem.
-   Einer Person, die anonym bleiben möchte, für den Hinweis auf ein in MS08-077 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über die [Microsoft Support Services](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos.
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (9. Dezember 2008): Bulletin Summary veröffentlicht.
-   V2.0 (10. Dezember 2008): Korrektur der betroffenen Software für MS08-076, um Windows Media Format Runtime 9.5 und Windows Media Format Runtime 11 als einzelne Updates unter Windows XP Professional x64 Edition und Windows XP Professional x64 Edition Service Pack 2 aufzuführen. Außerdem wurden fehlerhafte Verweise auf Windows Media Format Runtime 11 x64 Edition unter Windows XP Professional x64 Edition, Windows XP Professional x64 Edition Service Pack 2, Windows Server 2003 x64 Edition und Windows Server 2003 x64 Edition Service Pack 2 für MS08-076 entfernt.
-   V3.0 (17. Dezember 2008): Es wurde das Microsoft Security Bulletin MS08-078, Sicherheitsupdate für Internet Explorer (960714), hinzugefügt. Außerdem wurden die Bulletin-Webcastlinks für dieses außerplanmäßige Security Bulletin hinzugefügt.
-   V3.1 (18. Dezember 2008): Für MS08-078 wurde ein Hinweis hinzugefügt, dass Server Core-Installationen von Windows Internet Explorer 7 unter Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für x64-basierte Systeme nicht betroffen sind.
-   V3.2 (7. Januar 2009): Microsoft Office Word Viewer 2003 wurde aus der „Betroffenen Software“ für MS08-072 entfernt.
-   V4.0 (13. Januar 2009): Microsoft hat MS08-076 erneut veröffentlicht, um neue Updatepakete für Windows Media Format Runtime 9.5 unter Windows XP Service Pack 2 (KB952069) und Windows XP Service Pack 3 (KB952069) anzubieten. Benutzer, die alle anderen unterstützten und betroffenen Versionen von Windows Media-Komponenten ausführen und die ursprünglichen Sicherheitsupdatepakete von MS08-076 bereits installiert haben, müssen keine weiteren Aktionen durchführen. Außerdem wurden Windows Media Player 6.4 und Windows Media-Dienste 4.1 für MS08-076 unter allen Editionen von Microsoft Windows 2000 Service Pack 4 als betroffen aufgeführt. Benutzer, denen das Update KB954600 für Windows Media Player 6.4 oder KB952068 für Windows Media-Dienste 4.1 angeboten wurde, die es aber nicht installiert haben, müssen dies nachholen. Des Weiteren wurde Microsoft Office Word Viewer für MS08-072 als betroffen aufgeführt. Benutzer, die das Sicherheitsupdate KB956366 erfolgreich installiert haben, müssen dieses nicht erneut installieren.
-   V5.0 (28. Januar 2009): Der Tabelle **Betroffene Software** wurde eine Fußnote für MS08-074 hinzugefügt, die die Sicherheitsupdatepakete KB958437 und KB958439 für unterstützte Versionen von Microsoft Office Excel 2007 betrifft. An den Binärdateien des Sicherheitsupdates oder der Erkennungslogik wurden keine Änderungen vorgenommen. Benutzer mit Microsoft Office Excel 2007 oder Microsoft Office Excel 2007 Service Pack 1, die KB958437 und KB958439 bereits erfolgreich installiert haben, müssen diese nicht erneut installieren.
-   V6.0 (29. April 2009): Windows Media-Dienste 2008 (KB952068) unter 32-Bit und x64-basierten Editionen von Windows Server 2008 Service Pack 2 wurde als betroffene Software für MS08-076 hinzugefügt. Dies ist lediglich eine Erkennungsänderung. Die Binärdateien wurden nicht verändert. Benutzer, die KB952068 bereits erfolgreich installiert haben, müssen es nicht erneut installieren.

*Built at 2014-04-18T01:50:00Z-07:00*
