---
TOCTitle: 'MS13-SEP'
Title: Microsoft Security Bulletin Summary für September 2013
ms:assetid: 'ms13-sep'
ms:contentKeyID: 61225126
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms13-sep(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für September 2013
======================================================

Veröffentlicht: Dienstag, 10. September 2013 | Aktualisiert: Mittwoch, 6. November 2013

**Version:** 1.1

In diesem Bulletin Summary sind die im September 2013 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für September 2013 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 5. September 2013 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, dem 11. September 2013, um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im September.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032557378&culture=en-us) Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032557378&culture=en-us) zur Verfügung.

Microsoft stellt auch Informationen bereit, anhand derer Benutzer die Prioritäten für monatliche Sicherheitsupdates und alle nicht sicherheitsrelevanten Updates festlegen können, die an demselben Tag veröffentlicht werden wie die monatlichen Sicherheitsupdates. Bitte lesen Sie den Abschnitt **Weitere Informationen**.

### Bulletin-Informationen

#### Kurzzusammenfassungen

In der folgenden Tabelle sind die Security Bulletins für diesen Monat nach Schweregrad geordnet.

Weitere Informationen zu betroffener Software finden Sie im nächsten Abschnitt **Betroffene Software**.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen (2834052)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und neun vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office Server-Software. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung im Kontext des W3WP-Dienstkontos ermöglichen, wenn ein Angreifer speziell gestaltete Inhalte an den betroffenen Server sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=307055">MS13-068</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Outlook kann Remotecodeausführung ermöglichen (2756473)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Outlook. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer mit einer betroffenen Edition von Microsoft Outlook eine Vorschau einer speziell gestalteten E-Mail-Nachricht anzeigt oder öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2870699)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zehn vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der die schwerwiegendste dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320629">MS13-070</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in OLE kann Remotecodeausführung ermöglichen (2876217)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Datei öffnet, die ein speziell gestaltetes OLE-Objekt enthält. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314046">MS13-071</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Designdatei kann Remotecodeausführung ermöglichen (2864063)<br />
</strong><br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Windows-Design auf seinem System installiert. In allen Fällen kann ein Benutzer nicht gezwungen werden, die Datei zu öffnen oder das Design zu installieren. Damit ein Angriff erfolgreich ist, muss ein Benutzer dazu verleitet werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office können Remotecodeausführung ermöglichen (2845537)<br />
</strong><br />
Dieses Sicherheitsupdate behebt dreizehn vertraulich gemeldete Sicherheitsanfälligkeiten<strong></strong>in Microsoft Office. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn eine speziell gestaltete Datei in einer betroffenen Version der Microsoft Office-Software geöffnet wird. Ein Angreifer, der die schwerwiegendsten Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293351">MS13-073</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Excel können Remotecodeausführung ermöglichen (2858300)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Office-Datei mit einer betroffenen Version von Microsoft Excel oder anderer betroffener Microsoft Office-Software öffnet. Ein Angreifer, der die schwerwiegendsten Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=308989">MS13-074</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Access können Remotecodeausführung ermöglichen (2848637)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Access-Datei mit einer betroffenen Version von Microsoft Access öffnet. Ein Angreifer, der die Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=318022">MS13-075</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office IME (Chinesisch) kann Erhöhung von Berechtigungen ermöglichen (2878687)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office IME (Chinesisch). Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein angemeldeter Angreifer Internet Explorer von der Symbolleiste in Microsoft Pinyin IME für vereinfachtes Chinesisch startet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann im Kernel-Modus beliebigen Code ausführen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. Von dieser Sicherheitsanfälligkeit sind nur Implementierungen von Microsoft Pinyin IME 2010 betroffen. Andere Versionen von IME für vereinfachtes Chinesisch und weitere Implementierungen von IME sind nicht betroffen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Kernelmodus</strong> <strong>treibern können Erhöhung von Berechtigungen ermöglichen (2876315)</strong><br />
<br />
Dieses Sicherheitsupdate behebt sieben vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320630">MS13-077</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Dienststeuerungs-Manager kann Erhöhung von Berechtigungen ermöglichen (2872339)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer einen authentifizierten Benutzer dazu verleitet, eine speziell gestaltete Anwendung auszuführen. Um diese Sicherheitsanfälligkeit auszunutzen muss ein Angreifer entweder über gültige Anmeldeinformationen verfügen und sich lokal anmelden können, oder er muss einen Benutzer dazu verleiten, die speziell gestaltete Anwendung des Angreifers auszuführen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=318021">MS13-078</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in FrontPage kann Offenlegung von Information ermöglichen (2825621)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft FrontPage. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer ein speziell gestaltetes FrontPage-Dokument öffnet. Die Sicherheitsanfälligkeit kann nicht automatisch ausgenutzt werden. Damit ein Angriff erfolgreich ist, muss ein Benutzer dazu verleitet werden, das speziell gestaltete Dokument zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320666">MS13-079</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory kann Denial-of-Service ermöglichen (2853587)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Active Directory. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer eine speziell gestaltete Abfrage an den Lightweight Directory Access Protocol (LDAP)-Dienst sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SharePoint bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0081">CVE-2013-0081</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1315">CVE-2013-1315</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293351">MS13-073</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Deaktivierung von MAC</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1330">CVE-2013-1330</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in SharePoint XSS</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3179">CVE-2013-3179</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in POST durch siteübergreifende Skripterstellung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3180">CVE-2013-3180</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3847">CVE-2013-3847</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3848">CVE-2013-3848</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3849">CVE-2013-3849</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3857">CVE-2013-3857</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a><a href="https://go.microsoft.com/fwlink/?linkid=293350"></a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3858">CVE-2013-3858</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a><a href="https://go.microsoft.com/fwlink/?linkid=293350"></a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=307055">MS13-068</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Nachrichtenzertifikat</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3870">CVE-2013-3870</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3201">CVE-2013-3201</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3202">CVE-2013-3202</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3203">CVE-2013-3203</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3204">CVE-2013-3204</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3205">CVE-2013-3205</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3206">CVE-2013-3206</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3207">CVE-2013-3207</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3208">CVE-2013-3208</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3209">CVE-2013-3209</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320631">MS13-069</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3845">CVE-2013-3845</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Internet Explorer 11 ist nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320629">MS13-070</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLE-Eigenschaft</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3863">CVE-2013-3863</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314046">MS13-071</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows-Designdatei bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0810">CVE-2013-0810</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Auflösung XML-externer Entitäten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3160">CVE-2013-3160</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3847">CVE-2013-3847</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3848">CVE-2013-3848</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3849">CVE-2013-3849</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3850">CVE-2013-3850</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3851">CVE-2013-3851</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3852">CVE-2013-3852</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3853">CVE-2013-3853</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3854">CVE-2013-3854</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3855">CVE-2013-3855</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3856">CVE-2013-3856</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3857">CVE-2013-3857</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=299217">MS13-072</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Word bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3858">CVE-2013-3858</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293351">MS13-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1315">CVE-2013-1315</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit betrifft auch <a href="https://go.microsoft.com/fwlink/?linkid=293350">MS13-067</a>.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293351">MS13-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Office bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3158">CVE-2013-3158</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=293351">MS13-073</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Auflösung XML-externer Entitäten</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3159">CVE-2013-3159</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=308989">MS13-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Access durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3155">CVE-2013-3155</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=308989">MS13-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Access-Dateiformat bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3156">CVE-2013-3156</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=308989">MS13-074</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Access durch Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3157">CVE-2013-3157</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=318022">MS13-075</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in IME für Chinesisch</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3859">CVE-2013-3859</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1341">CVE-2013-1341</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1342">CVE-2013-1342</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1343">CVE-2013-1343</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1344">CVE-2013-1344</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3864">CVE-2013-3864</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3865">CVE-2013-3865</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320624">MS13-076</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3866">CVE-2013-3866</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit bezüglich Denial-of-Service unter Windows 8 und Windows Server 2012.<br />
<br />
Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.<br />
<br />
Dies ist eine Sicherheitsanfälligkeit durch Offenlegung von Informationen, die bei anderer betroffener Software zu einer Erhöhung von Berechtigungen ermöglichen kann.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320630">MS13-077</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Dienststeuerungs-Manager durch doppelte Freigabe</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3862">CVE-2013-3862</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=318021">MS13-078</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in XML bezüglich Offenlegung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3137">CVE-2013-3137</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=320666">MS13-079</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch remote anonymen Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3868">CVE-2013-3868</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.<br />
<br />
Windows 8.1 und Windows Server 2012 R2 sind nicht betroffen.</td>
</tr>
</tbody>
</table>
 

Betroffene Software
-------------------

In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.

**Wie verwende ich diese Tabellen?**  

In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt ist, ist die Bewertung des Schweregrads des Softwareupdates ebenfalls aufgeführt.

**Hinweis:** Für eine Sicherheitsanfälligkeit müssen Sie möglicherweise mehrere Sicherheitsupdates installieren. Durchsuchen Sie in der gesamten Spalte die einzelnen Kennungen der aufgeführten Bulletins, um basierend auf den auf Ihrem System installierten Programmen oder Komponenten zu überprüfen, welche Updates Sie installieren müssen.

#### Systemkomponenten des Windows-Betriebssystems

<p> </p>
<table style="border:1px solid black;">
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
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2870699)  
(Kritisch)  
Internet Explorer 7  
(2870699)  
(Kritisch)  
Internet Explorer 8  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2876217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2864063)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2876315)  
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
Internet Explorer 6  
(2870699)  
(Kritisch)  
Internet Explorer 7  
(2870699)  
(Kritisch)  
Internet Explorer 8  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2876217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2864063)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2876315)  
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
<th colspan="7" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2870699)  
(Mittel)  
Internet Explorer 7  
(2870699)  
(Mittel)  
Internet Explorer 8  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2876217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2864063)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2876315)  
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
Internet Explorer 6  
(2870699)  
(Mittel)  
Internet Explorer 7  
(2870699)  
(Mittel)  
Internet Explorer 8  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2876217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2864063)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2876315)  
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
Internet Explorer 6  
(2870699)  
(Mittel)  
Internet Explorer 7  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2876217)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2864063)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2876315)  
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
<th colspan="7" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2870699)  
(Kritisch)  
Internet Explorer 8  
(2870699)  
(Kritisch)  
Internet Explorer 9  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2864063)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2870699)  
(Kritisch)  
Internet Explorer 8  
(2870699)  
(Kritisch)  
Internet Explorer 9  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2864063)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
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
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2870699)  
(Mittel)  
Internet Explorer 8  
(2870699)  
(Mittel)  
Internet Explorer 9  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2864063)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2870699)  
(Mittel)  
Internet Explorer 8  
(2870699)  
(Mittel)  
Internet Explorer 9  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2864063)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2864063)  
(Keine Bewertung des Schweregrads)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2876315)  
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
<th colspan="7" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
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
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2870699)  
(Kritisch)  
Internet Explorer 9  
(2870699)  
(Kritisch)  
Internet Explorer 10  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2872339)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2870699)  
(Kritisch)  
Internet Explorer 9  
(2870699)  
(Kritisch)  
Internet Explorer 10  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2872339)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
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
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2870699)  
(Mittel)  
Internet Explorer 9  
(2870699)  
(Mittel)  
Internet Explorer 10  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2872339)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2872339)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows Server 2012
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2870699)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows RT
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
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
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2870699)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(2876315)  
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
<th colspan="7" style="border:1px solid black;">
Server Core-Installationsoption
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-069**](https://go.microsoft.com/fwlink/?linkid=320631)
</td>
<td style="border:1px solid black;">
[**MS13-070**](https://go.microsoft.com/fwlink/?linkid=320629)
</td>
<td style="border:1px solid black;">
[**MS13-071**](https://go.microsoft.com/fwlink/?linkid=314046)
</td>
<td style="border:1px solid black;">
[**MS13-076**](https://go.microsoft.com/fwlink/?linkid=320624)
</td>
<td style="border:1px solid black;">
[**MS13-077**](https://go.microsoft.com/fwlink/?linkid=320630)
</td>
<td style="border:1px solid black;">
[**MS13-079**](https://go.microsoft.com/fwlink/?linkid=320666)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr>
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2872339)
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
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
Windows Server 2012 (Server Core-Installation)  
(2876315)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory Services  
(2853587)  
(Hoch)  
Active Directory Lightweight Directory Service (AD LDS)  
(2853587)  
(Hoch)
</td>
</tr>
</table>
 

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Office 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3  
(MSO)  
(2817474)  
(Hoch)  
Microsoft Word 2003 Service Pack 3  
(2817682)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2003 Service Pack 3  
(2810048)  
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
<th colspan="6" style="border:1px solid black;">
Microsoft Office 2007
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des** **Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
**Keine**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2007 Service Pack 3  
(2825999)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 3  
(MSO)  
(2760411)  
(Hoch)  
Microsoft Office 2007 Service Pack 3  
(MSPTLS)  
(2597973)  
(Hoch)  
Microsoft Word 2007 Service Pack 3  
(2767773)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2007 Service Pack 3  
(2760583)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2007 Service Pack 3  
(2596825)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Office 2010
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
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
Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2010 Service Pack 1 (32-Bit-Editionen)  
(2794707)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Word 2010 Service Pack 1 (32-Bit-Editionen)  
(2760769)  
(Hoch)  
Microsoft Word 2010 Service Pack 1 (32-Bit-Editionen)  
(2767913)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2010 Service Pack 1 (32-Bit-Editionen)  
(2760597)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2010 Service Pack 1 (32-Bit-Editionen)  
(2687423)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Pinyin IME 2010 (32-Bit-Version)  
(2687413)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2010 Service Pack 2 (32-Bit-Editionen)  
(2794707)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2760769)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (32-Bit-Editionen)  
(2767913)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2010 Service Pack 2 (32-Bit-Editionen)  
(2760597)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2010 Service Pack 2 (32-Bit-Editionen)  
(2687423)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2010 Service Pack 1 (64-Bit-Editionen)  
(2794707)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Word 2010 Service Pack 1 (64-Bit-Editionen)  
(2760769)  
(Hoch)  
Microsoft Word 2010 Service Pack 1 (64-Bit-Editionen)  
(2767913)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2010 Service Pack 1 (64-Bit-Editionen)  
(2760597)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2010 Service Pack 1 (64-Bit-Editionen)  
(2687423)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Pinyin IME 2010 (64-Bit-Version)  
(2687413)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 Service Pack 2 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Outlook 2010 Service Pack 2 (64-Bit-Editionen)  
(2794707)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2760769)  
(Hoch)  
Microsoft Word 2010 Service Pack 2 (64-Bit-Editionen)  
(2767913)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Excel 2010 Service Pack 2 (64-Bit-Editionen)  
(2760597)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2010 Service Pack 2 (64-Bit-Editionen)  
(2687423)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Office 2013
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 (32-Bit-Editionen)  
(2768017)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2013 (32-Bit-Editionen)  
(2810009)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2013 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 (64-Bit-Editionen)  
(2768017)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Access 2013 (64-Bit-Editionen)  
(2810009)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2013 RT
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel 2013 RT  
(2768017)  
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
<th colspan="6" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011  
(2877813)  
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
<th colspan="6" style="border:1px solid black;">
Andere Microsoft Office-Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-068**](https://go.microsoft.com/fwlink/?linkid=307055)
</td>
<td style="border:1px solid black;">
[**MS13-072**](https://go.microsoft.com/fwlink/?linkid=299217)
</td>
<td style="border:1px solid black;">
[**MS13-073**](https://go.microsoft.com/fwlink/?linkid=293351)
</td>
<td style="border:1px solid black;">
[**MS13-074**](https://go.microsoft.com/fwlink/?linkid=308989)
</td>
<td style="border:1px solid black;">
[**MS13-075**](https://go.microsoft.com/fwlink/?linkid=318022)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2760823)  
(Hoch)
</td>
<td style="border:1px solid black;">
Microsoft Office Compatibility Pack Service Pack 3  
(2760588)  
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
Microsoft Word Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Word Viewer  
(2817683)  
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
<td style="border:1px solid black;">
Microsoft Excel Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Microsoft Excel Viewer  
(2760590)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 

#### Microsoft Server Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Portal Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Portal Server 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Windows SharePoint Services 2.0  
(2810061)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server 2007
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Windows SharePoint Services 3.0 Service Pack 3 (32-Bit-Versionen)  
(2760420)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Microsoft Windows SharePoint Services 3.0 Service Pack 3 (64-Bit-Versionen)  
(2760420)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server 2010
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 1 (wss)  
(2810067)  
(Kritisch)  
Microsoft SharePoint Server 2010 Service Pack 1 (coreserverloc)  
(2817393)  
(Kritisch)  
Microsoft SharePoint Server 2010 Service Pack 1 (wosrv)  
(2817372)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 2 (wss)  
(2810067)  
(Kritisch)  
Microsoft SharePoint Server 2010 Service Pack 2 (coreserver)  
(2817393)  
(Kritisch)  
Microsoft SharePoint Server 2010 Service Pack 2 (wosrv)  
(2817372)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server 2013
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013
</td>
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2013  
(2817315)  
(Hoch)  
Microsoft SharePoint Server 2013 (coreserverloc)  
(2810083)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-067**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Office-Dienste und Web Apps

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server 2007
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(2760589)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2007 Service Pack 3 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
Excel Services  
(2760589)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft SharePoint Server 2010
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Excel Services  
(2760595)  
(Kritisch)  
Microsoft Business Productivity Servers  
(2553408)  
(Kritisch)  
Word-Automatisierungsdienste  
(2760755)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Excel Services  
(2760595)  
(Kritisch)  
Microsoft Business Productivity Servers  
(2553408)  
(Kritisch)  
Word-Automatisierungsdienste  
(2760755)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office Web Apps 2010
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Microsoft Excel Web App 2010 Service Pack 1  
(2760594)  
(Kritisch)  
Microsoft Word Web App 2010 Service Pack 1  
(2817384)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Excel Web App 2010 Service Pack 2  
(2760594)  
(Kritisch)  
Microsoft Word Web App 2010 Service Pack 2  
(2817384)  
(Kritisch)
</td>
</tr>
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office Web Apps 2013
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-067**](https://go.microsoft.com/fwlink/?linkid=293350)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2013
</td>
<td style="border:1px solid black;">
Microsoft Office Web Apps Server 2013  
(2817305)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-067**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Produktivitätssoftware

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft FrontPage 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-078**](https://go.microsoft.com/fwlink/?linkid=318021)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft FrontPage 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft FrontPage 2003 Service Pack 3  
(2825621)  
(Hoch)
</td>
</tr>
</table>
 

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

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
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

**MS13-067**

-   Will Dormann vom [CERT/CC](https://www.cert.org/) für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung (CVE-2013-1315).
-   Alexandre Herzog der [Compass Security AG](https://www.csnc.ch/) für den Hinweis auf die Sicherheitsanfälligkeit durch Deaktivierung von MAC (CVE-2013-1330).
-   Benjamin Kunz Mejri vom Vulnerability Research Laboratory für den Hinweis auf Sicherheitsanfälligkeit in SharePoint durch siteübergreifende Skripterstellung (CVE-2013-3179).
-   Mateusz Jurczyk, Ivan Fratric und Ben Hawkes vom [Google Security Team](https://www.google.com/) für den Hinweis auf mehrere Sicherheitsanfälligkeiten bezüglich Speicherbeschädigung in Microsoft Word (CVE-2013-3847, CVE-2013-3848, CVE-2013-3849, CVE-2013-3857, CVE-2013-3858).

**MS13-068**

-   Alexander Klink von [n.runs AG](https://www.nruns.com/) für den Hinweis auf die Sicherheitsanfälligkeit im Nachrichtenzertifikat (CVE-2013-3870).

**MS13-069**

-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3201).
-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3202).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3203).
-   Ivan Fratric und Ben Hawkes vom [Google Security Team](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3204).
-   Peter ‘corelanc0d3 r‘ Van Eeckhoutte von [Corelan](https://www.corelangcv.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3205).
-   Bo Qu von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3205).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3206).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3207).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3208).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3209).
-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3845).

**MS13-070**

-   G. Geshev in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in OLE-Eigenschaft (CVE-2013-3863).

**MS13-071**

-   Eduardo Prado in Zusammenarbeit mit [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Windows-Designdatei bezüglich Remotecodeausführung (CVE-2013-0810).

**MS13-072**

-   Timur Yunusov, Alexey Osipov und Ilya Karpov von [Positive Technologies](https://www.ptsecurity.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Auflösung XML-externer Entitäten (CVE-2013-3160).
-   Mateusz Jurczyk, Ivan Fratric und Ben Hawkes vom [Google Security Team](https://www.google.com/) für den Hinweis auf mehrere Sicherheitsanfälligkeiten in Microsoft Word bezüglich Speicherbeschädigung (CVE-2013-3847, CVE-2013-3848, CVE-2013-3849, CVE-2013-3850, CVE-2013-3851, CVE-2013-3852, CVE-2013-3853, CVE-2013-3854, CVE-2013-3855, CVE-2013-3856, CVE-2013-3857, CVE-2013-3858).

**MS13-073**

-   Will Dormann vom [CERT/CC](https://www.cert.org/) für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung (CVE-2013-1315).
-   Will Dormann vom [CERT/CC](https://www.cert.org/) für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Office bezüglich Speicherbeschädigung (CVE-2013-3158).
-   Timur Yunusov, Alexey Osipov und Ilya Karpov von [Positive Technologies](https://www.ptsecurity.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Auflösung XML-externer Entitäten (CVE-2013-3159).

**MS13-074**

-   Kaveh Ghaemmaghami von [Secunia SVCRP](https://secunia.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Access durch Speicherbeschädigung (CVE-2013-3155).
-   Kaveh Ghaemmaghami von [Secunia SVCRP](https://secunia.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Access durch Speicherbeschädigung (CVE-2013-3156).
-   Kaveh Ghaemmaghami von [Secunia SVCRP](https://secunia.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Access durch Speicherbeschädigung (CVE-2013-3157).

**MS13-075**

-   Wei Wang von [VulnHunt](https://www.vulnhunt.com/) für den Hinweis auf die Sicherheitsanfälligkeit in IME für Chinesisch (CVE-2013-3859).

**MS13-076**

-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-1341).
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-1342).
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-1343).
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-1344).
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-3864).
-   [Gynvael Coldwind](https://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k durch mehrfaches Abrufen (CVE-2013-3865).
-   Guo Pengfei von [Qihoo 360 Security Center](https://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit in Win32k bezüglich der Erhöhung von Berechtigungen (CVE-2013-3866).

**MS13-078**

-   Timur Yunusov von [Positive Technologies](https://www.ptsecurity.com/) für den Hinweis auf die Sicherheitsanfälligkeit in XML bezüglich Offenlegung (CVE-2013-3137).

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (10. September 2013): Bulletin Summary veröffentlicht.
-   V1.1 (6. November 2013): In MS13-067 wurde der Produktname für das Update für den Microsoft Office Web Apps Server 2013 (2817305) korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*
