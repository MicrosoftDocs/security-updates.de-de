---
TOCTitle: 'MS11-DEC'
Title: Microsoft Security Bulletin Summary für Dezember 2011
ms:assetid: 'ms11-dec'
ms:contentKeyID: 61225093
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms11-dec(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Dezember 2011
=====================================================

Veröffentlicht: Dienstag, 13. Dezember 2011 | Aktualisiert: Mittwoch, 22. Februar 2012

**Version:** 2.1

In diesem Bulletin Summary sind die im Dezember 2011 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für Dezember 2011 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 28. Dezember 2011 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Am Mittwoch, den 14. Dezember 2011, um 11:00 Uhr pazifischer Zeit (USA und Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im Dezember.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032487961) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://go.microsoft.com/fwlink/?linkid=217214)

Am 29. Dezember 2011 um 13:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesem außerplanmäßigen Security Bulletin zu beantworten. [Registrieren Sie jetzt für den Security Bulletin-Webcast am 29. Dezember um 13:00 Uhr](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032502798&culture=en-us). Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](http://go.microsoft.com/fwlink/?linkid=217214)

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=233008">MS11-087</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-Kernelmodustreibern kann Remotecodeausführung ermöglichen (2639417)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument öffnet oder eine schädliche Webseite besucht, die TrueType-Schriftartdateien einbettet.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232507">MS11-090</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate von ActiveX-Kill Bits (2618451</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft-Software. Diese Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite in Internet Explorer aufruft, auf der Binärverhalten verwendet wird. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Dieses Update beinhaltet außerdem Kill Bits für vier ActiveX-Steuerelemente von Drittanbietern.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232517">MS11-092</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows Media</strong> <strong>kann Remotecodeausführung ermöglichen (2648048)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Media Player und Windows Media Center. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete DVR-MS-Datei (Microsoft Digital Video Recording-Datei) öffnet. In allen Fällen kann ein Benutzer nicht gezwungen werden, die Datei zu öffnen. Damit ein Angriff erfolgreich ist, muss ein Benutzer dazu verleitet werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227070">MS11-088</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Office IME</strong> <strong>(Chinesisch) kann Erhöhung von Berechtigungen ermöglichen (2652016)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office IME (Chinesisch). Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn ein angemeldeter Benutzer bestimmte Aktionen auf einem System durchführt, auf dem eine betroffene Version von Microsoft Pinyin (MSPY) Eingabemethoden-Editor (IME) für vereinfachtes Chinesisch installiert ist. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann im Kernel-Modus beliebigen Code ausführen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen administrativen Benutzerrechten erstellen. Von dieser Sicherheitsanfälligkeit sind nur Implementierungen von Microsoft Pinyin IME 2010 betroffen. Andere Versionen von IME für vereinfachtes Chinesisch und weitere Implementierungen von IME sind nicht betroffen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/bulletin/ms11-089">MS11-089</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft</strong> <strong>Office kann Remotecodeausführung ermöglichen (2590602)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Word-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235287">MS11-091</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Publisher können</strong> <strong>Remotecodeausführung ermöglichen (2607702)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Publisher-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232516">MS11-093</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in OLE kann Remotecodeausführung ermöglichen (2624667)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in allen unterstützten Editionen von Windows XP und Windows Server 2003. Dieses Sicherheitsupdate wird für alle unterstützten Editionen von Windows XP und Windows Server 2003 als Hoch eingestuft. Windows Vista, Windows Server 2008, Windows 7 und Windows Server 2008 R2 sind nicht von der Sicherheitsanfälligkeit betroffen.<br />
<br />
Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine Datei öffnet, die ein speziell gestaltetes OLE-Objekt enthält. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Endbenutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232493">MS11-094</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft PowerPoint können Remotecodeausführung ermöglichen (2639142)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei<strong></strong>vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Office. Die Sicherheitsanfälligkeiten können eine Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete PowerPoint-Datei öffnet. Ein Angreifer, dem es gelingt, eine der Sicherheitsanfälligkeiten auszunutzen, kann vollständige Kontrolle über das betroffene System erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232666">MS11-095</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory kann Remotecodeausführung ermöglichen (2640045)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Active Directory, Active Directory Application Mode (ADAM) und Active Directory Lightweight Directory Service (AD LDS). Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Angreifer sich bei einer Active Directory-Domäne anmeldet und eine speziell gestaltete Anwendung ausführt. Um diese Sicherheitsanfälligkeit auszunutzen, muss ein Angreifer zuerst Anmeldeinformationen erlangen, um sich bei einer Active Directory-Domäne anzumelden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232696">MS11-096</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Excel kann Remotecodeausführung ermöglichen (2640241)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der angemeldete Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten. Durch das Installieren und Konfigurieren von OFV (Office File Validation; Überprüfung von Office-Dateien) wird das Öffnen verdächtiger Dateien verhindert, um Angriffsmethoden zum Ausnutzen der in CVE-2011-3403 beschriebenen Sicherheitsanfälligkeiten zu unterbinden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232663">MS11-097</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Client/Server-</strong> <strong>Runtime-Subsystem kann Erhöhung von Berechtigungen ermöglichen (2620712)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt, die dafür entworfen wurde, einem Prozess mit höherer Integrität eine Geräte-Ereignismeldung zu senden. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232424">MS11-098</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows-Kernel kann Erhöhung von Berechtigungen ermöglichen (2633171)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei einem betroffenen System anmeldet und eine speziell gestaltete Anwendung ausführt, die zur Ausnutzung der Sicherheitsanfälligkeit ausgelegt ist. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen. Die Sicherheitsanfälligkeit kann nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232505">MS11-099</a></td>
<td style="border:1px solid black;"><strong>Kumulatives</strong> <strong>Sicherheitsupdate für Internet Explorer (2618444)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine gültige HTML-Datei (Hypertext Markup Language) öffnet, die sich im gleichen Verzeichnis befindet wie eine speziell gestaltete DLL-Datei (Dynamic Link Library).</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232432">MS11-100</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten</strong> <strong>in</strong> <strong>.NET Framework</strong> <strong>können</strong> <strong>Erhöhung von Berechtigungen ermöglichen</strong> <strong>(2638420)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft .NET Framework. Die schwerwiegendste dieser Sicherheitsanfälligkeiten kann Erhöhung von Berechtigungen ermöglichen, wenn ein nicht authentifizierter Angreifer eine speziell gestaltete Webanforderung an die Zielwebsite sendet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann auf der ASP.NET-Site beliebige Aktionen im Kontext eines vorhandenen Kontos durchführen, einschließlich des Ausführens willkürlicher Befehle. Um diese Sicherheitsanfälligkeit auszunutzen, muss ein Angreifer ein Konto auf der ASP.NET-Site registrieren können und einen vorhandenen Benutzernamen kennen.</td>
<td style="border:1px solid black;"><a href="http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Microsoft .NET Framework</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und dann nach CVE-ID geordnet. Nur Sicherheitsanfälligkeiten, deren Schweregrad in diesem Bulletin als „Kritisch“ oder „Hoch“ eingestuft wurde, sind enthalten.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/security/cc998259.aspx).
  
In den unten stehenden Spalten bezieht sich „Aktuelle Softwareversion“ auf die Themensoftware und „Ältere Softwareversionen“ auf alle älteren, unterstützten Versionen der Themensoftware, wie sie in den Tabellen „Betroffene Software“ und „Nicht betroffene Software“ im Bulletin aufgeführt ist.
 
<p> </p>
<table style="width:100%;">
<colgroup>
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
<col width="14%" />
</colgroup>
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=233008">MS11-087</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bei der Analyse von TrueType-Schriftarten</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3402">CVE-2011-3402</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit wurde öffentlich gemeldet.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=227070">MS11-088</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Pinyin IME durch Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2010">CVE-2011-2010</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/bulletin/ms11-089">MS11-089</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Word</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1983">CVE-2011-1983</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232507">MS11-090</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Time bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3397">CVE-2011-3397</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235287">MS11-091</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Publisher bezüglich außerhalb des Bereichs liegenden Arrayindexes</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3410">CVE-2011-3410</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235287">MS11-091</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Publisher aufgrund ungültigen Zeigers</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3411">CVE-2011-3411</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=235287">MS11-091</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Publisher bzgl. Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3412">CVE-2011-3412</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232517">MS11-092</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Windows Media Player DVR-MS</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3401">CVE-2011-3401</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232516">MS11-093</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OLE-Eigenschaft</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3400">CVE-2011-3400</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232493">MS11-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch nicht sichereres Laden von Bibliotheken in PowerPoint</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3396">CVE-2011-3396</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Microsoft PowerPoint 2010 ist nur betroffen, wenn das aktuelle Service Pack nicht installiert ist.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232493">MS11-094</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in OfficeArt-Shape bezüglich Remotecodeausführung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3413">CVE-2011-3413</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232666">MS11-095</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Active Directory durch Pufferüberlauf</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3406">CVE-2011-3406</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es sind nur Systeme betroffen, auf denen Active Directory, AD LDS oder ADAM ausgeführt wird.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232696">MS11-096</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Datensätzen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3403">CVE-2011-3403</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232663">MS11-097</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in CSRSS bezüglich der lokalen Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3408">CVE-2011-3408</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232424">MS11-098</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Ausnahmehandler</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2018">CVE-2011-2018</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232505">MS11-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Filter für siteübergreifende Skripterstellung durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-1992">CVE-2011-1992</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232505">MS11-099</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer durch das nicht sichere Laden von Bibliotheken</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-2019">CVE-2011-2019</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232432">MS11-100</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Konflikte in Hashtabelle können Denial-of-Service verursachen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3414">CVE-2011-3414</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Diese Sicherheitsanfälligkeit ist lediglich ein Denial-of-Service und wurde öffentlich gemeldet.
<div>
  
</div>
<div>
<a href="http://technet.microsoft.com/de-de/security/cc998259">Sicherheitsanfälligkeiten bezüglich Denial-of-Service erhalten eine Ausnutzbarkeitsindexbewertung von „3“.</a>
</div></td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232432">MS11-100</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ASP.NET durch Umgehung der Formularauthentifizierung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3416">CVE-2011-3416</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Erhöhung von Berechtigungen – Kontoübernahme</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=232432">MS11-100</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in der Formularauthentifizierung von ASP.NET durch Zwischenspeicherung von Tickets</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2011-3417">CVE-2011-3417</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Erhöhung von Berechtigungen – Kontoübernahme</td>
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b01bb041-005c-48c4-a606-66aa264ba0fa)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=21b4b999-2dbf-4921-80bd-cc7ab2cd1190)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=d85091b5-69bb-4d0f-839a-a65cd94e2887)  
(KB2619339)  
(Kritisch)  
[Windows XP Media Center Edition 2005 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=03bc6446-7cf3-47c4-8ed1-a53a4d53a429)  
(KB2619340)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=73531165-f299-4b62-b738-52fca410eaae)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=3b816964-d3c3-4f05-94c3-f54a6f54ca73)  
(KB2626416)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=edb594a4-14d2-4ffe-8d1c-2c283689fe8c)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0a872cd2-5f4d-400c-a1c4-a2d194746fb6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=126e8092-980d-471a-867d-d5939671b7df)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7d1d1e9a-603c-4895-a69f-b61186a75ad5)  
(KB2619339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a98bb7cf-9939-4927-8d21-ccb3845e7cb7)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=986f0087-c674-4060-8710-af3496adbfdd)  
(KB2626416)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9e1273e2-7775-40b4-b939-ab530677cd4a)  
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
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
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e84e6964-1580-41ef-9d3e-4d0c3ad4cb69)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dfb948c5-8aee-4bcd-babf-3564b78712dd)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6b555040-1117-4b06-a48c-02f0e1b686d8)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=01caf06f-777d-4ea8-95ca-e11d60a973ad)  
(KB2621146)  
(Hoch)  
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=6f7c7ccd-22a3-4fbc-bf21-bd0e42ab1da5)  
(KB2626416)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a14057e5-e2c2-4dde-8d26-542a9f162e98)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9d9f3667-3fd6-4948-83db-282783599f41)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2d37a8cb-2316-4db4-980c-11b6dcbdc696)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eb17782c-f754-42ab-905b-6f141df008c3)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=e1ba50cf-fc6b-4668-b71c-e9f75a8ac638)  
(KB2621146)  
(Hoch)  
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=1b610eb3-456c-4125-94b7-1ead4face8e3)  
(KB2626416)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7f595fd6-bdfd-4075-97e5-70efb7d49dff)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=1ecf72cd-6732-4cf3-aa22-8caf15ea633e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=7726ddbe-0578-44fb-a40f-49b804a45989)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=4cdde8a9-6d44-41fa-82c0-a25404cdfbb5)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=74099261-60ad-4c68-906c-60e131818955)  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=147ec6d3-3401-4aa3-a409-55346bcc7bd7)  
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
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
Keine
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
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7f69ec9d-43ad-4106-90ef-c191e7ec43af)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=1dd069a2-fb1a-4f31-88cc-bc031c3e2c80)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e9130fad-de8c-4be0-aea1-62cbaa310b76)  
(KB2619339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=470da512-2c8b-4ba9-b7bb-b9e6c45cd33f)  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=fa6e6d91-4aca-49a6-a6e8-c33ec413097e)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=ae1f1f86-6f13-4e1e-9f93-4f70b6c9927e)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=60fd5bf6-e820-44f6-8081-b98c0103acc1)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=b7c4bf05-eb2d-48ac-a6df-8afd88e811d8)  
(KB2619339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=8daf9a49-60cb-4813-ac7a-e9a4bf296889)  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c9794756-803d-48ba-86db-350fb577f01b)  
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
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
Keine
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
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c4ba344d-dd0d-4cfb-81d9-d364d7f37e25)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f485d4c3-a4af-4ae6-9404-e79afcbb4f6e)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory und Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=6f9ddcdb-a471-4e00-a697-92a24e4ea8d4)\*  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=6f934885-b134-400c-a452-50fd4eeedd5e)\*  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=058963f6-9654-41d0-86d2-f25a0c2ad416)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=28598ef6-13fb-44fd-8c76-599af7b0a01d)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory und Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=5253477b-422f-404a-941e-8b69da5a2670)\*  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7ade3832-bc20-4fce-8eac-8a3d072d2f1c)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=42cd1c33-11a7-4a29-ae85-f7272a626f91)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5915e19c-b576-453b-b621-5737774f5955)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
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
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4bd7a02b-c6d8-4eb5-a46d-e494a1233dc8)  
(Hoch)
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
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
Keine
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
Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0526727a-f2fb-4846-9b04-f1899f52f1f6)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d112623c-86ce-434a-8fe1-ec3e3e632763)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b6e44069-dec5-48f6-8fc4-8ab375a10b4e)  
(KB2619339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=d2e87199-6469-4bc0-a721-f43e817e4344)  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=0666bdf5-9eed-44c9-84ee-b45f9b3e14b3)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=cfd42c42-1595-419a-bf04-b23b64663629)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=81114ecd-0c73-4ca6-8a66-09c6c636a5db)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=f7997ab8-27e0-4714-845a-d237f4326587)  
(KB2619339)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=ba8d7aa9-8299-49a3-b0c0-b8b5eab48434)  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=620f94f9-1f61-45a0-a22e-e7510b56b9b8)  
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
[**MS11-087**](http://go.microsoft.com/fwlink/?linkid=233008)
</td>
<td style="border:1px solid black;">
[**MS11-090**](http://go.microsoft.com/fwlink/?linkid=232507)
</td>
<td style="border:1px solid black;">
[**MS11-092**](http://go.microsoft.com/fwlink/?linkid=232517)
</td>
<td style="border:1px solid black;">
[**MS11-093**](http://go.microsoft.com/fwlink/?linkid=232516)
</td>
<td style="border:1px solid black;">
[**MS11-095**](http://go.microsoft.com/fwlink/?linkid=232666)
</td>
<td style="border:1px solid black;">
[**MS11-097**](http://go.microsoft.com/fwlink/?linkid=232663)
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
Keine
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
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=d64a31ca-cccd-488a-98fd-c059b9e9e1ea)\*\*\*\*  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=bc018647-08cb-431a-8e7c-5dc04980eaa9)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Active Directory und Active Directory Lightweight Directory Service (AD LDS)](https://www.microsoft.com/download/details.aspx?familyid=a3e0d27c-8b29-4981-bdef-bcd037fd3408)\*  
(KB2621146)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=04878e9a-539a-4549-a5af-11d45add91da)\*  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=b46f6da7-6d24-4262-8e55-3b657db39813)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=9323b9b9-e9b0-4941-afe0-196d22df9ab4)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
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
[Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=5b2ebec4-cebb-47b6-864a-12d59a9a3e18)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*\*\*Server Core-Installation ist betroffen.** Dieses Update gilt, mit einer niedrigeren Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, wenn bei der Installation die Server Core-Installationsoption verwendet wurde. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-090**

<sup>[1]</sup> Dieses bestimmte Betriebssystem ist nicht von der Sicherheitsanfälligkeit betroffen, die in diesem Bulletin beschrieben ist. Das verfügbare Update setzt die Kill Bits für Steuerelemente von Drittanbietern.

**Tabelle 2**

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="4" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=7a6fcf8d-8c7b-4882-90d3-02db79a75238)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=caa9360b-2fd8-4f46-99e6-2decf1b60ca7)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=dc6dcd8c-c39f-4c4b-b5b2-b4c18c36973b)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=f3906245-b6f6-464a-84b6-e1b6b195df95)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eff633f7-abd9-45cc-acbd-4885123dbed2)  
(KB2656352)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=2fa77733-70f5-46ff-9cfe-2262d292b870)  
(Mittel)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a0c55d9b-8529-4d3d-910d-1a822a825be2)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=3e60e996-8850-4d25-b994-39646e2cc25e)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eff633f7-abd9-45cc-acbd-4885123dbed2)  
(KB2656352)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des** **Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=281e5bd4-4582-4aa9-af88-518ad3152132)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=759041cf-fd8b-4e04-b289-d74112bf978b)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=b1b4af92-3ff1-4727-9ba3-52764a7b81bb)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=1cbe9469-05f4-4305-bbfd-76b4a04cd598)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=7538762a-50e9-4f13-a60e-ff99aa8fbbf8)  
(KB2656358)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eff633f7-abd9-45cc-acbd-4885123dbed2)  
(KB2656352)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
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
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=5587eca8-86e9-4a63-81cb-81f68178a6c0)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=7a87f890-f106-41ab-bc53-4ca44dc99cb1)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=a42fa727-482c-4578-9a30-61fdf14ed4da)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eff633f7-abd9-45cc-acbd-4885123dbed2)  
(KB2656352)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=02d5c057-d551-411b-917b-43d7795111bc)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=2fccb214-6c79-4ef6-9d6e-df4f16ef792e)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eff633f7-abd9-45cc-acbd-4885123dbed2)  
(KB2656352)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
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
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a6c7c960-768d-40d4-8fe5-7d59f48ead1d)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=0adc422f-73f2-46ee-973f-9b7603a76d1e)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4327147b-0481-4172-a835-8786abc50596)  
(Hoch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=a0b19b35-1d48-4419-ba3d-66063cc472a7)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=49050cf2-949a-40e5-b2ee-6257a3837294)  
(KB2656362)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=8a3f2351-380b-4566-b186-906dca426d39)  
(Mittel)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=987f0966-01de-4edf-a0d6-4032d1d72966)  
(Hoch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c951044b-4596-462f-bc8f-bdd9d6734297)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=49050cf2-949a-40e5-b2ee-6257a3837294)  
(KB2656362)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
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
[**Niedrig**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5a4443f8-fec8-42be-ad67-8475920f1460)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=eaf587f0-9951-4480-a08b-377e61aaf72b)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=8f5af52f-dece-4f0c-9fc0-d4973e4f7b1a)\*\*  
(Niedrig)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=c03e65d6-4f92-4bc1-94b5-2f0183d0133e)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)\*\*  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=49050cf2-949a-40e5-b2ee-6257a3837294)\*\*  
(KB2656362)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)\*\*  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)\*\*<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=2f18fc98-984a-4c02-951f-b8438a9e4f6b)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)  
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=808d26f7-c8fa-446d-9d2f-e8c0babb0c4a)\*\*  
(Niedrig)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=b7a582f3-0a18-4fbf-9b99-21c664bfd979)\*\*  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)\*\*  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=49050cf2-949a-40e5-b2ee-6257a3837294)\*\*  
(KB2656362)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)\*\*  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)\*\*<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=fc62df39-7185-448b-b356-25a5a07886ec)  
(Keine Bewertung des Schweregrads<sup>[1]</sup>)
</td>
<td style="border:1px solid black;">
[Microsoft .NET Framework 1.1 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=471e1f51-c79c-4285-9f1e-aee1e4c4f189)  
(KB2656353)  
[Microsoft .NET Framework 2.0 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=49050cf2-949a-40e5-b2ee-6257a3837294)  
(KB2656362)  
[Microsoft .NET Framework 3.5 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=306acd0a-bea2-40dd-a639-f381587c9eb7)  
(KB2657424)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows 7
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[Windows 7 für 32-Bit-Systeme und Windows 7 für 32-Bit-Systeme Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=eb2bd108-5ef1-45be-9157-e7cbfc8afd2a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=018610bb-e80a-432a-8f32-f50451f71ad9)  
(Hoch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=ec2046a6-f069-4f02-9600-7640e57be0a3)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für 32-Bit-Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=2de28d32-1efd-4177-82e6-19a08266096c)  
(KB2656355)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)  
Nur Windows 7 für 32-Bit-Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=26e0b56d-9228-49cf-9276-0741257567a9)  
(KB2656356)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme und Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=dbe85b05-e252-4029-8e25-f2452db1c017)  
(Hoch)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=4c773b3d-0ca3-4b9b-af9a-9d6edcd261f7)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nur Windows 7 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=2de28d32-1efd-4177-82e6-19a08266096c)  
(KB2656355)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)  
Nur Windows 7 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=26e0b56d-9228-49cf-9276-0741257567a9)  
(KB2656356)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Windows Server 2008 R2
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-098**](http://go.microsoft.com/fwlink/?linkid=232424)
</td>
<td style="border:1px solid black;">
[**MS11-099**](http://go.microsoft.com/fwlink/?linkid=232505)
</td>
<td style="border:1px solid black;">
[**MS11-100**](http://go.microsoft.com/fwlink/?linkid=232432)
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
[**Kritisch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme und Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=2108b4ef-942f-4727-a1fc-ee7d0abb427c)\*\*  
(Niedrig)  
[Internet Explorer 9](https://www.microsoft.com/download/details.aspx?familyid=72c1654e-526f-4ece-b7ad-767a0710e076)\*\*  
(Hoch)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für x64-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=2de28d32-1efd-4177-82e6-19a08266096c)\*  
(KB2656355)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)  
Nur Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=26e0b56d-9228-49cf-9276-0741257567a9)\*  
(KB2656356)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)\*<sup>[1]</sup>
(KB2656351)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme und Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=74614510-e13c-43e8-90e7-d81e63895cf2)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nur Windows Server 2008 R2 für Itanium-basierte Systeme:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=2de28d32-1efd-4177-82e6-19a08266096c)  
(KB2656355)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)  
Nur Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1:  
[Microsoft .NET Framework 3.5.1](https://www.microsoft.com/download/details.aspx?familyid=26e0b56d-9228-49cf-9276-0741257567a9)  
(KB2656356)  
[Microsoft .NET Framework 4](https://www.microsoft.com/download/details.aspx?familyid=37a8fb34-e3ad-4605-980b-28361889ce72)<sup>[1]</sup>
(KB2656351)
</td>
</tr>
</table>
 
**Hinweise für Windows Server 2008 und Windows Server 2008 R2**

**\*Die Server Core-Installation ist betroffen.** Dieses Update gilt, mit der gleichen Bewertung des Schweregrads, wie angezeigt auch für unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2, unabhängig davon, ob bei der Installation die Server Core-Installationsoption verwendet wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**\*\*Die Server Core-Installation ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 oder Windows Server 2008 R2 wie angegeben nicht, wenn diese mit der Server Core-Installationsoption installiert wurden. Weitere Informationen zu dieser Installationsoption finden Sie in den TechNet-Artikeln [Verwalten einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ee441255(ws.10).aspx) und [Wartung einer Server Core-Installation](http://technet.microsoft.com/de-de/library/ff698994(ws.10).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 und Windows Server 2008 R2 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](http://www.microsoft.com/germany/windowsserver2008/editionen/r2-vergleich-server-core.mspx).

**Hinweis für MS11-099**

<sup>[1]</sup>Bewertungen des Schweregrads treffen für dieses Update für die angegebene Software nicht zu, da die in diesem Bulletin erörterten bekannten Angriffsmethoden in einer Standardkonfiguration blockiert werden. Microsoft empfiehlt jedoch den Benutzern dieser Software, dieses Sicherheitsupdate als tiefgreifende Verteidigungsmaßnahme zu installieren.

**Hinweis für MS11-100**

<sup>[1]</sup>**.NET Framework 4 und .NET Framework 4 Client Profile sind betroffen.** Die .NET Framework Version 4 Redistributable Packages sind in zwei Profilen verfügbar: .NET Framework 4 und .NET Framework 4 Client Profile. .NET Framework 4 Client Profile ist Teil von .NET Framework 4. Die in diesem Update behobene Sicherheitsanfälligkeit betrifft sowohl .NET Framework 4 als auch .NET Framework 4 Client Profile. Weitere Informationen finden Sie im MSDN-Artikel [Installieren von .NET Framework](http://msdn.microsoft.com/de-de/library/5a4x27ek.aspx).

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="6" style="border:1px solid black;">
Microsoft Office Suites und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-088**](http://go.microsoft.com/fwlink/?linkid=227070)
</td>
<td style="border:1px solid black;">
[**MS11-089**](http://technet.microsoft.com/de-de/security/bulletin/ms11-089)
</td>
<td style="border:1px solid black;">
[**MS11-091**](http://go.microsoft.com/fwlink/?linkid=235287)
</td>
<td style="border:1px solid black;">
[**MS11-094**](http://go.microsoft.com/fwlink/?linkid=232493)
</td>
<td style="border:1px solid black;">
[**MS11-096**](http://go.microsoft.com/fwlink/?linkid=232696)
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
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=13f3e884-37bf-4ed2-b3ed-a0e7fb48e44f)  
(KB2553084)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=5859014f-afc5-4958-82ea-6ba45a5ad4b3)  
(KB2596954)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2007 Service Pack 2 und Microsoft Office 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office 2007 Service Pack 2 und Microsoft Office 2007 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=e924cd85-5764-4056-bd32-b0e57dc25146)  
(KB2596785)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Publisher 2007 Service Pack 2 und Microsoft Publisher 2007 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=2856821e-f1fd-424b-b03c-e443685eea6d)  
(KB2596705)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=d0c3156c-c87c-4d3e-aca2-3fab9ff78711)  
(KB2596764)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2010 und Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Pinyin IME 2010 (32-Bit-Version)](https://www.microsoft.com/download/details.aspx?familyid=d812621e-c35a-4cb0-ba26-928363f3422d)  
(KB2596511)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 und Microsoft Office 2010 Service Pack 1 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=e47c0694-a9a5-4dd7-bfba-e470d9855c28)  
(KB2589320)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=fd32d083-46e7-4835-ba83-c33332b920bd)  
(KB2553185)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2010 und Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft Pinyin IME 2010 (64-Bit-Version)](https://www.microsoft.com/download/details.aspx?familyid=c8d3ac17-5aca-4da3-961f-b753be4a3634)  
(KB2596511)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2010 und Microsoft Office 2010 Service Pack 1 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=6c2d5273-eef9-4ff6-be6f-8d86f417f004)  
(KB2589320)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft PowerPoint 2010 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=f28b8cf6-8946-448a-ae4e-d11f8a76a679)  
(KB2553185)  
(Hoch)
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
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-088**](http://go.microsoft.com/fwlink/?linkid=227070)
</td>
<td style="border:1px solid black;">
[**MS11-089**](http://technet.microsoft.com/de-de/security/bulletin/ms11-089)
</td>
<td style="border:1px solid black;">
[**MS11-091**](http://go.microsoft.com/fwlink/?linkid=235287)
</td>
<td style="border:1px solid black;">
[**MS11-094**](http://go.microsoft.com/fwlink/?linkid=232493)
</td>
<td style="border:1px solid black;">
[**MS11-096**](http://go.microsoft.com/fwlink/?linkid=232696)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
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
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2004 für Mac
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
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=ef3b559c-0bd2-45dd-8049-6946f6431a2a)  
(KB2644358)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
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
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=2c4d0381-f7ab-49ed-a0c0-b381387d1e68)  
(KB2644354)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office für Mac 2011
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office für Mac 2011](https://www.microsoft.com/download/details.aspx?familyid=3c8017d6-232c-42a6-a133-96efe3ad3385)  
(KB2644347)  
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
<th colspan="6" style="border:1px solid black;">
Andere Microsoft Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS11-088**](http://go.microsoft.com/fwlink/?linkid=227070)
</td>
<td style="border:1px solid black;">
[**MS11-089**](http://technet.microsoft.com/de-de/security/bulletin/ms11-089)
</td>
<td style="border:1px solid black;">
[**MS11-091**](http://go.microsoft.com/fwlink/?linkid=235287)
</td>
<td style="border:1px solid black;">
[**MS11-094**](http://go.microsoft.com/fwlink/?linkid=232493)
</td>
<td style="border:1px solid black;">
[**MS11-096**](http://go.microsoft.com/fwlink/?linkid=232696)
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
Microsoft PowerPoint Viewer 2007 Service Pack 2
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
[Microsoft PowerPoint Viewer 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=4417592a-8db0-4e35-9895-d589bc341077)  
(KB2596912)  
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
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e799f654-7e2d-40c7-a3b8-32e44d1aa6ee)  
(KB2596843)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office Pinyin SimpleFast Style 2010 und Microsoft Office Pinyin – Neuer Eingabestil 2010 (32-Bit-Version)
</td>
<td style="border:1px solid black;">
Microsoft Office Pinyin SimpleFast Style 2010 und Microsoft Office Pinyin – Neuer Eingabestil 2010 (32-Bit-Version)<sup>[1]</sup>
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
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Pinyin SimpleFast Style 2010 und Microsoft Office Pinyin – Neuer Eingabestil 2010 (64-Bit-Version)
</td>
<td style="border:1px solid black;">
Microsoft Office Pinyin SimpleFast Style 2010 und Microsoft Office Pinyin – Neuer Eingabestil 2010 (64-Bit-Version)<sup>[1]</sup>
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
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweis für MS11-088**

<sup>[1]</sup>Diese Version von Microsoft Office Pinyin wird nicht mehr unterstützt.

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

-   Symantec und dem Laboratory of Cryptography and System Security (CrySyS) für die Zusammenarbeit mit uns an einem in MS11-087 beschriebenen Problem.
-   Yang Yanbei für den Hinweis auf ein in MS11-088 beschriebenes Problem.
-   Nikita Tarakanov (CIS Research Team) und Alexey Sintsov (Digital Security Research Group) in Zusammenarbeit mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [TippingPoint](http://www.tippingpoint.com/) für den Hinweis auf ein in MS11-089 beschriebenes Problem.
-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-090 beschriebenes Problem.
-   Will Dormann von [CERT/CC](http://www.cert.org/) für den Hinweis auf drei in MS11-091 beschriebene Probleme.
-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-092 beschriebenes Problem.
-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-093 beschriebenes Problem.
-   Greg MacManus von [iSIGHT Partners Labs](http://www.isightpartners.com/) für den Hinweis auf ein in MS11-094 beschriebenes Problem.
-   Einer Person, die mit [TippingPoint's](http://www.tippingpoint.com/)[Zero Day Initiative](http://www.zerodayinitiative.com/) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-094 beschriebenes Problem.
-   Einer Person, die mit [VeriSign iDefense Labs](http://labs.idefense.com) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf ein in MS11-096 beschriebenes Problem.
-   Alex Ionescu von Winsider Seminars & Solutions Inc. für den Hinweis auf ein in MS11-097 beschriebenes Problem.
-   Matthew Jurczyk in Zusammenarbeit mit [VeriSign iDefense Labs](http://labs.idefense.com/) für den Hinweis auf ein in MS11-098 beschriebenes Problem.
-   Thomas Stehle für den Hinweis auf ein in MS11-099 beschriebenes Problem
-   Andy Cooper vom [Citrix Security Team](http://www.citrix.com) für den Hinweis auf ein in MS11-099 beschriebenes Problem.
-   [Robert Swiecki](http://www.swiecki.net/) von [Google Inc.](http://www.google.com/) für den Hinweis auf ein in MS11-099 beschriebenes Problem.
-   [Yosuke Hasegawa](http://utf-8.jp/) für die Zusammenarbeit mit uns an einem in MS11-099 beschriebenen Problem.
-   [Jan Schejbal](http://janschejbal.wordpress.com/) für die Zusammenarbeit mit uns an in MS11-099 enthaltenen Tiefenverteidigungsänderungen.
-   Irene Abezgauz von [Seeker](http://www.seekersec.com) für den Hinweis auf ein in MS11-100 beschriebenes Problem.
-   Kestutis Gudinavicius von [SEC Consult](https://www.sec-consult.com/) für den Hinweis auf ein in MS11-100 beschriebenes Problem.
-   Oliver Dewdney von [LBi](http://www.lbi.com/) für den Hinweis auf ein in MS11-100 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](http://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](http://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](http://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (13. Dezember 2011): Bulletin Summary veröffentlicht.
-   V1.1 (13. Dezember 2011): In MS11-099 wurden die Bewertungen des Schweregrads in der Tabelle „Betroffene Software“ korrigiert. In MS11-088 wurde der wichtige Hinweis im Ausnutzbarkeitsindex korrigiert. Dies sind lediglich Informationsänderungen. An den Dateien des Sicherheitsupdates oder der Erkennungslogik wurden keine Änderungen vorgenommen.
-   V2.0 (29. Dezember 2011): Das Microsoft Security Bulletin MS11-100, „Sicherheitsanfälligkeiten in .NET Framework können Erhöhung von Berechtigungen ermöglichen (2638420)“, wurde hinzugefügt. Außerdem wurde der Bulletin-Webcastlink für dieses außerplanmäßige Security Bulletin hinzugefügt.
-   V2.1 (22. Februar 2012): In MS11-088 wurde der Produktsupportstatus für Microsoft Office Pinyin SimpleFast Style 2010 und Microsoft Office Pinyin – Neuer Eingabestil 2010 verdeutlicht. Diese Versionen von Microsoft Office Pinyin werden nicht mehr unterstützt. Weitere Informationen finden Sie im Bulletin.

*Built at 2014-04-18T01:50:00Z-07:00*