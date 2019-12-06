---
TOCTitle: 'MS11-JUN'
Title: Microsoft Security Bulletin Summary für Juni 2011
ms:assetid: 'ms11-jun'
ms:contentKeyID: 61225097
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Juni 2011
=================================================

Veröffentlicht: Dienstag, 14. Juni 2011 | Aktualisiert: Mittwoch, 18. Januar 2012

**Version:** 3.1

In diesem Bulletin Summary sind die im Juni 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Juni 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 9. Juni 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 15. Juni 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Juni.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032455073&eventcategory=4) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://go.microsoft.com/fwlink/?linkid=217214)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212284">MS11-038</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in OLE-Automatisierung kann Remotecodeausführung ermöglichen (2476490)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Microsoft Windows OLE-Automatisierung (Object Linking and Embedding). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Website besucht, die ein speziell gestaltetes WMF-Bild (Windows Metafile) enthält. Ein Angreifer kann Benutzer jedoch nicht zum Besuch einer solchen Website zwingen. Stattdessen muss ein Angreifer Benutzer dazu überreden, eine schädliche Website zu besuchen. Zu diesem Zweck wird der Endbenutzer normalerweise dazu gebracht, in einer E-Mail oder einer Instant Messenger-Anfrage auf einen Link zu klicken.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212287">MS11-039</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework und Microsoft Silverlight kann Remotecodeausführung ermöglichen (2514842)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework und Microsoft Silverlight. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) oder Silverlight-Anwendungen ausführen kann. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeit kann auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und dann ausführt, wie es in einem Webhostingszenario der Fall sein kann. Diese Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework,<br />
Microsoft Silverlight</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217470">MS11-040</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Threat Management Gateway-Firewallclient kann Remotecodeausführung ermöglichen (2520426)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft Forefront Threat Management Gateway (TMG) 2010 Client, vormals Microsoft Forefront Threat Management Gateway-Firewallclient. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Clientcomputer dazu nutzt, bestimmte Anforderungen an ein System zu stellen, auf dem der TMG-Firewallclient verwendet wird.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Forefront Threat Management Gateway</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217499">MS11-041</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Kernelmodustreibern kann Remotecodeausführung ermöglichen (2525694)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Netzwerkfreigabe besucht (oder eine Website besucht, die auf eine Netzwerkfreigabe zeigt), die eine speziell gestaltete OTF-Schriftart (Open Type Font) enthält. In keinem Fall jedoch kann ein Angreifer einen Benutzer zwingen, eine solche Website oder Netzwerkfreigabe zu besuchen. Stattdessen muss ein Angreifer einen Benutzer dazu verleiten, die Website oder Netzwerkfreigabe zu besuchen. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zu klicken.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Distributed File System können Remotecodeausführung ermöglichen (2535512)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten im Microsoft Distributed File System (DFS). Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete DFS-Antwort auf eine vom Client initiierte DFS-Anforderung sendet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code ausführen und vollständige Kontrolle über das betroffene System erlangen. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215841">MS11-043</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in SMB-Client können Remotecodeausführung ermöglichen (2536276)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer eine speziell gestaltete SMB-Antwort auf eine vom Client initiierte SMB-Anforderung sendet. Um die Sicherheitsanfälligkeit auszunutzen, muss ein Angreifer den Benutzer dazu verleiten, eine SMB-Verbindung zu einem speziell gestalteten SMB-Server zu initiieren.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=216436">MS11-044</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Remotecodeausführung ermöglichen (2538814)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) ausführen kann. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeit kann auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und dann ausführt, wie es in einem Webhostingszenario der Fall sein kann. Diese Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2530548)</strong><br />
<br />
Dieses Sicherheitsupdate behebt elf vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=218115">MS11-052</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in VML (Vector Markup Language) kann Remotecodeausführung ermöglichen (2544521)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Microsoft-Implementierung der Vector Markup Language (VML). Dieses Sicherheitsupdate wird für Internet Explorer 6, Internet Explorer 7 und Internet Explorer 8 auf Windows-Clients als Kritisch und für Internet Explorer 6, Internet Explorer 7 und Internet Explorer 8 auf Windows-Servern als Mittel eingestuft. Internet Explorer 9 ist nicht von dieser Sicherheitsanfälligkeit betroffen.<br />
<br />
Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217912">MS11-037</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in MHTML kann Offenlegung von Informationen ermöglichen (2544893)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im MHTML-Protokollhandler in Microsoft Windows. Die Sicherheitsanfälligkeit kann Offenlegung von Information ermöglichen, wenn ein Benutzer eine speziell gestaltete URL von der Website eines Angreifers öffnet. Ein Angreifer muss den Benutzer zum Besuch der Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zu klicken.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (2537146)</strong><br />
<br />
Dieses Sicherheitsupdate behebt acht vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale angemeldete erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Durch das Installieren und Konfigurieren der Überprüfung von Office-Dateien (OFV), um das Öffnen von verdächtigen Dateien zu verhindern, werden die Angriffsmethoden zum Ausnutzen der Sicherheitsanfälligkeiten blockiert, die in CVE-2011-1272, CVE-2011-1273 und CVE-2011-1279 beschrieben sind. Microsoft Excel 2010 ist nur von der in diesem Bulletin beschriebenen CVE-2011-1273 betroffen. Die automatisierte Microsoft Fix it-Lösung, „Bearbeiten in geschützter Ansicht für Excel 2010 deaktivieren“, die im Microsoft Knowledge Base-Artikel 2501584 verfügbar ist, blockiert die Angriffsmethoden zum Ausnutzen von CVE-2011-1273.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217464">MS11-046</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Treiber für zusätzliche Funktionen kann Erhöhung von Berechtigungen ermöglichen (2503665)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Microsoft Windows-Treiber für zusätzliche Funktionen (AFD). Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei dem System eines Benutzers anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217468">MS11-047</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Hyper-V kann Denial-of-Service ermöglichen (2525835)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Server 2008 Hyper-V und Windows Server 2008 R2 Hyper-V. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein authentifizierter Benutzer eine fehlerhafte Sequenz von Computeranweisungen auf einem der virtuellen Gastcomputer ausführt, die vom Hyper-V-Server gehostet wird. Ein Angreifer muss über gültige Anmeldeinformationen verfügen und speziell gestaltete Inhalte von einem virtuellen Gastcomputer senden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215840">MS11-048</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in SMB-Server kann Denial-of-Service ermöglichen (2536275)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer ein speziell gestaltetes SMB-Paket erstellt und das Paket an ein betroffenes System sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden, mit denen versucht wird, diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217077">MS11-049</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Microsoft XML-Editor kann Offenlegung von Informationen ermöglichen (2543893)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft XML-Editor. Die Sicherheitsanfälligkeit kann Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine speziell gestaltete Web Services Discovery-Datei (.disco) mit einer betroffenen Software öffnet, die in diesem Bulletin aufgeführt ist. Beachten Sie, dass diese Sicherheitsanfälligkeit einem Angreifer keine Codeausführung oder direkte Erhöhung von Berechtigungen ermöglicht, sondern dazu führt, dass der Angreifer Informationen sammelt, mit denen das betroffene System noch weiter gefährdet werden könnte.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft SQL Server,<br />
Microsoft Visual Studio</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217101">MS11-051</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in der Webregistrierung von Active Directory-Zertifikatsdiensten kann Erhöhung von Berechtigungen ermöglichen (2518295)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Webregistrierung von Active Directory-Zertifikatsdiensten. Die Sicherheitsanfälligkeit ist eine Sicherheitsanfälligkeit bezüglich siteübergreifender Skripterstellung (XSS), die eine Erhöhung von Berechtigungen ermöglichen kann, sodass ein Angreifer willkürliche Befehle auf der Site im Kontext des Zielbenutzers ausführen kann. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, muss einen speziell gestalteten Link senden und den Benutzer überzeugen, auf den Link zu klicken. Ein Angreifer kann einen Benutzer jedoch nicht zum Besuch einer solchen Website zwingen. Stattdessen muss der Angreifer den Benutzer zu einem Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer normalerweise dazu gebracht, auf einen Link in einer E-Mail-Nachricht oder Instant Messenger-Nachricht zu klicken, die den Benutzer zur anfälligen Site führt.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit durch Codeausführung für aktuelle Softwareversion</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit durch Codeausführung für ältere Softwareversionen</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit durch Denial-of-Service</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217912">MS11-037</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in MHTML bezüglich Mime-formatierter Anforderung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1894">CVE-2011-1894</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212284">MS11-038</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLE-Automatisierung bezüglich Unterlaufs</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0658">CVE-2011-0658</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=212287">MS11-039</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET Framework bezüglich Array-Offsets</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0664">CVE-2011-0664</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217470">MS11-040</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in TMG-Firewallclient bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1889">CVE-2011-1889</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217499">MS11-041</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bei OTF-Überprüfung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1873">CVE-2011-1873</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in DFS bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1868">CVE-2011-1868</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215838">MS11-042</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in DFS-Verweisantwort</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1869">CVE-2011-1869</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service führen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215841">MS11-043</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im SMB bezüglich Analyse von Antworten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1268">CVE-2011-1268</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=216436">MS11-044</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET Framework durch JIT-Optimierung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1271">CVE-2011-1271</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel durch unzureichende Datensatzüberprüfung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1272">CVE-2011-1272</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel durch fehlerhafte Datensatzanalyse</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1273">CVE-2011-1273</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich verbotenen Arrayzugriffs</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1274">CVE-2011-1274</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Heapüberschreibung im Speicher</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1275">CVE-2011-1275</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Pufferüberlaufs</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1276">CVE-2011-1276</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1277">CVE-2011-1277</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel in WriteAV</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1278">CVE-2011-1278</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217502">MS11-045</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Excel bezüglich verbotenen WriteAVs</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1279">CVE-2011-1279</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217464">MS11-046</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Treiber für zusätzliche Funktionen bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1249">CVE-2011-1249</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.<br />
<br />
Diese Sicherheitsanfälligkeit kann für eine Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217468">MS11-047</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im VMBus bezüglich beständigen Denial-of-Services</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1872">CVE-2011-1872</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service führen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=215840">MS11-048</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SMB bei der Anforderungsanalyse</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1267">CVE-2011-1267</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service führen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217077">MS11-049</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Auflösung XML-externer Entitäten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1280">CVE-2011-1280</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei Verarbeitung von Linkeigenschaften</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1250">CVE-2011-1250</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch DOM-Manipulation</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1251">CVE-2011-1251</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in toStaticHTML durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1252">CVE-2011-1252</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch Drag-and-Drop</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1254">CVE-2011-1254</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch Zeitelement</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1255">CVE-2011-1255</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch DOM-Modifizierung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1256">CVE-2011-1256</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung bei Layout</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1260">CVE-2011-1260</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch Auswahlobjekte</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1261">CVE-2011-1261</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217212">MS11-050</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch HTTP-Umleitung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1262">CVE-2011-1262</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=217101">MS11-051</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Active Directory bezüglich Zertifikatsdiensten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1264">CVE-2011-1264</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann für eine Erhöhung von Berechtigungen ausgenutzt werden.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=218115">MS11-052</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VML bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1266">CVE-2011-1266</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
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
  
**Tabelle 1**

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
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=2371079f-fb20-4fd5-999e-e73f3701818c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=67a25abd-f43c-4b01-b507-a109b739238f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=492310d3-bbb4-4fff-b5fe-3470c17e7681)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritisch)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=26ec66af-9727-4423-90da-012ed5b30856)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=4203a59a-a809-45db-a234-fef0ff5063f9)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4a49ec89-2a8f-41d9-8f0b-ee57fdf21f50)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b53d6631-4ded-48f5-a503-925b89b322b2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=035d5115-54b6-41d3-b9f0-890041ead178)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=af6b7627-c462-45fe-8948-70da37e60659)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e10a4c3c-2ef8-4cfc-ac9b-4d97bfa79ac1)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritisch)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=f6e05fef-ee8c-44ff-a106-d7b8659c8d91)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=9fc734db-a177-43d2-a74a-b1fe6ea6f779)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4e4e18a4-97dc-4c5e-a078-8466913aa29e)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7e6ff410-4552-4687-81ab-83d9c91f8af5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3aa8f1bc-07de-451a-8244-1733247e6f2e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2719e0fb-3cfd-47b2-906d-3e07b0e3c978)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritisch)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=638f6dd6-bea0-4356-b23a-45e865a6b28b)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a3bd0012-4a45-4f96-8a51-3ff1f85d1e37)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=19557984-5088-44cc-b5ba-9bab33df8e7e)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9c1a539f-1472-4394-8354-bd549d8332e0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4aa8c003-0353-4a5b-8aea-c01a103af393)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e9018258-5a72-47a1-8584-3d1aa52317c3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c962531e-f580-4195-989b-cf348cc96fa7)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritisch)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=ce616970-343d-49f1-994d-4269b9a11448)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=70ece3b4-e5bb-469c-bfef-c8310681f5a7)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c92d94c5-5e8f-45aa-a24a-f4d0efd93732)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=c194dd35-b9db-44a5-a252-38f9f803802f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=686e5192-63e4-410e-b653-2cfddd5b409f)  
(KB2478656)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3db8a718-4441-4e1a-889f-abcc4bde1125)  
(KB2478658)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=2e07b5fa-c9fa-495b-9352-c07ce46a7e8b)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=96309c49-4822-4c47-b364-2ba65327cac5)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ea18a916-03cf-4eac-bacc-ceb006491f24)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=c7e115a1-486b-4a2b-a7d6-42c4018fc02d)  
(KB2530095)  
(Kritisch)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=960f8920-906b-48a8-8700-94f09babc628)  
(KB2518864)  
(Kritisch)  
[Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=f58ebc9e-00e1-413c-8076-d7a44003d0c7)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=80231a27-b37c-4101-a34f-19a26a040836)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f33c9e54-c2e5-498d-a798-5bbfe9e4249c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritisch)  
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritisch)  
Nur Windows Vista Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritisch)  
Windows Vista Service Pack 1 und Windows Vista Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=aded8f20-479d-40c1-9560-c0581c6f77a2)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a62edfd8-9016-4bb5-bf48-885498fa0042)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritisch)  
Nur Windows Vista Service Pack 1: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritisch)  
Nur Windows Vista Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritisch)  
Windows Vista Service Pack 1 und Windows Vista Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=fea735a8-032b-4fa6-8337-1fa411df0b88)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4cddfc68-eff6-4587-8607-63307d039489)  
(Kritisch)  
Nur Windows Vista Service Pack 2: [Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=392316fc-f531-469c-aa60-4ecf061a5354)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4566528f-62ee-4d78-b3af-131a7cc15e1f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritisch)  
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a519a5d7-bfe3-4e53-99e9-d85f7e34237f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=962cb40c-680c-4c37-98d4-ca9789ca7270)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=cb561ba6-af4d-40cc-947c-923f9cca9a7e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 1: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritisch)  
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=49dcb47b-3c79-4f69-ba07-f471304c16e2)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e0a8fbac-2c31-4cf8-9967-6171edabd560)  
(Kritisch)  
Nur Windows Vista x64 Edition Service Pack 2: [Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=44b2aa73-c318-47ac-ad87-0d24afd9cdd7)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0c9614d9-6f61-463d-b1fa-bd5eb2c1a5c5)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)\*\*  
(KB2478657)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)\*\*  
(KB2478659)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)\*\*  
(KB2478660)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*\*<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8ebfa067-0236-4454-8605-df1b99742f90)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8ab9679e-6a69-4ca3-9210-7ca4fb1980c2)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritisch)  
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*\*<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=b6547ff0-b059-495d-8816-bb094ac11be7)\*\*  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c9650c47-ac52-433d-b409-ce1cfe8d3e87)\*\*  
(Kritisch)  
Nur Windows Server 2008 für 32-Bit-Systeme Service Pack 2: [Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7f9b1ba2-8247-494b-990c-f62003188c5a)\*\*  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=36698775-0e4e-4980-ae4c-43542de424ca)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)\*\*  
(KB2478657)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)\*\*  
(KB2478659)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)\*\*  
(KB2478660)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*\*<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=cd8f3713-b408-4db6-aecd-7eed2176a715)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f1d76b82-9996-4d08-894b-9c16a4b3bb1e)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=22c63fc3-2c5a-4e50-9026-2e04a6e74210)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)\*\*  
(KB2518863)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)\*\*  
(KB2518865)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)\*\*  
(KB2518866)  
(Kritisch)  
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*\*<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=feff3364-4bfd-45f5-99da-9192b47ef5d4)\*\*  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7dff9f08-19cb-41dd-a315-84c1dac81510)\*\*  
(Kritisch)  
Nur Windows Server 2008 für x64-basierte Systeme Service Pack 2: [Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=fdf88a52-c099-44eb-95a0-650129c0e678)\*\*  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3edb613f-5bf0-4e28-9835-4afbb6ef0e01)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 1 und Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=2eabacce-394f-4b9a-8306-0875ca19a3a9)  
(KB2478657)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=55fd3254-7e59-4cf9-afa8-45ae66bc7390)  
(KB2478659)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2 und Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=afa11dda-a543-42a7-b997-5292fd869a8b)  
(KB2478660)  
(Kritisch)  
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5a61f888-c81e-4b8a-8932-2fe67df4b2ad)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f80c89c6-27ab-4f6a-afad-9c8e92cbbce4)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5bb889de-8ff6-4587-8ef9-ffb13e8d60fd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)  
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=5f7092fe-079d-4175-b8b7-412f259ff7e4)  
(KB2518863)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=80423e37-0a54-413d-b44a-41c68c2030b8)  
(KB2518865)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme Service Pack 2: [Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritisch)  
Nur Windows Server 2008 für Itanium-basierte Systeme Service Pack 2: [Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1e3ca981-5565-41a8-ab5e-941c92e74c7d)  
(KB2518866)  
(Kritisch)  
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=d81a9219-da95-4fbf-af7f-898f553b0572)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=50ae36ff-2406-48a4-97cc-12782b6d30ac)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritisch)  
Nur Windows 7 für 32-Bit-Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritisch)  
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=9de1bf5d-6f25-496d-bc44-a32c5e8920fe)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=19a15098-1754-4536-a9ca-ff07d16464b7)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritisch)  
Nur Windows 7 für 32-Bit-Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritisch)  
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=91b98f02-a09e-48f1-9f78-a949f7268542)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=79f846da-3b17-43c9-9016-a055c2c56975)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1241f0f8-a5c7-420a-a5b7-b6c3caa9e5e2)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für x64-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritisch)  
Nur Windows 7 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritisch)  
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e7f52b13-5b3d-438c-ae14-86da50c8b67a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=50d1c677-57aa-4e3f-bdfc-6f01b5d3bfe2)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b449f23e-b3df-46e5-bfe3-98268d20ad54)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für x64-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritisch)  
Nur Windows 7 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritisch)  
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=264107cc-68b4-401c-82f7-de64b535c18d)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=e87a09f2-b755-48ef-9b85-fc78d0bfce43)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-038**](http://go.microsoft.com/fwlink/?linkid=212284)
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-041**](http://go.microsoft.com/fwlink/?linkid=217499)
</td>
<td style="border:1px solid black;">
[**MS11-042**](http://go.microsoft.com/fwlink/?linkid=215838)
</td>
<td style="border:1px solid black;">
[**MS11-043**](http://go.microsoft.com/fwlink/?linkid=215841)
</td>
<td style="border:1px solid black;">
[**MS11-044**](http://go.microsoft.com/fwlink/?linkid=216436)
</td>
<td style="border:1px solid black;">
[**MS11-050**](http://go.microsoft.com/fwlink/?linkid=217212)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8181c359-cd79-438a-87be-093b363d0b04)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)\*  
(KB2478661)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)\*  
(KB2478662)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)\*<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b77e5be6-d3eb-4e3a-9be2-831578f0447c)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9d66b1e7-dbf9-4475-a973-49fb85557eca)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=06008192-3cac-477b-a913-83eed39d8718)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)\*  
(KB2518867)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)\*  
(KB2518869)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)\*<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=8b18e6f9-96b8-4dec-bcd0-d71f1bac3eb0)\*\*  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=81814b15-ebdf-4817-932b-5ea7a37fa6ed)\*\*  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6b63a1eb-445a-4cd3-b357-9a1dd82d7a35)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für Itanium-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=9720a317-ca4c-4a47-b99c-2c66301e62c6)  
(KB2478661)  
(Kritisch)  
Nur Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=c8152a18-0367-4c00-a3c7-669325a899f4)  
(KB2478662)  
(Kritisch)  
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=c72635e4-c733-4fa1-9db0-75de6ead9e1c)<sup>[1]</sup>
(KB2478663)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c00a33bc-c874-4693-b0f7-5034c5df9424)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3c8455f1-b8a0-4ba2-84a2-043d25ef75c5)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=93a32bd9-7e67-4ace-8c45-116f91b032f9)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für Itanium-basierte Systeme: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=bff13134-ed84-4370-beb4-340c340a5d98)  
(KB2518867)  
(Kritisch)  
Nur Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1: [Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=dab623bf-d23d-42a9-9e74-ae75d779b980)  
(KB2518869)  
(Kritisch)  
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1: [Microsoft .NET Framework 4.0](https://www.microsoft.com/download/details.aspx?familyid=f7afba05-974f-48f8-b600-9e131ceb7951)<sup>[1]</sup>
(KB2518870)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ab2406a8-06f7-4f88-9af4-dc136d64bc35)  
(Kritisch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweise für MS11-039**

<sup>[1]</sup>**.NET Framework 4.0 und .NET Framework 4.0 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4.0 und .NET Framework 4.0 Client Profile. .NET Framework 4.0 Client Profile ist Teil von .NET Framework 4.0. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4.0 als auch .NET Framework 4.0 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](http://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweise für MS11-044**

<sup>[1]</sup>**.NET Framework 4.0 und .NET Framework 4.0 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4.0 und .NET Framework 4.0 Client Profile. .NET Framework 4.0 Client Profile ist Teil von .NET Framework 4.0. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4.0 als auch .NET Framework 4.0 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](http://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

<sup>[2]</sup>Bewertungen des Schweregrads treffen nicht auf dieses Update zu, da diese Software nicht von der Sicherheitsanfälligkeit betroffen ist, die in diesem Bulletin erörtert wird. Als Tiefenverteidigungsmaßnahme zum Schutz vor möglicherweise in der Zukunft entdeckten Sicherheitsanfälligkeiten empfiehlt Microsoft jedoch den Benutzern dieser Software, dieses Sicherheitsupdate zu installieren.

**Tabelle 2**

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
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=6c760c7f-94f1-437f-a645-fd33b50d03f4)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0b88f9e9-3439-44e5-92c8-66a3c97cb03d)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=03b45ad8-cc6b-473b-8112-bd513ed97f5d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=ce5bc2d7-9438-4bf0-be5e-be9dd00c3286)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=a1db7736-f3e4-45df-af1d-52746978a0a8)  
(Hoch)
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
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=c94c0d17-fdbe-41b3-a23d-98f43f907b89)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=ff955dc3-58ca-40ea-b7f1-9ff40c37f997)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ed502ece-737e-44cb-84fd-8a0d1bc321c8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7b211b02-a005-46a3-ad1d-d4baaeec8289)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=71497891-41a2-476d-b524-4eb5cecb9639)  
(Hoch)
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
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Niedrig**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5dafb455-969e-4be9-8735-d4ee0682d22f)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=ba3beb80-a921-489e-a6ff-a7b2d665ada6)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=a8038325-0d14-445b-a5d9-ce7ac1fa44b5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6427ea5d-05d0-4367-805c-9cb305802b3c)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c614cb8b-223e-4f84-b94c-f15747760aa5)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ef90d6c1-ea7f-4c32-9c90-0303e04c7436)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=e78829d0-8215-4e56-8959-ebd3bc8e9a91)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=3bec943e-5758-4439-a947-a8fafd30edec)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5f7bcbad-f647-4fbb-88d4-b19c54db6f00)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7f65891-32c0-4817-b3b2-d8be73145df9)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9a951087-25c5-4f5c-8407-a1585491ae0b)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=62944095-33d6-4131-be32-a79d9ec4d4a9)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=1e822515-9f0a-4ef0-bb70-d4889d200f47)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=47a0fdc6-7576-4c32-b8fd-cbb05d57599d)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ca8b1d09-9f80-417b-99b1-8f86e86e1f11)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=dd48b93b-24fa-45a3-91fb-9f9f9418c49f)  
(Hoch)
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
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
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
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=e541f1bb-c9bf-4dc8-96ec-58a3de5ba7fd)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=cd059690-52b0-4b37-9fbb-d9906ae46fed)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ebea38a7-1fbe-4141-a529-52d7a7326d6a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b69e3bda-940b-4524-a724-0af4ae0ec719)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5f0007c3-8d11-4940-8766-1112e3777aae)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=6c7d7162-ef19-49f4-a8fc-5db7415445a4)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=256bb26f-df9e-4259-881b-e8313a9fafa8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=54833350-a385-4a31-995a-9ddc38798c21)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e3a26bc5-1757-4b38-9cae-419c919f4877)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fadf6f12-1f09-4d49-93b1-8fce01400b4f)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Niedrig**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=4446121a-0aab-4fbc-ba74-68d7650e8bca)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ed089de4-c9ec-4ac7-a711-5f7cb29c05bc)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6a3bbd67-94db-40b2-8786-cb39a493ec92)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e34e4cf9-cdae-4240-8574-950c0be00822)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8960dd62-7cf7-41cb-97b2-b082bd1750aa)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=46ade106-e0cb-4c71-8230-793a15062823)\*\*  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=01399fc7-dc2b-461e-a1a5-751a3b61bde0)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=dd32b7c6-daa1-47aa-807f-25a678790cf2)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4cb870f3-9878-4075-b8fd-2ee90c8e3bc8)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a3604f05-26b2-451b-9153-0e718158371e)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=24789423-72b7-48d1-bdc1-f0e5174d99bb)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0abc6908-ac6a-4da3-843a-af6841ccc1db)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6141a1c5-ecaf-4553-9d27-dd6e5c4a13fd)\*\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=16a8b78a-3979-4cc7-bbe5-6d962aa64336)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e1243011-00e6-49f2-a676-c04cb805d36a)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e8a82b44-e1d8-45f8-b8b8-b1f74e1efce0)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=057f1356-9c70-4457-a1df-69334fdab467)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=27e767d8-84e3-434f-bb8d-3b2303774ad0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c3647646-658a-423b-b0cb-bba7613b67e7)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=63d8b801-5178-474b-a21e-72a0ce501d3e)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=cf9e5ecd-68f7-4982-b4ed-be80859b757c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=747ba56a-0d47-4946-99a4-bae1f11ea748)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=7996511d-4b8e-49c3-a0fa-4da907a6c947)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=cd7d3cb9-cb60-4b62-b0df-a38fe21802e9)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=2707650a-604c-4044-acc4-07a30b5640d8)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-052**](http://go.microsoft.com/fwlink/?linkid=218115)
</td>
<td style="border:1px solid black;">
[**MS11-037**](http://go.microsoft.com/fwlink/?linkid=217912)
</td>
<td style="border:1px solid black;">
[**MS11-046**](http://go.microsoft.com/fwlink/?linkid=217464)
</td>
<td style="border:1px solid black;">
[**MS11-047**](http://go.microsoft.com/fwlink/?linkid=217468)
</td>
<td style="border:1px solid black;">
[**MS11-048**](http://go.microsoft.com/fwlink/?linkid=215840)
</td>
<td style="border:1px solid black;">
[**MS11-051**](http://go.microsoft.com/fwlink/?linkid=217101)
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
[**Niedrig**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=cff7f53d-0fd6-48f8-a9d6-bf19e0a32905)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=40354f73-4f4d-4a4a-abac-f8a3d4c3ae5f)\*\*  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e67c73ca-d0f9-40c1-8b6e-25b1b13caa3a)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c9c6c36d-a455-42f7-b7d4-9fb9824c07cb)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=f9824310-772d-4e1e-980e-11e2db3ac53e)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1da04414-6210-43ea-8e0a-cf21cf144076)\*\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4dd2c0f4-b29c-4648-a123-83d3ae6a878f)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=22853823-8f63-4258-8991-1ad50e58a0d9)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=72d1d6b6-e8bd-492b-b65a-82060beef441)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0533d293-e186-4d39-a925-ab3d9ed46290)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

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
Microsoft Office Suites und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=853c0663-94f7-4634-98ad-47ca4b1f7b1e)  
(KB2541003)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f38f183a-9c64-406b-9bf6-807cb2d55e56)  
(KB2541025)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5b271f87-a279-419f-9437-ded224fa19f1)<sup>[1]</sup>
(KB2541007)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=baba7ec1-4a5e-4e13-9d0e-9085a39a0554)  
(KB2523021)  
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
[Microsoft Excel 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=d6e9f422-43b0-4da5-8356-c38482e8eebb)  
(KB2523021)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=d12d0868-4f28-4c0a-ab61-338878064b70)  
(KB2555786)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=9e2d348b-c753-4eab-838c-370cd5af5e14)  
(KB2555785)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=3c58555c-1eba-42fe-a10f-b30af9031e44)  
(KB2555784)  
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
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=6118d5f5-b6fd-4584-be25-209534772379)  
(KB2555787)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft InfoPath
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft InfoPath 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=88eedb0b-a2cf-4a1b-b1b9-0b2926c25872)  
(KB2510061)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft InfoPath 2010 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=90ffe910-bd9c-48aa-8007-2b43e1a99999)  
(KB2510065)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft InfoPath 2010 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=f3244003-fb63-44d8-bedc-6399c39aacba)  
(KB2510065)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-045**](http://go.microsoft.com/fwlink/?linkid=217502)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
[Microsoft Excel Viewer Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=77c1e7e2-207f-46fd-81f2-43a25eddc010)  
(KB2541015)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3512a033-871d-49ec-a8d2-1b9c7dec4936)  
(KB2541012)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS11-045**

<sup>[1]</sup>Für Microsoft Office Excel 2007 Service Pack 2 müssen Benutzer zusätzlich zum Sicherheitsupdatepaket KB2541007 auch das Sicherheitsupdate für Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2 (KB2541012) installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

**Hinweis für MS11-049**

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
Microsoft SQL Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
SQL Server 2005 Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 für Itanium-basierte Systeme Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 x64 Edition Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 x64 Edition Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 x64 Edition Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 für Itanium-basierte Systeme Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 für Itanium-basierte Systeme Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Express Edition Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Express Edition Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2005 Express Edition mit Advanced Services Service Pack 3
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=faca7f7a-c346-48e3-9bf5-f140a51aae4e)  
(KB2494113)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d214763c-5a16-4959-90ff-08112345d867)  
(KB2494112)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2005 Express Edition mit Advanced Services Service Pack 4
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2aba4a2e-477f-4267-9ebe-ab7b29d218ad)  
(KB2494120)  
(Hoch)  
QFE-Update:  
[SQL Server 2005 Express Edition mit Advanced Services Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=2975ad1a-1852-4771-b3fa-2be79899be57)  
(KB2494123)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server Management Studio Express (SSMSE) 2005
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server Management Studio Express (SSMSE) 2005](https://www.microsoft.com/download/details.aspx?familyid=34c3ba21-b158-4e6d-82ba-831053d41161)  
(KB2546869)  
(Hoch)  
QFE-Update:  
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server Management Studio Express (SSMSE) 2005 x64 Edition
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server Management Studio Express (SSMSE) 2005 x64 Edition](https://www.microsoft.com/download/details.aspx?familyid=34c3ba21-b158-4e6d-82ba-831053d41161)  
(KB2546869)  
(Hoch)  
QFE-Update:  
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2008 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)<sup>[1]</sup>
(KB2494096)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)<sup>[1]</sup>
(KB2494100)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2008 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)<sup>[1]</sup>
(KB2494096)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)<sup>[1]</sup>
(KB2494100)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2008 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ae7db514-d96b-4cff-a13d-c74f4cf8cf0c)  
(KB2494096)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=312a39c4-cb32-4216-8672-1b1c0937ba6c)  
(KB2494100)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)<sup>[1]</sup>
(KB2494089)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)<sup>[1]</sup>
(KB2494094)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)<sup>[1]</sup>
(KB2494089)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)<sup>[1]</sup>
(KB2494094)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6f4767bf-257d-4822-b768-7b6702261276)  
(KB2494089)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=23240963-e2c6-4d40-8179-661117b53e91)  
(KB2494094)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2008 R2 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 R2 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)<sup>[1]</sup>
(KB2494088)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 R2 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)<sup>[1]</sup>
(KB2494086)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
SQL Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)<sup>[1]</sup>
(KB2494088)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)<sup>[1]</sup>
(KB2494086)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
SQL Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
GDR-Update:  
[SQL Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=80e98567-1b28-49b1-a646-579f8c115a41)  
(KB2494088)  
(Hoch)  
QFE-Update:  
[SQL Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9df95137-d1b3-4fac-8958-8042aa2010c4)  
(KB2494086)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise** **für MS11-049**

<sup>[1]</sup>Dieses Update gilt auch für die Express und Express mit Advanced Series Editionen.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Entwicklertools und Software

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
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8) bei Installation unter Mac  
(KB2512827)  
(Kritisch)  
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8) bei Installation unter allen Versionen von Microsoft Windows-Clients  
(KB2512827)  
(Kritisch)  
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=2f71b104-b66f-4146-9d70-fcde766c91b8) bei Installation unter allen Versionen von Microsoft Windows-Servern\*\*  
(KB2512827)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Visual Studio
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-039**](http://go.microsoft.com/fwlink/?linkid=212287)
</td>
<td style="border:1px solid black;">
[**MS11-049**](http://go.microsoft.com/fwlink/?linkid=217077)
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2005 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2005 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e5ce8a9a-e89b-4095-9f21-7e6f307fbf2b)  
(KB2251481)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visual Studio 2008 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2008 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=cc01bce9-3f38-4590-9c6e-a4048c886d33)  
(KB2251487)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visual Studio 2010
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Visual Studio 2010](https://www.microsoft.com/download/details.aspx?familyid=213b820f-dcba-4895-b339-b50eeb92524d)  
(KB2251489)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für MS11-039**

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweis für MS11-049**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

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
Microsoft Forefront
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-040**](http://go.microsoft.com/fwlink/?linkid=217470)
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
Microsoft Forefront Threat Management Gateway 2010 Client
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Threat Management Gateway 2010 Client](https://www.microsoft.com/download/details.aspx?familyid=d1c85acd-a6df-4634-9cd4-c562ad92097e)  
(Kritisch)
</td>
</tr>
</table>
 

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheitscenter](http://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](http://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](http://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](http://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](http://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://technet.microsoft.com/de-de/windowsserver/bb332157).

**System Center Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](http://www.microsoft.com/germany/systemcenter/sccm/evaluation/updatemgmt.mspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](http://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](http://support.microsoft.com/common/international.aspx?rdpath=dm;de-de;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](http://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc749197(ws.10).aspx), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/en-us/wsus/bb456965.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Billy Rios und Eduardo Vela Nava vom [Google Security Team](http://www.google.com/) für die Zusammenarbeit mit uns an den Änderungen zu MS11-037.
-   Yamata Li von [Palo Alto Networks](http://www.paloaltonetworks.com/) für den Hinweis auf ein in MS11-038 beschriebenes Problem.
-   Michael J. Liu für den Hinweis auf ein in MS11-039 beschriebenes Problem.
-   Koro von [www.korosoft.net](http://www.korosoft.net/) für den Hinweis auf ein in MS11-041 beschriebenes Problem.
-   Laurent Gaffié von [NGS Software](http://www.ngssoftware.com/) für den Hinweis auf ein in MS11-042 beschriebenes Problem.
-   Dan Kaminsky für die Zusammenarbeit mit uns an einem in MS11-044 beschriebenen Problem.
-   Bing Liu von [Fortinets FortiGuard Labs](http://www.fortiguard.com/) für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Einer Person, die mit [iDefense VCP](http://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Omair in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Einer Person, die mit [iDefense VCP](http://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Nicolas Gregoire von [Agarri](http://www.agarri.fr/), in Zusammenarbeit mit den [VeriSign iDefense Labs](http://labs.idefense.com/), für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Omair für den Hinweis auf ein in MS11-045 beschriebenes Problem.
-   Will Dormann von [CERT/CC](http://www.cert.org/) für den Hinweis auf zwei in MS11-045 beschriebene Probleme.
-   Steven Adair von der [Shadowserver Foundation](http://www.shadowserver.org) und Chris S. für den Hinweis auf ein in MS11-046 beschriebenes Problem.
-   Nicolas Economou von [Core Security Technologies](http://www.coresecurity.com/) für den Hinweis auf ein in MS11-047 beschriebenes Problem.
-   Jesse Ou von [Cigital](http://www.cigital.com) für den Hinweis auf ein in MS11-049 beschriebenes Problem.
-   Robert Swiecki von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   [NSFOCUS Security Team](http://www.nsfocus.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Einer Person, die mit dem [Beyond Security's SecuriTeam Secure Disclosure](http://www.beyondsecurity.com/ssd.html)-Programm zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Adi Cohen von [IBM Rational Application Security](http://blog.watchfire.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   [Trend Micro](http://www.trendmicro.com/) für die Zusammenarbeit mit uns an einem in MS11-050 beschriebenen Problem.
-   Nirmal Singh Bhary von [Norman](http://www.norman.com) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Damian Put in Zusammenarbeit mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Yoel Gluck, Yogesh Badwe und Varun Badhwar vom Produktsicherheitsteam von [salesforce.com](http://www.salesforce.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Peter Winter-Smith in Zusammenarbeit mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) für den Hinweis auf ein in MS11-050 beschriebenes Problem.
-   Stephen Fewer von [Harmony Security](http://www.harmonysecurity.com/) in Zusammenarbeit mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) für die Zusammenarbeit mit uns an den in MS11-050 behobenen Tiefenverteidigungsänderungen.
-   Ruggero Strabla, [Emaze](http://www.emaze.net/) Networks; [Saipem Security Team](http://www.saipem.com/) für den Hinweis auf ein in MS11-051 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-052 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (14. Juni 2011): Bulletin Summary veröffentlicht.
-   V1.1 (14. Juni 2011): Für MS11-042 wurden Windows 7 für 32-Bit-Systeme Service Pack 1, Windows 7 für x64-basierte Systeme Service Pack 1, Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1 aus dem Unterabschnitt **Betroffene Software und Downloadadressen** entfernt. Dies ist lediglich eine Informationsänderung. An den Dateien des Sicherheitsupdates oder der Erkennungslogik wurden keine Änderungen vorgenommen.
-   V2.0 (9. August 2011): MS11-043 wurde erneut veröffentlicht, um das Update für alle unterstützten Betriebssysteme neu anzubieten und ein Stabilitätsproblem zu beheben. Endbenutzer, die ihre Systeme bereits erfolgreich aktualisiert haben, sollten MS11-043 erneut installieren. Außerdem wurde MS11-049 erneut veröffentlicht, um eine Erkennungsänderung am Update für Microsoft Visual Studio 2005 Service Pack 1 anzukündigen, um Erkennung für verwandte Software hinzuzufügen. Es gab keine Änderungen an den Sicherheitsupdatedateien in MS11-049. Endbenutzer, die ihre Systeme bereits erfolgreich aktualisiert haben, müssen MS11-049 nicht erneut installieren.
-   V2.1 (26. Oktober 2011): Für MS11-039 und MS11-044 wurde die Anwendbarkeit der Server Core-Installation für .NET Framework 4 unter Windows Server 2008 R2 für x64-basierte Systeme korrigiert.
-   V3.0 (8. November 2011): MS11-037 wird erneut angeboten, um das Update für alle unterstützten Editionen von Windows XP und Windows Server 2003 erneut anzubieten. Benutzer, die Windows XP oder Windows Server 2003 verwenden, einschließlich jener, die das ursprünglich am 14. Juni 2011 angebotene Update bereits erfolgreich installiert haben, sollten das erneut angebotene Update installieren.
-   V3.1 (18. Januar 2012): Für MS11-049 wurde dem Abschnitt „Betroffene Software und Downloadadressen“ ein Hinweis hinzugefügt, um zu erklären, dass dieses Update auch für 32-Bit- und x64-basierte SQL Server 2008 und SQL Server 2008 R2 Express und Express Advanced Editionen gilt.

*Built at 2014-04-18T01:50:00Z-07:00*