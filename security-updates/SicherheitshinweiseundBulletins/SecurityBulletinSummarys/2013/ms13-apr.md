---
TOCTitle: 'MS13-APR'
Title: Microsoft Security Bulletin Summary für April 2013
ms:assetid: 'ms13-apr'
ms:contentKeyID: 61225115
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms13-apr(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für April 2013
==================================================

Veröffentlicht: Dienstag, 9. April 2013 | Aktualisiert: Dienstag, 25. Juni 2013

**Version:** 4.0

In diesem Bulletin Summary sind die im April 2013 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für April 2013 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 4. April 2013 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](http://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](http://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, dem 10. April 2013, um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für den Security Bulletin-Webcast im April](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538640&culture=en-us). Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032538640&culture=en-us) zur Verfügung.

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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285215">MS13-028</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2817183)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt, können diese Sicherheitsanfälligkeiten Remotecodeausführung ermöglichen. Ein Angreifer, der diese Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286679">MS13-029</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Remote</strong> <strong>desktopclient kann Remotecodeausführung ermöglichen (2828223)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Windows Remotedesktopclient. Wenn ein Benutzer eine speziell gestaltete Webseite anzeigt, kann diese Sicherheitsanfälligkeit Remotecodeausführung ermöglichen. Ein Angreifer, der die Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286577">MS13-030</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in SharePoint kann Offenlegung von Information ermöglichen (2827663)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft SharePoint Server. Die Sicherheitsanfälligkeit kann Offenlegung von Informationen ermöglichen, wenn ein Angreifer die Adresse oder den Speicherort einer bestimmten SharePoint-Liste ermittelt und Zugang zu der SharePoint-Website erhält, auf der die Liste verwaltet wird. Der Angreifer muss die Authentifizierungsanforderungen der SharePoint-Website erfüllen, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-031">MS13-031</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (2813170)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=280660">MS13-032</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory kann Denial-of-Service ermöglichen (2830914)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Active Directory. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer eine speziell gestaltete Abfrage an den Lightweight Directory Access Protocol (LDAP)-Dienst sendet.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286700">MS13-033</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Windows Client/Server-Runtime-Subsystem (CSRSS) kann Erhöhung von Berechtigungen ermöglichen (2820917)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in allen unterstützten Editionen von Windows XP, Windows Vista, Windows Server 2003 und Windows Server 2008. Die Sicherheitsanfälligkeit ermöglicht eine Erhöhung von Berechtigungen, wenn ein Angreifer sich bei einem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeit auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=276805">MS13-034</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Antimalware-Client kann Erhöhung von Berechtigungen ermöglichen (2823482)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Microsoft Antimalware-Client. Die Sicherheitsanfälligkeit kann eine Erhöhung von Berechtigungen ermöglichen, verursacht durch die Pfadnamen, die vom Microsoft Antimalware-Client verwendet werden. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann beliebigen Code ausführen und vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Ein Angreifer muss über gültige Anmeldeinformationen verfügen, um diese Sicherheitsanfälligkeit ausnutzen zu können. Die Sicherheitsanfälligkeit kann nicht von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Sicherheitssoftware</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285672">MS13-035</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in HTML-Bereinigung kann Erhöhung von Berechtigungen ermöglichen (2821818)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Office. Die Sicherheitsanfälligkeit kann Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer einem Benutzer speziell gestaltete Inhalte sendet.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office,<br />
Microsoft Server Software</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=281927">MS13-036</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Kernelmodustreiber können Erhöhung von Berechtigungen ermöglichen (2829996)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die schwerste dieser Sicherheitsanfälligkeiten kann eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer bei dem System anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um die schwersten Sicherheitsanfälligkeiten auszunutzen.</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
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
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, innerhalb von 30 Tagen Angriffe durch Codeausführung und Denial-of-Service stattfinden. Sehen Sie sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen an, um Prioritäten für die Bereitstellung der Updates dieses Monats festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](http://technet.microsoft.com/de-de/security/cc998259).
  
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
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285215">MS13-028</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1303">CVE-2013-1303</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285215">MS13-028</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1304">CVE-2013-1304</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285215">MS13-028</a></td>
<td style="border:1px solid black;">Use-after-free-Sicherheitsanfälligkeit in Internet Explorer</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1338">CVE-2013-1338</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286679">MS13-029</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Remotecodeausführung im ActiveX-Steuerelement RDP</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1296">CVE-2013-1296</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286577">MS13-030</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich Offenlegung von Informationen durch falsche Zugriffsrechte</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1290">CVE-2013-1290</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-031">MS13-031</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung im Kernel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1284">CVE-2013-1284</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/bulletin/ms13-031">MS13-031</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung im Kernel</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1294">CVE-2013-1294</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=280660">MS13-032</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Auslastung des Arbeitsspeichers</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1282">CVE-2013-1282</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=286700">MS13-033</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in CSRSS bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1295">CVE-2013-1295</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Unter Windows Server 2003 und Windows XP Professional x64 Edition ist dies eine Sicherheitsanfälligkeit bezüglich Erhöhung von Berechtigungen.<br />
<br />
Unter Windows XP, Windows Vista und Windows Server 2008 ist dies eine Sicherheitsanfälligkeit bezüglich Denial-of-Service.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=276805">MS13-034</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Antimalware durch fehlerhaften Pfadnamen</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-0078">CVE-2013-0078</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=285672">MS13-035</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit bezüglich HTML-Bereinigung</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1289">CVE-2013-1289</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Microsoft ist sich gezielter Angriffe bewusst, bei denen versucht wird, die Sicherheitsanfälligkeit auszunutzen.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=281927">MS13-036</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1283">CVE-2013-1283</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="http://go.microsoft.com/fwlink/?linkid=281927">MS13-036</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit durch Racebedingung in Win32k</td>
<td style="border:1px solid black;"><a href="http://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-1292">CVE-2013-1292</a></td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="http://technet.microsoft.com/de-de/security/cc998259.aspx">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
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
<th colspan="7" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=f7b699b1-7655-4c8f-bd1a-535ff210b338)  
(2817183)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e9f9848e-b926-4487-9dc2-b2a6b6f5f98e)  
(2817183)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=4cf0de09-2e8d-4be0-bbbf-d040164f22e0)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=353812de-b1eb-4245-82e3-7829cb72bba3)  
(2813345)  
(Kritisch)  
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=1754fdde-4744-4783-b6d3-e38eb2874b58)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=69de7e3c-d99b-432a-b286-f45841edc4a7)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=8adb6ced-6065-454b-ba67-b0acd621df76)  
(2801109)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=f47a73d3-05f6-4c7d-b063-c83dd0070c2d)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 3](http://www.microsoft.com/downloads/details.aspx?familyid=75914c2a-37bb-4541-81ed-a602acb27a14)  
(2808735)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=4496bce8-809e-458c-b199-49b32eef7b21)  
(2817183)  
(Kritisch)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9d792ad9-c2d7-4972-9f27-4580af04571c)  
(2817183)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c3bdbbb8-57a2-4474-9b86-239f7a77e658)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=f413845a-84e0-48d9-b5bc-56a37109ab33)  
(2813345)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=74855fb1-cad1-463f-a02d-1c27a39667c9)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=9fb780b9-bbca-45ec-98db-da413f0ccddf)  
(2801109)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c143a028-2c38-469f-a563-be8030ec76e3)  
(2820917)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=20a1f311-5cdc-4675-a228-32993d8be3f9)  
(2808735)  
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
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=8d834fd2-eaa0-4742-a8a2-93277ca41f91)  
(2817183)  
(Mittel)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b0cbbaaf-be40-4088-b3d3-ca85410807b7)  
(2817183)  
(Mittel)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=cd2731b3-406e-4b73-bd70-4f2bb16dfb08)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=75b00750-80c3-4ffa-adbf-5f40a41309b9)  
(2813345)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=2c242d48-8dbe-4474-ba39-f7e3ebe9a604)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=c27666a5-67ff-4e2d-b9d7-2cef19da1edd)  
(2772930)  
(Hoch)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=13eb9459-0a39-4652-b577-6d8509801f62)  
(2801109)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=63ffbd1a-79a9-47c8-a904-b6e9a0fb626f)  
(2820917)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=0722d681-eda8-48af-b079-36d45eb20f98)  
(2808735)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=7149ecda-78d3-4289-81b2-5133cd9b4564)  
(2817183)  
(Mittel)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=f22de9fa-96e0-4a09-8923-8731e0de38c9)  
(2817183)  
(Mittel)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=08c55acd-4c5e-4d5e-b524-19fd449e5c50)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=7efb8816-ca23-4a75-a0cc-53a663eac3a9)  
(2813345)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=b7af0c30-0d09-434a-85d6-69e7e9ee9e29)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=1b009894-8503-42b6-85d1-1285ed14bef9)  
(2772930)  
(Hoch)  
[Active Directory Application Mode (ADAM)](http://www.microsoft.com/downloads/details.aspx?familyid=30c0c8d8-df70-4637-bea4-96e2e4d2cb28)  
(2801109)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=bf96696e-13a4-4b01-a8d9-60654d7d1ac5)  
(2820917)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=fc5f39a7-e89b-4ef0-887c-873ad546fb65)  
(2808735)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 6](http://www.microsoft.com/downloads/details.aspx?familyid=b10b94db-b281-46b6-b301-58f14de327d2)  
(2817183)  
(Mittel)  
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=9d799925-5f8e-43c8-8674-19437a7a6c99)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=54e286a0-22f5-4b34-a246-c98c0647f093)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory](http://www.microsoft.com/downloads/details.aspx?familyid=0b65be9e-724d-469d-ba3b-93d8b174aecb)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=c56d776a-4293-4d3c-bcac-cd5f50eeb328)  
(2820917)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=dd159949-e0f0-4515-876d-837758a3fd51)  
(2808735)  
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
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=5591feef-5bc6-4e3e-9bbb-cd2205757340)  
(2817183)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=e244c3f1-3c4e-4648-b1f9-e216b0009f1e)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=190a78a5-e557-44f3-b214-7d3c904f7bd8)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=20500712-2c0f-41e2-95a8-db1a5dcf717a)  
(2813345)  
(Kritisch)  
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=1bf2935a-2fa4-4a26-bccf-fe0b63a16b37)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=7f1aa4bd-a14e-4797-b542-4220e3d9d0d7)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=e1b1a3b4-7aae-4934-96cc-990cd1ce962d)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=10664eeb-f759-4a0e-b1df-c463aae43902)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3881a7f9-a5f1-4a28-b652-7b7f20c05259)  
(2808735)  
(Hoch)  
[Windows Vista Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=55d753f3-b912-401c-bca6-61c212ffa0df)  
(2840149)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=1bcd238f-2758-49f7-a347-7ec998637d5c)  
(2817183)  
(Kritisch)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=c35f53d6-eceb-4966-9487-2dfc2652c775)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=6cfdb0d5-9c47-405f-bc60-0e4dd3eaff12)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=4c6f006c-fcb8-499f-bd91-9c8acb3ec3c3)  
(2813345)  
(Kritisch)  
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=201eb194-e7c9-479c-bb03-646b22f2bbd1)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=d6b3ef0e-16e3-42cb-bffe-4b046f995771)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=ca2182ae-cd47-48d7-9bb0-4aeda4ee26cc)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=c12ce8b7-e8e2-47ac-bdaa-874dff5a6115)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e5ba88a4-e0ec-45d7-8c0a-611521351890)  
(2808735)  
(Hoch)  
[Windows Vista x64 Edition Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=89f1556f-442f-4888-b21a-ffbedaa8792e)  
(2840149)  
(Mittel)
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
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=09bd431a-e94f-4fc5-bea9-569ebc17b0f3)  
(2817183)  
(Mittel)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=76f96697-0f07-49ad-9169-47cfe2f6a362)  
(2817183)  
(Mittel)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=2d8c4080-ff7a-42ef-95f4-36b642c0a089)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=92bd1819-46f9-4a9b-bf2b-ea6aaaee9890)  
(2813345)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=527ea8cd-88db-448a-b8e4-0fdf87fa369c)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=dd955bf1-e51f-4738-82bf-759e9dea0895)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31561241-07c8-4396-ad80-9c62a2394658)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e598863e-7ca1-42a6-9cb4-3f3a10f0ce71)  
(2808735)  
(Hoch)  
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a4bdfe68-4de2-41fa-a593-2e07de105081)  
(2840149)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=e46e002e-40b2-4bb3-89ad-63d320273ffa)  
(2817183)  
(Mittel)  
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=b93153dc-f83a-4891-8230-765e3472614d)  
(2817183)  
(Mittel)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=08abb2ce-0a07-4f25-b9ad-5ec87c07f0bf)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=6518cdc6-10a6-46ed-a2f6-6f58216fe319)  
(2813345)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=604709f7-8712-4162-ab86-5988b19084f9)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=38d1cd8c-977b-47be-b703-a326a1b4f445)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46ef3ace-30b2-4099-aa9d-142de82b0257)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a9dd92b5-4137-47d1-85a3-506f1eaacee0)  
(2808735)  
(Hoch)  
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1c36a50c-023d-420d-830a-d4cb2eda6ef2)  
(2840149)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
[Internet Explorer 7](http://www.microsoft.com/downloads/details.aspx?familyid=b0d20b3f-f6cb-4cbc-9af1-1d33b4a6dfb2)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 6.1](http://www.microsoft.com/downloads/details.aspx?familyid=4807c3fe-bc54-4db6-a9b0-ee21bdd9820f)  
(2813345)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=6133c84a-b2ce-4a2e-8afc-7386caf80cc8)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=94971d7b-df42-4566-97eb-0a7572b0e2da)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=3e9ccb95-284a-478e-b521-f3a0acbae8da)  
(2808735)  
(Hoch)  
[Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=738b2263-e1eb-4ada-a7f0-5165f42bc5c9)  
(2840149)  
(Mittel)
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
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ec9c221a-065b-4f5c-95b6-9b650c24cffa)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=041fd330-0998-44b5-bedd-d3e47965370d)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=d7623f17-783d-431a-8274-17d71df72202)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=90d2c454-c31c-4ac4-ab94-b341d1244ee6)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=37b3e861-35fb-471b-b81a-a8b58bd26647)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=1abeaf49-c458-4046-a001-8aee0ba35b3a)  
(2808735)  
(Hoch)  
[Windows 7 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=808ac8c6-394d-406b-b34e-07d03c760c27)  
(2840149)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=ec9c221a-065b-4f5c-95b6-9b650c24cffa)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=041fd330-0998-44b5-bedd-d3e47965370d)  
(2817183)  
(Kritisch)  
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=cf49622e-8494-4082-a9aa-a6699711d827)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.1](http://www.microsoft.com/downloads/details.aspx?familyid=d7623f17-783d-431a-8274-17d71df72202)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=90d2c454-c31c-4ac4-ab94-b341d1244ee6)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=37b3e861-35fb-471b-b81a-a8b58bd26647)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für 32-Bit-Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1abeaf49-c458-4046-a001-8aee0ba35b3a)  
(2808735)  
(Hoch)  
[Windows 7 für 32-Bit-Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=808ac8c6-394d-406b-b34e-07d03c760c27)  
(2840149)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=01f4b588-38e3-43a7-ae5c-674b9c03fc42)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=ac93c656-2c9c-4378-9ae3-a60636b8ce6f)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=5595efaa-3d57-4c9a-8b53-7cfa06093f1e)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=ebc1ea79-158f-4c81-ab49-3d3fca870363)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=94d19c2a-2457-4fa7-ade6-ad37d0e7f56a)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=84275cfd-f5a3-4830-895d-beaf162cdc27)  
(2808735)  
(Hoch)  
[Windows 7 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=737a0cd0-eee6-4095-b9b1-2822024dd825)  
(2840149)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=01f4b588-38e3-43a7-ae5c-674b9c03fc42)  
(2817183)  
(Kritisch)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=ac93c656-2c9c-4378-9ae3-a60636b8ce6f)  
(2817183)  
(Kritisch)  
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=775536fa-a8a2-4733-a0f0-08e742be1122)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.1](http://www.microsoft.com/downloads/details.aspx?familyid=5595efaa-3d57-4c9a-8b53-7cfa06093f1e)  
(2813347)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ebc1ea79-158f-4c81-ab49-3d3fca870363)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=94d19c2a-2457-4fa7-ade6-ad37d0e7f56a)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 7 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=84275cfd-f5a3-4830-895d-beaf162cdc27)  
(2808735)  
(Hoch)  
[Windows 7 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=737a0cd0-eee6-4095-b9b1-2822024dd825)  
(2840149)  
(Mittel)
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
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung** **des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d8ffa592-6336-494d-bcd0-535ea2821525)  
(2817183)  
(Mittel)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7f68500e-6699-4341-b129-2dbd5bc508ac)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=79c870b9-b800-4f59-a5ea-19a5c890af52)  
(2813347)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd2e3d-1b37-4173-9955-e6fceb7bcd45)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=78d11246-06b0-4a22-a2b0-c772aa60e726)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=cbaac7fb-b673-4cf5-8c6f-57bedcb5285d)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=3e96483f-ec2d-4335-8c50-8686eed06018)  
(2840149)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=d8ffa592-6336-494d-bcd0-535ea2821525)  
(2817183)  
(Mittel)  
[Internet Explorer 9](http://www.microsoft.com/downloads/details.aspx?familyid=7f68500e-6699-4341-b129-2dbd5bc508ac)  
(2817183)  
(Mittel)  
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=752ffe45-b251-4cdf-9848-4d15f75d4452)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.1](http://www.microsoft.com/downloads/details.aspx?familyid=79c870b9-b800-4f59-a5ea-19a5c890af52)  
(2813347)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd2e3d-1b37-4173-9955-e6fceb7bcd45)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=78d11246-06b0-4a22-a2b0-c772aa60e726)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cbaac7fb-b673-4cf5-8c6f-57bedcb5285d)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e96483f-ec2d-4335-8c50-8686eed06018)  
(2840149)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2dec754b-4d51-4792-bee6-67e94a1a8157)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.0](http://www.microsoft.com/downloads/details.aspx?familyid=c7047403-8c2a-42de-bea5-d7354847730a)  
(2813347)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=5cfc2f18-4cde-4e21-8604-f694d69da535)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=6c577423-cd17-4317-98a3-5f6e767513c0)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für Itanium-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=3f1abf13-14c3-4a92-b4c1-4caa40e29e7b)  
(2840149)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
[Internet Explorer 8](http://www.microsoft.com/downloads/details.aspx?familyid=2dec754b-4d51-4792-bee6-67e94a1a8157)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Remotedesktopverbindungs-Client 7.1](http://www.microsoft.com/downloads/details.aspx?familyid=c7047403-8c2a-42de-bea5-d7354847730a)  
(2813347)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=5cfc2f18-4cde-4e21-8604-f694d69da535)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=6c577423-cd17-4317-98a3-5f6e767513c0)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3f1abf13-14c3-4a92-b4c1-4caa40e29e7b)  
(2840149)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="7" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Niedrig**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=159c43ec-beaf-4ac3-8c3a-06a9716ac9ae)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=02d6d10e-3708-4424-8618-88414694c973)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=c7a7ba4d-1fe1-40ed-81f2-6fbb6dde2cf6)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 32-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=882f2d67-b8e0-4859-871b-6a7cef27e3e5)  
(2808735)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=3309f621-4087-4688-b991-c2ef54532cb6)  
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=18992e76-70f3-43a2-b47f-199c9728c7ca)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=bafaac33-2bef-4a5e-9451-23ca69c0a132)  
(2772930)  
(Niedrig)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows 8 für 64-Bit-Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=852dac0f-75fe-443f-9b3d-1dbcac166b3d)  
(2808735)  
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
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2012
</td>
<td style="border:1px solid black;">
[Internet Explorer 10](http://www.microsoft.com/downloads/details.aspx?familyid=5015e763-6fb8-4737-9305-2e5850ef853d)  
(2817183)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2012](http://www.microsoft.com/downloads/details.aspx?familyid=ef106525-c42b-4b25-83bf-e290e2bcad5a)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Services](http://www.microsoft.com/downloads/details.aspx?familyid=209e3d5f-9333-469e-8b2c-212dc4ec764a)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2012](http://www.microsoft.com/downloads/details.aspx?familyid=fbf53f06-1ee2-49c4-a5a8-3b1e9823b1b9)  
(2808735)  
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
**Kennung des** **Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Kritisch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows RT
</td>
<td style="border:1px solid black;">
Internet Explorer 10<sup>[1]</sup>
(2817183)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT<sup>[1]</sup>
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT<sup>[1]</sup>
(2808735)  
(Hoch)
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
[**MS13-028**](http://go.microsoft.com/fwlink/?linkid=285215)
</td>
<td style="border:1px solid black;">
[**MS13-029**](http://go.microsoft.com/fwlink/?linkid=286679)
</td>
<td style="border:1px solid black;">
[**MS13-031**](https://technet.microsoft.com/de-de/security/bulletin/ms13-031)
</td>
<td style="border:1px solid black;">
[**MS13-032**](http://go.microsoft.com/fwlink/?linkid=280660)
</td>
<td style="border:1px solid black;">
[**MS13-033**](http://go.microsoft.com/fwlink/?linkid=286700)
</td>
<td style="border:1px solid black;">
[**MS13-036**](http://go.microsoft.com/fwlink/?linkid=281927)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
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
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=527ea8cd-88db-448a-b8e4-0fdf87fa369c) (Server Core-Installation)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=dd955bf1-e51f-4738-82bf-759e9dea0895)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=31561241-07c8-4396-ad80-9c62a2394658) (Server Core-Installation)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=e598863e-7ca1-42a6-9cb4-3f3a10f0ce71) (Server Core-Installation)  
(2808735)  
(Hoch)  
[Windows Server 2008 für 32-Bit-Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a4bdfe68-4de2-41fa-a593-2e07de105081) (Server Core-Installation)  
(2840149)  
(Mittel)
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
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=604709f7-8712-4162-ab86-5988b19084f9) (Server Core-Installation)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=38d1cd8c-977b-47be-b703-a326a1b4f445)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=46ef3ace-30b2-4099-aa9d-142de82b0257) (Server Core-Installation)  
(2820917)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=a9dd92b5-4137-47d1-85a3-506f1eaacee0) (Server Core-Installation)  
(2808735)  
(Hoch)  
[Windows Server 2008 für x64-basierte Systeme Service Pack 2](http://www.microsoft.com/downloads/details.aspx?familyid=1c36a50c-023d-420d-830a-d4cb2eda6ef2) (Server Core-Installation)  
(2840149)  
(Mittel)
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
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd2e3d-1b37-4173-9955-e6fceb7bcd45) (Server Core-Installation)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=78d11246-06b0-4a22-a2b0-c772aa60e726)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=cbaac7fb-b673-4cf5-8c6f-57bedcb5285d) (Server Core-Installation)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für x64-basierte Systeme](http://www.microsoft.com/downloads/details.aspx?familyid=3e96483f-ec2d-4335-8c50-8686eed06018) (Server Core-Installation)  
(2840149)  
(Mittel)
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
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=dbbd2e3d-1b37-4173-9955-e6fceb7bcd45) (Server Core-Installation)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory-Dienste und Active Directory Lightweight Directory Service (AD LDS)](http://www.microsoft.com/downloads/details.aspx?familyid=78d11246-06b0-4a22-a2b0-c772aa60e726)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=cbaac7fb-b673-4cf5-8c6f-57bedcb5285d) (Server Core-Installation)  
(2808735)  
(Hoch)  
[Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=3e96483f-ec2d-4335-8c50-8686eed06018) (Server Core-Installation)  
(2840149)  
(Mittel)
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
[Windows Server 2012](http://www.microsoft.com/downloads/details.aspx?familyid=ef106525-c42b-4b25-83bf-e290e2bcad5a) (Server Core-Installation)  
(2813170)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Active Directory Services](http://www.microsoft.com/downloads/details.aspx?familyid=209e3d5f-9333-469e-8b2c-212dc4ec764a)  
(2772930)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2012](http://www.microsoft.com/downloads/details.aspx?familyid=fbf53f06-1ee2-49c4-a5a8-3b1e9823b1b9) (Server Core-Installation)  
(2808735)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-028, MS13-031,** **und MS13-036**

<sup>[1]</sup>Sicherheitsupdates für Windows RT werden über [Windows Update](http://update.microsoft.com/windowsupdate/) bereitgestellt.

#### Microsoft Office Suites und Software

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-035**](http://go.microsoft.com/fwlink/?linkid=285672)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft InfoPath 2010 Service Pack 1 (32-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 Service Pack 1 (32-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?familyid=63f6a338-a195-4923-908e-8c21713c7373)  
(2687422)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
[Microsoft InfoPath 2010 Service Pack 1 (32-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?familyid=f1cd73d2-411b-4a58-b8c0-04fd58922dae)  
(2760406)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft InfoPath 2010 Service Pack 1 (64-Bit-Editionen)
</td>
<td style="border:1px solid black;">
[Microsoft InfoPath 2010 Service Pack 1 (64-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?familyid=ae2069d0-55b5-4dfe-9131-41888d6bbec3)  
(2687422)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
[Microsoft InfoPath 2010 Service Pack 1 (64-Bit-Editionen)](http://www.microsoft.com/downloads/details.aspx?familyid=f206071a-4502-432a-9e5b-50bb4e3f1757)  
(2760406)  
(Keine Bewertung des Schweregrads)<sup>[1]</sup>
</td>
</tr>
</table>
 
**Hinweise** **für MS13-035**

<sup>[1]</sup>In diesem Update gibt es für die angegebene Software keine Bewertung des Schweregrads, da die bekannten Angriffsmethoden für die Sicherheitsanfälligkeit blockiert sind.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

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
[**MS13-030**](http://go.microsoft.com/fwlink/?linkid=286577)
</td>
<td style="border:1px solid black;">
[**MS13-035**](http://go.microsoft.com/fwlink/?linkid=285672)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft SharePoint Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2010 Service Pack 1 (wosrv)](http://www.microsoft.com/downloads/details.aspx?familyid=6c7d007f-5c8d-464c-af04-4e7800a2e2a6)<sup>[1]</sup>
(2687421)  
(Hoch)  
[Microsoft SharePoint Server 2010 Service Pack 1 (coreserver)](http://www.microsoft.com/downloads/details.aspx?familyid=c59c0d25-8d6c-4dda-a06b-e42891a9ddae)<sup>[1]</sup>
(2760408)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Server 2013
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Server 2013 (coreserverloc)](http://www.microsoft.com/downloads/details.aspx?familyid=2e5b1e49-0355-4111-a464-224bb2192029)<sup>[1]</sup>
(2737969)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft Groove Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-030**](http://go.microsoft.com/fwlink/?linkid=286577)
</td>
<td style="border:1px solid black;">
[**MS13-035**](http://go.microsoft.com/fwlink/?linkid=285672)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Groove Server 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Groove Server 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=d63ee461-b823-4eb1-9e6d-82f380627fb5)  
(2687424)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="3" style="border:1px solid black;">
Microsoft SharePoint Foundation
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-030**](http://go.microsoft.com/fwlink/?linkid=286577)
</td>
<td style="border:1px solid black;">
[**MS13-035**](http://go.microsoft.com/fwlink/?linkid=285672)
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
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft SharePoint Foundation 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft SharePoint Foundation 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=ac805c46-8661-4e99-84da-c395dc05beb0)  
(2810059)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-030**

<sup>[1]</sup>Dieses Update erfordert die vorherige Installation des kumulativen Updates für Project Server 2013 (2768001). Weitere Informationen zu dem Update und Downloadadressen finden Sie im [Microsoft Knowledge Base-Artikel 2768001](http://support.microsoft.com/kb/2768001).

**Hinweise** **für MS13-035**

<sup>[1]</sup>Bei unterstützten Editionen von Microsoft SharePoint Server 2010 müssen Endbenutzer zusätzlich zu den Sicherheitsupdatepaketen für Microsoft SharePoint 2010 (2687421 und 2760408) auch das Sicherheitsupdate für Microsoft SharePoint Foundation 2010 (2810059) installieren, um vor den Sicherheitsanfälligkeiten geschützt zu sein, die in diesem Bulletin beschrieben werden.

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Office Web Apps

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Microsoft Office Software
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-035**](http://go.microsoft.com/fwlink/?linkid=285672)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office Web Apps 2010 Service Pack 1
</td>
<td style="border:1px solid black;">
[Microsoft Office Web Apps 2010 Service Pack 1](http://www.microsoft.com/downloads/details.aspx?familyid=1d35b235-305a-45c8-a395-7658792d177e)  
(2760777)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis** **für MS13-035**

Weitere Updatedateien finden Sie außerdem unter anderen Softwarekategorien im Abschnitt **Betroffene Software und Downloadadressen** unter der gleichen Kennung des Bulletins. Dieses Bulletin umfasst mehr als eine Softwarekategorie.

#### Microsoft Sicherheitssoftware

<p> </p>
<table style="border:1px solid black;">
<tr>
<th colspan="2" style="border:1px solid black;">
Antimalware
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-034**](http://go.microsoft.com/fwlink/?linkid=276805)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](http://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Defender für Windows 8 und Windows RT
</td>
<td style="border:1px solid black;">
Windows Defender für Windows 8 und Windows RT<sup>[1]</sup>
(2781197)  
(Hoch)
</td>
</tr>
</table>
 
**Hinweis für MS13-034**

<sup>[1]</sup>Das Update ist über [Windows-Update](http://update.microsoft.com/windowsupdate/) verfügbar.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](http://technet.microsoft.com/de-de/updatemanagement/bb245732). Im [TechNet Sicherheitscenter](http://technet.microsoft.com/de-de/security/default.aspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Endbenutzer können das [Microsoft-Sicherheitscenter](http://www.microsoft.com/de-de/security/default.aspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind unter [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) und [Windows Update](http://update.microsoft.com/windowsupdate/) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. und können am einfachsten durch eine Suche nach dem Begriff „Sicherheitsupdate“ ermittelt werden.

Benutzern von Microsoft Office für Mac kann Microsoft AutoUpdate für Mac helfen, Ihre Microsoft-Software auf dem neuesten Stand zu halten. Weitere Informationen zur Verwendung von Microsoft AutoUpdate für Mac finden Sie unter [Automatisch nach Softwareupdates suchen](http://mac2.microsoft.com/help/office/14/de-de/word/item/ffe35357-8f25-4df8-a0a3-c258526c64ea).

Außerdem können Sicherheitsupdates vom [Microsoft Update-Katalog](http://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS13-001“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](http://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung:**

Microsoft stellt Anleitungen zur Erkennung und Bereitstellung von Sicherheitsupdates bereit. Diese Anleitungen enthalten Empfehlungen und Informationen, anhand derer IT-Experten verstehen können, wie die verschiedenen Tools für die Erkennung und Bereitstellung der Sicherheitsupdates verwendet werden. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 961747](http://support.microsoft.com/kb/961747/de).

**Microsoft Baseline Security Analyzer**

Der Microsoft Baseline Security Analyzer (MBSA) ermöglicht Administratoren die Überprüfung von lokalen und Remotesystemen im Hinblick auf fehlende Sicherheitsupdates sowie auf häufig falsch konfigurierte Sicherheitsparameter. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](http://technet.microsoft.com/de-de/security/cc184924.aspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS) können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Microsoft Windows 2000 und neuere Betriebssysteme, Office XP und höher, Exchange Server 2003 und SQL Server 2000 bis Microsoft Windows 2000 und neuere Betriebssysteme schnell und sicher bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](http://technet.microsoft.com/de-de/windowsserver/bb332157.aspx).

**SystemCenter Configuration Manager**

System Center Configuration Manager-Softwareupdateverwaltung vereinfacht die komplizierte Aufgabe des Bereitstellens und Verwaltens von Updates auf IT-Systemen im gesamten Unternehmen. Mit System Center Configuration Manager können IT-Administratoren Updates von Microsoft-Produkten auf verschiedenen Geräten bereitstellen, einschließlich Desktops, Laptops, Servern und mobilen Geräten.

Die automatisierte Bewertung der Sicherheitsanfälligkeiten in System Center Configuration Manager erkennt den Bedarf an Updates und berichtet über empfohlene Aktionen. Die Softwareupdateverwaltung in System Center Configuration Manager ist auf Microsoft Windows Software Update Services (WSUS) aufgebaut, eine lange erprobte Updateinfrastruktur, die IT-Administratoren weltweit vertraut ist. Weitere Informationen zu System Center Configuration Manager finden Sie auf der Website [System Center Technical Resources](http://technet.microsoft.com/de-de/systemcenter/bb980621).

**Systems Management Server 2003**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen.

**Hinweis:** System Management Server 2003 wurde am 12. Januar 2010 aus dem grundlegenden Support genommen. Weitere Informationen zu Produktlebenszyklen finden Sie auf der Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de). Die nächste Version von SMS, System Center Configuration Manager, ist jetzt verfügbar (siehe den früheren Abschnitt, **System Center Configuration Manager**).

Weitere Informationen dazu, wie Administratoren mithilfe von SMS 2003 Sicherheitsupdates bereitstellen können, finden Sie in [Szenarien und Vorgehensweisen für Microsoft Systems Management Server 2003: Softwareverteilung und Patchverwaltung](http://www.microsoft.com/downloads/details.aspx?familyid=32f2bb4c-42f8-4b8d-844f-2553fd78049f). Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server TechCenter](http://technet.microsoft.com/de-de/systemcenter/bb545936).

**Hinweis:** SMS verwendet den Microsoft Baseline Security Analyzer für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](http://technet.microsoft.com/en-us/library/cc917507.aspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können diese Updates mit dem Elevated Rights Deployment Tool (im [SMS 2003 Administration Feature Pack](http://www.microsoft.com/de-de/download/details.aspx?id=1846) verfügbar) installieren.

**Updatekompatibilitätsbewertung und Anwendungskompatibilitäts-Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](http://technet.microsoft.com/de-de/library/cc749197), die im [Anwendungskompatibilitäts-Toolkit](http://www.microsoft.com/downloads/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen schädlicher Software

Für die Veröffentlichung des Bulletins, die am zweiten Dienstag jedes Monats stattfindet, hat Microsoft eine aktualisierte Version des Microsofts Windows-Tool zum Entfernen schädlicher Software in Windows Update, Microsoft Update, den Windows Server Update Services und dem Download Center veröffentlicht. Für außerplanmäßige Veröffentlichungen des Security Bulletins ist keine aktualisierte Version des Microsoft Windows-Tool zum Entfernen schädlicher Software erhältlich.

#### Nicht sicherheitsrelevante Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](http://support.microsoft.com/kb/894199/de): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Updates für Windows Server Update Services aus den vergangenen Monaten](http://technet.microsoft.com/de-de/windowsserver/bb332157.aspx). Zeigt alle neuen, überarbeiteten und veröffentlichten Updates für andere Microsoft-Produkte als Microsoft Windows an.

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](http://go.microsoft.com/fwlink/?linkid=215201) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](http://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](http://www.microsoft.com/de-de/download/search.aspx?q=security%20update) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](http://go.microsoft.com/fwlink/?linkid=40747&displaylang=de) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](http://support.microsoft.com/kb/913086/de).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](http://technet.microsoft.com/de-de/security/cc136632.aspx) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](http://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

**MS13-028**

-   Ivan Fratric und Ben Hawkes vom [Google Security Team](http://www.google.com/) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer (CVE-2013-1303).
-   Ivan Fratric und Ben Hawkes vom [Google Security Team](http://www.google.com/) für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer (CVE-2013-1304).
-   Einer Person, die mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [HP](http://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Use-after-free-Sicherheitsanfälligkeit in Internet Explorer (CVE-2013-1338).
-   Einer Person, die anonym bleiben möchte, für die Zusammenarbeit mit uns an in diesem Bulletin enthaltenen Tiefenverteidigungsänderungen.

**MS13-029**

-   c1d2d9acc746ae45eeb477b97fa74688, in Zusammenarbeit mit der [Zero Day Initiative](http://www.zerodayinitiative.com/) von [HP](http://www.hpenterprisesecurity.com/products), für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Remotecodeausführung im ActiveX-Steuerelement RDP (CVE-2013-1296).

**MS13-031**

-   [Gynvael Coldwind](http://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Racebedingung im Kernel (CVE-2013-1284).
-   [Gynvael Coldwind](http://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Racebedingung im Kernel (CVE-2013-1294).

**MS13-033**

-   George Georgiev Valkov für den Hinweis auf die Sicherheitsanfälligkeit in CSRSS bezüglich Speicherbeschädigung (CVE-2013-1295).

**MS13-034**

-   Bruce Monroe von [Intel](http://www.intel.com/) für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Antimalware durch fehlerhaften Pfadnamen (CVE-2013-0078).
-   Shai Sarfaty für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Antimalware durch fehlerhaften Pfadnamen (CVE-2013-0078).
-   Tony Robotham von Centrica für den Hinweis auf die Sicherheitsanfälligkeit in Microsoft Antimalware durch fehlerhaften Pfadnamen (CVE-2013-0078).

**MS13-035**

-   Drew Hintz und Andrew Lyons vom [Google Security Team](http://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich HTML-Bereinigung (CVE-2013-1289).

**MS13-036**

-   [Gynvael Coldwind](http://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Racebedingung in Win32k (CVE-2013-1283).
-   Wang Yu vom [Qihoo 360 Security Center](http://www.360.cn/) für den Hinweis auf die Sicherheitsanfälligkeit beim Analysieren von Win32k-Schriftarten (CVE-2013-1291).
-   [Gynvael Coldwind](http://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit durch Racebedingung in Win32k (CVE-2013-1292).
-   [Gynvael Coldwind](http://gynvael.coldwind.pl/) und [Mateusz “j00 ru“ Jurczyk](http://j00ru.vexillium.org/) von [Google Inc](http://www.google.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in NTFS durch NULL-Zeigerdereferenzierung (CVE-2013-1293).

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](http://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](http://technet.microsoft.com/de-de/security/bb980617)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](http://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](http://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (9. April 2013): Bulletin Summary veröffentlicht.
-   V1.1 (10. April 2013): Für MS13-029 wurde die Versionsnummer für Remotedesktopverbindungs-Client unter Windows 7 Service Pack 1 und Windows Server 2008 R2 Service Pack 1 von 7.0 in 7.1 korrigiert. Dies ist lediglich eine Informationsänderung. Die Dateien des Sicherheitsupdates wurden nicht verändert.
-   V2.0 (11. April 2013): In MS13-036 wurden die Verknüpfungen zum Sicherheitsupdate 2823324 aufgrund eines bekannten Installationsproblems entfernt. Weitere Informationen finden Sie im Bulletin.
-   V3.0 (23. April 2013): In MS13-036 wurde das Update 2823324 durch das Update 2840149 NTFS.sys ersetzt, wenn es unter einer unterstützen Edition von Windows Vista, Windows Server 2008, Windows 7 oder Windows Server 2008 R2 installiert wird. Weitere Informationen finden Sie im Bulletin.
-   V3.1 (24. April 2013): In MS13-028 wurde dem **Ausnutzbarkeitsindex** für CVE-2013-1338 eine Bewertung der Ausnutzbarkeit hinzugefügt. Dies ist lediglich eine Informationsänderung.
-   V4.0 (25. Juni 2013): In MS13-029 wurde das Bulletin überarbeitet, um das Update 2813347 für den Remotedesktopverbindungs-Client 7.0 unter Windows XP Service Pack 3 erneut zu veröffentlichen. Weitere Informationen finden Sie im Bulletin.

*Built at 2014-04-18T01:50:00Z-07:00*