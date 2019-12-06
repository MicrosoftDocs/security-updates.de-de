---
TOCTitle: 'MS11-APR'
Title: Microsoft Security Bulletin Summary für April 2011
ms:assetid: 'ms11-apr'
ms:contentKeyID: 61225091
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2011
==================================================

Veröffentlicht: Dienstag, 12. April 2011 | Aktualisiert: Mittwoch, 26. Oktober 2011

**Version:** 6.1

In diesem Bulletin Summary sind die im April 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für April 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 7. April 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://technet.microsoft.com/security/bulletin/advance).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 13. April 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455069&eventcategory=4). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2497640)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Internet Explorer. Dieses Sicherheitsupdate wird für Internet Explorer 6, Internet Explorer 7 und Internet Explorer 8 auf Windows-Clients als Kritisch und für Internet Explorer 6, Internet Explorer 7 und Internet Explorer 8 auf Windows-Servern als Mittel eingestuft. Internet Explorer 9 ist nicht von den Sicherheitsanfälligkeiten betroffen.<br />
<br />
Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SMB-Client können Remotecodeausführung ermöglichen (2511455)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die schwerwiegenderen dieser Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete SMB-Antwort auf eine vom Client initiierte SMB-Anforderung sendet. Um die Sicherheitsanfälligkeit auszunutzen, muss ein Angreifer den Benutzer dazu verleiten, eine SMB-Verbindung zu einem speziell gestalteten SMB-Server zu initiieren.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in SMB-Server kann Remotecodeausführung ermöglichen (2508429)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer ein speziell gestaltetes SMB-Paket erstellt und das Paket an ein betroffenes System sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden, mit denen versucht wird, diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214005">MS11-027</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (2508272)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft-Software. Diese Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite anzeigt, die mit Internet Explorer ein bestimmtes ActiveX-Steuerelement instanziiert. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Dieses Update beinhaltet außerdem Kill Bits für drei ActiveX-Steuerelemente von Drittanbietern.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Remotecodeausführung ermöglichen (2484015)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) ausführen kann. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeit kann auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und dann ausführt, wie es in einem Webhostingszenario der Fall sein kann. Diese Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in GDI+ kann Remotecodeausführung ermöglichen (2489979)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows GDI+. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Bilddatei mithilfe betroffener Software anzeigt oder eine Website durchsucht, die speziell gestaltete Inhalte enthält. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in DNS-Auflösung kann Remotecodeausführung ermöglichen (2509553)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows DNS-Auflösung. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer Zugang zum Netzwerk erhält und dann ein benutzerdefiniertes Programm erstellt, um speziell gestaltete LLMNR-Übertragungsabfragen an die Zielsysteme zu senden. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen. In diesem Fall sollten die LLMNR-Ports vom Internet blockiert werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in den Skriptmodulen</strong> <strong>JScript und VBScript kann Remotecodeausführung ermöglichen (2514666)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den Skriptmodulen JScript und VBScript. Wenn ein Benutzer eine speziell gestaltete Website besucht, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer kann Benutzer nicht zum Besuch einer bestimmten Website zwingen. Der Angreifer müsste statt dessen den Benutzer zum Besuch dieser Webseite verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im OpenType CFF-Treiber (Compact Font Format) kann Remotecodeausführung ermöglichen (2507618)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im OpenType CFF-Treiber (Compact Font Format). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer Inhalte anzeigt, die in einer speziell gestalteten CFF-Schriftart dargestellt werden. Ein Angreifer kann Benutzer nicht zwingen, die speziell gestalteten Inhalte anzuzeigen. Der Angreifer müsste statt dessen den Benutzer zum Besuch einer Webseite verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (2489279)</strong><br />
<br />
Dieses Sicherheitsupdate behebt neun vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale angemeldete erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft PowerPoint können Remotecodeausführung ermöglichen (2489283)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft PowerPoint. Die Sicherheitsanfälligkeiten können eine Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete PowerPoint-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die im <a href="https://support.microsoft.com/kb/2501584">Microsoft Knowledge Base-Artikel 2501584</a> verfügbare automatisierte <strong>Microsoft Fix it</strong>-Lösung für PowerPoint 2010, „Bearbeiten in geschützter Ansicht für PowerPoint 2010 deaktivieren“, blockiert die Angriffsmethoden zum Ausnutzen der in CVE-2011-0655 und CVE-2011-0656 beschriebenen Sicherheitsanfälligkeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server-Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (2489293)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Office-Datei oder eine gültige Office-Datei öffnet, die sich in demselben Netzwerkverzeichnis befindet wie eine speziell gestaltete Bibliotheksdatei. Ein Angreifer, der eine dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokal angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Faxdeckblatt-Editor kann Remotecodeausführung ermöglichen (2527308)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Faxdeckblattdatei (.cov) mit dem Windows Faxdeckblatt-Editor öffnet. Ein Angreifer, der eine dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale angemeldete erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in MFC-Bibliothek (Microsoft Foundation Class) kann Remote</strong> <strong>codeausführung ermöglichen (2500212)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in bestimmten Anwendungen, die mithilfe der MFC-Bibliothek (Microsoft Foundation Class) erstellt wurden. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine gültige Datei öffnet, die einer solchen betroffenen Anwendung zugeordnet ist, und die Datei sich in demselben Netzwerkordner befindet wie eine speziell gestaltete Bibliotheksdatei. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von der betroffenen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Entwicklertools und Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in MHTML kann Offenlegung von Informationen ermöglichen (2503658)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im MHTML-Protokollhandler in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht. In einem webbasierten Angriffsszenario kann eine Website einen speziell gestalteten Link enthalten, mit dem diese Sicherheitsanfälligkeit ausgenutzt wird. Ein Angreifer muss Benutzer dazu verleiten, die Website zu besuchen und den speziell gestalteten Link zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in WordPad-Textkonvertern kann Remotecodeausführung ermöglichen (2485663)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Dieses Sicherheitsupdate wird für alle unterstützten Editionen von Windows XP und Windows Server 2003 als Hoch eingestuft. Alle unterstützten Editionen von Windows Vista, Windows Server 2008, Windows 7 und Windows Server 2008 R2 sind nicht von der Sicherheitsanfälligkeit betroffen.<br />
<br />
Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Datei mittels WordPad öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2506223)</strong><br />
<br />
Dieses Sicherheitsupdate behebt dreißig vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach absteigender Bewertung der Ausnutzbarkeit und dann CVE ID aufgeführt. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie** **verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259.aspx).

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Ausnutzbarkeitsindex – Bewertung</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=209720">MS11-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch nicht sichereres Laden von Bibliotheken in MFC</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3190">CVE-2010-3190</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207931">MS11-028</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET Framework bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3958">CVE-2010-3958</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212224">MS11-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OpenType-Schriftart bezüglich Stapelüberlaufs</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0034">CVE-2011-0034</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208524">MS11-029</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in GDI+ durch Ganzzahlüberlauf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0041">CVE-2011-0041</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei der Verarbeitung von Layouts</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0094">CVE-2011-0094</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wird in</strong> <strong>beschränkten, gezielten Angriffen ausgenutzt.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Ganzzahlüberlaufs</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0097">CVE-2011-0097</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Heapüberlaufs</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0098">CVE-2011-0098</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bei Datensatzanalyse in WriteAV</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0101">CVE-2011-0101</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in einer Office-Komponente aufgrund des nicht sicheren Ladens von Bibliotheken</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0107">CVE-2011-0107</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MSHTML bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0346">CVE-2011-0346</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB-Client bezüglich Analyse von Antworten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0660">CVE-2011-0660</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212236">MS11-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei der Analyse von SMB-Transaktionen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0661">CVE-2011-0661</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0662">CVE-2011-0662</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0665">CVE-2011-0665</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0666">CVE-2011-0666</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0667">CVE-2011-0667</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0670">CVE-2011-0670</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0671">CVE-2011-0671</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0672">CVE-2011-0672</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0673">CVE-2011-0673</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0674">CVE-2011-0674</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0675">CVE-2011-0675</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0676">CVE-2011-0676</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0677">CVE-2011-0677</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OfficeArt Atom bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0976">CVE-2011-0976</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Arrayindizierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0978">CVE-2011-0978</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich beschädigter verknüpfter Liste</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0979">CVE-2011-0979</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich verbleibender Zeiger</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0980">CVE-2011-0980</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1225">CVE-2011-1225</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1226">CVE-2011-1226</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1227">CVE-2011-1227</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1228">CVE-2011-1228</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1229">CVE-2011-1229</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1230">CVE-2011-1230</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1231">CVE-2011-1231</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1232">CVE-2011-1232</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1233">CVE-2011-1233</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1235">CVE-2011-1235</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1236">CVE-2011-1236</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1237">CVE-2011-1237</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1239">CVE-2011-1239</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1240">CVE-2011-1240</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1241">CVE-2011-1241</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1242">CVE-2011-1242</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Objektverwaltung bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1345">CVE-2011-1345</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wird in beschränkten,</strong> <strong>gezielten Angriffen ausgenutzt.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208110">MS11-033</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in WordPad-Konverter bei Analyse</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0028">CVE-2011-0028</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0103">CVE-2011-0103</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Pufferüberschreibung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0104">CVE-2011-0104</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210121">MS11-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Dateninitialisierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0105">CVE-2011-0105</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212314">MS11-019</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Suchdienst aufgrund von Poolbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0654">CVE-2011-0654</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit aufgrund von Gleitkomma in Techno-color Time Bandit bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0655">CVE-2011-0655</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210727">MS11-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in persistentem Verzeichnis bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0656">CVE-2011-0656</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212595">MS11-030</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch DNS-Abfragen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0657">CVE-2011-0657</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212243">MS11-031</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei Skripterstellung durch Speicherneuzuteilung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0663">CVE-2011-0663</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=210206">MS11-023</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bezüglich Grafikobjekt-Dereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0977">CVE-2011-0977</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1234">CVE-2011-1234</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung im Faxdeckblatt-Editor</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3974">CVE-2010-3974</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212226">MS11-024</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Faxdeckblatt</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4701">CVE-2010-4701</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=212523">MS11-026</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MHTML bezüglich Mime-formatierter Anforderung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0096">CVE-2011-0096</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=211826">MS11-034</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1238">CVE-2011-1238</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=214126">MS11-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in JavaScript durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1245">CVE-2011-1245</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
</tbody>
</table>
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=c3a8cec0-f947-4d4e-a6ae-c7f4f1f311b0)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0b7d0403-8965-4c62-970c-20b561f66713)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=689c5496-56c4-48a6-9f3d-b5f5aaf3e566)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f5378e7b-4619-4c42-9d9f-87b209c6d878)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=ccb08a8a-f4d9-4320-8ffb-3fd4fe217987)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b031a496-aa74-4367-b2ae-24843c061745)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=59266a9d-a319-4309-a046-7f15c6da0136)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=2d433adb-bcaf-4c59-9405-a4892f8ccba3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=637f4d4c-de07-4c6a-95f8-3bd0cbfe77b2)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=fbe1e7e3-1d5f-4daf-a4a5-67fe79292963)  
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=9080c5a1-e638-4047-a70a-9367f1acced7)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=50fc3869-f2fc-43c8-8049-aad62f2cb332)  
(KB2491683)  
(Hoch)  
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=a8220a21-02fc-4ad6-988d-844276b2fd66)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=7f0a4616-8e3e-4925-9d95-ce6e614e45ae)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=6753ca98-feb4-4c7f-9969-9294038a2bbb)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=39e55bbf-c1c5-4696-bfe7-632e997cd98e)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=986f07ae-0fdc-4be2-8a74-5eb56d4300ef)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=ed88f183-dd06-46f6-ae8a-a594a752f248)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=6d3433ee-c2e1-433f-a3d9-c049d66e2190)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c01441da-8933-4f60-923b-d9b00db8ba3d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7ee202da-a711-42ee-bea3-7202a70e4ea0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eddd2964-9765-461d-9df8-2c05402948e8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3797009a-b9a4-4e83-8614-e1589c8b5090)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=29ff546e-a232-4f23-a223-c029c71ff1c6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[JScript 5.6 und VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=a5586246-2908-4def-9298-c16060098197)  
(KB2510587)  
(Kritisch)  
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=3a5f65e0-bb00-4e55-b8b5-77751349a3ec)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=57aa7ee2-254d-40b5-9ff0-cba969daf45a)  
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2374e09a-cb3e-4bc3-bb4b-53b611025121)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b93311b4-1b8f-478d-8833-750c5e01e6f8)  
(KB2491683)  
(Hoch)  
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0f60fc99-cd88-4237-8b31-a4e618502f7e)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b01fe9a5-66a4-4683-963b-e78aea214579)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3c94bc96-99ea-44a1-9052-e69de5e21f81)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=83771177-284e-4918-86a9-980e8229c7c9)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=b902c58a-9e2f-4352-8d2f-fffda5344598)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=5c464287-3dab-4342-a38d-a12719d3b158)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=45feb35b-b24e-4160-adb0-d0b7ae530e90)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d46fe0bf-28c2-4696-87bc-dd3c8287fc28)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=64c550d4-c927-4382-91e1-473ed6790819)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=53756404-39e4-43af-81e9-81471536aa66)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fd284233-e177-4064-9b02-f83dcb727dbe)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=753ed6e3-df2e-4b2d-9e9f-7275cd94d214)  
(Hoch)
</td>
<td style="border:1px solid black;">
[JScript 5.6 und VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=e026f2ed-8a20-4268-9b29-04a78bde1999)  
(KB2510587)  
(Kritisch)  
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=5b0ed0b2-07f9-43da-bb5d-5be5a45969ee)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=01aa2beb-9fc1-40f0-a2a4-bcd3d9cb31f8)  
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5d71d3f5-fd6b-4f3b-8389-37c899748d4b)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=edda8cce-b764-4ef1-afbe-391fbd087362)  
(KB2491683)  
(Hoch)  
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bf084b4c-aac9-4cc6-bb30-87fc96ba9430)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0209a004-f23a-40d9-991f-864046f4605f)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9fbfc742-6c74-49a2-b3cc-e1d5d8c84b77)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=af320f27-bb3a-4e76-a279-4632267c8761)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5d8f14d1-85cc-478f-8b50-5c355a331f59)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=9d8bbea9-c456-4569-ad96-c2cd0f5fae7e)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=979d2ec5-5114-4ec7-aa97-e9289c590cbb)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ca0fb4d3-7651-4760-83fa-b71c86cbe459)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ef62db94-4f72-4245-ac9f-6391035e2516)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c8d59f49-45ec-4527-b3a8-4925f710bbfd)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d5adaf4e-4cd7-42ea-8202-31b5c856f5e3)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a0192dbc-4d0d-4555-9ef7-3e10209a6389)  
(Hoch)
</td>
<td style="border:1px solid black;">
[JScript 5.6 und VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=83ce6c99-a57d-4ed1-972b-a6b6798e6675)  
(KB2510587)  
(Kritisch)  
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=af791715-77a1-405b-a69e-d63f75dd7ccd)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=bf0a2966-25c4-4717-bcd6-016ce610d220)  
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3a498ff0-21d9-493a-b127-6bc20f1baf95)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f04d939a-da11-4a9f-9e03-b6c3bf3ca58b)  
(KB2491683)  
(Hoch)  
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=12b01f3a-ccf8-41c1-ac5a-e417a6ddbe95)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6c287571-54ea-4298-8b7d-b98b2c830cc3)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=897b97b0-1bab-4b1b-b417-950fab0d4a65)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9c95f81c-9812-4070-88d7-34422c638e42)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=8afe86fc-58b4-4a95-b047-c09138fa4f5e)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f1abfb48-3c8a-4b2d-b739-cc61628b387d)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=87eb8b93-9829-45ec-9528-52787732044e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=79aeb3cd-7c73-467b-b91e-02c6ea01e911)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9c784734-f44f-4a3c-8223-6289f7dc2ad8)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ce925e76-cb85-48f6-8c0f-e53fa2b09be6)  
(KB2446704)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=72a513bb-f901-4992-8562-d1afe1afec8a)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=f5ad6963-2d6a-4d59-9e25-4fc088647fcd)  
(Hoch)
</td>
<td style="border:1px solid black;">
[JScript 5.6 und VBScript 5.6](https://www.microsoft.com/download/details.aspx?familyid=b7d36bae-7ca4-4a40-9efb-13f484fa5518)  
(KB2510587)  
(Kritisch)  
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=3f519013-ed14-41a8-aa45-cf8b095d3152)  
(KB2510581)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=c71f4398-2e3b-4b81-a650-8806e618db7f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=efb575c7-3259-49b1-b59c-89d9544e37a6)  
(KB2491683)  
(Hoch)  
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=03a7ee49-7bd6-4215-9779-1b48c10d08b9)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3fb450a0-d087-4f36-9301-05ffbf94cc1a)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ede38974-4e57-4ea1-8731-b91e96534693)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=f58cf64a-bf31-4496-be75-5775a123338b)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=00c3c176-feff-4022-ac4c-2d4732ca3d78)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5ea94705-4f76-4b0d-bbbc-afb5e75204bf)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=da8dd55d-6630-484e-836c-9feeab5cc311)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d6eddff4-a242-4dec-9d84-72891db2b754)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80bf050a-9aff-4cd4-8e2f-196b0a92b1c0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritisch)  
Nur Windows Vista Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritisch)  
Windows Vista Service Pack 1 und Windows Vista Service Pack 2:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4ff2e440-79c2-4045-b225-913d1740fdb9)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2a17e44f-54aa-423d-b3c7-a4f404f7c28b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=719e2c86-30e5-4cd5-94f4-d6de54efee5f)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript](https://www.microsoft.com/download/details.aspx?familyid=21decb84-75ef-4bde-a802-1e661a505e94)5.8<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7c4fc81-d1ef-4378-862b-e955d75fb2de)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=11a8f240-51b3-4e31-a24a-a235179f3396)  
(KB2491683)  
(Hoch)  
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e6cba040-9d7c-4777-a2f7-e4dd11dfb845)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c8fce0fb-4c90-479b-8ce9-75e60d52d256)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b4743167-9614-445a-9e91-10efdac505a8)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=79f52733-44e4-47b6-86ca-1395a095b4e7)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=bc63b233-9db0-4fb1-a61c-fa7e9e44ba10)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=040f8b46-f458-4a72-a1b0-ad8a65a1194c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2878c587-6544-40b4-9288-fc3b3ce1128d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a81412d0-2516-4bf4-87f7-3e41ebf6b82b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista x64 Edition Service Pack 1:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritisch)  
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4d826026-e62a-4cec-8682-49fbe7f65cd6)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e708d24f-e348-4c4d-99ed-e78dd1689d01)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=89b9d01e-bcbc-4f2c-973b-51051494f406)  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript](https://www.microsoft.com/download/details.aspx?familyid=d4ac199e-7bf8-4661-a4e5-c53719b2673a)5.8<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8d654a78-0e4f-452c-8874-fbf478813857)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=61db662e-88d7-4454-b4b7-e987728fb137)  
(KB2491683)  
(Hoch)  
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1c942282-0f80-46c1-aeef-1ef948e105a3)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7da10b64-d0a9-4e42-aa3a-87c657122a8c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7e410d5c-b9f7-4a63-8300-36b2d57c6128)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=7d8603b8-bb52-4cf6-be8b-bb3475d30fc5)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d5d76e90-1cef-47e8-9d8d-2c5a43f42ba3)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f8c9390a-5ca1-492a-9e35-a516de48deb5)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=31c48ba9-7774-4633-862d-5c27c3703584)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c3247886-76d0-4292-be9d-3e9b0221c46a)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für 32-Bit-Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fbada866-7d36-4b85-acde-fd856a998737)\*\*\*  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9894be38-a582-4c15-ad0e-cc3afab2aebc)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=d8b33ffd-eff1-4a10-b6fc-3c8f01e0fec5)\*\*  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=afd128ff-717f-4d98-b214-f2c28d59623d)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9105377e-83c7-4010-8fd6-26e42e98c2cc)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=90f56368-776b-4d45-ad68-91afbd316d25)\*\*  
(KB2491683)  
(Hoch)  
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fa972742-1166-4a9e-ab64-6a4f968f9c6d)\*  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=036f1285-7484-4e3b-8799-2c6c08166596)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c6ac26b8-8cc8-40fe-baab-22bf13df1aa8)\*  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=c6d58f64-bdd5-4fe6-96f4-9641b8e7b570)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=51203a31-368b-4b47-96a5-9e9e5a55cd76)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b0cfd5e0-6de5-4863-b5e4-b223a0e36d72)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=de843115-cf98-4511-aa93-f620e4572555)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=51521b6b-94a7-4bcf-ad5f-fc304728b10f)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für x64-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)\*\*  
(KB2449741)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)\*\*  
(KB2449742)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*\*<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8f4ddfcb-374d-4cad-8c61-2b988b46f628)\*\*\*  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2d7d2021-020f-4cc9-a027-258d7e5faec9)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=6c2e6b87-afcd-461a-8a43-9a2fb277b18a)\*\*  
(KB2510581)  
(Kritisch)  
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=40e8beca-0b5a-43b0-98f8-b32a82ad65d6)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=060e8b20-edca-4427-9d60-eb57261eb668)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=22a001fc-5c2e-4539-85c9-0c2054a1777d)\*\*  
(KB2491683)  
(Hoch)  
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fc250c8a-ebaf-4264-9393-dc23cc372d9f)\*  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1438cec8-8dab-4510-ad75-dc6959dac0d8)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ac49f5d3-5e2f-4916-99be-a3254278da7e)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f6f6f22c-fc7f-4e96-b6b5-be3c1acecf6e)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8eaf51cd-2f6e-4bbc-bc4f-9deed03649ac)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b89b8e28-cd98-4bcc-8729-5e51d52d1e92)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7c38b0d-7240-420a-88d3-2749a40e386f)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=94b6a1b3-e048-437b-a224-2a64b3735bc3)  
(KB2449741)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1407aaec-b3e0-404c-b84f-0c8e808614c4)  
(KB2449742)  
(Kritisch)  
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2fd71543-0e18-4907-89b9-355d24d7db69)  
(KB2412687)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c0275df0-10ac-4500-ab86-b7e9a34f8e1d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.7 und VBScript 5.7](https://www.microsoft.com/download/details.aspx?familyid=afb49d24-1913-4e5f-a3ea-c6c9642e2017)  
(KB2510581)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2b8571cb-2dae-4bff-9f13-feb89840044c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=421024f1-aa86-459e-b6de-53851a3fcba2)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f35ecdd1-6b5c-40e7-a00b-ca083bdf5cba)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3b93de4f-01f4-4efd-afc1-31d87b92fad2)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
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
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=59676b71-8b9d-4230-a9e0-b20db3e3ec7e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0dcba089-19f7-46ca-9e52-24eaebad4715)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d3ef905b-3584-4842-9ec2-cf3856305d49)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=46510959-e4a2-4c21-b33c-fd3d97b3ac3d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritisch)  
Nur Windows 7 für 32-Bit-Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritisch)  
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8fdae09b-d1bb-4ef5-aa45-2a05f2a5e12d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.8 und VBScript](https://www.microsoft.com/download/details.aspx?familyid=17ebf291-fdae-4e78-9377-871b3103ce16)5.8<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=751c45ea-0943-4948-807f-8716c6ff9198)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=bf762b86-b949-4e84-8ca4-93ebe669c1b8)  
(KB2491683)  
(Hoch)  
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0f5a122e-dd5e-4b08-881a-f13b38642720)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=aed201c1-f1fb-4df9-8875-6f57ea0eb15b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6e7ff003-ff3f-49bb-8e45-d869885dd8d7)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3a998678-2678-489e-8711-39322663147d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b7fd356a-56d0-4638-8901-40acfa600f25)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=7ddc943b-6868-4e8f-a869-89b47133c287)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=432555cf-aed8-4329-a74f-526441521082)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritisch)  
Nur Windows 7 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritisch)  
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=40879dfb-efa4-41ba-8d5c-22e926a55eef)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.8 und VBScript](https://www.microsoft.com/download/details.aspx?familyid=c95ad86d-da58-4d7a-9ffd-8441f92baaa5)5.8<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=976c882a-bc07-4128-927f-82a2df46cf45)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=a6793ecf-a3f6-4989-8e4c-c5c0005f9ac4)  
(KB2491683)  
(Hoch)  
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=658301f1-103a-48a2-9b67-61cf8e1dad50)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1a32bf04-7eed-4d27-a8e4-054b4a5b76cb)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0c0aef7e-501c-4ca3-ae7f-497a8c169121)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="14" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-018**](https://go.microsoft.com/fwlink/?linkid=214126)
</td>
<td style="border:1px solid black;">
[**MS11-019**](https://go.microsoft.com/fwlink/?linkid=212314)
</td>
<td style="border:1px solid black;">
[**MS11-020**](https://go.microsoft.com/fwlink/?linkid=212236)
</td>
<td style="border:1px solid black;">
[**MS11-027**](https://go.microsoft.com/fwlink/?linkid=214005)
</td>
<td style="border:1px solid black;">
[**MS11-028**](https://go.microsoft.com/fwlink/?linkid=207931)
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-030**](https://go.microsoft.com/fwlink/?linkid=212595)
</td>
<td style="border:1px solid black;">
[**MS11-031**](https://go.microsoft.com/fwlink/?linkid=212243)
</td>
<td style="border:1px solid black;">
[**MS11-032**](https://go.microsoft.com/fwlink/?linkid=212224)
</td>
<td style="border:1px solid black;">
[**MS11-024**](https://go.microsoft.com/fwlink/?linkid=212226)
</td>
<td style="border:1px solid black;">
[**MS11-026**](https://go.microsoft.com/fwlink/?linkid=212523)
</td>
<td style="border:1px solid black;">
[**MS11-033**](https://go.microsoft.com/fwlink/?linkid=208110)
</td>
<td style="border:1px solid black;">
[**MS11-034**](https://go.microsoft.com/fwlink/?linkid=211826)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c7b2482b-44bf-4c01-99d8-f93868659a24)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=27a3847b-695b-4f60-aea5-86b0dbe68945)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c4352802-9c5a-4c07-8303-3a4b78d3f954)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e4fa8ed0-acb0-4864-be18-29a27f8501de)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)\*  
(KB2446709)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)\*  
(KB2446710)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)\*<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=2084c726-187e-41f9-9bea-da18f490d29e)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.8 und VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=aecc2c7a-285c-409d-be23-c5b4b5449496)\*\*<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6f2a52cc-4833-448d-becc-2eac1a447410)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=465c0478-6a74-4b00-8608-938cc492549f)\*\*  
(KB2491683)  
(Hoch)  
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=4c5c3a0f-0672-49d0-bcbd-c7f40e11d092)\*  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=665faa7e-2368-4421-9dd5-ea6df2c79498)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=2fc66224-45c6-4e8f-ad00-6a1ec30b4505)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=af6db318-fbec-4286-a3a7-4081620146e5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e7d3f21-bdbd-4826-855d-85422aa5f836)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0005377b-443f-44ca-a890-620b2dcea6f1)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d7bcf4d7-b697-4c5f-adbc-a2b3700e0ad5)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=157aa425-953c-4fc9-ab76-4e65d4be8baa)  
(KB2446709)  
(Kritisch)  
Nur Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=8f87b8aa-1a2a-405e-aee0-9247d553756a)  
(KB2446710)  
(Kritisch)  
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=91aa6772-4811-4a58-9bc0-8aa271ed99df)<sup>[1]</sup>
(KB2446708)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=34d2793e-a2cd-49f6-b524-6598ea86175f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[JScript 5.8 und VBScript](https://www.microsoft.com/download/details.aspx?familyid=e1bc0ed8-5a93-4d01-b407-919dfd894b5f)5.8<sup>[1]</sup>
(KB2510531)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c6ca0b7c-8151-4d54-aa9b-5ec2b75d8ab6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1a993f8c-d28a-4a95-a3c6-059f06e75461)  
(KB2506212)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=140ea384-2877-401f-ac3b-f84f6966e970)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=485ccf96-27a0-499e-9f52-2836b73d26d2)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten wirken sich nicht wie angegeben auf unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 aus, wenn diese mit der Server Core-Installationsoption installiert wurden, obwohl von dieser Sicherheitsanfälligkeit betroffene Dateien auf dem System vorhanden sein können. Benutzern mit den betroffenen Dateien wird dieses Update jedoch immer noch angeboten, da die Updatedateien neuer sind (höhere Versionsnummern haben) als die Dateien, die derzeit auf Ihrem System vorhanden sind. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-027**

<sup>[1]</sup> Dieses bestimmte Betriebssystem ist nicht von den Sicherheitsanfälligkeiten betroffen, die in diesem Bulletin beschrieben sind. Das verfügbare Update setzt die Kill Bits für Steuerelemente von Drittanbietern.

**Hinweis für MS11-028**

<sup>[1]</sup>**.NET Framework 4.0 und .NET Framework 4.0 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4.0 und .NET Framework 4.0 Client Profile. .NET Framework 4.0 Client Profile ist Teil von .NET Framework 4.0. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4.0 als auch .NET Framework 4.0 Client Profile. Weitere Informationen finden Sie unter: [Installieren von .NET Framework](https://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

**Hinweis für MS11-029**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweis für MS11-031**

<sup>[1]</sup>Systeme mit Internet Explorer 9 sind nicht betroffen und benötigen dieses Update nicht. Auf Systemen, die nicht mit Internet Explorer 9 aktualisiert wurden, muss das richtige Update für die Versionen von JScript und VBScript installiert sein. Anweisungen zum Ermitteln, welche Versionen von JScript und VBScript auf Ihrem System installiert sind, finden Sie im Bulletin.

**Hinweis für MS11-024**

Wenn für das gleiche Betriebssystem zwei Updates verfügbar sind, installieren Sie beide Updates.

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
Microsoft Office Suites und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](https://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](https://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](https://go.microsoft.com/fwlink/?linkid=210206)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des** **Gesamtschweregrads**
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=db2c5cfe-588c-4646-b86a-3fb8248f7af4)  
(KB2466169)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=0d215ab6-c9be-4f43-9501-658bb7ef008e)  
(KB2464617)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=6c87c2a9-3705-4680-8a9b-63b6ec83674d)  
(KB2509461)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=916a076d-d754-4092-b23d-c8826db7e397)  
(KB2502786)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=2ce8349f-79b1-41ef-a1c0-cbe40ccf9f20)  
(KB2464588)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=8b68cf68-1606-4649-b860-a64702c6cf33)  
(KB2509503)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5ae34fe0-03bd-48a9-a7ac-de8f7b1aff90)<sup>[1]</sup>
(KB2464583)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6b2526fe-a061-4a17-992e-ac867bef130e)  
(KB2464594)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dbba0cd4-ab72-4e2b-9524-fd6be27f0b02)  
(KB2509488)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=a427f0e2-b74d-4ef3-bec4-0a101d09bfa3)  
(KB2466146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=549ca7f0-44bf-4965-a9d2-aa5e8dac2238)  
(KB2519975)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=13dca35d-2209-4c5c-9150-d6db2bb3b496)  
(KB2466146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=ef62deae-2b07-41c9-a4bf-b746566e59ee)  
(KB2519975)  
(Hoch)
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
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](https://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](https://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](https://go.microsoft.com/fwlink/?linkid=210206)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=f756d836-6ab2-4adb-9dee-6cb523d7c1f5)  
(KB2505924)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=84dfe3f4-a2a1-47b9-8da1-29ae67230918)  
(KB2505927)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=ef1e612f-d8e3-4628-9fe4-ad136f0debd3)  
(KB2525412)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=0c323a12-6385-4666-ad39-a9516a8eda14)  
(KB2505935)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="5" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-029**](https://go.microsoft.com/fwlink/?linkid=208524)
</td>
<td style="border:1px solid black;">
[**MS11-021**](https://go.microsoft.com/fwlink/?linkid=210121)
</td>
<td style="border:1px solid black;">
[**MS11-022**](https://go.microsoft.com/fwlink/?linkid=210727)
</td>
<td style="border:1px solid black;">
[**MS11-023**](https://go.microsoft.com/fwlink/?linkid=210206)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Excel Viewer Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2d75786a-2368-4ef2-970b-fa2e57d63ca9)  
(KB2466158)  
(Hoch)
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
Microsoft Office PowerPoint Viewer 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office PowerPoint Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6e23d3c3-2944-42ea-80b3-0663af60d0f1)  
(KB2464623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft PowerPoint Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Viewer](https://www.microsoft.com/download/details.aspx?familyid=44a703f5-b581-4900-bdbb-0f0e8d9bf0e6)  
(KB2519984)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=946cc611-4d75-4728-b9d3-1c8b557b02c2)  
(KB2466156)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=913efc28-7deb-47b8-8c22-8eb5fc2631e4)  
(KB2464635)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS11-029**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweis für MS11-021**

<sup>[1]</sup>Für Microsoft Office Excel 2007 Service Pack 2 müssen Benutzer zusätzlich zum Sicherheitsupdatepaket KB2464583 auch das Sicherheitsupdate für Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2 (KB2466156) installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

**Hinweis für MS11-022**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

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
Microsoft Office Web Apps
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-022**](https://go.microsoft.com/fwlink/?linkid=210727)
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
Microsoft Office Web Apps
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint Web App](https://www.microsoft.com/download/details.aspx?familyid=9847dc05-7d4a-4a64-9e6a-622d3fa171f9)  
(KB2520047)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS11-022**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

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
[**MS11-025**](https://go.microsoft.com/fwlink/?linkid=209720)
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
Microsoft Visual Studio .NET 2003 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio .NET 2003 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e9501082-a651-452b-8c1a-43987ffd3102)  
(KB2465373)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ee64d83b-6c06-4ccf-b12d-99e2a7a7b18d)  
(KB2538218)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e6a8e024-12ee-43d5-9aae-4c721505d6df)  
(KB2538241)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010 und Microsoft Visual Studio 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](https://www.microsoft.com/download/details.aspx?familyid=7fd643a8-8e05-4d27-8853-33f79f01cb26)  
(KB2542054)  
(Hoch)  
[Microsoft Visual Studio 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1a21c9db-dfa3-4a07-a1e0-89a8069b7c17)  
(KB2565057)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package](https://www.microsoft.com/download/details.aspx?familyid=ae2e1a40-7b45-4fe9-a20f-2ed2923aca62)  
(KB2538242)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual C++ 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package](https://www.microsoft.com/download/details.aspx?familyid=a821847e-4c44-45c0-9128-61c822bb3280)  
(KB2538243)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual C++ 2010 und Microsoft Visual C++ 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Visual C++ 2010 Redistributable Package](https://www.microsoft.com/download/details.aspx?familyid=fe558aed-9274-415f-8a0f-d9d8622fb35b)  
(KB2467173)  
(Hoch)  
[Microsoft Visual C++ 2010 Redistributable Package Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=7557d29b-731b-4abb-8815-2b87a4132efb)  
(KB2565063)  
(Hoch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheitscenter](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

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

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Einer Person, die mit [VeriSign iDefense Labs](https://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-018 beschriebenes Problem.
-   [MITRE](https://mitre.org/) für die Zusammenarbeit mit uns an einem in MS11-018 beschriebenen Problem.
-   Michal Zalewski von [Google Inc.](https://www.google.com/) für die Zusammenarbeit mit uns an einem in MS11-018 beschriebenen Problem.
-   David Bloom von [Google Inc.](https://www.google.com/) für den Hinweis auf zwei in MS11-018 beschriebene Probleme.
-   Stephen Fewer von [Harmony Security](https://www.harmonysecurity.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) für den Hinweis auf ein in MS11-018 beschriebenes Problem.
-   Alin Rad Pop von [Secunia Research](https://secunia.com/) für den Hinweis auf zwei in MS11-021 beschriebene Probleme.
-   Muhammad Junaid Bohio von [Telus Security Labs](https://www.telussecuritylabs.com) für den Hinweis auf ein in MS11-021 beschriebenes Problem.
-   Aniway in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) für den Hinweis auf drei in MS11-021 beschriebene Probleme.
-   Einer Person, die mit [VeriSign iDefense Labs](https://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-021 beschriebenes Problem.
-   Rodrigo Rubira Branco vom [Check Point Vulnerability Discovery Team](https://www.checkpoint.com/) (VDT) für den Hinweis auf ein in MS11-021 beschriebenes Problem.
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-021 beschriebenes Problem.
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [TippingPoint](https://www.tippingpoint.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-021 beschriebenes Problem.
-   [TippingPoint's](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf drei in MS11-022 beschriebene Probleme.
-   Haifei Li von [Fortinets FortiGuard Labs](https://www.fortiguard.com/) für den Hinweis auf ein in MS11-023 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-023 beschriebenes Problem.
-   Carsten H. Eiram von [Secunia](https://secunia.com/) für die Zusammenarbeit mit uns an einem in MS11-024 beschriebenen Problem
-   Dem [Google Security Team](https://www.google.com/) für die Zusammenarbeit mit uns an einem in MS11-026 beschriebenen Problem.
-   Chris Ries vom Büro für Informationssicherheit der Carnegie Mellon-Universität für den Hinweis auf ein in MS11-027 beschriebenes Problem.
-   RadLSneak in Zusammenarbeit mit [iSIGHT Partners](https://www.isightpartners.com/) Global Vulnerability Partnership für den Hinweis auf ein in MS11-027 beschriebenes Problem.
-   Nicolas Joly und Chaouki Bekrar vom [VUPEN Threat Protection Program](https://www.vupen.com/english/services/tpp-index.php) für den Hinweis auf ein in MS11-029 beschriebenes Problem.
-   Neel Mehta von [Google Inc.](https://www.google.com/) für den Hinweis auf ein in MS11-030 beschriebenes Problem.
-   [Jesse Ruderman](https://www.squarefree.com/) von [Mozilla](https://www.mozilla.org/) für die Zusammenarbeit mit uns an einem in MS11-031 beschriebenen Problem.
-   Adam Twardoch von [Fontlab Ltd.](https://www.fontlab.com/) für den Hinweis auf ein in MS11-032 beschriebenes Problem.
-   Carsten Eiram von [Secunia](https://secunia.com/) für den Hinweis auf ein in MS11-033 beschriebenes Problem.
-   Tarjei Mandt von [Norman](https://www.norman.com/) für den Hinweis auf 30 in MS11-034 beschriebene Probleme.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (12. April 2011): Bulletin Summary veröffentlicht.
-   V1.1 (13. April 2011): Für MS11-019 wurde die Beschreibung der Sicherheitsanfälligkeit in der Kurzzusammenfassung verdeutlicht.
-   V2.0 (15. April 2011): In MS11-032 wurde die Ausnutzbarkeitsindexbewertung für CVE-2011-0034 auf „1 – Konsistenter Angreifercode wahrscheinlich“ erhöht.
-   V3.0 (21. April 2011): Überarbeitet, um das erneut veröffentlichte Sicherheitsupdate für MS11-025 anzubieten.
-   V3.1 (27. April 2011): Für MS11-024 wurde der Ausnutzbarkeitsindex korrigiert, um CVE-2010-4701 als Sicherheitsanfälligkeit hinzuzufügen, die durch dieses Update behoben wird. Dies ist lediglich eine Informationsänderung.
-   V4.0 (16. Mai 2011): Erneute Veröffentlichung des Bulletins MS11-018, um das Update für Internet Explorer 7 unter unterstützten Editionen von Windows XP und Windows Server 2003 erneut anzubieten. Dies ist lediglich eine Erkennungsänderung. Die Binärdateien wurden nicht verändert. Das Update wird ausschließlich betroffenen Benutzern angeboten. Benutzer, die das Update manuell installiert haben, sowie Benutzer, die die Konfigurationen ausführen, die von der Änderung an der Erkennungslogik nicht betroffen sind, müssen keine Maßnahmen ergreifen.
-   V5.0 (14. Juni 2011): Für MS11-025 wurde das Update für Microsoft Visual Studio 2005 Service Pack 1, Microsoft Visual Studio 2008 Service Pack 1, Microsoft Visual Studio 2010, Microsoft Visual C++ 2005 Service Pack 1 Redistributable Package und Microsoft Visual C++ 2008 Service Pack 1 Redistributable Package erneut angeboten. Benutzer, die dieses Update bereits installiert haben, sollten die neuen Pakete auf den betroffenen Systemen installieren.
-   V6.0 (9. August 2011): Für MS11-025 hat Microsoft Visual Studio 2010 Service Pack 1 (KB2565057) und Microsoft Visual C++ 2010 Redistributable Package Service Pack 1 (KB2565063) als betroffene Software hinzugefügt.
-   V6.1 (26. Oktober 2011): Für MS11-028 wurde die Anwendbarkeit der Server Core-Installation für .NET Framework 4 unter Windows Server 2008 R2 für x64-basierte Systeme korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*
