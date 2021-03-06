---
TOCTitle: 'MS11-OCT'
Title: Microsoft Security Bulletin Summary für Oktober 2011
ms:assetid: 'ms11-oct'
ms:contentKeyID: 61225101
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-oct(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Oktober 2011
====================================================

Veröffentlicht: Dienstag, 11. Oktober 2011 | Aktualisiert: Mittwoch, 26. Oktober 2011

**Version:** 1.1

In diesem Bulletin Summary sind die im Oktober 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Oktober 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 6. Oktober 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 12. Oktober 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Oktober.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487956) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://go.microsoft.com/fwlink/?linkid=217214)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework und Microsoft Silverlight kann Remotecodeausführung ermöglichen (2604930)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft .NET Framework und Microsoft Silverlight. Die Sicherheitsanfälligkeit kann Remotecodeausführung auf einem Clientsystem ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAPs) oder Silverlight-Anwendungen ausführen kann. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Die Sicherheitsanfälligkeit kann auch Remotecodeausführung auf einem Serversystem ermöglichen, auf dem IIS ausgeführt wird, wenn dieser Server die Verarbeitung von ASP.NET-Seiten zulässt und ein Angreifer erfolgreich eine speziell gestaltete ASP.NET-Seite auf den Server hochlädt und dann ausführt, wie es in einem Webhostingszenario der Fall sein kann. Diese Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft .NET Framework, Microsoft Silverlight</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2586448)</strong><br />
<br />
Dieses Sicherheitsupdate behebt acht vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Active Accessibility kann Remotecodeausführung ermöglichen (2623699)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Microsoft Active Accessibility-Komponente. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine gültige Datei zu öffnen, die sich im selben Netzwerkverzeichnis befindet wie eine speziell gestaltete DLL-Datei (Dynamic Link Library). Beim Öffnen der gültigen Datei kann die Microsoft Active Accessibility-Komponente dann versuchen, die DLL-Datei zu laden und den darin enthaltenen Code auszuführen. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und an diesem Ort ein Dokument öffnen, das dann von einer anfälligen Anwendung geladen wird.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media Center kann Remotecodeausführung ermöglichen (2604926)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Windows Media Center. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer einen Benutzer dazu verleitet, eine gültige Datei zu öffnen, die sich im selben Netzwerkverzeichnis befindet wie eine speziell gestaltete DLL-Datei (Dynamic Link Library). Wenn dann die legitime Datei geöffnet wird, kann Windows Media Center versuchen, die DLL-Datei zu laden und den darin enthaltenen Code auszuführen. Damit ein Angriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und dort eine gültige Datei öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Remotecodeausführung ermöglichen (2567053)</strong><br />
<br />
Dieses Sicherheitsupdate behebt vier vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Schriftartdatei (z. B. eine FON-Datei) in einer Netzwerkfreigabe, einem UNC oder einem WebDAV-Speicherort öffnet oder eine E-Mail-Anlage öffnet. Damit ein Remoteangriff erfolgreich ist, muss ein Benutzer einen nicht vertrauenswürdigen Speicherort eines Remotedateisystems oder eine WebDAV-Freigabe besuchen und die speziell gestaltete Schriftartdatei öffnen, oder die Datei als E-Mail-Anlage öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Forefront Access Gateway können Remotecodeausführung ermöglichen (2544641)</strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten in Forefront Unified Access Gateway (UAG). Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Remotecodeausführung ermöglichen, wenn ein Benutzer mit einer speziell gestalteten URL eine betroffene Website besucht. Ein Angreifer kann Benutzer jedoch nicht zum Besuch einer Website zwingen. Er muss den Benutzer zum Besuch dieser Website verleiten. Zu diesem Zweck wird der Benutzer meist dazu gebracht, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Forefront United Access Gateway</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Treiber für zusätzliche Funktionen kann Erhöhung von Berechtigungen ermöglichen (2592799)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft Windows-Treiber für zusätzliche Funktionen (AFD). Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei dem System eines Benutzers anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Host Integration Server können Denial-of-Service ermöglichen (2607670)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Host Integration Server. Die Sicherheitsanfälligkeiten können Denial-of-Service ermöglichen, wenn ein Remoteangreifer einem Host Integration Server, der den UDP-Port 1478 oder die TCP-Ports 1477 und 1478 abhört, speziell gestaltete Netzwerkpakete sendet. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen. In diesem Fall sollten die Host Integration Server-Ports vom Internet blockiert werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Host Integration Server</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/security/cc998259.aspx).
  
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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=221538">MS11-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in aktiven Eingabehilfen bezüglich nicht sicheren Ladens von Bibliotheken</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1247">CVE-2011-1247</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227073">MS11-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Media Center aufgrund nicht sicheren Ladens von Bibliotheken</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2009">CVE-2011-2009</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich NULL-Zeigerdereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1985">CVE-2011-1985</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Pufferüberlauf in der Schriftartbibliotheksdatei</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2003">CVE-2011-2003</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=225915">MS11-077</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit durch Win32k-Verwendung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2011">CVE-2011-2011</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227075">MS11-078</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in .NET Framework durch Vererbung in Klassen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1253">CVE-2011-1253</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">3</a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Antwortaufteilung in ExcelTable aufgrund siteübergreifender Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1895">CVE-2011-1895</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Offenlegung von Information auf bestimmten Plattformen, auf die im Bulletin verwiesen wird</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ExcelTable aufgrund reflektierter siteübergreifender Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1896">CVE-2011-1896</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Offenlegung von Information auf bestimmten Plattformen, auf die im Bulletin verwiesen wird</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit aufgrund reflektierter siteübergreifender Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1897">CVE-2011-1897</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Offenlegung von Information auf bestimmten Plattformen, auf die im Bulletin verwiesen wird</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Ausführung vergifteten Codes</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1969">CVE-2011-1969</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=217472">MS11-079</a></td>
<td style="border:1px solid black;">Cookieabsturz in Null-Sitzung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2012">CVE-2011-2012</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service führen</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=227486">MS11-080</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Treiber für zusätzliche Funktionen bezüglich Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2005">CVE-2011-2005</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung durch Bildlaufereignis</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1993">CVE-2011-1993</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLEAuto32.dll bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1995">CVE-2011-1995</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Optionselement bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1996">CVE-2011-1996</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung aufgrund von OnLoad-Ereignis</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1997">CVE-2011-1997</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Jscript9.dll bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1998">CVE-2011-1998</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Select-Element bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1999">CVE-2011-1999</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Textelement bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2000">CVE-2011-2000</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=226382">MS11-081</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung durch Beschädigung der virtuellen Funktionstabelle</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2001">CVE-2011-2001</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich DoS durch Endlosschleife in snabase.exe</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2007">CVE-2011-2007</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.<br />
<br />
Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=228596">MS11-082</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich DoS durch Zugriff auf nicht zugewiesenen Speicher</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2008">CVE-2011-2008</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.<br />
<br />
Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des** **Gesamtschweregrads**
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
Keine
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
[Microsoft .NET Framework 1.0 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=a54a7ad5-0504-4cc6-9eca-ba9f31c35a17)  
(KB2572066)  
(Nur Media Center Edition 2005 und Tablet PC Edition 2005)  
(Kritisch)  
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=822f91f5-bf92-42c4-ad33-b971be37d772)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=e942554d-6cb6-4e48-a876-3470671a95a2)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=a911b5b0-5e46-4a37-83e7-595e20585c56)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=96af60b9-4b8d-4a9b-b125-10775bb48252)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=9157e677-ab3f-44b0-9735-192bc7421ba7)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f1b2dceb-5bef-4522-9001-8dff0545d805)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=6260318c-e579-4cdf-93e3-4608892bc79e)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=f04ad852-1418-4fc4-bd57-f47895bbf3a8)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=67ebf641-1341-4642-96ba-bab5446d7b5d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c8fcf427-17d0-4caa-b406-50703f980862)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0f2444ac-61bd-47cf-9c1e-da86a2b0cfb5)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9a37864e-8543-4c52-aa73-e3c190860d76)  
(Hoch)
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b968b0bd-577b-4ea2-a192-a80fe7c20791)  
(KB2572069)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=172c55f3-6249-4ba3-a4a4-677a03262ff3)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=6ffbdb93-7b92-4197-bb6c-5c305e8072a8)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=14ef20d4-3530-49b2-91b7-d278d9098023)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=09e178f8-2bd2-46e1-b975-4938ee1f304d)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3bd62bf6-3400-4c03-95fe-148112b341e8)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=29228167-b811-43d7-b4a0-91e385b598a5)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=f5a0a8db-34d4-4f0a-ab6b-7b2fb420ab91)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=7379b3bf-6af0-43cb-bf8b-505e8563fc84)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=b35c95f5-30b0-43a9-aa6a-6db63cab0dcb)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9b8030db-1f47-4666-8cb5-1c56577f2340)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b73f4e87-9655-46d5-beb2-ea245dcd280d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0816d729-6769-4ca6-a14e-71750eca8d29)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=719b3da5-52ca-4d56-a2c5-69711039e59d)  
(KB2572073)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5825cb4a-47d5-423f-b4c5-2d0fc50856c0)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=11c4878e-df58-4369-b9c0-cb0a230c92dd)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=82653b8c-0e58-440d-9702-8847f599caed)  
(KB2605295)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a618cc19-5ebc-462e-a518-d9bfe41ed98e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=42465652-2664-4fd5-9a22-ae847b08e7c8)  
(Hoch)
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=630335ac-5a30-46b4-acc1-c4d8bd289668)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=76c8124e-81b9-4a6a-bd53-fbdaf45189aa)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7de276a3-a20d-49de-82b0-51cb22ad73af)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=96b089c0-a2e7-44cb-9fc4-9569b3993afa)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=44f7f10b-86ff-470f-996a-d4aa51c4d18f)  
(KB2579686)  
(Hoch)  
[Windows Media Center TV Pack für Windows Vista (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=60e50f72-4001-423c-831c-8ff1f1b8f090)<sup>[1]</sup>
(KB2579692)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ff53d01b-97b7-40d2-af88-4978f1099a7c)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=9aabd7a2-0b2f-4c42-a9cf-2ec69ae6b82d)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3454940c-acc2-4e09-8154-075b4be1b697)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=3df0c31b-344a-4163-93d2-79df1653b339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b79a389c-8340-4dd2-9ab1-a0943c5a220f)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=cbb66cd7-2688-410f-8a03-fd28e6ef5b01)  
(KB2579686)  
(Hoch)  
[Windows Media Center TV Pack für Windows Vista (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=371c7dab-5aa6-4502-80ee-ae69b736b972)<sup>[1]</sup>
(KB2579692)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=47322e11-f1cf-4f70-b939-8cac9bbfc2bc)  
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=5660e23c-13a3-4275-ac69-38f03f17491a)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=bd144435-1afd-4d6e-a100-fbd613eee409)\*\*  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=1a7f9855-20ce-4fe0-a903-bd1f145075df)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7cd1ecec-8a3f-4cb2-833c-a177c9602ff5)\*  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c7498ee-eba4-44fd-8846-0b2e96c96705)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)\*\*  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)\*\*  
(KB2572075)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*\*<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=415b1c59-f3dc-4f4f-b2eb-68692d6efc05)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=b0c4949f-bce0-4255-a5f2-cf5ecf7416da)\*\*  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=28a09e42-5865-48b2-af26-ebc8162c3286)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=456e450c-3928-4130-8127-e4d3f482c1ca)\*  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=40386742-f397-402e-8810-63d3d6ba12a6)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=6100e577-deb5-4395-b851-e19e0ca79507)  
(KB2572067)  
(Kritisch)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c27128d-eaf9-4416-b8b1-9edab9102feb)  
(KB2572075)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=31e68c7f-4db5-463f-a315-92f574af080b)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2e9930d3-ba13-446d-bfa0-60720c48203b)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3633402b-96cb-4f36-b137-d07d1baf28c7)  
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritisch)  
Nur Windows 7 für 32-Bit-Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4de175be-bbb7-4912-ba4e-d6fe96606c9e)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b49876c7-7c65-4b6d-be9a-9f18be23037b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=02d28e59-b38f-433a-a568-e86f9d43dd42)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=76fcf0ec-9062-4090-acb2-401355341a2b)  
(KB2579686)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9e40bc26-f77f-4b57-9b3d-9d053c19ac56)  
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
Nur Windows 7 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritisch)  
Nur Windows 7 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=16fd238e-6f65-4d38-88ae-2689817588e1)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=cc0773f2-6099-4d55-9971-ee6546369c7f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=904dec69-e8b9-4b23-a5ea-d3e7e9b9df07)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=78c099b7-4bcb-4da7-8967-512c6541c541)  
(KB2579686)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=219554e6-eb5a-42d0-90c0-42b4d0772cfd)  
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
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
</td>
<td style="border:1px solid black;">
[**MS11-081**](https://go.microsoft.com/fwlink/?linkid=226382)
</td>
<td style="border:1px solid black;">
[**MS11-075**](https://go.microsoft.com/fwlink/?linkid=221538)
</td>
<td style="border:1px solid black;">
[**MS11-076**](https://go.microsoft.com/fwlink/?linkid=227073)
</td>
<td style="border:1px solid black;">
[**MS11-077**](https://go.microsoft.com/fwlink/?linkid=225915)
</td>
<td style="border:1px solid black;">
[**MS11-080**](https://go.microsoft.com/fwlink/?linkid=227486)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)\*  
(KB2572076)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)\*  
(KB2572077)  
(Kritisch)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)\*<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=8435781e-0f77-41d0-abb9-9b70f5b02d33)\*\*  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=646a9a56-c343-45cb-a255-303602aa5a64)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c7bd50b7-03f1-4ea4-ad71-d428822c62f8)\*  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=39bd4cfb-fe61-41b8-a5a2-73a9e720fc72)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=81be7ff1-3ba2-430c-9edf-619cc246daf2)  
(KB2572076)  
(Kritisch)  
Nur Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=98403988-7438-4260-95b5-a4796dbe0618)  
(KB2572077)  
(Kritisch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=770e7b58-6544-4f59-9893-b3eadf6d6c8a)<sup>[1]</sup>
(KB2572078)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=2676597e-c1d4-4397-8dc4-515ce3d0c5fd)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=aa816682-9652-433c-b1b4-5d0bc17b6a87)  
(KB2564958)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0d35c6d0-6d2d-42bf-a97f-4c5e01b1937e)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise** **für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-078**

<sup>[1]</sup>**.NET Framework 4 und .NET Framework 4 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4 und .NET Framework 4 Client Profile. .NET Framework 4 Client Profile ist Teil von .NET Framework 4. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4 als auch .NET Framework 4 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](https://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

**Hinweis für MS11-076**

<sup>[1]</sup>Windows Media Center TV Pack für Windows Vista ist nur auf OEM-Installationen (Originalgerätehersteller) der Home Premium- und Ultimate-Editionen von Windows Vista als optionale Komponente verfügbar. Benutzer, die diese optionale Komponente auf ihren x64-basierten Systemen installiert haben, sollten beide verfügbaren Updates installieren. Im Einklang mit den empfohlenen Vorgehensweisen empfiehlt Microsoft, das Update des Betriebssystems (KB2579686) zu installieren, bevor das Windows Media Center TV Pack-Update (KB2579692) installiert wird. Endbenutzer, die das Media Center TV Pack auf 32-Bit-Systemen installiert haben, müssen nur KB2579692 installieren.

#### Microsoft Server-Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Host Integration Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-082**](https://go.microsoft.com/fwlink/?linkid=228596)
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
Microsoft Host Integration Server 2004
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2004 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b7536139-63ea-482a-8d1c-0faad1fcfaa4)  
(KB2578757)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2006
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2006 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=3bc0c89c-56b2-4463-b671-2a58bed9667b)  
(KB2579597)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Host Integration Server 2009
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2009](https://www.microsoft.com/download/details.aspx?familyid=28716ed4-f215-4c69-b6b8-63fbeecefc5b)  
(KB2579598)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Host Integration Server 2010
</td>
<td style="border:1px solid black;">
[Microsoft Host Integration Server 2010](https://www.microsoft.com/download/details.aspx?familyid=dbbd67d8-68aa-424d-8eaf-a273a71624d1)  
(KB2579599)  
(Hoch)
</td>
</tr>
</table>
 

#### Microsoft Entwicklertools und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Silverlight
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-078**](https://go.microsoft.com/fwlink/?linkid=227075)
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
Microsoft Silverlight 4
</td>
<td style="border:1px solid black;">
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) bei Installation unter Mac  
(KB2617986)  
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Clients  
(KB2617986)  
[Microsoft Silverlight 4](https://www.microsoft.com/download/details.aspx?familyid=8bde4992-bdf7-4345-835a-4e1fbfcd8c5f) bei Installation unter allen unterstützten Versionen von Microsoft Windows-Servern\*\*  
(KB2617986)
</td>
</tr>
</table>
 
**Hinweise** **für MS11-078**

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft-Software für Remotezugriff

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Forefront Unified Access Gateway
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-079**](https://go.microsoft.com/fwlink/?linkid=217472)
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
Microsoft Forefront Unified Access Gateway
</td>
<td style="border:1px solid black;">
[Microsoft Forefront Unified Access Gateway 2010](https://www.microsoft.com/download/details.aspx?familyid=770ad8ba-4d9a-404e-9515-6ed1e41682df)<sup>[1]</sup>
(KB2522482)  
(Hoch)  
[Microsoft Forefront Unified Access Gateway 2010 Update 1](https://www.microsoft.com/download/details.aspx?familyid=b0de8d20-9c25-41c0-9c02-d263b9ed22fa)<sup>[1]</sup>
(KB2522483)  
(Hoch)  
[Microsoft Forefront Unified Access Gateway 2010 Update 2](https://www.microsoft.com/download/details.aspx?familyid=166bdfcb-5088-4471-9d51-a3071ac13b73)<sup>[1]</sup>
(KB2522484)  
(Hoch)  
[Microsoft Forefront Unified Access Gateway 2010 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8b6ad2ae-e168-45d9-bd3f-5590e0cbd2b5)<sup>[1]</sup>
(KB2522485)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis** **für MS11-079**

<sup>[1]</sup>Dieses Update ist nur im Microsoft Download Center verfügbar.

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

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://technet.microsoft.com/de-de/windowsserver/bb332157).

**System Center Configuration Manager 2007**

Configuration Manager 2007-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit Configuration Manager 2007 können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in Configuration Manager 2007 erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in Configuration Manager 2007 ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen dazu, wie Administratoren mithilfe von Configuration Manager 2007 Updates bereitstellen können, finden Sie in [Softwareupdateverwaltung](https://www.microsoft.com/germany/systemcenter/sccm/evaluation/updatemgmt.mspx). Weitere Informationen zu Configuration Manager finden Sie auf der Website [System Center Configuration Manager](https://www.microsoft.com/germany/systemcenter/sccm/default.mspx).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/common/international.aspx?rdpath=dm;de-de;lifecycle). Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager 2007**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/downloads/en/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f&displaylang=en). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/en-us/systemcenter/bb545936.aspx).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/downloads/de-de/details.aspx?familyid=7bd3a16e-1899-4e0b-bb99-1320e816167d&displaylang=de) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

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

-   [Mila Parkour](https://contagiodump.com) in Zusammenarbeit mit Anshul Kothari und Nishant Kaushik von [Adobe Systems, Inc.](https://www.adobe.com) für den Hinweis auf ein in MS11-075 beschriebenes Problem
-   Andrei Lutas von [BitDefender](https://www.bitdefender.com/) für den Hinweis auf ein in MS11-077 beschriebenes Problem
-   Tarjei Mandt von [Norman](https://www.norman.com/) für den Hinweis auf ein in MS11-077 beschriebenes Problem
-   Maik Wellmann für den Hinweis auf ein in MS11-077 beschriebenes Problem
-   Will Dormann von [CERT/CC](https://www.cert.org/) für den Hinweis auf ein in MS11-077 beschriebenes Problem
-   Einer Person, die mit dem [Beyond Security's SecuriTeam Secure Disclosure](https://www.beyondsecurity.com/ssd.html)-Programm zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-078 beschriebenes Problem
-   [Tenable Network Security](https://www.tenable.com/) für den Hinweis auf drei in MS11-079 beschriebene Probleme
-   Elisabeth Demeter von [SEC Consult Unternehmensberatung GmbH](https://www.sec-consult.com/) für den Hinweis auf ein in MS11-079 beschriebenes Problem.
-   Bo Zhou von der [National University of Defense Technology](https://www.nudt.edu.cn/) für den Hinweis auf ein in MS11-080 beschriebenes Problem
-   Vishwas Sharma von McAfee Labors für den Hinweis auf ein in MS11-081 beschriebenes Problem
-   David Bloom von [Greplin](https://www.greplin.com) für den Hinweis auf in MS11-081 beschriebene Probleme
-   Ivan Fratric in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com) von [TippingPoint](https://www.tippingpoint.com) für den Hinweis auf in MS11-081 beschriebene Probleme
-   [GWSlabs](https://www.gwslabs.com) in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com) für den Hinweis auf ein in MS11-081 beschriebenes Problem
-   Sebastian Apelt in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com) von [TippingPoint](https://www.tippingpoint.com) und für den Hinweis auf ein in MS11-081 beschriebenes Problem
-   Einer Person, die mit [Zero Day Initiative](https://www.zerodayinitiative.com) von [TippingPoint](https://www.tippingpoint.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-081 beschriebenes Problem
-   Eduardo Vela Nava von [Google Inc.](https://www.google.com) und David Bloom von [Greplin](https://www.greplin.com) für die Zusammenarbeit mit uns an in MS11-081 enthaltenen Tiefenverteidigungsänderungen
-   [Soroush Dalili](https://www.secproject.com) für die Zusammenarbeit mit uns an in MS11-081 enthaltenen Tiefenverteidigungsänderungen.
-   Billy Rios von [Google Inc.](https://www.google.com) für die Zusammenarbeit mit uns an den tiefgreifenden Verteidigungsänderungen in MS11-081

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (11. Oktober 2011): Bulletin Summary veröffentlicht.
-   V1.1 (26. Oktober 2011): Für MS11-078 wurde die Anwendbarkeit der Server Core-Installation für .NET Framework 4 unter Windows Server 2008 R2 für x64-basierte Systeme korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*