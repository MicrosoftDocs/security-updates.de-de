---
TOCTitle: 'MS13-FEB'
Title: Microsoft Security Bulletin Summary für Februar 2013
ms:assetid: 'ms13-feb'
ms:contentKeyID: 61225118
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms13-feb(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Februar 2013
====================================================

Veröffentlicht: Dienstag, 12. Februar 2013 | Aktualisiert: Mittwoch, 13. Februar 2013

**Version:** 1.2

In diesem Bulletin Summary sind die im Februar 2013 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Februar 2013 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 7. Februar 2013 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, den 13. Februar 2013 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Februar](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538626&culture=en-us). Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538626&culture=en-us) zur Verfügung.

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

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
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2792100)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt dreizehn vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=275837">MS13-010</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Vector Markup Language kann Remotecodeausführung ermöglichen (2797052)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Microsoft-Implementierung der Vector Markup Language (VML). Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=271307">MS13-011</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Mediendekomprimierung kann Remotecodeausführung ermöglichen (2780091)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Mediendatei (z. B. eine MPG-Datei) oder ein Microsoft Office-Dokument (z. B. eine PPT-Datei) mit einer speziell gestalteten eingebetteten Mediendatei öffnet oder speziell gestaltete Streaming-Inhalte empfängt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=279801">MS13-012</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen (2809279)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete Sicherheitsanfälligkeiten in Microsoft Exchange Server. Die schwerste Sicherheitsanfälligkeit liegt in Microsoft Exchange Server WebReady Document Viewing vor und kann Remotecodeausführung im Sicherheitskontext des Transcodierungsdienstes auf dem Exchange Server ermöglichen, wenn ein Benutzer von Outlook Web App (OWA) eine Vorschau einer speziell gestalteten Datei anzeigt. Der Transcodierungsdienst in Exchange, der für WebReady Dokument Viewing verwendet wird, wird im LocalService-Konto ausgeführt. Das LocalService-Konto hat Mindestberechtigungen auf dem lokalen Computer und präsentiert im Netzwerk anonyme Anmeldeinformationen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=279005">MS13-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in OLE-Automatisierung kann Remotecodeausführung ermöglichen (2802968)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Microsoft Windows OLE-Automatisierung (Object Linking and Embedding). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Datei öffnet. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=272434">MS13-013</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in der Analyse von FAST Search</strong> <strong>Server 2010 für SharePoint können Remotecodeausführung ermöglichen (2784242)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt öffentlich gemeldete Sicherheitsanfälligkeiten in der Microsoft FAST Search Server 2010 für SharePoint. Die Sicherheitsanfälligkeiten können Remotecodeausführung im Sicherheitskontext eines Benutzerkontos mit eingeschränktem Token ermöglichen. FAST Search Server für SharePoint ist nur von diesem Problem betroffen, wenn das erweiterte Filterpaket aktiviert ist. Standardmäßig ist das erweiterte Filterpaket deaktiviert.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=276948">MS13-014</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in NFS-Server</strong> <strong>kann Denial-of-Service ermöglichen (2790978)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer versucht, auf einer schreibgeschützten Freigabe einen Dateivorgang durchzuführen. Ein Angreifer, der diese Sicherheitsanfälligkeit ausnutzt, kann bewirken, dass das betroffene System nicht mehr reagiert und dann neu startet. Die Sicherheitsanfälligkeit betrifft nur Windows-Server, auf denen die NFS-Rolle aktiviert ist.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=275736">MS13-015</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in .NET Framework kann Erhöhung von Berechtigungen ermöglichen (2800277)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit<strong></strong>in .NET Framework. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in einem Webbrowser anzeigt, der XAML-Browseranwendungen (XBAP) ausführen kann. Die Sicherheitsanfälligkeit kann auch von Windows .NET-Anwendungen verwendet werden, um Einschränkungen durch die Codezugriffssicherheit (CAS) zu umgehen. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Microsoft .NET Framework</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Windows-Kernelmodustreiber können</strong> <strong>Erhöhung von Berechtigungen ermöglichen (2778344)</strong><br />
Dieses Sicherheitsupdate behebt dreißig vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-017">MS13-017</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (2799494)</strong><br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in allen unterstützten Veröffentlichungen von Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-018">MS13-018</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in TCP/IP kann zu Denial-of-Service führen (2790655)<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein nicht authentifizierter Angreifer ein speziell gestaltetes Paket zum Beenden einer Verbindung an den Server sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=278896">MS13-019</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Client/Server-Runtime-Subsystem (CSRSS) kann Erhöhung von Berechtigungen ermöglichen (2790113)<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/de-de/security/cc998259).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.

<p> </p>
<table style="border:1px solid black;">
<thead>
<tr class="header">
<th style="border:1px solid black;" >Kennung des Bulletins</th>
<th style="border:1px solid black;" >Titel der Sicherheitsanfälligkeit</th>
<th style="border:1px solid black;" >CVE-ID</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit für ältere Softwareversionen</th>
<th style="border:1px solid black;" >Bewertung der Ausnutzbarkeit durch Denial-of-Service</th>
<th style="border:1px solid black;" >Wichtige Hinweise</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Shift JIS bezüglich Zeichencodierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0015">CVE-2013-0015</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer SetCapture</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0018">CVE-2013-0018</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer COmWindowProxy</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0019">CVE-2013-0019</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CMarkup</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0020">CVE-2013-0020</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer vtable</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0021">CVE-2013-0021</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer LsGetTrailInfo</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0022">CVE-2013-0022</a></td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CDispNode</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0023">CVE-2013-0023</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer pasteHTML</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0024">CVE-2013-0024</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer SLayoutRun</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0025">CVE-2013-0025</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer InsertElement</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0026">CVE-2013-0026</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CPasteCommand</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0027">CVE-2013-0027</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CObjectElement</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0028">CVE-2013-0028</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-009">MS13-009</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer CHTML</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0029">CVE-2013-0029</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=275837">MS13-010</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in VML bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0030">CVE-2013-0030</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Microsoft ist sich dessen bewusst, dass diese Sicherheitsanfälligkeit in beschränkten, gezielten Angriffen die Offenlegung von Informationen ermöglicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=271307">MS13-011</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Mediendekomprimierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0077">CVE-2013-0077</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=279801">MS13-012</a></td>
<td style="border:1px solid black;">Oracle Outside In enthält mehrere ausnutzbare Sicherheitsanfälligkeiten</td>
<td style="border:1px solid black;">Mehrere*</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">*Mehrere Sicherheitsanfälligkeiten; weitere Informationen finden Sie im Bulletin MS13-012.<br />
<br />
Diese Sicherheitsanfälligkeiten wurden veröffentlicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=272434">MS13-013</a></td>
<td style="border:1px solid black;">Oracle Outside In enthält mehrere ausnutzbare Sicherheitsanfälligkeiten</td>
<td style="border:1px solid black;">Mehrere*</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">*Mehrere Sicherheitsanfälligkeiten; weitere Informationen finden Sie im Bulletin MS13-013.<br />
<br />
Diese Sicherheitsanfälligkeiten wurden veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=276948">MS13-014</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch NULL-Dereferenzierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1281">CVE-2013-1281</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=275736">MS13-015</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich der Erhöhung von Berechtigungen bei WinForms-Rückruf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0073">CVE-2013-0073</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1248">CVE-2013-1248</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Dies ist eine Tiefenverteidigungsmaßnahme für die aktuelle Software.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1249">CVE-2013-1249</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Dies ist eine Tiefenverteidigungsmaßnahme für die aktuelle Software.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1250">CVE-2013-1250</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1251">CVE-2013-1251</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1252">CVE-2013-1252</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1253">CVE-2013-1253</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1254">CVE-2013-1254</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1255">CVE-2013-1255</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1256">CVE-2013-1256</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1257">CVE-2013-1257</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1258">CVE-2013-1258</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1259">CVE-2013-1259</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1260">CVE-2013-1260</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1261">CVE-2013-1261</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1262">CVE-2013-1262</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1263">CVE-2013-1263</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1264">CVE-2013-1264</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1265">CVE-2013-1265</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1266">CVE-2013-1266</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1267">CVE-2013-1267</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1268">CVE-2013-1268</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1269">CVE-2013-1269</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1270">CVE-2013-1270</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1271">CVE-2013-1271</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1272">CVE-2013-1272</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1273">CVE-2013-1273</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1274">CVE-2013-1274</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1275">CVE-2013-1275</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1276">CVE-2013-1276</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-016">MS13-016</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1277">CVE-2013-1277</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-017">MS13-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung im Kernel</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1278">CVE-2013-1278</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-017">MS13-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung im Kernel</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1279">CVE-2013-1279</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-017">MS13-017</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Referenzzähler des Windows-Kernel</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1280">CVE-2013-1280</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-018">MS13-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in TCP-FIN-Wartezeit</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0075">CVE-2013-0075</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=278896">MS13-019</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Referenzzähler</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0076">CVE-2013-0076</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=279005">MS13-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung durch OLE-Automatisierung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1313">CVE-2013-1313</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
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

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="11" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=9bf087e7-4487-48bf-84e9-04b816411a0f)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=4501ef62-7d06-49b7-af86-c84e399e6275)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=2ab64eac-8ecf-4178-9a01-5f10fc2f049e)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=daed0c2e-bd9a-4685-a5f9-1c01f7fdeccf)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=fd693211-bcc8-4267-9aa1-86bac45e25bf)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e8924d23-f6e2-41bf-9542-f8991d084db9)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=95f5acea-32a0-42a5-a14d-837edf313984)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=3a8ddbab-5999-48b7-9de8-423954f345b6)  
(KB2802968)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb202940-0ece-4631-83d5-8cf52c7dbf36)  
(KB2789643)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=cdaa7282-c354-4d70-938a-a025631205a2)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=9100bf70-8723-4635-9b78-f7c3048a950f)  
(KB2799494)  
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
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=c42347dd-5ec8-4760-a685-2cd7b6bb7bb2)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=6513176c-e9cb-4863-a228-5bc369135996)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=25e15457-ffd2-4466-aff9-1d0830e967d7)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=dd9383b9-a6df-44a7-bea9-8f7d088bc488)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=b042e717-bf4e-44a1-a1ba-6359bf551e8e)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c8618c96-25c0-415b-b147-5713ec5ab5b1)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=06ef35a1-f76f-4e99-a8b2-6b086c7e51be)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb202940-0ece-4631-83d5-8cf52c7dbf36)  
(KB2789643)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f72228df-8379-4bd9-b446-cb9505e9d228)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9a945336-b037-4ee6-9ea2-dfb885747b97)  
(KB2799494)  
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
<th colspan="11" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=35b58c7a-aae3-4445-957a-42ee708d77a5)  
(KB2792100)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=3ee73b80-b8f6-4843-afba-41c7b55faf17)  
(KB2792100)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d67754e2-7ebd-484d-a008-ed8719e0c72d)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=9b96ebfc-93e9-41bb-81f9-35c433ca5479)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=b902617d-1f35-4b17-9a44-235c0d3c27d2)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=47ca5d22-b957-4ac9-91e9-c440b0614728)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=e3b0b928-0f76-4b51-871a-aeda2ee3b7d5)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb202940-0ece-4631-83d5-8cf52c7dbf36)  
(KB2789643)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8daebdb5-eba2-4685-b781-ead5c2185548)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c005c0a0-4025-4a07-a76d-c57ed5afbd68)  
(KB2799494)  
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
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=075de724-b996-413f-8ff3-74f435d94b9b)  
(KB2792100)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a90d6861-7ff6-4501-9200-f72b5a9f1817)  
(KB2792100)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=319a7a93-c03e-4c0b-a5c4-6a4f379d781e)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=b3ca28b1-9d3c-4df5-b8d7-f31d70f6e714)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=e13c9366-9cb6-4e62-bf6c-a09fe7842463)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=80aab9c7-4511-4d44-b570-c77cdb50e542)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=493377a4-4ce2-4dd9-ba84-090466248669)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb202940-0ece-4631-83d5-8cf52c7dbf36)  
(KB2789643)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e7d03ef2-517b-4442-a968-5aaa300dd2ba)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dc004424-61f9-49ed-9cb3-b89ed9e98aef)  
(KB2799494)  
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
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=92ce1fa1-4b12-4fd5-9a02-21fc9b119fb9)  
(KB2792100)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=5965ce09-c5d7-4072-bad3-df46f9b76478)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=63791740-00e2-4569-967e-36086efe6ca6)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=d1a9b2b2-191c-4ffe-9c8a-8ef641a45eb7)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=8e9a09fd-f360-4471-ac89-481dc2935cec)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb202940-0ece-4631-83d5-8cf52c7dbf36)  
(KB2789643)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=2a3039a4-9b46-4db8-a539-07d52bbf1b92)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3cad66f1-6651-4948-9579-9df050fdaa1b)  
(KB2799494)  
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
<th colspan="11" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=eea43429-2691-4a31-a640-d74035145d2d)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5c195229-8e63-4fff-a304-13c13b2fa132)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7f7ce868-28ce-497e-882f-3abfdd9b89e8)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=4f946407-cd81-48b5-a279-1ab81388b70b)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e0cfc24f-293c-4817-a69c-f9cfd514e1c1)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=4fab0417-5c9a-4e5d-864d-b1b3bee6fc89)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=d730eacf-e30a-45aa-89da-dfec5e87906a)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b59753f0-b7cb-41c2-9c31-4f2de8356477)  
(KB2789646)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0ff0475c-cc1b-4886-971e-1a71e6b311c3)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4de1249f-012e-47cb-ad08-4fd5bddb0879)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=80b766e7-3b7f-4d04-9a80-71864a13df8c)  
(KB2790655)  
(Mittel)
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
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=308d99ff-7575-4d70-958f-0d57fd6bffab)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d9d4987e-95ad-4246-a52b-7ac859a40e67)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=74b370c0-29f5-4acb-a3cd-bd2c2b708bb7)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=6ffb3215-1c90-4eb2-9143-0866efc98374)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=649dbf4e-654b-48a2-bd35-2df7f34fbb56)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=44fbe00c-eeb4-4a80-a934-7ce58c02d6ec)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=4cd6b10c-b310-4aee-bbca-f23049c14455)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b59753f0-b7cb-41c2-9c31-4f2de8356477)  
(KB2789646)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e5043a08-a9e4-422b-8455-80a5091d38b9)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=448ac43a-0a6f-4049-be2b-c853b5dbfab3)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=92bad797-5b66-422c-a096-8070d02bb8b2)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=71c805ed-a68b-4d3e-97ca-922557cfbf67)  
(KB2792100)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=775ea105-4a71-4b7b-9dc0-50f1eecab96d)  
(KB2792100)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=ccdf8abc-9657-4aff-8d73-4824a558c168)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=d432acb3-10a0-4f4c-a793-381aedd4bdd1)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=b91ce04a-a464-4388-9386-54dd2815b8dd)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=58f0810c-f253-4740-ac9f-75b8a4506b06)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=86cc3b51-818a-49a6-abab-488ac316e021)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b59753f0-b7cb-41c2-9c31-4f2de8356477)  
(KB2789646)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=850e319f-dd6e-4480-86c3-a5129f084817)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d7a74c8-de4b-4bcb-8b3f-581858d0776b)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c24aa6f3-82a5-4b1f-adc8-4aece948161c)  
(KB2790655)  
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
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=de1b96b7-a5ac-4a39-9808-c00c6b1a4325)  
(KB2792100)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e5775802-e529-4894-b1cf-2839948706c2)  
(KB2792100)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=51df1e78-f014-4492-8a3d-83b3c821458b)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=152f90b3-efae-42e6-a845-59052383a8a0)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=304ac41e-b4e5-4bf8-94d2-f2bd9a07bcff)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7b85336a-d3f7-4077-b6eb-55b3042f5335)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=fe239f9b-d986-4828-a01d-8abd494037ec)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b59753f0-b7cb-41c2-9c31-4f2de8356477)  
(KB2789646)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8978769b-447b-4b01-848a-cbcdf692f17a)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c9fbb7cc-c33b-4af9-8416-9d16015e79c1)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2738fbe4-2163-4e77-82e6-208a7a08a70c)  
(KB2790655)  
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
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=61c1964f-9307-4128-9470-bcb20e07856b)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=1a2af9dc-e9a7-477e-9943-8132eb7fea81)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Quartz.dll (DirectShow)](https://www.microsoft.com/download/details.aspx?familyid=4b3e48e3-0dbe-449b-9bca-0ba8bbdcbab0)  
(KB2780091)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b59753f0-b7cb-41c2-9c31-4f2de8356477)  
(KB2789646)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0f84e24c-43f4-4851-932c-8849171b2505)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f3e18038-b8a1-4eba-9542-8396903a3709)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c269c175-f47c-456a-9360-f38bbdfd7ed0)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)****
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)****
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)****
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4df9414b-02da-4254-ab29-5091151e2900)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b21bd7b3-2eb8-433a-b6c2-8243c5128038)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d7d64177-deec-4fd3-9716-b7816fe3c623)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=04a101c6-d553-426f-b3cd-412eefeec580)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=3b25dd48-053d-4d9e-9774-905c66c3aca9)  
(KB2789644)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=631adede-ba0f-461f-85e1-82b60a7efec1)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=912ac2e1-e737-43fb-acc8-a01a918a8475)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=cb4270c4-cec5-49e0-a56b-97539d6352a0)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=d4d02ef9-b0a4-46a3-ad92-7508aa26ad3b)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4df9414b-02da-4254-ab29-5091151e2900)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b21bd7b3-2eb8-433a-b6c2-8243c5128038)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d7d64177-deec-4fd3-9716-b7816fe3c623)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=04a101c6-d553-426f-b3cd-412eefeec580)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=0da657e5-161d-46bc-a2b7-7c4696e37062)  
(KB2789645)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=631adede-ba0f-461f-85e1-82b60a7efec1)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=912ac2e1-e737-43fb-acc8-a01a918a8475)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=cb4270c4-cec5-49e0-a56b-97539d6352a0)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d4d02ef9-b0a4-46a3-ad92-7508aa26ad3b)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=6ef9cbf9-d131-420d-b566-6b0f94f2e1c1)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=4b2402ff-035a-47c4-b982-00d428eab379)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d503795a-b1a3-48dc-b1e6-27628aeb150a)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=36eb59be-6703-40c0-b01c-0fffb1456719)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=3b25dd48-053d-4d9e-9774-905c66c3aca9)  
(KB2789644)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=8dab3aca-fde1-4bd9-b82a-e4805a2e8d39)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=0d1601cc-fb76-4276-bf0b-a46b7f8055ae)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=5d93cb19-7854-4b49-9743-8d6a11be2dd6)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=77277398-c5b4-4ba4-8425-465710b0bef2)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=6ef9cbf9-d131-420d-b566-6b0f94f2e1c1)  
(KB2792100)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=4b2402ff-035a-47c4-b982-00d428eab379)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d503795a-b1a3-48dc-b1e6-27628aeb150a)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=36eb59be-6703-40c0-b01c-0fffb1456719)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=0da657e5-161d-46bc-a2b7-7c4696e37062)  
(KB2789645)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8dab3aca-fde1-4bd9-b82a-e4805a2e8d39)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0d1601cc-fb76-4276-bf0b-a46b7f8055ae)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5d93cb19-7854-4b49-9743-8d6a11be2dd6)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=77277398-c5b4-4ba4-8425-465710b0bef2)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e7b455a3-6a44-430c-a7d1-30c03ef7f141)  
(KB2792100)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7e9d97f2-c006-4e5a-bc80-10450069b8c5)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7a36109b-f1e2-4cde-9ede-9f7449c5412c)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=be2fd20a-4c37-47a6-a322-e16acd99db2c)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=aadb2003-ed7b-46ee-afd0-33cec4ac39b4)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=3b25dd48-053d-4d9e-9774-905c66c3aca9)  
(KB2789644)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ca5a8735-1568-454d-8b4c-b83107eac036)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=201e6d1f-425b-406e-84a1-37cee035dddb)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=01284b28-043a-4e27-b363-c1e641164a01)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=97241fdb-991d-4411-8fe1-ea56172360ab)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=e7b455a3-6a44-430c-a7d1-30c03ef7f141)  
(KB2792100)  
(Mittel)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=7e9d97f2-c006-4e5a-bc80-10450069b8c5)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=7a36109b-f1e2-4cde-9ede-9f7449c5412c)  
(KB2797052)  
(Kritisch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=be2fd20a-4c37-47a6-a322-e16acd99db2c)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=aadb2003-ed7b-46ee-afd0-33cec4ac39b4)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=0da657e5-161d-46bc-a2b7-7c4696e37062)  
(KB2789645)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ca5a8735-1568-454d-8b4c-b83107eac036)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=201e6d1f-425b-406e-84a1-37cee035dddb)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=01284b28-043a-4e27-b363-c1e641164a01)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=97241fdb-991d-4411-8fe1-ea56172360ab)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c1eb941e-833d-46f0-bf65-d9701d67bc20)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c2e1c1b3-5b75-47cf-91d5-82d413b358e6)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=8e37196c-2f43-457d-8d87-336d8775c0bf)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=3b25dd48-053d-4d9e-9774-905c66c3aca9)  
(KB2789644)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=99320f36-1481-446c-bc3e-d33fcfd1f2c1)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9f0b132a-8616-49cd-8927-393f35d0cf21)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=e1be5dea-dd13-42b5-a37f-4bcd828cc65f)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=9fbc37dd-53ec-4de1-b1c1-9761a8f83ab8)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c1eb941e-833d-46f0-bf65-d9701d67bc20)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=c2e1c1b3-5b75-47cf-91d5-82d413b358e6)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=8e37196c-2f43-457d-8d87-336d8775c0bf)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=0da657e5-161d-46bc-a2b7-7c4696e37062)  
(KB2789645)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(KB2789642)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=99320f36-1481-446c-bc3e-d33fcfd1f2c1)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9f0b132a-8616-49cd-8927-393f35d0cf21)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=e1be5dea-dd13-42b5-a37f-4bcd828cc65f)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9fbc37dd-53ec-4de1-b1c1-9761a8f83ab8)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=7966de38-c6a6-4137-8b7e-8ccd3306521a)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=0389b515-59bf-4733-aab4-ffb822efdbea)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=639674a0-12a3-4185-9858-b2a31ed2f014)  
(KB2789650)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=27d83684-d4f7-4fe0-a54d-25a3d2009be0)  
(KB2789649)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=d5395864-1822-4151-a10c-f6a036f8853f)  
(KB2778344)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=5b74e5b3-7b8d-4669-b403-c776e70bf072)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=e7739ba6-9c62-4180-a095-47fdb6c741e9)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=d6720d21-269b-4605-b95e-573bc327afd9)  
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=c1859853-d43f-4497-b212-e6a4daa43485)  
(KB2797052)  
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
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=639674a0-12a3-4185-9858-b2a31ed2f014)  
(KB2789650)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=27d83684-d4f7-4fe0-a54d-25a3d2009be0)  
(KB2789649)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=79aaaa3a-747a-4320-9fd2-5f4a6de3d13c)  
(KB2778344)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=a41a2b38-5e5c-48bc-8727-e19402519f12)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](https://www.microsoft.com/download/details.aspx?familyid=dd2042b8-c784-4dfc-8fca-61905693cda5)  
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows Server 2012
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=8e3fdcd0-ab75-4500-aac7-7ecb4f39fca7)  
(KB2792100)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](https://www.microsoft.com/download/details.aspx?familyid=3b39813e-5ee2-412e-b1f1-a16617a70f43)  
(KB2797052)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=b284296a-1db5-47dc-af2c-bf55d0ad09e6)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=639674a0-12a3-4185-9858-b2a31ed2f014)  
(KB2789650)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=27d83684-d4f7-4fe0-a54d-25a3d2009be0)  
(KB2789649)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=aac38d33-fad6-4060-bad4-61cf7c059af9)  
(KB2778344)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=4e427f56-436e-43d0-b4f8-eee8427b3741)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=f74a104d-4749-4dd5-b144-2e4ce9c284a2)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Windows RT
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10<sup>[1]</sup>
(KB2792100)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Internet Explorer 10<sup>[1]</sup>
(KB2797052)  
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
Windows RT<sup>[1]</sup>
(KB2778344)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
Windows RT<sup>[1]</sup>
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows RT<sup>[1]</sup>
(KB2790655)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="11" style="border:1px solid black;">
Server Core-Installationsoption
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-009**](https://technet.microsoft.com/de-de/security/bulletin/ms13-009)
</td>
<td style="border:1px solid black;">
[**MS13-010**](https://go.microsoft.com/fwlink/?linkid=275837)
</td>
<td style="border:1px solid black;">
[**MS13-011**](https://go.microsoft.com/fwlink/?linkid=271307)
</td>
<td style="border:1px solid black;">
[**MS13-020**](https://go.microsoft.com/fwlink/?linkid=279005)
</td>
<td style="border:1px solid black;">
[**MS13-014**](https://go.microsoft.com/fwlink/?linkid=276948)
</td>
<td style="border:1px solid black;">
[**MS13-015**](https://go.microsoft.com/fwlink/?linkid=275736)
</td>
<td style="border:1px solid black;">
[**MS13-016**](https://technet.microsoft.com/de-de/security/bulletin/ms13-016)
</td>
<td style="border:1px solid black;">
[**MS13-017**](https://technet.microsoft.com/de-de/security/bulletin/ms13-017)
</td>
<td style="border:1px solid black;">
[**MS13-018**](https://technet.microsoft.com/de-de/security/bulletin/ms13-018)
</td>
<td style="border:1px solid black;">
[**MS13-019**](https://go.microsoft.com/fwlink/?linkid=278896)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=850e319f-dd6e-4480-86c3-a5129f084817) (Server Core-Installation)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6d7a74c8-de4b-4bcb-8b3f-581858d0776b) (Server Core-Installation)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c24aa6f3-82a5-4b1f-adc8-4aece948161c) (Server Core-Installation)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=8978769b-447b-4b01-848a-cbcdf692f17a) (Server Core-Installation)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c9fbb7cc-c33b-4af9-8416-9d16015e79c1) (Server Core-Installation)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2738fbe4-2163-4e77-82e6-208a7a08a70c) (Server Core-Installation)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme (Server Core-Installation)
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
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=aadb2003-ed7b-46ee-afd0-33cec4ac39b4) (Server Core-Installation)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=3b25dd48-053d-4d9e-9774-905c66c3aca9) (Server Core-Installation)  
(KB2789644)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=ca5a8735-1568-454d-8b4c-b83107eac036) (Server Core-Installation)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=201e6d1f-425b-406e-84a1-37cee035dddb) (Server Core-Installation)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=01284b28-043a-4e27-b363-c1e641164a01) (Server Core-Installation)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=97241fdb-991d-4411-8fe1-ea56172360ab) (Server Core-Installation)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)
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
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=aadb2003-ed7b-46ee-afd0-33cec4ac39b4) (Server Core-Installation)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=0da657e5-161d-46bc-a2b7-7c4696e37062) (Server Core-Installation)  
(KB2789645)  
(Hoch)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=182f4d35-f18b-4485-be22-43becbd3cc05)<sup>[1]</sup>
(Server Core-Installation) (KB2789642)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=b5cfc358-e5ff-445c-8d43-3f79fead6139) (Server Core-Installation)  
(KB2789648)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=ca5a8735-1568-454d-8b4c-b83107eac036) (Server Core-Installation)  
(KB2778344)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=201e6d1f-425b-406e-84a1-37cee035dddb) (Server Core-Installation)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=01284b28-043a-4e27-b363-c1e641164a01) (Server Core-Installation)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=97241fdb-991d-4411-8fe1-ea56172360ab) (Server Core-Installation)  
(KB2790113)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)
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
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=b284296a-1db5-47dc-af2c-bf55d0ad09e6) (Server Core-Installation)  
(KB2790978)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 3.5](https://www.microsoft.com/download/details.aspx?familyid=639674a0-12a3-4185-9858-b2a31ed2f014) (Server Core-Installation)  
(KB2789650)  
(Hoch)  
[Microsoft .NET Framework 4.5](https://www.microsoft.com/download/details.aspx?familyid=27d83684-d4f7-4fe0-a54d-25a3d2009be0) (Server Core-Installation)  
(KB2789649)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=aac38d33-fad6-4060-bad4-61cf7c059af9) (Server Core-Installation)  
(KB2778344)  
(Keine Bewertung des Schweregrads<sup>[2]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=4e427f56-436e-43d0-b4f8-eee8427b3741) (Server Core-Installation)  
(KB2799494)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2012](https://www.microsoft.com/download/details.aspx?familyid=f74a104d-4749-4dd5-b144-2e4ce9c284a2) (Server Core-Installation)  
(KB2790655)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise** **für MS13-009, MS13-010,** **MS13-017 und MS13-018**

<sup>[1]</sup>Sicherheitsupdates für Windows RT werden über [Windows Update](https://update.microsoft.com/windowsupdate/) bereitgestellt.

**Hinweise für MS13-015**

<sup>[1]</sup>**.NET Framework 4 und .NET Framework 4 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4 und .NET Framework 4 Client Profile. .NET Framework 4 Client Profile ist Teil von .NET Framework 4. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4 als auch .NET Framework 4 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](https://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

**Hinweise für MS13-016**

<sup>[1]</sup>Sicherheitsupdates für Windows RT werden über [Windows Update](https://update.microsoft.com/windowsupdate/) bereitgestellt.

<sup>[2]</sup>Bewertungen des Schweregrads treffen für dieses Update für die angegebene Software nicht zu. Microsoft empfiehlt jedoch den Benutzern dieser Software, dieses Sicherheitsupdate als tiefgreifende Verteidigungsmaßnahme zu installieren.

#### Microsoft Server Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft SharePoint Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-012**](https://go.microsoft.com/fwlink/?linkid=279801)
</td>
<td style="border:1px solid black;">
[**MS13-013**](https://go.microsoft.com/fwlink/?linkid=272434)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2007 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=316a1aff-b72d-4d96-8ee5-bd86b0e29e6f)  
(KB2788321)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Exchange Server 2010 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=498e7612-73b5-4e28-99a4-b3157ac69932)  
(KB2746164)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft FAST Search Server 2010 für SharePoint
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-012**](https://go.microsoft.com/fwlink/?linkid=279801)
</td>
<td style="border:1px solid black;">
[**MS13-013**](https://go.microsoft.com/fwlink/?linkid=272434)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft FAST Search Server 2010 für SharePoint Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Erweitertes Filterpaket](https://www.microsoft.com/download/details.aspx?familyid=0ae86754-69a8-4c82-855c-2ee2b7887fa5)<sup>[1]</sup>
(KB2553234)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-013**

<sup>[1]</sup>Dieses Update ist nur im Microsoft Download Center verfügbar.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/bb245732). Im [TechNet Sicherheitscenter](https://technet.microsoft.com/de-de/security/default.aspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Endbenutzer können das [Microsoft-Sicherheitscenter](https://www.microsoft.com/de-de/security/default.aspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](https://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. und können am einfachsten durch eine Suche nach dem Begriff „Sicherheitsupdate“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](https://www.microsoft.com/germany/mac).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS13-001“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](https://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://technet.microsoft.com/de-de/security/cc184924.aspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx).

**SystemCenter Configuration Manager**

System Center Configuration Manager-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit System Center Configuration Manager können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in System Center Configuration Manager erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in System Center Configuration Manager ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen zu System Center Configuration Manager finden Sie auf der Website [System Center Technical Resources](https://technet.microsoft.com/de-de/systemcenter/bb980621).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de). Die nächste Version von SMS, System Center Configuration Manager, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](https://www.microsoft.com/download/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](https://technet.microsoft.com/de-de/systemcenter/bb545936).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/de-de/download/details.aspx?id=1846) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc749197), die im [Anwendungskompatibilitäts-Toolkit](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](https://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Masato Kinugawa für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   [Omair](https://krash.in/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf zwei in MS13-009 beschriebene Probleme.
-   SkyLined in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Arthur Gerkis in Zusammenarbeit mit Exodus Intelligence für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Stephen Fewer von [Harmony Security](https://www.harmonysecurity.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf zwei in MS13-009 beschriebene Probleme.
-   [Aniway.Aniway@gmail.com](mailto:aniway.aniway@gmail.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Tencent PC Manager für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com) für den Hinweis auf zwei in MS13-009 beschriebene Probleme.
-   Jose A Vazquez von Yenteasy Security Research in Zusammenarbeit mit Exodus Intelligence für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Jose A Vazquez von Yenteasy Security Research in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Mark Yason von IBM X-Force für den Hinweis auf ein in MS13-009 beschriebenes Problem.
-   Ollie Whitehouse von [NCC Group](https://www.nccgroup.com/) für die Zusammenarbeit mit uns an in MS13-009 enthaltenen Tiefenverteidigungsänderungen.
-   [Tencent Security Team](https://security.tencent.com/) für den Hinweis auf ein in MS13-011 beschriebenes Problem.
-   James Forshaw von [Context Information Security](https://www.contextis.com/) für den Hinweis auf ein in MS13-015 beschriebenes Problem.
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com) und [Tencent Security Team](https://security.tencent.com/) für den Hinweis auf zwei in MS13-016 beschriebene Probleme.
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf fünfundzwanzig in MS13-016 beschriebene Probleme.
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com) für den Hinweis auf drei in MS13-016 beschriebene Probleme.
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com) für den Hinweis auf zwei in MS13-017 beschriebene Probleme.
-   Max DeLiso für die Zusammenarbeit mit uns an einem in MS13-019 beschriebenen Problem.
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS13-020 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617.aspx)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (12. Februar 2013): Bulletin Summary veröffentlicht.
-   V1.1 (12. Februar 2013): Für MS13-009 wurde die Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen im **Ausnutzbarkeitsindex** für CVE-2013-0022 korrigiert.
-   V1.2 (13. Februar 2013): Für MS13-014 wurde die Bewertung der Ausnutzbarkeit für aktuelle Softwareversionen im **Ausnutzbarkeitsindex** für CVE-2013-1281 korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*