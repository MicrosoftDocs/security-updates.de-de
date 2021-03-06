---
TOCTitle: 'MS13-AUG'
Title: Microsoft Security Bulletin Summary für August 2013
ms:assetid: 'ms13-aug'
ms:contentKeyID: 61225116
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms13-aug(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für August 2013
===================================================

Veröffentlicht: Dienstag, 13. August 2013 | Aktualisiert: Dienstag, 27. August 2013

**Version:** 3.0

In diesem Bulletin Summary sind die im August 2013 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Security Bulletins für August 2013 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 8. August 2013 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://go.microsoft.com/fwlink/?linkid=217213).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://technet.microsoft.com/de-de/security/dd252948.aspx).

Am Mittwoch, dem 14. August 2013, um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im August.](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032557295&culture=en-us) Ab diesem Datum steht dieser Webcast [auf Anfrage](https://msevents.microsoft.com/cui/eventdetail.aspx?eventid=1032557295&culture=en-us) zur Verfügung.

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (2862772)</strong> <strong><br />
<br />
</strong>Dieses Sicherheitsupdate behebt elf vertraulich gemeldete Sicherheitsanfälligkeiten in Internet Explorer. Die schwerwiegendsten Sicherheitsanfälligkeiten können Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Ein Angreifer, der die schwerwiegendste dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann die gleichen Benutzerrechte erlangen wie der aktuelle Benutzer. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows,<br />
Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314044">MS13-060</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit im Unicode-Schriftprozessor kann Remotecodeausführung ermöglichen (2850869)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in dem in Microsoft Windows enthaltenen Unicode-Schriftprozessor. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer ein speziell gestaltetes Dokument bzw. eine speziell gestaltete Webseite mit einer Anwendung anzeigt, die eingebettete OpenType-Schriftarten unterstützt. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der aktuelle Benutzer erlangen. Für Endbenutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=317381">MS13-061</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Exchange können Remotecodeausführung ermöglichen</strong> <strong>(2876063)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt drei öffentlich gemeldete Sicherheitsanfälligkeiten in Microsoft Exchange Server. Die Sicherheitsanfälligkeiten liegen in den Funktionen „WebReady Document Viewing“ und „Schutz vor Datenverlust“ des Microsoft Exchange Servers vor. Die Sicherheitsanfälligkeiten können Remotecodeausführung im Sicherheitskontext des Transcodierungsdienstes auf dem Exchange-Server ermöglichen, wenn ein Benutzer mithilfe von Outlook Web App (OWA) eine Vorschau einer speziell gestalteten Datei anzeigt. Der Transcodierungsdienst in Exchange, der für WebReady Dokument Viewing verwendet wird, verwendet die Anmeldeinformationen des LocalService-Kontos. Die Funktion „Schutz vor Datenverlust“ stellt Code bereit, der Remotecodeausführung im Sicherheitskontext des Dienstes „Filtering Management“ ermöglichen kann, wenn Exchange Server eine speziell gestaltete Nachricht erhält. Der Dienst „Filtering Management“ in Exchange verwendet die Anmeldeinformationen des LocalService-Kontos. Das LocalService-Konto verfügt auf dem lokalen System über Mindestberechtigungen und präsentiert im Netzwerk anonyme Anmeldeinformationen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Server Software</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309337">MS13-062</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Remoteprozeduraufruf kann Erhöhung von Berechtigungen ermöglichen (2849470)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann die Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer eine speziell gestaltete RPC-Anforderung sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309338">MS13-063</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (2859537)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und drei vertraulich gemeldete Sicherheitsanfälligkeiten in Microsoft Windows. Die schwerwiegendsten Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn sich ein Angreifer lokal anmeldet und eine speziell gestaltete Anwendung ausführt. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314043">MS13-064</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Windows-NAT-Treiber kann Denial of Service ermöglichen (2849568)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit im Windows-NAT-Treiber in Microsoft Windows. Die Sicherheitsanfälligkeit kann Denial-of-Service ermöglichen, wenn ein Angreifer ein speziell gestaltetes ICMP-Paket an einen Zielserver sendet, auf dem der Windows-NAT-Treiber ausgeführt wird.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314047">MS13-065</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in ICMPv6 kann zu einem Denial-of-Service führen (2868623)<br />
<br />
</strong>Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Windows. Die Sicherheitsanfälligkeit kann einen Denial-of-Service ermöglichen, wenn der Angreifer ein speziell gestaltetes ICMP-Paket an das Zielsystem sendet.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
DoS (Denial of Service)</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309325">MS13-066</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Active Directory-Verbunddiensten kann Offenlegung von Information ermöglichen (2873872)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den Active Directory-Verbunddiensten. Mit der Sicherheitsanfälligkeit können Informationen offengelegt werden, die zu dem Dienstkonto gehören, das von den Active Directory-Verbunddiensten verwendet wird. Ein Angreifer kann dann versuchen, sich von außerhalb des Unternehmensnetzwerks anzumelden. was zu einer Sperrung des von ADFS verwendeten Dienstkontos führt, falls eine Kontosperrungsrichtlinie konfiguriert wurde. Dies wiederum führt zu einem Denial-of-Service für alle Anwendungen, die sich auf die ADFS-Instanz stützen.</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/gg309177.aspx">Hoch</a><br />
Offenlegung von Informationen</td>
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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3184">CVE-2013-3184</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3187">CVE-2013-3187</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3188">CVE-2013-3188</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3189">CVE-2013-3189</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3190">CVE-2013-3190</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3191">CVE-2013-3191</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3193">CVE-2013-3193</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3194">CVE-2013-3194</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=313330">MS13-059</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3199">CVE-2013-3199</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314044">MS13-060</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Uniscribe-Schriftartenanalysemodul bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3781">CVE-2013-3181</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=317381">MS13-061</a></td>
<td style="border:1px solid black;">Oracle Outside In enthält mehrere ausnutzbare Sicherheitsanfälligkeiten</td>
<td style="border:1px solid black;">Mehrere*</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">2</a> – Angreifercode wäre schwer zu erstellen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">*Mehrere Sicherheitsanfälligkeiten; weitere Informationen finden Sie im Bulletin MS13-061.<br />
<br />
Diese Sicherheitsanfälligkeiten wurden veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309337">MS13-062</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Remoteprozeduraufruf</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3175">CVE-2013-3175</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309338">MS13-063</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ASLR durch Umgehung der Sicherheitsfunktion</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-2556">CVE-2013-2556</a></td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Nicht anwendbar</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit aufgrund der Umgehung von Sicherheitsfunktionen.<br />
<br />
Diese Sicherheitsanfälligkeit wurde veröffentlicht.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309338">MS13-063</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3196">CVE-2013-3196</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309338">MS13-063</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3197">CVE-2013-3197</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309338">MS13-063</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3198">CVE-2013-3198</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">1</a> – Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314043">MS13-064</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Windows NAT bezüglich Denial-of-Service</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3182">CVE-2013-3182</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Nicht betroffen</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=314047">MS13-065</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ICMPv6</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3183">CVE-2013-3183</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dauerhaft</td>
<td style="border:1px solid black;">Es handelt sich bei dieser Sicherheitsanfälligkeit um einen Denial-of-Service-Angriff.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=309325">MS13-066</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in ADFS durch Offenlegung von Informationen</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2013-3185">CVE-2013-3185</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/de-de/security/cc998259">3</a> – Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Vorläufig</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit, die sich auf die Offenlegung von Informationen bezieht.</td>
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
<th colspan="8" style="border:1px solid black;">
Windows XP  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
(2862772)  
(Kritisch)  
Internet Explorer 7  
(2862772)  
(Kritisch)  
Internet Explorer 8  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2850869)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows XP Service Pack 3  
(2859537)  
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
Internet Explorer 6  
(2862772)  
(Kritisch)  
Internet Explorer 7  
(2862772)  
(Kritisch)  
Internet Explorer 8  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2850869)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2  
(2849470)  
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
<th colspan="8" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
(2862772)  
(Mittel)  
Internet Explorer 7  
(2862772)  
(Mittel)  
Internet Explorer 8  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2850869)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 1.x  
(nur Windows Server 2003 R2 Service Pack 2)  
(2868846)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2862772)  
(Mittel)  
Internet Explorer 7  
(2862772)  
(Mittel)  
Internet Explorer 8  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2850869)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2  
(2849470)  
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
Active Directory-Verbunddienste 1.x  
(nur Windows Server 2003 R2 x64 Edition Service Pack 2)  
(2868846)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 6  
(2862772)  
(Mittel)  
Internet Explorer 7  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2850869)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme  
(2849470)  
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
<th colspan="8" style="border:1px solid black;">
Windows Vista
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2862772)  
(Kritisch)  
Internet Explorer 8  
(2862772)  
(Kritisch)  
Internet Explorer 9  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista Service Pack 2  
(2868623)  
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
Internet Explorer 7  
(2862772)  
(Kritisch)  
Internet Explorer 8  
(2862772)  
(Kritisch)  
Internet Explorer 9  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Vista x64 Edition Service Pack 2  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(2862772)  
(Mittel)  
Internet Explorer 8  
(2862772)  
(Mittel)  
Internet Explorer 9  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(2843638)  
(Hoch)  
Active Directory-Verbunddienste 1.x  
(2868846)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2862772)  
(Mittel)  
Internet Explorer 8  
(2862772)  
(Mittel)  
Internet Explorer 9  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(2843638)  
(Hoch)  
Active Directory-Verbunddienste 1.x  
(2868846)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Internet Explorer 7  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für Itanium-basierte Systeme Service Pack 2  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2862772)  
(Kritisch)  
Internet Explorer 9  
(2862772)  
(Kritisch)  
Internet Explorer 10  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für 32-Bit-Systeme Service Pack 1  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2862772)  
(Kritisch)  
Internet Explorer 9  
(2862772)  
(Kritisch)  
Internet Explorer 10  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 7 für x64-basierte Systeme Service Pack 1  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(2862772)  
(Mittel)  
Internet Explorer 9  
(2862772)  
(Mittel)  
Internet Explorer 10  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.0  
(2843638)  
(Hoch)  
Active Directory-Verbunddienste 1.x  
(2868846)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1
</td>
<td style="border:1px solid black;">
Internet Explorer 8  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für Itanium-basierte Systeme Service Pack 1  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows 8
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
<td style="border:1px solid black;">
**Keine**
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 32-Bit-Systeme  
(2868623)  
(Hoch)
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
Internet Explorer 10  
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows 8 für 64-Bit-Systeme  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2012
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
Windows Server 2012
</td>
<td style="border:1px solid black;">
Internet Explorer 10  
(2862772)  
(Mittel)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2849568)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2012  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Active Directory-Verbunddienste 2.1  
(2843638)  
(Hoch)  
Active Directory-Verbunddienste 2.1  
(2843639)  
(Keine Bewertung des Schweregrads)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows RT
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
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
(2862772)  
(Kritisch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows RT  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Server Core-Installationsoption
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-059**](https://go.microsoft.com/fwlink/?linkid=313330)
</td>
<td style="border:1px solid black;">
[**MS13-060**](https://go.microsoft.com/fwlink/?linkid=314044)
</td>
<td style="border:1px solid black;">
[**MS13-062**](https://go.microsoft.com/fwlink/?linkid=309337)
</td>
<td style="border:1px solid black;">
[**MS13-063**](https://go.microsoft.com/fwlink/?linkid=309338)
</td>
<td style="border:1px solid black;">
[**MS13-064**](https://go.microsoft.com/fwlink/?linkid=314043)
</td>
<td style="border:1px solid black;">
[**MS13-065**](https://go.microsoft.com/fwlink/?linkid=314047)
</td>
<td style="border:1px solid black;">
[**MS13-066**](https://go.microsoft.com/fwlink/?linkid=309325)
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
<td style="border:1px solid black;">
[**Hoch**](https://technet.microsoft.com/de-de/security/gg309177.aspx)
</td>
<td style="border:1px solid black;">
**Keine**
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
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme Service Pack 2 (Server Core-Installation)  
(2868623)  
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
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 für x64-basierte Systeme Service Pack 2 (Server Core-Installation)  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2859537)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2008 R2 für x64-basierte Systeme Service Pack 1 (Server Core-Installation)  
(2868623)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
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
Windows Server 2012 (Server Core-Installation)  
(2849470)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Windows Server 2012 (Server Core-Installation)  
(2868623)  
(Hoch)
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
Microsoft Exchange Server
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS13-061**](https://go.microsoft.com/fwlink/?linkid=317381)
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
Microsoft Exchange Server 2007 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2007 Service Pack 3  
(2873746)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 2
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 2  
(2874216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 3
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2010 Service Pack 3  
(2866475)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 1
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 1  
(2874216)  
(Kritisch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 2
</td>
<td style="border:1px solid black;">
Microsoft Exchange Server 2013 Kumulatives Update 2  
(2874216)  
(Kritisch)
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

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/2862973): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
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

**MS13-059**

-   Peter ‘corelanc0d3 r‘ Van Eeckhoutte von [Corelan](https://www.corelangcv.com/) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3184).
-   Fermin J. Serna vom [Google Security Team](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit bei der Zuweisung von Prozessintegritätsebenen (CVE-2013-3186).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3187).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3188).
-   Scott Bell von [Security-Assessment.com](https://www.security-assessment.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3189).
-   Ivan Fratric und Ben Hawkes vom [Google Security Team](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3190).
-   Ivan Fratric und Ben Hawkes vom [Google Security Team](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3191).
-   Alex Inführ für den Hinweis auf die Sicherheitsanfälligkeit in EUC-JP-Zeichencodierung (CVE-2013-3192).
-   Jose Antonio Vazquez Gonzalez in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit in Internet Explorer bezüglich Speicherbeschädigung (CVE-2013-3193).
-   Arthur Gerkis in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3194).
-   Einer Person, die mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) zusammenarbeitet, aber anonym bleiben möchte, für den Hinweis auf die Sicherheitsanfälligkeit bezüglich Speicherbeschädigung in Internet Explorer (CVE-2013-3199).
-   [VUPEN Security](https://www.vupen.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für die Zusammenarbeit mit uns an in diesem Bulletin enthaltenen Tiefenverteidigungsänderungen.

**MS13-060**

-   Bob Clary von [Mozilla](https://www.mozilla.org/) für den Hinweis auf die Sicherheitsanfälligkeit im Uniscribe-Schriftartenanalysemodul bezüglich Speicherbeschädigung (CVE-2013-3181).

**MS13-063**

-   [VUPEN Security](https://www.vupen.com) in Zusammenarbeit mit der [Zero Day Initiative](https://www.zerodayinitiative.com/) von [HP](https://www.hpenterprisesecurity.com/products) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in ASLR durch Umgehung der Sicherheitsfunktion (CVE-2013-2556).
-   Yang Yu vom [Nsfocus Security Team](https://www.nsfocus.com/) für die Zusammenarbeit mit uns an der Sicherheitsanfälligkeit in ASLR durch Umgehung der Sicherheitsfunktion (CVE-2013-2556).
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung (CVE-2013-3196).
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung (CVE-2013-3197).
-   [Mateusz “j00 ru“ Jurczyk](https://j00ru.vexillium.org/) von [Google Inc](https://www.google.com/) für den Hinweis auf die Sicherheitsanfälligkeit im Windows-Kernel bezüglich Speicherbeschädigung (CVE-2013-3198).

**MS13-065**

-   Basil Gabriel von Symantec für den Hinweis auf die Sicherheitsanfälligkeit in ICMPv6 (CVE-2013-3183).

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle&displaylang=de), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Sicherheitslösungen für IT-Experten: [TechNet Sicherheit – Problembehandlung und Support](https://technet.microsoft.com/de-de/security/bb980617)
-   So schützen Sie Ihren Computer, auf dem Windows ausgeführt wird, vor Viren und schädlicher Software: [Viruslösung und Security Center](https://support.microsoft.com/contactus/cu_sc_virsec_master)
-   Lokaler Support entsprechend Ihrem Land: [Internationaler Support](https://support.microsoft.com/common/international.aspx)

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für Sie.

#### Revisionen

-   V1.0 (13. August 2013): Bulletin Summary veröffentlicht.
-   V2.0 (19. August 2013): Das Bulletin wurde wegen MS13-066 überarbeitet, um das erneute Anbieten des Updates 2843638 für Active Directory-Verbunddienste 2.0 unter Windows Server 2008 und Windows Server 2008 R2 anzukündigen. Weitere Informationen finden Sie im Bulletin.
-   V3.0 (27. August 2013): Das Bulletin für MS13-061 wurde überarbeitet, um das erneute Anbieten des Updates 2874216 für Microsoft Exchange Server 2013 kumulatives Update 1 und Microsoft Exchange Server 2013 kumulatives Update 2 anzukündigen. Weitere Informationen finden Sie im Bulletin.

*Built at 2014-04-18T01:50:00Z-07:00*