---
TOCTitle: 'MS09-JUN'
Title: Microsoft Security Bulletin Summary für Juni 2009
ms:assetid: 'ms09-jun'
ms:contentKeyID: 61225073
ms:mtpsurl: 'https://technet.microsoft.com/de-DE/library/ms09-jun(v=Security.10)'
---

Security Bulletin Summary

Microsoft Security Bulletin Summary für Juni 2009
=================================================

Veröffentlicht: Dienstag, 9. Juni 2009 | Aktualisiert: Mittwoch, 10. Juni 2009

**Version:** 1.1

In diesem Bulletin Summary sind die im Juni 2009 veröffentlichten Security Bulletins aufgeführt.

Mit der Veröffentlichung der Bulletins für Juni 2009 ersetzt dieses Bulletin Summary die Bulletin Advance Notification, die erstmalig am 4. Juni 2009 veröffentlicht wurde. Weitere Informationen zum Bulletin Advance Notification-Service finden Sie unter [Microsoft Security Bulletin Advance Notification](https://www.microsoft.com/germany/technet/sicherheit/bulletins/bulletinadvance.mspx).

Weitere Informationen zum Erhalten automatischer Benachrichtigungen über die Veröffentlichung von Microsoft Security Bulletins finden Sie unter [Microsoft Technische Sicherheitsbenachrichtigungen](https://www.microsoft.com/germany/technet/sicherheit/bulletins/notify.mspx).

Am Mittwoch, den 10. Juni 2009 um 11:00 Uhr pazifischer Zeit (USA & Kanada) stellt Microsoft einen Webcast bereit, um Kundenfragen zu diesen Bulletins zu beantworten. [Registrieren Sie sich jetzt für das Security Bulletin-Webcast im Juni.](https://msevents.microsoft.com/cui/webcasteventdetails.aspx?culture=en-us&eventid=1032395225) Ab diesem Datum steht dieser Webcast auf Anfrage zur Verfügung. Weitere Informationen dazu finden Sie unter [Microsoft Security Bulletin Zusammenfassungen und Webcasts.](https://technet.microsoft.com/security/bulletin/summary)

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Active Directory können Remotecodeausführung ermöglichen (971055)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten in Implementierungen von Active Directory unter Microsoft Windows 2000 Server und Windows Server 2003 sowie im Active Directory Application Mode (ADAM) bei Installation unter Windows XP Professional und Windows Server 2003. Die schwerere Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen. Nutzt ein Angreifer diese Sicherheitsanfälligkeit erfolgreich aus, kann er die vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in der Windows-Druckwarteschlange können Remotecodeausführung ermöglichen (961501)</strong><br />
<br />
Dieses Sicherheitsupdate behebt drei vertraulich gemeldete Sicherheitsanfälligkeiten in der Windows-Druckwarteschlange. Die schwerste Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein betroffener Server eine speziell gestaltete RPC-Anforderung empfängt. Mithilfe empfohlener Vorgehensweisen für die Firewall und standardisierten Firewallkonfigurationen können Netzwerke vor Remoteangriffen von außerhalb des Unternehmens geschützt werden. Eine bewährte Methode besteht darin, für Systeme, die mit dem Internet verbunden sind, nur eine minimale Anzahl von Ports zu öffnen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;"><strong>Kumulatives Sicherheitsupdate für Internet Explorer (969897)</strong><br />
<br />
Dieses Sicherheitsupdate behebt sieben vertraulich gemeldete Sicherheitsanfälligkeiten und eine öffentlich gemeldete Sicherheitsanfälligkeit in Internet Explorer. Die schwerere Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Webseite mit Internet Explorer anzeigt. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows, Internet Explorer</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (969514)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei vertraulich gemeldete Sicherheitsanfälligkeiten, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Word-Datei öffnet. Ein Angreifer, dem es gelingt, eine dieser Sicherheitsanfälligkeiten auszunutzen, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</strong><br />
<br />
Dieses Sicherheitsupdate behebt mehrere vertraulich gemeldete Sicherheitsanfälligkeiten, die Remotecodeausführung ermöglichen können, wenn ein Benutzer eine speziell gestaltete Excel-Datei öffnet, die ein fehlerhaftes Datensatzobjekt enthält. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=128104">MS09-024</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in Microsoft Works-Konvertern kann Remotecodeausführung ermöglichen (957632)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in den Microsoft Works-Konvertern. Die Sicherheitsanfälligkeit kann Remotecodeausführung ermöglichen, wenn ein Benutzer eine speziell gestaltete Works-Datei öffnet. Ein Angreifer, der diese Sicherheitsanfälligkeit erfolgreich ausnutzt, kann die gleichen Benutzerrechte wie der lokale Benutzer erlangen. Für Benutzer, deren Konten mit weniger Benutzerrechten konfiguriert sind, kann dies geringere Auswirkungen haben als für Benutzer, die mit administrativen Benutzerrechten arbeiten.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Kritisch</a><br />
Remotecodeausführung</td>
<td style="border:1px solid black;">Erfordert u. U. Neustart</td>
<td style="border:1px solid black;">Microsoft Office</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150174">MS09-026</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in RPC kann Erhöhung von Berechtigungen ermöglichen (970238)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit in der Windows-RPC-Funktionalität (Remote Procedure Call, Remoteprozeduraufruf), bei der das RPC-Marshallingmodul seinen internen Zustand nicht richtig aktualisiert. Die Sicherheitsanfälligkeit kann einem Angreifer ermöglichen, beliebigen Code auszuführen und vollständige Kontrolle über das betroffene System zu erlangen. Unterstützte Editionen von Microsoft Windows werden ohne RPC-Server oder -Clients geliefert, die von dieser Sicherheitsanfälligkeit betroffen sein könnten. In einer Standardkonfiguration können Benutzer nicht durch Ausnutzung dieser Sicherheitsanfälligkeit angegriffen werden. Die Sicherheitsanfälligkeit ist jedoch in der Microsoft Windows-RPC-Laufzeit vorhanden und kann RPC-Anwendungen von Drittanbietern betreffen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (968537)</strong><br />
<br />
Dieses Sicherheitsupdate behebt zwei öffentlich gemeldete und zwei vertraulich gemeldete Sicherheitsanfälligkeiten im Windows-Kernel, die eine Erhöhung von Berechtigungen ermöglichen können. Ein Angreifer, der eine dieser Sicherheitsanfälligkeiten erfolgreich ausnutzt, kann beliebigen Code ausführen und vollständige Kontrolle über das betroffene System erlangen. Ein Angreifer kann dann Programme installieren, Daten anzeigen, ändern oder löschen oder neue Konten mit sämtlichen Benutzerrechten erstellen. Ein Angreifer benötigt gültige Anmeldeinformationen und muss sich lokal anmelden können, um diese Sicherheitsanfälligkeiten auszunutzen. Die Sicherheitsanfälligkeiten können nicht per Remotezugriff oder von anonymen Benutzern ausgenutzt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeiten in Internet Information Services (IIS) können Erhöhung von Berechtigungen ermöglichen (970483)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine öffentlich gemeldete Sicherheitsanfälligkeit und eine vertraulich gemeldete Sicherheitsanfälligkeit in Microsoft Internet Information Services (IIS). Die Sicherheitsanfälligkeiten können eine Erhöhung von Berechtigungen ermöglichen, wenn ein Angreifer eine speziell gestaltete HTTP-Anforderung an eine Website sendet, die eine Authentifizierung erfordert. Diese Sicherheitsanfälligkeiten ermöglichen einem Angreifer, die IIS-Konfiguration zu umgehen, die angibt, welche Art von Authentifizierung zulässig ist, aber nicht die dateisystembasierte ACL-Kontrolle (access control list, Zugriffssteuerungsliste), die überprüft, ob eine Datei für einen gegebenen Benutzer zugänglich ist. Eine erfolgreiche Ausnutzung dieser Sicherheitsanfälligkeiten würde den Angreifer immer noch auf die Berechtigungen beschränken, die dem anonymen Benutzerkonto durch die Dateisystem-ACLs gewährt werden.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Hoch</a><br />
Erhöhung von Berechtigungen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=143550">MS09-023</a></td>
<td style="border:1px solid black;"><strong>Sicherheitsanfälligkeit in der Windows-Suche kann Offenlegung von Informationen ermöglichen (963093)</strong><br />
<br />
Dieses Sicherheitsupdate behebt eine vertraulich gemeldete Sicherheitsanfälligkeit in der Windows-Suche. Die Sicherheitsanfälligkeit kann eine Offenlegung von Informationen ermöglichen, wenn ein Benutzer eine Suche durchführt, bei der als erstes Ergebnis eine speziell gestaltete Datei zurückgegeben wird, oder wenn der Benutzer eine speziell gestaltete Datei aus den Suchergebnissen in der Vorschau anzeigt. Standardmäßig ist die Windows-Suche unter Microsoft Windows XP und Windows Server 2003 nicht vorinstalliert. Dies ist eine optionale Komponente, die heruntergeladen werden kann. Die Windows-Suche, die unter unterstützten Editionen von Windows Vista und Windows Server 2008 installiert ist, ist von dieser Sicherheitsanfälligkeit nicht betroffen.</td>
<td style="border:1px solid black;"><a href="https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx">Mittel</a><br />
Offenlegung von Informationen</td>
<td style="border:1px solid black;">Erfordert Neustart</td>
<td style="border:1px solid black;">Microsoft Windows</td>
</tr>
</tbody>
</table>
  
Ausnutzbarkeitsindex  
--------------------
  
In der folgenden Tabelle wird eine Bewertung der Ausnutzbarkeit aller Sicherheitsanfälligkeiten bereitgestellt, die diesen Monat behoben werden. Die Sicherheitsanfälligkeiten sind nach Kennung des Bulletins und CVE-ID geordnet.
  
**Wie verwende ich diese Tabelle?**  
  
Verwenden Sie diese Tabelle, um etwas über die Wahrscheinlichkeit zu erfahren, dass für die einzelnen Sicherheitsupdates, die Sie möglicherweise installieren müssen, funktionierender Angreifercode veröffentlicht wird. Sie sollten sich unter Berücksichtigung Ihrer konkreten Konfiguration jede der unten stehenden Bewertungen ansehen, um Prioritäten für Ihre Bereitstellung festzulegen. Weitere Informationen zur Bedeutung und Festlegung dieser Bewertungen finden Sie im [Microsoft-Ausnutzbarkeitsindex](https://technet.microsoft.com/en-us/security/cc998259.aspx).

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
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Active Directory können Remotecodeausführung ermöglichen (971055)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1138">CVE-2009-1138</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Konsistenter Angreifercode ist wahrscheinlich, der auf Windows 2000-Servern, die den LDAP- oder LDAPS-Dienst im Netzwerk verfügbar machen, Denial of Service bewirken kann. Aufgrund zusätzlicher Überprüfungen des Heap ist eine funktionerende Remotecodeausführung jedoch sehr unwahrscheinlich.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=151361">MS09-018</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Active Directory können Remotecodeausführung ermöglichen (971055)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1139">CVE-2009-1139</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Die Auswirkung dieser Sicherheitsanfälligkeit ist ein Speicherverlust, der schließlich zu einem Denial-of-Service führen kann. Codeausführung ist nicht möglich.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2007-3091">CVE-2007-3091</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1140">CVE-2009-1140</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit bezüglich domänenübergreifenden Zugriffs auf Informationen, die höchstwahrscheinlich zu einer Offenlegung von Information führt, nicht zu einer Codeausführung.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1141">CVE-2009-1141</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1528">CVE-2009-1528</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1529">CVE-2009-1529</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1530">CVE-2009-1530</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1531">CVE-2009-1531</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150860">MS09-019</a></td>
<td style="border:1px solid black;">Kumulatives Sicherheitsupdate für Internet Explorer (969897)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1532">CVE-2009-1532</a></td>
<td style="border:1px solid black;">Für IE8 für Windows XP und Windows Vista ohne DEP:<br />
<a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> - Konsistenter Angreifercode wahrscheinlich<br />
<br />
Für IE8 für Windows Vista mit DEP, Windows Server 2003 und Windows Server 2008:<br />
<a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> - Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Konsistenter Angreifercode ist am wahrscheinlichsten für Internet Explorer 8 für Windows XP sowie Windows Vista, wenn DEP nicht aktiviert ist.<br />
<br />
Für Internet Explorer 8 für Windows Vista mit aktivierter DEP ist funktionierender Angreifercode unwahrscheinlich. ASLR/DEP und die Tatsache, dass .NET-Komponenten in der Internetzone standardmäßig deaktiviert sind, mildern das Risiko.<br />
<br />
Für Internet Explorer 8 für Windows Server 2003 und Windows Server 2008 ist funktionierender Angreifercode unwahrscheinlich, da die verstärkte Sicherheitskonfiguration Skripts in der Internetzone deaktiviert.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Internet Information Services (IIS) können Erhöhung von Berechtigungen ermöglichen (970483)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1122">CVE-2009-1122</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Eine Codeausführung ist unwahrscheinlich, aber eine Offenlegung von Information aufgrund von Authentifizierungsumgehungsbedingungen ist sehr wahrscheinlich.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150568">MS09-020</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Internet Information Services (IIS) können Erhöhung von Berechtigungen ermöglichen (970483)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1535">CVE-2009-1535</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Öffentlicher Code für eine Offenlegung von Information ist verfügbar.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0549">CVE-2009-0549</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0557">CVE-2009-0557</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0558">CVE-2009-0558</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0559">CVE-2009-0559</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Eine Bedrohung durch Codeausführung existiert nur für Office 2000. Bei Angriffen gegen höhere Versionen von Office ist die Wahrscheinlichkeit einer Codeausführung gering.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0560">CVE-2009-0560</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0561">CVE-2009-0561</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147294">MS09-021</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Excel können Remotecodeausführung ermöglichen (969462)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1134">CVE-2009-1134</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in der Windows-Druckwarteschlange können Remotecodeausführung ermöglichen (961501)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0228">CVE-2009-0228</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in der Windows-Druckwarteschlange können Remotecodeausführung ermöglichen (961501)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0229">CVE-2009-0229</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">Dies ist eine Sicherheitsanfälligkeit durch Offenlegung von Informationen ohne die Möglichkeit von Codeausführung.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=141786">MS09-022</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in der Windows-Druckwarteschlange können Remotecodeausführung ermöglichen (961501)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0230">CVE-2009-0230</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=143550">MS09-023</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in der Windows-Suche kann Offenlegung von Informationen ermöglichen (963093)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0239">CVE-2009-0239</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>3</strong></a> – Funktionierender Angreifercode unwahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=128104">MS09-024</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in Microsoft Works-Konvertern kann Remotecodeausführung ermöglichen (957632)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1533">CVE-2009-1533</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (968537)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1123">CVE-2009-1123</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (968537)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1124">CVE-2009-1124</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (968537)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1125">CVE-2009-1125</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150248">MS09-025</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten im Windows-Kernel können Erhöhung von Berechtigungen ermöglichen (968537)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-1126">CVE-2009-1126</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Konsistenter Angreifercode ist für Windows 2000 am wahrscheinlichsten. Die Wahrscheinlichkeit von Codeausführung durch diese Sicherheitsanfälligkeit durch stapelbasierten Pufferüberlauf ist auf Windows XP und Windows Server 2003 aufgrund des /GS-Schutz geringer.</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=150174">MS09-026</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeit in RPC kann Erhöhung von Berechtigungen ermöglichen (970238)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0568">CVE-2009-0568</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">Nicht jede Microsoft-Software ist direkt von dieser Sicherheitsanfälligkeit betroffen. Arbeitsstationen, auf denen RPC-Dienste von unabhängigen Softwareanbietern implementiert wurden, sind jedoch möglicherweise für Remotecodeausführung anfällig, wenn dieses Sicherheitsupdate nicht installiert wurde.</td>
</tr>
<tr class="even">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (969514)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0563">CVE-2009-0563</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>2</strong></a> – Inkonsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
<tr class="odd">
<td style="border:1px solid black;"><a href="https://go.microsoft.com/fwlink/?linkid=147416">MS09-027</a></td>
<td style="border:1px solid black;">Sicherheitsanfälligkeiten in Microsoft Office Word können Remotecodeausführung ermöglichen (969514)</td>
<td style="border:1px solid black;"><a href="https://www.cve.mitre.org/cgi-bin/cvename.cgi?name=cve-2009-0565">CVE-2009-0565</a></td>
<td style="border:1px solid black;"><a href="https://technet.microsoft.com/en-us/security/cc998259.aspx"><strong>1</strong></a> – Konsistenter Angreifercode wahrscheinlich</td>
<td style="border:1px solid black;">(Keine)</td>
</tr>
</tbody>
</table>
  
Betroffene Software und Downloadadressen  
----------------------------------------
  
In den folgenden Tabellen sind die Bulletins nach Hauptsoftwarekategorie und Schweregrad aufgeführt.
  
**Wie verwende ich diese Tabellen?**  
  
In diesen Tabellen finden Sie Informationen zu Sicherheitsupdates, die Sie möglicherweise installieren sollten. Alle aufgeführten Softwareprogramme bzw. -komponenten sollten überprüft werden, um zu sehen, ob Sicherheitsupdates für Ihre Installation zutreffen. Wenn ein Softwareprogramm oder eine Komponente aufgeführt sind, dann ist das verfügbare Softwareupdate über einen Hyperlink verknüpft, und die Bewertung des Schweregrads des Softwareupdates ist ebenfalls aufgeführt.
  
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
<th style="border:1px solid black;" >
</th>
<th style="border:1px solid black;" >
</th>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Microsoft Windows 2000  
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-018**](https://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](https://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](https://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](https://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](https://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](https://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](https://go.microsoft.com/fwlink/?linkid=143550)
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
Microsoft Windows 2000 Service Pack 4
</td>
<td style="border:1px solid black;">
[Active Directory unter Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=bba6e20a-0345-46ae-a6f1-fd27fdee7c21)  
(KB969805)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=86378753-db24-44c2-a27d-cc0239f40ab8)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 5.01 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=d645ad82-13c3-4030-808b-834e86ed3298)  
(Kritisch)  
[Microsoft Internet Explorer 6 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=fe8b3796-a407-4f41-89eb-35b4bcc24ff6)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=155a79c1-e5e4-4f62-b4b0-53aca59f20ac)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Windows 2000 Service Pack 4](https://www.microsoft.com/download/details.aspx?familyid=79b0481d-a3d7-477b-928a-a98cc79374af)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.0](https://www.microsoft.com/download/details.aspx?familyid=8515a294-4f25-4dc5-860a-e7ad9b6c1c01)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows XP
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-018**](https://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](https://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](https://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](https://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](https://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](https://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](https://go.microsoft.com/fwlink/?linkid=143550)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows XP Service Pack 2 und Windows XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM) unter Windows XP Professional Service Pack 2 und Windows XP Professional Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=cb2c9b76-0c65-4754-9941-d45a7c74a29a)  
(KB970437)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f2119aca-a98e-4810-be52-f38241443baf)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=3d7f63ee-d7c3-48a5-902e-60625405e97d)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=827b735c-660b-4723-b688-3297e107153a)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=d9e27ce1-4e7c-437f-9477-e7805a33da08)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f033fa78-c451-44f8-aa6c-a49622c37f40)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Service Pack 2 und Windows XP Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=6349e046-a3f8-4ae5-b8c3-c9879cc99e8f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 5.1 unter Windows XP Professional Service Pack 2 und Windows XP Professional Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=97da589f-4534-42f6-9f29-967b5a33c542)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows-Suche 4.0](https://www.microsoft.com/download/details.aspx?familyid=759f22cb-ea7f-49dd-a200-19cb83fffd8d)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows XP Professional x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=2ef3aaf0-a2a9-4c17-99ab-a0dc3d3f7e86)  
(KB970437)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=22699d09-1e68-456a-8733-bfad6667ebf5)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=088f70eb-c5c5-426a-880a-18ed386d0b56)  
(Kritisch)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=e5d2c81e-ffab-4e3b-a59a-a55000597213)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=a24aedf0-7a31-4ee8-a9a6-998f1160c700)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=20734b70-37f1-47dd-bc09-d56f93577a55)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows XP Professional x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3769800e-af93-4a44-8a1e-b30cc54b226f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](https://www.microsoft.com/download/details.aspx?familyid=8982e6d2-e1f7-4208-88e3-80b159a8e21a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows-Suche 4.0](https://www.microsoft.com/download/details.aspx?familyid=50c56dd6-c34d-4632-a779-8bcf8fdb341b)  
(Mittel)
</td>
</tr>
<tr>
<th colspan="8" style="border:1px solid black;">
Windows Server 2003
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-018**](https://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](https://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](https://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](https://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](https://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](https://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](https://go.microsoft.com/fwlink/?linkid=143550)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
</td>
<td style="border:1px solid black;">
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=d814ce65-a193-4027-a6cd-106d388830a6)   
(KB969805)  
(Hoch)  
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=f6f99957-f74f-4446-8734-a468283eebae)   
(KB970437)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=865414f8-3f77-4fee-acc6-6684a3dc0aa4)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=72a23752-86fb-4cc9-ab8e-63ffdfae5bec)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a980b867-c67f-4c61-b6db-e55c2ca68dc0)  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=298143f2-f37a-4a2c-86ac-9804d4ff1dad)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=62bb9e22-4f4b-4ffc-ba76-f626e94c79d5)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=9356404c-d89a-4de0-b9b4-f6e1bdadf745)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](https://www.microsoft.com/download/details.aspx?familyid=2bd4e410-dbd8-431a-b316-e1e2f1825c3a)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows-Suche 4.0](https://www.microsoft.com/download/details.aspx?familyid=e72ef31f-5161-4fe6-8ed3-6206e02cef31)  
(Mittel)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Server 2003 x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=0d1f23c8-06eb-4996-92eb-0eb635fd6a42)  
(KB969805)  
(Hoch)  
[Active Directory Application Mode (ADAM)](https://www.microsoft.com/download/details.aspx?familyid=1a2badc7-c0a5-4032-a009-73ebe9d76313)  
(KB970437)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=197a6cc7-4ba3-4d2e-b621-0ef3da645ef2)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=2a03d3c4-e39d-43a3-8d42-216e9551be96)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=5e7d6372-9c8c-449d-88fd-afd4f92ad9e6)  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=4a5401d7-ca97-4734-a0e9-d7ffe0777e34)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=888b8dd8-d76c-42f5-a377-1f1750d3cf56)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5a3123af-173d-49eb-9997-14e82e764aee)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](https://www.microsoft.com/download/details.aspx?familyid=ea363223-535d-4142-9aba-3890960c6259)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows-Suche 4.0](https://www.microsoft.com/download/details.aspx?familyid=7ffc3680-f9bf-423b-96a7-102f4cc9c240)  
(Mittel)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Windows Server 2003 mit SP2 für Itanium-basierte Systeme
</td>
<td style="border:1px solid black;">
[Active Directory](https://www.microsoft.com/download/details.aspx?familyid=92e7808b-92ff-449d-bb73-ee8638e9ccd1)  
(KB969805)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=719efd62-fb33-447d-b6dd-2aaafbbad881)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Explorer 6](https://www.microsoft.com/download/details.aspx?familyid=58efde2c-e0b8-4259-b19e-80564b834882)  
(Mittel)  
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a2d2907e-67ae-44a4-a805-8670e659ea57)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=3084f46e-02b9-4d99-a7a1-033817f9bd9f)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2003 mit SP2 für Itanium-basierte Systeme](https://www.microsoft.com/download/details.aspx?familyid=13b50993-410f-4e7a-a33a-6d9b48dbb4d1)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Internet Information Services 6.0](https://www.microsoft.com/download/details.aspx?familyid=e6b806eb-e2c4-4436-8964-720db593055d)  
(Hoch)
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
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-018**](https://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](https://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](https://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](https://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](https://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](https://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](https://go.microsoft.com/fwlink/?linkid=143550)
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
Keine
</td>
<td style="border:1px solid black;">
Keine
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=3ad8f037-2434-4dea-bfc3-9d3b4008b828)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=e60215c3-b8b9-4e45-9d9f-b3fb0b47cce1)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=6f2730e9-b4fc-4f20-96cf-73f1be63f374)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=5ca227c0-f2dd-429c-a542-e08e93527214)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista, Windows Vista Service Pack 1 und Windows Vista Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=c31b36f8-330c-4a0c-9a3d-7cbe9a1ab8c8)  
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
Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=85c317cd-2a14-4747-9f50-3af3ddd3ae1b)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=88185088-8c2c-4bc6-89b2-87f4d4849cf7)  
(Kritisch)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=5edb14f7-11ec-4180-9f0f-b2673f1c8d83)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=188adafe-1feb-46ad-b237-a88d35104dcd)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Vista x64 Edition, Windows Vista x64 Edition Service Pack 1 und Windows Vista x64 Edition Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7d70a65f-07ce-4992-8bec-28fefd7587bc)  
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
<th colspan="8" style="border:1px solid black;">
Windows Server 2008
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-018**](https://go.microsoft.com/fwlink/?linkid=151361)
</td>
<td style="border:1px solid black;">
[**MS09-022**](https://go.microsoft.com/fwlink/?linkid=141786)
</td>
<td style="border:1px solid black;">
[**MS09-019**](https://go.microsoft.com/fwlink/?linkid=150860)
</td>
<td style="border:1px solid black;">
[**MS09-026**](https://go.microsoft.com/fwlink/?linkid=150174)
</td>
<td style="border:1px solid black;">
[**MS09-025**](https://go.microsoft.com/fwlink/?linkid=150248)
</td>
<td style="border:1px solid black;">
[**MS09-020**](https://go.microsoft.com/fwlink/?linkid=150568)
</td>
<td style="border:1px solid black;">
[**MS09-023**](https://go.microsoft.com/fwlink/?linkid=143550)
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
[**Hoch**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
</td>
<td style="border:1px solid black;">
[**Mittel**](https://www.microsoft.com/germany/technet/datenbank/articles/527029.mspx)
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
<tr>
<td style="border:1px solid black;">
Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=0f18356d-9f09-4d24-8361-970c0d1ccac4)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=a0e3f975-57da-43fa-ac12-3d14fd6ce939)\*\*  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=aaad301c-d232-4733-a0df-8e5d41bbfde8)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=eaa26c6c-5bf7-4099-bb21-1e03de3a25ca)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für 32-Bit-Systeme und Windows Server 2008 für 32-Bit-Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=98ba52b2-da1a-4939-a10e-d43b3a7e7ed4)\*  
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
Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7d0a6e8d-a31d-4f3d-a7d7-e61215bfebed)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=758edce7-2a82-4b2e-bd71-5b7075cc4b17)\*\*  
(Mittel)  
[Windows Internet Explorer 8](https://www.microsoft.com/download/details.aspx?familyid=faac92d4-4a2b-4bb5-8bd1-1519a9fa8147)\*\*  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=447aaa4f-946b-4f23-b151-dcf46ea9f80e)\*  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für x64-basierte Systeme und Windows Server 2008 für x64-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=dbaa5a72-c267-4907-a207-525c2803d7b9)\*  
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
Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=bbac3deb-6c93-45aa-832c-02b915ac7f44)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Internet Explorer 7](https://www.microsoft.com/download/details.aspx?familyid=67d4c189-030d-42eb-98b9-7957ccd92592)  
(Mittel)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=f33012b9-5d5b-4f72-8d49-a8e1c8bc1337)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Windows Server 2008 für Itanium-basierte Systeme und Windows Server 2008 für Itanium-basierte Systeme Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=e0e3ad56-a363-44ba-af4d-b7f551c88afd)  
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
 
**Hinweise für Windows Server 2008**

**\*Die Server Core-Installation von Windows Server 2008 ist betroffen.** Für unterstützte Editionen von Windows Server 2008 gilt dieses Update mit der gleichen Bewertung des Schweregrads. Dabei spielt es keine Rolle, ob Windows Server 2008 mit der Server Core-Installationsoption installiert wurde oder nicht. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

**\*\*Die Server Core-Installation von Windows Server 2008 ist nicht betroffen.** Die durch dieses Update behobenen Sicherheitsanfälligkeiten betreffen unterstützte Editionen von Windows Server 2008 nicht, wenn Windows Server 2008 mit der Server Core-Installationsoption installiert wurde. Weitere Informationen zu dieser Installationsoption finden Sie unter [Server Core](https://msdn.microsoft.com/en-us/library/ms723891(vs.85).aspx). Beachten Sie, dass die Server Core-Installationsoption für bestimmte Editionen von Windows Server 2008 nicht gilt; siehe dazu [Vergleichen von Server Core-Installationsoptionen](https://www.microsoft.com/germany/windowsserver2008/editionen/core.mspx).

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
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Microsoft Office Suites, Systeme und Komponenten
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-027**](https://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](https://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](https://go.microsoft.com/fwlink/?linkid=128104)
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
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2000 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=3663e9f2-a952-4238-b902-90b5b09feb38)  
(KB969600)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=dd16e243-b8e2-4afb-86b6-4d60214598eb)  
(KB969683)  
(Kritisch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2000 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=4bf95806-3d32-411b-9779-a81aebad45e9)  
(KB957838)  
(Kritisch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office XP Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=f1323be1-15f2-491b-abae-c03ba1394398)  
(KB969602)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=dd80ce95-0aec-4493-b9d1-c3dad95c3415)  
(KB969680)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2002 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=b0ba8c9e-75ee-46bd-9e92-d4e6599309ad)  
(KB957646)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office 2003 Service Pack 3
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=7cbc2587-2c8c-49b4-9f40-e4cdccb61ecd)  
(KB969603)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=10156044-a5a4-4312-98a7-1b1ced625ddb)  
(KB969681)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2003 Service Pack 3 mit den Microsoft Works 6–9-Dateikonvertern](https://www.microsoft.com/download/details.aspx?familyid=a7ba3ea7-d06a-4c14-9107-9b92ef68fcae)\*\*\*  
(KB968326)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office System 2007 Service Pack 1 und Microsoft Office System 2007 Service Pack 2
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1 und Microsoft Office Word 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=7e205108-4c28-4cab-a4d0-4ed3fd696473)  
(KB969604)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel 2007 Service Pack 1 und Microsoft Office Excel 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=2bcd565a-6acb-407d-80da-0398526ddf99)\*  
(KB969682)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Word 2007 Service Pack 1](https://www.microsoft.com/download/details.aspx?familyid=bd47e1e5-cd2e-4c08-9864-471e97f38ca3)  
(KB969559)  
(Hoch)
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Microsoft Office für Mac
</th>
</tr>
<tr>
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-027**](https://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](https://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](https://go.microsoft.com/fwlink/?linkid=128104)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office 2004 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2004 für Mac](https://www.microsoft.com/download/details.aspx?familyid=5557bfb7-ebb4-4c42-8042-41e830c4e550)  
(KB969661)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Office 2008 für Mac
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office 2008 für Mac](https://www.microsoft.com/download/details.aspx?familyid=58326da2-eb75-4b42-b1bc-e70319defb58)  
(KB971822)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Open XML-Dateiformatkonverter für Mac
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Open XML-Dateiformatkonverter für Mac](https://www.microsoft.com/download/details.aspx?familyid=9d6d9eaa-8442-4184-8886-faab2803bde6)  
(KB971824)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<th colspan="4" style="border:1px solid black;">
Weitere Office-Software
</th>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
**Kennung des Bulletins**
</td>
<td style="border:1px solid black;">
[**MS09-027**](https://go.microsoft.com/fwlink/?linkid=147416)
</td>
<td style="border:1px solid black;">
[**MS09-021**](https://go.microsoft.com/fwlink/?linkid=147294)
</td>
<td style="border:1px solid black;">
[**MS09-024**](https://go.microsoft.com/fwlink/?linkid=128104)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
**Bewertung des Gesamtschweregrads**
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
Microsoft Office Excel Viewer
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office Excel Viewer 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=20e6933d-85f8-4cec-9534-893789cd053e)  
(KB969685)  
(Hoch)  
[Microsoft Office Excel Viewer](https://www.microsoft.com/download/details.aspx?familyid=ac0530dc-7f63-4ad0-85c1-784ad28156cf)  
(KB969686)  
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
[Microsoft Office Word Viewer 2003 Service Pack 3](https://www.microsoft.com/download/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
(Hoch)  
[Microsoft Office Word Viewer](https://www.microsoft.com/download/details.aspx?familyid=82980a40-f10c-4f02-b06c-3a12d4434a6b)  
(KB969614)  
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
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=63bd8f14-e736-46ce-af66-d30f17461e5a)  
(KB969613)  
(Hoch)
</td>
<td style="border:1px solid black;">
[Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2)  
(KB969679)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Works 8.5
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 8.5](https://www.microsoft.com/download/details.aspx?familyid=628280fe-e035-4274-85f2-393d9bad543c)  
(KB967043)  
(Hoch)
</td>
</tr>
<tr class="alternateRow">
<td style="border:1px solid black;">
Microsoft Works 9
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Works 9](https://www.microsoft.com/download/details.aspx?familyid=f6fa110e-45c6-450f-ae47-c89a06e3f762)  
(KB967044)  
(Hoch)
</td>
</tr>
<tr>
<td style="border:1px solid black;">
Microsoft Office SharePoint Server
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
<td style="border:1px solid black;">
[Microsoft Office SharePoint Server 2007 Service Pack 1 und Microsoft Office SharePoint Server 2007 Service Pack 2 (32-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=862e6ad1-8124-4060-93b1-2b882ef5ce3d)\*\*  
(KB969737)  
(Hoch)  
[Microsoft Office SharePoint Server 2007 Service Pack 1 und Microsoft Office SharePoint Server 2007 Service Pack 2 (64-Bit-Editionen)](https://www.microsoft.com/download/details.aspx?familyid=b7b6e611-2c5d-4639-add9-972055789ecd)\*\*  
(KB969737)  
(Hoch)
</td>
<td style="border:1px solid black;">
Nicht anwendbar
</td>
</tr>
</table>
 
**Hinweise für MS09-021**

\*Für Microsoft Office Excel 2007 Service Pack 1 und Microsoft Office Excel 2007 Service Pack 2 müssen Benutzer zusätzlich zum Sicherheitsupdatepaket KB969682 auch das Sicherheitsupdate für [Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 1 und Microsoft Office Compatibility Pack für die Dateiformate von Word, Excel und PowerPoint 2007 Service Pack 2](https://www.microsoft.com/download/details.aspx?familyid=a8be8457-b0b6-455e-907e-d13be883adf2) (KB969679) installieren, um vor den in diesem Bulletin beschriebenen Sicherheitsanfälligkeiten geschützt zu sein.

\*\*Dieses Update gilt für Server, auf denen Excel Services installiert ist, z. B. die Standardkonfiguration von Microsoft Office SharePoint Server 2007 Enterprise und Microsoft Office SharePoint Server 2007 für Websites. Microsoft Office SharePoint Server 2007 Standard enthält Excel Services nicht.

**Hinweis für MS09-024**

\*\*\*Microsoft Office Word 2003 ist betroffen, wenn ein anfälliger Works-Konverter installiert ist. Works-Konverter sind für Microsoft Office Word 2003 als Download unter [Microsoft Works 6–9-Dateikonverter](https://www.microsoft.com/download/details.aspx?displaylang=de&familyid=bf41401e-70fa-465d-ae2e-cf44dbf05297) verfügbar.

Tools und Anleitungen zur Erkennung und Bereitstellung
------------------------------------------------------

**Sicherheitsportal:**

Verwalten Sie die Software und die Sicherheitsupdates, die Sie den Servern, Desktops und mobilen Computer in Ihrer Organisation bereitstellen müssen. Weitere Informationen finden Sie im [TechNet Update Management Center](https://technet.microsoft.com/de-de/updatemanagement/default.aspx). Im [TechNet Sicherheits-Center](https://www.microsoft.com/germany/technet/sicherheit/default.mspx) werden zusätzliche Informationen zur Sicherheit in Microsoft-Produkten zur Verfügung gestellt. Verbraucher können die Seite [Sicherheit zu Hause](https://www.microsoft.com/germany/athome/security/default.mspx) besuchen, wo diese Informationen auch durch einen Klick auf „Die neuesten Sicherheitsupdates“ verfügbar sind.

Sicherheitsupdates sind auch über [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747), [Windows Update](https://go.microsoft.com/fwlink/?linkid=21130) und [Office Update](https://office.microsoft.com/de-de/downloads/default.aspx) verfügbar. Sicherheitsupdates sind auch im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar. Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.

Außerdem können Sicherheitsupdates vom [Windows Update-Katalog](https://go.microsoft.com/fwlink/?linkid=96155) heruntergeladen werden. Der Microsoft Update-Katalog stellt einen durchsuchbaren Katalog der Inhalte bereit, die über Windows Update und Microsoft Update zur Verfügung gestellt werden, einschließlich Sicherheitsupdates, Treiber und Service Packs. Indem Sie mit der Nummer des Security Bulletins suchen (z. B. „MS07-036“), können Sie Ihrem Warenkorb alle anwendbaren Updates (einschließlich verschiedener Sprachen für ein Update) hinzufügen und in den Ordner Ihrer Wahl herunterladen. Weitere Informationen zum Microsoft Update-Katalog, finden Sie unter [Häufig gestellte Fragen zum Microsoft Update-Katalog](https://catalog.update.microsoft.com/v7/site/faq.aspx).

**Anleitungen zur Erkennung und Bereitstellung**

Zu den Sicherheitsupdates dieses Monats stellt Microsoft Anleitungen zur Erkennung und Bereitstellung zur Verfügung: Diese Anleitungen geben auch IT-Profis Informationen zum Einsatz der verschiedenen Tools und zur Bereitstellung des Sicherheitsupdates. Behandelt werden u. a. Windows Update, Microsoft Update, Office Update, Microsoft Baseline Security Analyzer (MBSA), Office Detection Tool, Microsoft Systems Management Server (SMS) und das Erweiterte Sicherheitsupdate-Inventurprogramm (ESUIT). Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 910723](https://support.microsoft.com/kb/910723).

**Microsoft Baseline Security Analyzer**

Mit dem Microsoft Baseline Security Analyzer können Sie als Administrator Systeme sowohl lokal als auch remote auf fehlende Sicherheitspatches und fehlerhafte Konfigurationen überprüfen. Weitere Informationen zu MBSA finden Sie auf der Website [Microsoft Baseline Security Analyzer](https://www.microsoft.com/germany/technet/sicherheit/tools/mbsa/2_0.mspx).

**Windows Server Update Services**

Mithilfe der Windows Server Update Services (WSUS), können Administratoren die neuesten wichtigen Aktualisierungen und Sicherheitsupdates für Windows 2000 und höher, Office XP und höher, Exchange Server 2003 und SQL Server 2000 für Windows 2000 und neuere Betriebssysteme schnell und zuverlässig bereitstellen.

Weitere Informationen zum Bereitstellen dieses Sicherheitsupdates mithilfe der Windows Server Update Services finden Sie auf der [Windows Server Update Services Website](https://www.microsoft.com/germany/technet/prodtechnol/windowsserver/wsus/default.mspx).

**Systems Management Server**

Der Systems Management Server von Microsoft stellt eine wertvolle Hilfe beim Bereitstellen von Sicherheitsupdates in Ihrer IT-Umgebung dar. Durch die Verwendung von SMS können Administratoren auf Windows basierte Systeme identifizieren, für die Sicherheitsupdates erforderlich sind, und für eine kontrollierte Bereitstellung dieser Updates im gesamten Unternehmen bei minimalen Unterbrechungen für Endbenutzer sorgen. Die nächste Version von SMS, System Center Configuration Manager 2007, ist jetzt verfügbar (siehe auch [System Center Configuration Manager 2007](https://technet.microsoft.com/en-us/library/bb735860.aspx)). Weitere Informationen zur Verwendung von SMS 2003 durch Administratoren für die Bereitstellung von Sicherheitsupdates finden Sie unter [SMS 2003 Security Patch Management](https://go.microsoft.com/fwlink/?linkid=22939). Benutzer von SMS 2.0 können auch die Website [Software Updates Service Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2/downloads/featurepacks/suspack/default.mspx) besuchen, um Hilfe bei der Bereitstellung von Sicherheitsupdates zu erhalten. Weitere Informationen zu SMS finden Sie auf der Website [Microsoft Systems Management Server](https://www.microsoft.com/germany/smserver/default.mspx).

**Hinweis:** SMS nutzt Microsoft Baseline Security Analyzer und das Microsoft Office Detection-Tool für eine breite Unterstützung bei der Erkennung und der Bereitstellung von Security Bulletin-Updates. Einige Softwareupdates werden von diesen Tools möglicherweise nicht erkannt. Administratoren können in diesen Fällen die Inventurfunktionen von SMS nutzen, um Updates auf ausgewählten Systemen zu installieren. Weitere Informationen zu diesem Verfahren finden Sie auf der Website [Bereitstellen von Softwareupdates mit der Funktion zur Softwareverteilung von SMS](https://www.microsoft.com/technet/sms/2003/patchupdate.mspx). Bei einigen Sicherheitsupdates, die einen Neustart des Systems erfordern, sind unter Umständen administrative Rechte nötig. Administratoren können das im [SMS 2003 Administration Feature Pack](https://www.microsoft.com/technet/prodtechnol/sms/sms2003/downloads/featurepacks/adminpack.mspx) und im [SMS 2.0 Administration Feature Pack](https://go.microsoft.com/fwlink/?linkid=21161) enthaltene Elevated Rights Deployment Tool verwenden, um diese Updates zu installieren.

**Updatekompatibilitätsbewertung und Microsoft Application Compatibility Toolkit**

Updates bearbeiten oft dieselben Dateien und Registrierungseinstellungen, die zum Ausführen Ihrer Anwendungen benötigt werden. Dies kann eine Inkompatibilität auslösen und die Bereitstellung von Sicherheitsupdates verzögern. Mit den Komponenten zur [Updatekompatibilitätsbewertung](https://technet.microsoft.com/de-de/library/cc766043.aspx), die im [Microsoft Application Compatibility Toolkit 5.0](https://www.microsoft.com/download/details.aspx?familyid=24da89e9-b581-47b0-b45e-492dd6da2971&displaylang=en) enthalten sind, können Sie die Vereinbarkeit von Windows-Updates mit installierten Anwendungen testen und überprüfen.

Das Microsoft Application Compatibility Toolkit (ACT) enthält alle notwendigen Tools und Dokumentationen, um die Anwendungskompatibilität zu prüfen und eventuelle Probleme zu beheben, bevor Microsoft Windows Vista, ein Windows-Update, ein Microsoft-Sicherheitsupdate oder eine neue Version von Windows Internet Explorer in Ihrer Umgebung bereitgestellt wird.

### Weitere Informationen:

#### Windows-Tool zum Entfernen bösartiger Software

Microsoft hat eine aktualisierte Version des Microsoft Windows-Tools zum Entfernen bösartiger Software in Windows Update, Microsoft Update, Windows Server Update Services und dem Download Center veröffentlicht.

#### Nicht sicherheitsrelevante, wichtige Updates unter MU, WU und WSUS:

Weitere Informationen zu nicht sicherheitsrelevanten Veröffentlichungen auf Windows-Update und Microsoft Update finden Sie unter:

-   [Microsoft Knowledge Base-Artikel 894199](https://support.microsoft.com/kb/894199): Beschreibung der Änderungen an den Inhalten von Software Update Services und Windows Server Update Services. Umfasst alle Windows-Inhalte.
-   [Neue, überarbeitete und veröffentlichte Updates für andere Microsoft-Produkte als Microsoft Windows](https://technet.microsoft.com/en-us/wsus/dd573344.aspx).

#### Microsoft Active Protections Program (MAPP)

Um den Sicherheitsschutz für Benutzer zu verbessern, stellt Microsoft den wichtigsten Sicherheitssoftwareanbietern vor der monatlichen Veröffentlichung der Sicherheitsupdates Informationen zu Sicherheitsanfälligkeiten bereit. Anbieter von Sicherheitssoftware können diese Informationen zu Sicherheitsanfälligkeiten dann verwenden, um Benutzern aktualisierten Schutz über ihre Sicherheitssoftware oder ihre Geräte bereitzustellen, z. B. Antivirus, netzwerkbasierte Angriffserkennungssysteme oder hostbasierte Angriffsverhinderungssysteme. Wenn Sie erfahren möchten, ob von den Sicherheitssoftwareanbietern aktiver Schutz verfügbar ist, besuchen Sie die von den Programmpartnern bereitgestellte Active Protections-Websites, die unter [MAPP-Partner (Microsoft Active Protections Program)](https://www.microsoft.com/security/msrc/mapp/partners.mspx) aufgeführt sind.

#### Sicherheitsstrategien und Community

**Strategien für die Verwaltung von Sicherheitspatches:**

Auf der Seite [Patchmanagement](https://www.microsoft.com/germany/technet/sicherheit/themen/patchmanagement.mspx) werden zusätzliche Informationen zu den empfohlenen Vorgehensweisen für die Anwendung von Sicherheitsupdates von Microsoft bereitgestellt.

**Weitere Sicherheitsupdates**

Updates für andere Sicherheitsrisiken sind unter den folgenden Adressen erhältlich:

-   Sicherheitsupdates sind im [Microsoft Download Center](https://www.microsoft.com/downloads/results.aspx?displaylang=de&freetext=sicherheitsupdate) verfügbar Sie können am einfachsten durch eine Suche nach dem Begriff „security update“ ermittelt werden.
-   Updates für Benutzerplattformen sind auf [Microsoft Update](https://go.microsoft.com/fwlink/?linkid=40747) verfügbar.
-   Die Sicherheitsupdates, die in diesem Monat über Windows Update veröffentlicht wurden, können Sie auch im „Security and Critical Releases ISO CD Image“ über Microsoft Download Center erhalten. Weitere Informationen finden Sie im [Microsoft Knowledge Base-Artikel 913086](https://support.microsoft.com/kb/913086).

**IT Pro Security Community:**

Erfahren Sie, wie Sie die Sicherheit Ihrer IT-Umgebung erhöhen und Ihren IT-Betrieb optimieren können. Diskutieren Sie auf der [IT Pro Security Zone](https://go.microsoft.com/fwlink/?linkid=21164) Website mit anderen IT-Profis über das Thema Sicherheit.

#### Danksagungen

Microsoft [dankt](https://www.microsoft.com/germany/technet/sicherheit/bulletins/policy.mspx) den folgenden Personen, dass sie zum Schutz unserer Kunden mit uns zusammengearbeitet haben:

-   Joshua J. Drake von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS09-018 beschriebenes Problem.
-   Justin Wyatt vom [Beaverton School District](https://www.beaverton.k12.or.us/home/) für den Hinweis auf ein in MS09-018 beschriebenes Problem.
-   David Bloom von [Google Inc.](https://www.google.com/) für die Zusammenarbeit bezüglich eines in MS09-019 beschriebenen Problems.
-   Jorge Luis Alvarez Medina von [Core Security Technologies](https://www.coresecurity.com/) für den Hinweis auf ein in MS09-019 beschriebenes Problem.
-   Haifei Li von Fortinets [FortiGuard Global Security Research Team](https://www.microsoft.com/technet/security/bulletin/www.fortiguardcenter.com) für den Hinweis auf ein in MS09-019 beschriebenes Problem.
-   [TippingPoint](https://www.tippingpoint.com/) und [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-019 beschriebenes Problem
-   Peter Vreugdenhil in Zusammenarbeit mit [TippingPoint](https://www.tippingpoint.com/) und [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-019 beschriebenes Problem.
-   Wushi in Zusammenarbeit mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf zwei in MS09-019 beschriebene Probleme.
-   Nils in Zusammenarbeit mit [TippingPoint](https://www.tippingpoint.com/) und der [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-019 beschriebenes Problem.
-   Yamata Li von [Palo Alto Networks](https://www.paloaltonetworks.com/) für den Hinweis auf ein in MS09-020 beschriebenes Problem.
-   Bing Liu von Fortinets [FortiGuard Global Security Research Team](https://www.fortiguardcenter.com/) für den Hinweis auf drei in MS09-021 beschriebene Probleme.
-   Carsten H. Eiram von [Secunia](https://secunia.com/) für den Hinweis auf zwei in MS09-021 beschriebene Probleme.
-   [TELUS Security Labs Vulnerability Research Team](https://telussecuritylabs.com/) für den Hinweis auf ein in MS09-021 beschriebenes Problem.
-   Sean Larsson und Joshua Drake von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS09-021 beschriebenes Problem.
-   [TippingPoint](https://www.tippingpoint.com/) und [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-021 beschriebenes Problem
-   Jun Mao von [VeriSign iDefense Labs](https://labs.idefense.com/) für den Hinweis auf ein in MS09-022 beschriebenes Problem.
-   Yair Amit von [IBM Rational Application Security](https://blog.watchfire.com/) für den Hinweis auf ein in MS09-023 beschriebenes Problem.
-   Shaun Colley von [NGS Software](https://www.ngssoftware.com/) und Yuji Ukai von [Fourteenforty Research Institute, Inc.](https://www.fourteenforty.jp/) für den Hinweis auf ein in MS09-024 beschriebenes Problem.
-   Thomas Garnier für den Hinweis auf zwei in MS09-025 beschriebene Probleme.
-   Wushi von [team509](https://www.team509.com/) in Zusammenarbeit mit [Zero Day Initiative](https://www.zerodayinitiative.com/) für den Hinweis auf ein in MS09-027 beschriebenes Problem.
-   Nicolas Joly von [VUPEN Security](https://www.vupen.com/) für den Hinweis auf ein in MS09-027 beschriebenes Problem.

#### Support

-   Die betroffene Software wurde getestet, um die betroffenen Versionen zu ermitteln. Andere Versionen haben das Ende ihrer Supportlebenszyklen erreicht. Besuchen Sie die Website [Microsoft Support Lifecycle](https://support.microsoft.com/default.aspx?scid=fh;%5Bln%5D;lifecycle), um den Supportlebenszyklus für Ihre Softwareversion zu ermitteln.
-   Technischer Support ist über den [Security Support](https://go.microsoft.com/fwlink/?linkid=21131) erhältlich. Supportanrufe zu Sicherheitsupdates sind kostenlos. Weitere Informationen zu verfügbaren Supportoptionen finden Sie auf der [Microsoft-Website „Hilfe und Support“](https://support.microsoft.com/).
-   Kunden außerhalb der USA erhalten Support bei ihren regionalen Microsoft-Niederlassungen. Supportanfragen zu Sicherheitsupdates sind kostenlos. Weitere Informationen dazu, wie Sie Microsoft in Bezug auf Supportfragen kontaktieren können, finden Sie auf der Website [Internationale Hilfe und Support](https://go.microsoft.com/fwlink/?linkid=21155).

#### Haftungsausschluss

Die Informationen der Microsoft Knowledge Base werden wie besehen und ohne jede Gewährleistung bereitgestellt. Microsoft schließt alle anderen Garantien, gleich ob ausdrücklich oder konkludent, einschließlich der Garantien der Handelsüblichkeit oder Eignung für einen bestimmten Zweck aus. In keinem Fall kann Microsoft Corporation und/oder deren jeweilige Lieferanten haftbar gemacht werden für Schäden irgendeiner Art, einschließlich direkter, indirekter, zufällig entstandener Schäden, Folgeschäden, Folgen entgangenen Gewinns oder spezieller Schäden, selbst dann nicht, wenn Microsoft Corporation und/oder deren jeweilige Lieferanten auf die mögliche Entstehung dieser Schäden hingewiesen wurde. Weil in einigen Staaten/Rechtsordnungen der Ausschluss oder die Beschränkung einer Haftung für zufällig entstandene Schäden oder Folgeschäden nicht gestattet ist, gilt die obige Einschränkung eventuell nicht für sie.

#### Revisionen

-   V1.0 (9. Juni 2009): Bulletin Summary veröffentlicht.
-   V1.1 (10. Juni 2009): Die Bewertung und Wichtigen Hinweise zu CVE-2009-1138 im Ausnutzbarkeitsindex wurden korrigiert.

*Built at 2014-04-18T01:50:00Z-07:00*
