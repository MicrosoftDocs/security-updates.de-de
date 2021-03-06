---
TOCTitle: 'MS11-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2011
ms:assetid: 'ms11-feb'
ms:contentKeyID: 61225094
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-feb(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Februar 2011
====================================================

Veröffentlicht: Dienstag, 8. Februar 2011 | Aktualisiert: Freitag, 18. März 2011

**Version:** 4.0

In diesem Bulletin Summary sind die im Februar 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Februar 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 3. Februar 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 9. Februar 2011 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Februar](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?eventid=1032455047&eventcategory=4). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2482017)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete und zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mithilfe von Internet Explorer anzeigt, oder wenn ein Benutzer eine gültige HTML-Datei öffnet, die eine speziell gestaltete Bibliotheksdatei lädt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit bei Grafikverarbeitung in Windows Shell kann Remotecodeausführung ermöglichen (2483185)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Grafikprozessor von Windows Shell. Wenn ein Benutzer ein speziell gestaltetes Miniaturbild anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im OpenType CFF-Treiber (Compact Font Format) kann Remotecodeausführung ermöglichen (2485376)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows OpenType CFF-Treiber (Compact Font Format). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer Inhalte anzeigt, die in einer speziell gestalteten CFF-Schriftart dargestellt werden. Ein Angreifer kann Benutzer nicht zwingen, die speziell gestalteten Inhalte anzuzeigen. Der Angreifer müsste statt dessen den Benutzer zum Besuch einer Webseite verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im FTP-Dienst der Internetinformationsdienste kann Remotecodeausführung ermöglichen (2489256)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit im Microsoft-FTP-Dienst für Internetinformationsdienste (IIS). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein FTP-Server einen speziell gestalteten FTP-Befehl erhält. Der FTP-Dienst ist nicht standardmäßig auf IIS installiert.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory kann Denial-of-Service ermöglichen (2478953)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Active Directory. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer ein speziell gestaltetes Paket an einen betroffenen Active Directory-Server sendet. Der Angreifer muss gültige lokale Administratorberechtigungen auf dem Computer haben, der einer Domäne angehört, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Visio können Remotecodeausführung ermöglichen (2451879)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Visio. Die Sicherheitsanfälligkeiten können eine Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Visio-Datei öffnet. Ein Angreifer, der eine dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale angemeldete erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in den Skriptmodulen JScript und VBScript kann Offenlegung von Information ermöglichen (2475792)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den Skriptmodulen JScript und VBScript. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine speziell gestaltete Website besucht. Ein Angreifer kann Benutzer nicht zum Besuch dieser Websites zwingen. Der Angreifer müsste statt dessen den Benutzer zum Besuch dieser Webseite verleiten, z. B. indem er den Benutzer dazu auffordert, in einer E-Mail oder einer Instant Messenger-Nachricht auf einen Link zur Website des Angreifers zu klicken.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Client/Server-Runtime-Subsystem kann Erhöhung von Berechtigungen ermöglichen (2476687)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft Windows Client/Server-Runtime-Subsystem (CSRSS) in Windows XP und Windows Server 2003.<br />
<br />
Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich beim System eines Benutzers anmeldet und eine speziell gestaltete Anwendung startet, die weiter ausgeführt wird, nachdem der Angreifer sich abgemeldet hat. Dadurch erhält jener die Anmeldeinformationen nachfolgender Benutzer. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (2393802)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreibern können Erhöhung von Berechtigungen ermöglichen (2479628)</strong><br />
<br />
Dieses Sicherheitsupdate behebt fünf vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Kerberos können Erhöhung von Berechtigungen ermöglichen (2496930)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit und eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die schwerwiegendere dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein lokaler, authentifizierter Angreifer einen schädlichen Dienst auf einem Computer installiert, der einer Domäne angehört.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Subsystemdienst für die lokale Sicherheitsautorität kann Erhöhung lokaler Berechtigungen ermöglichen (2478960)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im LSASS-Dienst (Local Security Authority Subsystem Service, Subsystemdienst für die lokale Sicherheitsautorität) in Windows XP und Windows Server 2003.<br />
<br />
Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
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
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Ausnutzbarkeitsindex - Bewertung</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208146">MS11-006</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows Shell bezüglich Überlaufs bei Grafikverarbeitung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3970">CVE-2010-3970</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet und Angreifercode ist verfügbar</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in CSS</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3971">CVE-2010-3971</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet und wird in der Internetumgebung ausgenutzt</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch fehlerhafte Wechselwirkung von Treibern mit Windows-Kernel</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-4398">CVE-2010-4398</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207840">MS11-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in CSRSS durch Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0030">CVE-2011-0030</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0035">CVE-2011-0035</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208304">MS11-003</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung aufgrund von Nichtinitialisierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0036">CVE-2011-0036</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208395">MS11-014</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in LSASS bezüglich Längenüberprüfung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0039">CVE-2011-0039</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in nicht verschlüsselten Kerberos-Prüfsummen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0043">CVE-2011-0043</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</strong></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208365">MS11-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows-Kernel aufgrund von Ganzzahlabschneidung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0045">CVE-2011-0045</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k aufgrund fehlerhafter Überprüfung von Benutzereingaben</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0086">CVE-2011-0086</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k aufgrund unzureichender Überprüfung von Benutzereingaben</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0087">CVE-2011-0087</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich Verwechslung der Fensterklassenzeiger</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0088">CVE-2011-0088</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich fehlerhafter Zeigerüberprüfung in Fensterklasse</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0089">CVE-2011-0089</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208362">MS11-012</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0090">CVE-2011-0090</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch Visio-Objekte</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0092">CVE-2011-0092</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=204799">MS11-008</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung durch Visio-Datentypen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0093">CVE-2011-0093</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> - Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208522">MS11-004</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im FTP-Dienst für IIS bezüglich Pufferüberlaufs im Heap</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2010-3972">CVE-2010-3972</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> - Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet, und u. U. ist PoC-Code verfügbar</strong></td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208059">MS11-007</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch in OpenType-Schriftart codierte Zeichen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0033">CVE-2011-0033</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> - Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207839">MS11-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Skriptmodulen durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0031">CVE-2011-0031</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=207843">MS11-005</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Active Directory bezüglich SPN-Überprüfung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0040">CVE-2011-0040</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><strong>Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet</strong><br />
<br />
Diese Sicherheitsanfälligkeit kann zu einem Denial-of-Service führen</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=208523">MS11-013</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Kerberos bzgl. Spoofing</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-0091">CVE-2011-0091</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dies ist lediglich eine Sicherheitsanfälligkeit bezüglich Spoofing.</td>
</tr>
</tbody>
</table>
  
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
<th colspan="12" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=ae343de6-ec61-4891-b136-cfc4234d97d9)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=85bf88b7-2dd9-4204-8492-b2c1d8d2264e)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c72fbb97-2313-45f6-842d-99db373822dd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=bbea7ead-6c5c-4da8-aa03-a40325fd2de3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f86e9e64-801a-431a-b24e-772011dfa66d)  
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
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=cfa10178-9859-4e03-bedc-e3f5297a0251)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=a511d33a-9ae0-46ee-a225-9d97390de7d1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=56f4f43e-c313-49dc-a278-e3e8a83a907e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=486d1969-6814-4556-8dc0-5bfbaee528b0)  
(KB2478971)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=541f228f-79b3-402a-8ff9-366c1e595227)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=d431100d-a627-4ea0-b75b-2d4157e38df2)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a795de21-13f4-4035-a4d5-4257ddc92fe7)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=69dfa24b-7c56-4521-850c-1485b062154a)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bcb7217e-624a-4d61-86a1-f2440a1afd57)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=074396f0-a68c-4190-8dac-0b883d56e3f1)  
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
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9f0b7b77-5b90-4a4b-97a4-0c1ce6a70126)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7273a85-ce96-464b-8c4f-2710701213e3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e80db313-b470-4d71-bc34-70bfbfb6579f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a210c796-7077-4617-a9a8-9ea99fe11a5e)  
(KB2478971)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=82189bf2-3f34-4949-92da-eea98036d18e)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5e0f4bf2-f727-483a-af3a-9a2abf0c36bb)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=45e504d4-c17d-4b73-b08e-d9c0cb3f4918)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=74238e08-fae2-4f17-ac72-681226a53a40)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2aa94528-5063-427b-97f7-2a0a55cbb6bf)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a99c2b13-db81-4f18-9cf7-c20614ba0132)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=651c1f4f-4e69-4d17-8aa2-72681dfc5463)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=aed08b96-24cc-4e23-8fd5-c7e52f8ef41a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6bf2eeec-8225-477f-a606-263d3ee434d6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=54fe2669-8a63-4d96-8b82-5b10f45b293e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8a1e2675-0bf0-4d94-b48a-6e846dd6d9f5)  
(KB2478971)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4e31e6b1-577e-468e-9c94-67227d2273c2)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=0592b520-88d1-45bc-8b15-d3f0c8fa2181)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=29adcfb5-540f-4980-b2ca-9a22aa7bba13)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ebef4869-9812-46ce-9c01-2fb8c866ec90)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6e740922-6ce4-46ec-a35e-e94201a9e398)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=aeed45fb-9395-4c2b-a674-e38b04fe0914)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=ec962b0e-e951-4e70-8d97-8c2afd360c28)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ca7879e1-e295-445d-a658-0a31be1928cc)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ec544894-ee98-4a2b-ac4d-33b0c3754213)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4632e1ce-6ae8-431c-9104-9a8840e5ac63)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e79bbbd4-8d5a-4c4c-8427-21c14400f041)  
(KB2478971)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=76e3c229-d812-433c-ad05-7cbd1f9c6a6d)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=b2298b32-238a-4970-bc1f-2ede51a6c361)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=c41a0094-204b-4d05-ab39-a32915201af1)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a4f9ec46-35b2-44c9-abf6-647f7a474b99)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=bc09e42b-2eed-41b3-a03f-cb8cc94adfee)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=4ac66eae-e6d8-4e8b-b4ea-e7a77cc74db0)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=50855101-a15c-4c81-ad81-a7fe3f1d2026)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=fcd48499-1bb4-4304-b9cc-27d9d92e11cd)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a09c3e6e-c55c-492a-b7ad-3e3d35711643)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=856fbcc2-ead9-4ec1-92dd-988e6d22dae9)  
(KB2478971)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=a0cde8d8-7c85-4fcb-bcf7-205064970b41)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=b176777e-4897-4cf1-9fc0-dd608930bb4c)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=77971c3c-55ec-4a9c-bcb8-8fb8c61431e3)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0c18ecca-afb9-4738-bc7b-76a0e815dfb8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d60a2098-7351-4fce-83b2-2c1c3a24faa0)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=c09ccc72-8f94-416b-9a7f-ed16e90342a2)<sup>[1]</sup>
(Hoch)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=da9b7982-1c6b-45ac-8dd0-d7101bb83949)<sup>[1]</sup>
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
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=66978514-bb7f-42cc-9360-2fd1c686f4e6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6fb7ebcc-2052-457b-b5bc-1bbcb17696b9)  
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
Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=20ad0136-c6df-4c7b-811f-d6b3dd9e2c56)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d3580784-aada-4118-b7f2-3a23aec2ed04)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=62dc454f-4b1e-4ac0-8ffe-6c73112f8d4d)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=065ad8fe-1caf-488e-a2e1-96db29f2fa57)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=e88d072f-0f5f-4c85-ad2f-91b9b8bf6b3a)<sup>[1]</sup>
(Hoch)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=6e4b9878-b5d2-4025-8839-b41515932cf2)<sup>[1]</sup>
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
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8fdb8c37-1b22-457b-bdc0-21f6a5061dd3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=88d68757-1ab0-4585-9578-52a474b10882)  
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
<th colspan="12" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=ee61f0dd-9797-4e11-8281-a05b201d0c0b)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=ef1ae382-8835-4f60-83bd-e84a3400d55c)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=253c47a0-69ac-437a-ad3e-778c37fa37cb)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=88ba83b9-c14e-499a-8335-04bac1c49c0c)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=3cc55af7-5cd9-4923-8ec5-462ff201d734)<sup>[1]</sup>\*  
(Hoch)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=4dfa0a25-b7e3-4fb6-a351-58ec3f8a8435)<sup>[1]</sup>\*  
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
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4b37418a-e044-415e-b566-4507f157934a)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80494972-db45-475f-97cd-dac46b9486a1)\*  
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
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=558bc86a-a49d-4d6c-b5e4-f12956f6b61b)\*\*  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5607df02-93fa-45fe-a928-e5f6329851f3)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ec7101aa-96c2-4931-a3e4-0c55cbc74d9c)\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7c74d7f4-6372-4809-89b8-c79b05e54cdd)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft FTP-Dienst 7.0 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=f485b30d-dcaf-47c3-ac62-982b14670a1f)<sup>[1]</sup>\*  
(Hoch)  
[Microsoft-FTP-Dienst 7.5 für IIS 7.0](https://www.microsoft.com/download/details.aspx?familyid=a98a74c1-0c91-446d-b822-fe57ff06d90b)<sup>[1]</sup>\*  
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
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=163d3aca-3703-452e-b1cb-73932e2bcf8c)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5597d449-17e3-440f-8b0e-56a902a96569)\*  
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
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=8c2abba5-0597-4565-9b87-a37e574690e0)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e62493cb-8d25-4975-bbe6-a368e039872b)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=91d5d34b-9d7e-4e83-89a4-f1aa388dc4e4)  
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
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=55b07bc0-dff5-4cd7-87c9-c08e5a49197d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d10eda21-b3c3-4d8e-8596-bc45e4165f93)  
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
<th colspan="12" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
Keine
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
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=07aa7ffc-47c7-4611-b32c-ecb3fbcad32f)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=1da57fbc-9ea4-4fc4-911d-d5c7825e012c)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=9dabd1d1-3f1e-46d1-b171-aafd3f08d291)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[JScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=54a64215-e407-4b7b-8536-28817ef23bac)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=e1224c90-b0bc-4e4b-999a-efae327213b4)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=078fe6c0-1b2c-4896-a345-25cc1b1105e2)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit Systeme und Windows 7 für 32-Bit Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ffed7c76-0b75-4f57-9b63-3961a8b449f6)  
(KB2425227)  
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
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=2b8ffafe-78bb-4fa7-aea2-01208b6a3dfe)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=587adb89-2f6a-4893-9906-b6d6d9ada2bd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=66fb4efe-bcd3-4e90-8e35-b013e014a952)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[JScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Hoch)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=b854d76e-6891-426d-8c09-0ed8243a3b8d)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ddcf352e-742c-485e-9ed5-19cdba673562)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b42642b3-fb78-4700-bfe8-bfa997b90c16)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=c26cebcf-683f-4a51-be75-76535fb979a7)  
(KB2425227)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="12" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-003**](https://go.microsoft.com/fwlink/?linkid=208304)
</td>
<td style="border:1px solid black;">
[**MS11-006**](https://go.microsoft.com/fwlink/?linkid=208146)
</td>
<td style="border:1px solid black;">
[**MS11-007**](https://go.microsoft.com/fwlink/?linkid=208059)
</td>
<td style="border:1px solid black;">
[**MS11-004**](https://go.microsoft.com/fwlink/?linkid=208522)
</td>
<td style="border:1px solid black;">
[**MS11-005**](https://go.microsoft.com/fwlink/?linkid=207843)
</td>
<td style="border:1px solid black;">
[**MS11-009**](https://go.microsoft.com/fwlink/?linkid=207839)
</td>
<td style="border:1px solid black;">
[**MS11-010**](https://go.microsoft.com/fwlink/?linkid=207840)
</td>
<td style="border:1px solid black;">
[**MS11-011**](https://go.microsoft.com/fwlink/?linkid=208365)
</td>
<td style="border:1px solid black;">
[**MS11-012**](https://go.microsoft.com/fwlink/?linkid=208362)
</td>
<td style="border:1px solid black;">
[**MS11-013**](https://go.microsoft.com/fwlink/?linkid=208523)
</td>
<td style="border:1px solid black;">
[**MS11-014**](https://go.microsoft.com/fwlink/?linkid=208395)
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
Keine
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=38b67efb-dd4b-4e8c-8460-0f40f0367441)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=638318ed-4000-4b1a-bb4b-65b795f59784)\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=1e075f57-1723-4933-9b8e-7bce4a44a1c1)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[JScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Mittel)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=f482bd40-f0b9-4534-a768-45879f1e7285)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=70f5056a-72ad-46ff-a43f-ee151639b9a7)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d2c53f44-12eb-4293-9fa5-2a14075b636e)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=46bb3ef1-24c3-41cb-8141-0fdbd85093f7)\*  
(KB2425227)  
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
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=0e41cbe5-5e5e-4ece-a71a-71f4b6319f0d)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=4688ea0d-a467-4f24-ac52-104d05c8cae8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft-FTP-Dienst 7.5 für IIS 7.5](https://www.microsoft.com/download/details.aspx?familyid=bfddd539-c64f-4467-88ee-6bdfe645b478)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[JScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Mittel)  
[VBScript 5.8](https://www.microsoft.com/download/details.aspx?familyid=f05a3de0-381c-4d17-83ee-ca4f6da1bdb0)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=1646b3a5-714f-4ea5-b109-566fa9b933b6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8c6bf720-f544-4f58-9b1c-2399957ec43d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=01737933-e7de-451b-b02f-b7ca24693965)  
(KB2425227)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ee441255) und [Wartung einer Server Core-Installation](https://technet.microsoft.com/de-de/library/ff698994). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-004**

<sup>[1]</sup>Nicht der standardmäßige FTP-Dienst für dieses Betriebssystem

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
[**MS11-008**](https://go.microsoft.com/fwlink/?linkid=204799)
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
Microsoft Visio 2002 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2002 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=273d8078-0dc7-43d8-bcae-54c811e49e0e)  
(KB2434711)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Visio 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Visio 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f1067eaa-d18d-4bff-a02e-1d990c36ca7f)  
(KB2434733)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Visio 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Visio 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=097a642b-b786-4724-a907-79f37cded836)  
(KB2434737)  
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

-   Yuki Chen von [Trend Micro](https://www.trendmicro.com) für den Hinweis auf ein in MS11-003 beschriebenes Problem.
-   SkyLined von [Google Inc.](https://www.google.com/) für den Hinweis auf ein in MS11-003 beschriebenes Problem.
-   Haifei Li von [Fortinets FortiGuard Labs](https://www.fortiguard.com/) für den Hinweis auf ein in MS11-003 beschriebenes Problem
-   Kobi Pariente und Yaniv Miron in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS11-006 beschriebenes Problem.
-   Procyun Zusammenarbeit mit [TippingPoints](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS11-008 beschriebenes Problem.
-   Xin Ouyang von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf zwei in MS11-008 beschriebene Probleme.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS11-009 beschriebenes Problem.
-   Sihan Qing (Professor), Weiping Wen (Außerordentlicher Professor), Liang Yin und Husheng Zhou (Studenten im Aufbaustudium) vom [Department of Information Security, Beijing University](https://www.ss.pku.edu.cn/en/) für den Hinweis auf ein in MS11-010 beschriebenes Problem.
-   Zhengwenbin von [360safe](https://www.360.cn) für den Hinweis auf ein in MS11-011 beschriebenes Problem.
-   Guo Bojun für den Hinweis auf ein in MS11-011 beschriebenes Problem.
-   Wei Zhang für den Hinweis auf ein in MS11-011 beschriebenes Problem.
-   Marco Giuliani von [Prevx](https://www.prevx.com/) für die Zusammenarbeit mit uns an einem in MS11-011 beschriebenen Problem.
-   std\_logic in Zusammenarbeit mit [TippingPoints](https://www.tippingpoint.com/)[Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS11-011 beschriebenes Problem.
-   Tarjei Mandt von [Norman](https://www.norman.com) für den Hinweis auf fünf in MS11-012 beschriebene Probleme.
-   [Das MIT Kerberos Team](https://web.mit.edu/kerberos) für den Hinweis auf ein in MS11-013 beschriebenes Problem.
-   Scott Stender von [iSEC Partners](https://www.isecpartners.com/) für den Hinweis auf ein in MS11-013 beschriebenes Problem.
-   Sicherheitstester Jorge Moura von Primavera BSS für den Hinweis auf ein in MS11-014 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (8. Februar 2011): Bulletin Summary veröffentlicht.
-   V1.1 (9. Februar 2011): In MS11-013 wurde die Ausnutzbarkeitsindexbewertung für CVE-2011-0091 auf „3 - Funktionierender Angreifercode unwahrscheinlich“ korrigiert. Dies ist lediglich eine Informationsänderung.
-   V2.0 (8. März 2011): Die Tabelle „Betroffene Software“ wurde erweitert, um Windows 7 für 32-Bit-Systeme Service Pack 1, Windows 7 für x64-basierte Systeme Service Pack 1, Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1 für MS11-003, MS11-004, MS11-007 und MS11-009 zu umfassen. Weitere Informationen finden Sie in den häufig gestellten Fragen (FAQs) zum Update dieses Bulletins.
-   V3.0 (16. März 2011): Die Tabelle „Betroffene Software“ wurde erweitert, um Windows 7 für 32-Bit-Systeme Service Pack 1, Windows 7 für x64-basierte Systeme Service Pack 1, Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1 für MS11-013 zu umfassen. Weitere Informationen finden Sie in den häufig gestellten Fragen (FAQs) zum Update dieses Bulletins.
-   V4.0 (18. März 2011): Die Tabelle „Betroffene Software“ wurde erweitert, um Windows 7 für 32-Bit-Systeme Service Pack 1, Windows 7 für x64-basierte Systeme Service Pack 1, Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1 für MS11-012 zu umfassen. Weitere Informationen finden Sie in den häufig gestellten Fragen (FAQs) zum Update dieses Bulletins.

*Built at 2014-04-18T01:50:00Z-07:00*